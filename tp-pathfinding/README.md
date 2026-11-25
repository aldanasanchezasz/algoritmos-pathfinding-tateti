# Buscador de caminos

Visualizador interactivo de algoritmos de búsqueda sobre una grilla con obstáculos.

## Algoritmos implementados

| Algoritmo | Archivo | Frontera | Óptimo |
|---|---|---|---|
| Depth First Search | `src/pathfinder/search/dfs.py` | Pila | No |
| Breadth First Search | `src/pathfinder/search/bfs.py` | Cola | Sí, con costos uniformes |
| Uniform Cost Search | `src/pathfinder/search/ucs.py` | Cola de prioridad por costo | Sí |
| Greedy Best First Search | `src/pathfinder/search/gbfs.py` | Cola de prioridad por heurística | No |
| A* | `src/pathfinder/search/astar.py` | Cola de prioridad por costo + heurística | Sí |

La heurística de Greedy y A* es la **distancia Manhattan** al objetivo, que es admisible en una grilla con movimientos horizontales y verticales.

## Funcionalidades

- Generación de laberintos.
- Animación de los nodos explorados y del camino final, con tres velocidades.
- Comparación de algoritmos sobre el mismo laberinto o sobre laberintos distintos.

## Ejecución

Requiere Python 3.10 o superior.

```bash
pip install -r requirements.txt
python run.pyw
```

## Créditos

Interfaz basada en el proyecto de Tauseef Hilal Tantary (licencia MIT, ver [LICENSE](LICENSE)), provisto por la cátedra. Los algoritmos de búsqueda son implementación propia.

## Requerimientos
* Python 3.10 o superior (https://www.python.org/downloads/).
* Pygame.

## Licencia
This project is licensed under the MIT License.
