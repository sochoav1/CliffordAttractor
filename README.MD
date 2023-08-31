# Atractor de Clifford

El atractor de Clifford es un sistema dinámico que produce patrones fractales. Basado en un conjunto de ecuaciones matemáticas, es capaz de generar visualizaciones complejas y hermosas a partir de parámetros simples.

## Visualización Gráfica

El atractor de Clifford transforma cada punto \( (x, y) \) en un nuevo punto \( (x', y') \) utilizando las siguientes ecuaciones:

\[
x' = \sin(a \cdot y) + c \cdot \cos(a \cdot x)
\]
\[
y' = \sin(b \cdot x) + d \cdot \cos(b \cdot y)
\]

Los parámetros \( a \), \( b \), \( c \), y \( d \) pueden ser ajustados por el usuario, permitiendo la creación de distintos patrones pseudoaleatorios. Al iterar estas ecuaciones repetidamente, se obtiene un conjunto de puntos que, al ser graficados, revelan patrones fascinantes.

### Ejemplos de implementación

![Atractor con constantes \( a, b, c, d \) = (-1.5, -2, -2, 3)](./Outputs/a,%20b,%20c,%20d%20=%20-1.5,%20-2,%20-2,%203.png)

![Atractor con constantes \( a, b, c, d \) = (1, -4, -1.8, 3)](./Outputs/a,%20b,%20c,%20d%20=%201,%20-4,%20-1.8,%203.png)

## Atractor de Clifford para Cifrado

Exploramos el uso del atractor de Clifford para crear un método de cifrado simple y único.

### Descripción

Usando el atractor de Clifford, generamos una secuencia pseudoaleatoria que posteriormente se utiliza para cifrar mensajes a través de operaciones XOR.

### Uso

1. Elije valores para los parámetros \( a \), \( b \), \( c \), y \( d \). Estos actuarán como tu clave.
2. Usa la función `encrypt` para cifrar tu mensaje.
3. Usa la función `decrypt` para descifrar un mensaje cifrado, empleando la misma clave.

#### Ejemplo de uso

Utilizando valores \( a, b, c, d \) = (-1.3, -1.3, -1.8, -1.9), podemos cifrar un mensaje utilizando la fractalidad del atractor de Clifford:

**Input**: 'Hello, World!'
**Output**: 'p\x00\x1e\x94éCÒ«v¹m±\x12'
