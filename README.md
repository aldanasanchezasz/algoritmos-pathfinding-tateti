# Algoritmos de búsqueda: pathfinding y tateti con Minimax

Dos proyectos de Inteligencia Artificial clásica (TUIA – UNR), con visualización interactiva en Pygame.

**Stack:** Python · Pygame · unittest

## 🧭 [Buscador de caminos](tp-pathfinding/)

Implementación de algoritmos de búsqueda sobre una grilla con obstáculos, con animación paso a paso de la exploración:

| Algoritmo | Tipo | ¿Encuentra el camino óptimo? |
|---|---|---|
| Depth First Search (DFS) | No informada | No |
| Breadth First Search (BFS) | No informada | Sí, si todos los pasos cuestan igual |
| Uniform Cost Search (UCS) | No informada | Sí |
| Greedy Best First Search | Informada | No |
| **A\*** (heurística: distancia Manhattan) | Informada | Sí |

La interfaz permite generar laberintos, elegir la velocidad de la animación y **comparar los algoritmos** sobre el mismo laberinto o sobre laberintos distintos.

## ❌⭕ [Tateti con Minimax](tp-tateti/)

Agente que juega tateti de forma óptima con el algoritmo **Minimax**: explora el árbol completo de jugadas y nunca pierde. Tres modos de juego (humano vs. humano, humano vs. máquina y máquina vs. máquina) y una suite de 18 tests unitarios.

## Cómo ejecutarlo

Requiere Python 3.10 o superior.

```bash
pip install pygame

# Buscador de caminos
cd tp-pathfinding
python run.pyw

# Tateti
cd tp-tateti
python main.py
python test.py      # tests
```

## Créditos

La interfaz gráfica del buscador de caminos parte del proyecto de Tauseef Hilal Tantary (licencia MIT), provisto por la cátedra. Los algoritmos de búsqueda y la estrategia Minimax son implementación propia.
