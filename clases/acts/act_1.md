[regresar a la clase 5](../5_19-11-2026.md)
# Actividad
### hacer que los enemigos bajen verticalmente sin que se muevan en horizontal

### Issue:
**Titulo:**
```
T03 - Movimiento vertical de la nave
```
```
La nave debe
- [x] Moverse horizontalmente
- [x] No moverse verticalmente
```
### Codigo final
```kt
//movimiento vertical
    LaunchedEffect(Unit) {
        while (true) {
            delay(30L)
            if (gameStarted && screenWidth > 0f && enemies.isNotEmpty()) {
                val enemyWidth = 60f
                val margin = enemyWidth / 2
                val speed = 50f
                val dropDistance = 20f
                enemyDirection *= -1f
                enemies = enemies.map { enemy -> enemy.copy(y = enemy.y + dropDistance) }
            }
        }
    }
```
### Solucion
Modifica solamente `//Movimiento horizontal de los enemigos`
1. Elmina los valores que hacen el movimiento vertical
2. Quitar el movimiento vetical de la condicion
```diff
LaunchedEffect(Unit) {
            while (true) {
                delay(30L)
                if (gameStarted && screenWidth > 0f && enemies.isNotEmpty()) {
                    val enemyWidth = 60f
                    val margin = enemyWidth / 2
                    val speed = 50f
                    val dropDistance = 20f
-                   val leftEdge = enemies.minOf { it.x - margin }
-                   val rightEdge = enemies.maxOf { it.x + margin }
-                   val reachedEdge = (enemyDirection > 0f && rightEdge + speed >= screenWidth) ||
                            (enemyDirection < 0f && leftEdge - speed <= 0f)

-                   if (reachedEdge) {
                        enemyDirection *= -1f
                        enemies = enemies.map { enemy ->
                            enemy.copy(y = enemy.y + dropDistance)
                        }
-                   }
-                   enemies = enemies.map { enemy ->
-                       enemy.copy(x = enemy.x + speed * enemyDirection)
-                   }
                }
            }
        }
```
### Movimiento vertical de enemigos:
```kt
enemyDirection *= -1f
enemies = enemies.map { enemy -> enemy.copy(y = enemy.y + dropDistance)}
```