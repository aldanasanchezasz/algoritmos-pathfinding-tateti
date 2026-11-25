# Tateti con Minimax

Agente que juega tateti (tic-tac-toe) de forma óptima usando el algoritmo **Minimax** de búsqueda entre adversarios.

## Cómo funciona

- `tateti.py` formula el juego según la teoría de juegos: estado inicial, jugador de turno, acciones posibles, resultado de cada acción, test terminal y utilidad.
- `estrategias.py` implementa dos estrategias:
  - **Aleatoria:** elige cualquier casilla libre (sirve como rival de referencia).
  - **Minimax:** recorre recursivamente el árbol de jugadas alternando nodos MAX y MIN y elige la acción con mejor valor garantizado. Contra este agente, lo mejor que se puede conseguir es un empate.

## Modos de juego

- Humano vs. humano
- Humano vs. máquina
- Máquina vs. máquina

## Estructura

```
tp-tateti/
├── tateti.py         # Formulación del juego
├── estrategias.py    # Estrategias aleatoria y Minimax
├── gui_pygame.py     # Interfaz gráfica
├── main.py           # Punto de entrada
├── test.py           # 18 tests unitarios
└── requirements.txt
```

## Ejecución

Requiere Python 3.10 o superior.

```bash
pip install -r requirements.txt
python main.py    # jugar
python test.py    # correr los tests
```

## Bibliografía

Russell, S. y Norvig, P. *Artificial Intelligence: A Modern Approach*, capítulo 5 (búsqueda entre adversarios).
