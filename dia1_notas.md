# Día 1 - Introducción a Python

En esta jornada se abordan los fundamentos más básicos del lenguaje.
Cada bloque incluye un ejercicio de práctica junto con su solución.

## Hola mundo
Tu primer programa en Python es como saludar en voz alta a una sala vacía.
Solo imprime un mensaje para comprobar que todo funciona.
```python
print('Hola, mundo!')
```

## Variables y tipos de datos
Piensa en las **variables** como cajas etiquetadas donde guardas datos.
Los **tipos** indican qué guardas dentro: números para contar, cadenas para
texto y booleanos para respuestas de "sí" o "no".

### Ejercicio 1
**Enunciado:** Imagina que tienes 10 manzanas y tu amigo te regala 7. Crea una
variable para cada cantidad, súmalas y muestra el total de manzanas.

Pasos a seguir:
1. Define `mis_manzanas` y `manzanas_amigo`.
2. Suma ambas en una variable `total`.
3. Muestra el resultado con `print()`.

**Solución**
```python
mis_manzanas = 10
manzanas_amigo = 7
total = mis_manzanas + manzanas_amigo
print(total)
```

## Operadores aritméticos
Sirven para hacer cálculos como los de una calculadora: sumar, restar,
multiplicar o dividir.
```python
total = 3 * 4 + 2
print(total)
```

### Ejercicio 2
**Enunciado:** Compraste una pizza de 25 USD y debes agregarle un 8 % de impuesto.
Descompón el problema así:
1. Calcula el valor del impuesto.
2. Suma el impuesto al precio base.
3. Muestra el total en pantalla.

**Solución**
```python
precio = 25
impuesto = precio * 0.08
final = precio + impuesto
print(final)
```

## Entrada de usuario y conversión de tipos
Sirve para conversar con quien usa tu programa. Pides datos por teclado y los
conviertes al tipo que necesites, como cuando anotas un número de teléfono y
lo guardas como dígitos.
```python
nombre = input('¿Cómo te llamas? ')
edad = int(input('Ingresa tu edad: '))
print(nombre, edad)
```

### Ejercicio 3
**Enunciado:** Tu abuela solo entiende grados Fahrenheit. Pide al usuario una
temperatura en Celsius y conviértela.

Pasos sugeridos:
1. Solicita la temperatura en Celsius con `input()`.
2. Usa la fórmula de conversión a Fahrenheit.
3. Muestra el resultado en pantalla.

**Solución**
```python
celsius = float(input('Temperatura en °C: '))
fahrenheit = celsius * 1.8 + 32
print(fahrenheit)
```

## Comentarios en el código
Los comentarios comienzan con `#` y sirven para explicar el código.
Son como anotaciones en una receta que recuerdan por qué haces cada paso;
Python las ignora al ejecutar.
```python
# Este es un comentario
print('Usando comentarios')
```

### Ejercicio 4
**Enunciado:** Construye un recordatorio de cumpleaños que imprima tu nombre y tu edad en líneas separadas. Comienza el programa con un comentario que indique lo que hará.

Pasos recomendados:
1. Escribe el comentario introductorio.
2. Usa `print()` para mostrar tu nombre.
3. Vuelve a usar `print()` para mostrar tu edad.

**Solución**
```python
# Imprime nombre y edad
print('Ana')
print(25)
```

## Conversión de tipos
Permite cambiar un dato de un tipo a otro, como transformar la cadena "5" en el
número 5 usando `int()`. Las funciones `int()`, `float()` y `str()` son las
herramientas básicas para lograrlo.

### Ejercicio 5
**Enunciado:** Estás siguiendo una receta que requiere una vez y media la can­tidad
de cierto ingrediente. Pide un número entero, conviértelo a flotante y multiplícalo por 1.5.

Divide el reto así:
1. Pide la cantidad original con `input()`.
2. Convierte el valor a flotante.
3. Multiplica por 1.5 y muestra el resultado.

**Solución**
```python
num = int(input('Ingresa un entero: '))
resultado = float(num) * 1.5
print(resultado)
```
