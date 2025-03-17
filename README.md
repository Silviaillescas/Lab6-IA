# Lab6-IA
Michelle Mejía 22596 - Silvia Illescas 22376

## Descripción
Este proyecto implementa una inteligencia artificial (IA) para jugar **Connect Four** utilizando el **algoritmo Minimax** con la opción de **poda alfa-beta**. Se incluyen dos modos de juego:
- **Jugador humano vs IA**
- **IA vs IA** (comparación entre Minimax con y sin poda alfa-beta)

---

## Instrucciones de Instalación

### Prerrequisitos
Asegúrate de tener instalado **Python 3.x** y las siguientes librerías:
```bash
pip install numpy
```

### Clonar el repositorio
```bash
git clone <https://github.com/Silviaillescas/Lab6-IA.git>
cd connect-four-ai
```

---

## Modo de Uso

### Ejecutar el juego
Para jugar contra la IA:
```bash
python connect_four.py
```
Al ejecutar el script, aparecerá un menú para elegir el modo de juego:
1. **Jugador vs IA**
   - El usuario ingresa un número del **0 al 6** para colocar una ficha en la columna deseada.
   - La IA responde con su movimiento usando el algoritmo Minimax.
   - Gana el primer jugador en conectar **cuatro fichas consecutivas** (horizontal, vertical o diagonal).

2. **IA vs IA (comparación con/sin poda alfa-beta)**
   - Se ejecutarán **10 juegos** automáticamente.
   - Una IA usará poda alfa-beta y la otra no.
   - Se mostrará el rendimiento y los resultados al final.

Para iniciar IA vs IA directamente:
```bash
python connect_four.py --auto
```

---

## Explicación del Algoritmo

### Minimax
El **algoritmo Minimax** evalúa todos los posibles movimientos en un árbol de juego y elige la mejor jugada.

### Poda Alfa-Beta
La **poda alfa-beta** optimiza Minimax descartando ramas irrelevantes, **reduciendo el tiempo de cálculo** sin afectar la decisión óptima.

**Comparación entre IA con y sin poda alfa-beta:**
| Estrategia        | Evaluación de nodos | Velocidad |
|-------------------|--------------------|-----------|
| **Minimax puro**  | Explora todas las ramas posibles | Más lento |
| **Poda alfa-beta** | Reduce nodos innecesarios | Más rápido |

**Resultado esperado**: La IA con poda alfa-beta debería jugar más rápido y tener un mejor rendimiento en juegos IA vs IA.

---

## Video de Demostración
El video de la demostración se encuentra disponible en:

https://www.youtube.com/watch?v=zqg54iFdg7k