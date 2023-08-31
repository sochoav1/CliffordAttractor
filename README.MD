# Atractor de Clifford, visualización gráfica
Un atractor de Cliffor es un tipo de sistema dinámico que produce patrones fractálicos. Es un sistema discreto en el que cada punto (x,y) se transforma en un punto (x´, y´) usando las ecuaciones

x' = \sin(a \cdot y) + c \cdot \cos(a \cdot x)

y' = \sin(b \cdot x) + d \cdot \cos(b \cdot y)

siendo a,b,c,d parámetros elegidos por el usuario, estos parámetros se pueden ajustar para producir distintos patrones pseudo aleatorios

Al iterar estas ecuaciones muchas veces, se obtiene un conjunto de puntos que, cuando se grafican, forman patrones interesantes y a menudo hermosos.

##Ejemplo de implementación


![Atractor con Constantes a,b,c,d = -1,5,-2,3](./Outputs/a,%20b,%20c,%20d%20=%20-1.5,%20-2,%20-2,%203.pngejemplo.png)

![Atractor con Constantes a,b,c,d = 1,-4,-1.8,3](./Outputs/a,%20b,%20c,%20d%20=%201,%20-4,%20-1.8,%203.png)


# Atractor de Clifford para Cifrado

Este proyecto explora el uso del atractor de Clifford, un sistema dinámico que produce patrones fractales, para crear un método simple de cifrado.

## Descripción

El atractor de Clifford es un sistema discreto que transforma puntos usando las siguientes ecuaciones:


x' = \sin(a \cdot y) + c \cdot \cos(a \cdot x)

y' = \sin(b \cdot x) + d \cdot \cos(b \cdot y)


Para el cifrado, usamos estos atractores para generar una secuencia pseudoaleatoria que luego se utiliza para cifrar un mensaje a través de operaciones XOR.

## Uso

1. Elija valores para los parámetros \(a\), \(b\), \(c\), y \(d\). Estos actuarán como su clave.
2. Use la función `encrypt` para cifrar su mensaje.
3. Use la función `decrypt` para descifrar un mensaje cifrado, usando la misma clave.

### Ejemplo de uso

usando valores de a,b,c,d = key = (-1.3, -1.3, -1.8, -1.9) podemos encriptar un input utilizando la fractalidad del atractor de Clifford

Input = 'Hello, World!'
Output = 'p\x00\x1e\x94éCÒ«v¹m±\x12'



