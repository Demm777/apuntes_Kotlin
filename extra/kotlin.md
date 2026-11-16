[regresar a **principal**](../principal.md)\
# APLICACIONES ANDROID
## Descargar android studio
1. empty activit
2. nombre del projecto "Game3315298"
3. crear

## Crear proyecto en github
1. perfil
2. projects
3. new project
4. board
   1. poner nombre
   2. asignar al repositorio
   3. **crear**
5. Renombrar tarjetas:
   1. ### BACKLOG
    ```
    Todo lo que queremos que tenga el juego, pero que todavia no hemos seleccionado para un Sprint  
    ```
    2. ### POR HACER
    ```
    Trabajo seleccionado para el Sprint actual, pero que todavia no hemos comenzado
    ```
    3. ### EN DESARROLLO
    ```
    Estamos programando o contruyendo esta funcionalidad
    ```
6. Crear nueva columna (+)

   4. ### EN REVISION
   ```
   la funcionalidad esta terminada tecnicamente, pero falta probarla
   ```
   5. ### TERMINADO
   ```
   La funcionalidad fue implementada y probada correctamente
   ```
   debe quedar en este orden:
   ![orden_tarjetas](/markdown/images/image2.png)

## Asignar estados
En el proyecto:
1. Settings
2. Fields -> ( + )
3. ### Create a project field:
   1. #### Tipo
   - Single select:
    > Historia de usuario <br>
    Tarea <br>
    Bug <br>
    Mejora <br>
    -  Create
    2. #### Prioridad
    - Single select:
    > Alta <br>
    Media <br>
    Baja <br>
    -  Create
    3. #### Story Points
    - Number
    - Create
    4. #### Sprint
    - Iteration
    - "dejar valores por defecto"
    - Create

### subir a github
1. git
2. commit
3. unversioned files
### descargar emulador de celular
1. device manager (arriba derecha)
2. ( + ) -> Create virtual device
3. #### Pixel 6:
   1. **API:** API 35 "VanillaIceCream; Android 15,0"
   2. Descargar *System image* "la que tiene la estrella ⭐"
   3. Finish

***
> <center> 15/10/2026
***

## Agregar el proyecto al repositorio
1. abrir el repositorio del proyecto
2. Projects
3. Link a project
4. añadir el proyecto
5. Issues
6. ### New Issue
   - nombre: HU-01: Mover la nave en la pantalla
   - write:
    ### Como | Quiero | Para
    ```
    # Historia de usuario

    **Como** jugador,
    **quiero** mover la nave horizontalmente en la pantalla,
    **para** poder controlar su posicion durante la partida
    ```
    ### metodologia Scrum:
    metodo que ayuda a equipos a a estructurar bien el proyecto trbajando en Sprints (pequeños proyectos que suman) <br>
    ***Roles:*** <br>
    **Product Owner:** define la vision del producto <br>
    **Scrum master:** asegura y supervisa que continue el proceso <br>
    **Equipo de desarrollo:** personas que contribuyen y crean el producto

    ### Criterios de aceptacion:
    ```
    ## Criterios de aceptacion

   - [ ] La nave aparece dentro del area del juego. en la parte inferior centrado
    - [ ] El jugador puede tocar y arrastrar la nave.
    - [ ] La nave responde al movimiento del dedo.
    - [ ] La  nave puede desplazarse horizontalmente
    - [ ] La nave no puede salir de los limites de la pantalla
    - [ ] El movimiento funciona correctamente en el dispositivo
    ```

    ### Resultado esperado
    ```
    ## Resultado esperado
    El jugador puede controlar la posicion horizontal de la nave medianteb un gesto tactil
    ```
7. finish / publicar
8. project
9. "projecto"
10. ### en backlog
    - add item
    - ( + )
    - add item from repository
    - agregar issue creada anteriormente
11. click en el issue
12. asignar estos valores:

    ![img1](/markdown/images/image1.png)

    story points: ***Serie fibonacci*** <br>
    Cada numero es el resultado de sumar los anteriores empezando desde 0 <br>
    | # + # | =   |
    | ----- | --- |
    | 0+1   | 1   |
    | 1+1   | 2   |
    | 1+2   | 3   |
    | 2+3   | 5   |
    | 3+5   | 8   |
    etc...
    [lista](https://www.math.net/list-of-fibonacci-numbers)

### Nuevo issue:
### nombre: HU-02: Disparar desde la nave
### Write: 
```
# Historia de usuario

**Como** jugador
**quiero** disparar desde la nave
**para** poder atacar a los enemigos

## Criterios de aceptacion
- [ ] El jugador puede realizar la accion de disparo
- [ ] El disparo se genera desde la posicion de la nave
- [ ] El proyectil se desplaza hacia la parte superior de la pantalla
- [ ] El proyectil permanece dentro del area del juego
- [ ] El disparo puede interactuar posteriormente con el enemigo

## Resultado esperado
El jugador puede disparar proyectiles desde la nave durante la partida
```
> ### agragar al backlog
> ### Historia de usuario | ALTA
 
### Issue 3
### Nombre: HU-03: Generar enemigos en la pantalla
### Write:
```
# Historia de usuario

**Como** jugador
**quiero** que aparezcan enemigos en la pantalla 
**para** tener objetivos contra los cuales luchar

## Criterios de aceptacion
- [ ] Los enemigos aparecen dentro del area de juego
- [ ] Los enemigos se generan en posiciones variables
- [ ] Los enemigos permanecen dentro de los limites definidos
- [ ] Los enemigos se mueven hacia la parte inferior de la pantalla
- [ ] Se pueden generar varios enemigos durante la partida

## Resultado esperado
El juego presenta enemigos que el jugador puede enfrentar con la nave
```
> ### agragar al backlog
> ### Historia de usuario | ALTA





> ## tarea final: aplicar al proyecto formativo