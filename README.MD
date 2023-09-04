# Clifford Attractor

The Clifford attractor is a dynamical system that produces fractal patterns. Based on a set of mathematical equations, it is capable of generating complex and beautiful visualizations from simple parameters.

## Graphical Visualization

The Clifford attractor transforms each point \( (x, y) \) into a new point \( (x', y') \) using the following equations:

\[
x' = \sin(a \cdot y) + c \cdot \cos(a \cdot x)
\]
\[
y' = \sin(b \cdot x) + d \cdot \cos(b \cdot y)
\]

The parameters \( a \), \( b \), \( c \), and \( d \) can be adjusted by the user, allowing for the creation of various pseudo-random patterns. By iterating these equations repeatedly, a set of points is obtained. When plotted, these points reveal fascinating patterns that captivate the eye. These patterns can vary from scattered points to intricate spirals, depending on the parameter values.

### Implementation Examples

![Attractor with constants \( a, b, c, d \) = (-1.5, -2, -2, 3)](./Outputs/a,%20b,%20c,%20d%20=%20-1.5,%20-2,%20-2,%203.png)

![Attractor with constants \( a, b, c, d \) = (1, -4, -1.8, 3)](./Outputs/a,%20b,%20c,%20d%20=%201,%20-4,%20-1.8,%203.png)

## Clifford Attractor for Encryption

We explore the use of the Clifford attractor to create a simple and unique encryption method.

### Description

Using the Clifford attractor, we generate a pseudo-random sequence that is subsequently used to encrypt messages through XOR operations. This encryption method leverages the unpredictability and intricacy of the attractor, making it difficult to decipher without the correct key.

### Usage

1. Choose values for the parameters \( a \), \( b \), \( c \), and \( d \). These will act as your key.
2. Use the `encrypt` function to encrypt your message.
3. Use the `decrypt` function to decipher an encrypted message, employing the same key.

#### Usage Example

Using values \( a, b, c, d \) = (-1.3, -1.3, -1.8, -1.9), we can encrypt a message leveraging the fractality of the Clifford attractor:

**Input**: 'Hello, World!'
**Output**: 'p\x00\x1e\x94éCÒ«v¹m±\x12'
