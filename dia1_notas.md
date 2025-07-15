# Día 1 - Introducción a Python

En esta jornada se abordan los fundamentos más básicos del lenguaje.
Cada bloque incluye un ejercicio de práctica junto con su solución.

## Hola mundo
```python
print('Hola, mundo!')
```

## Variables y tipos de datos
Explicación breve de números, cadenas y booleanos.

### Ejercicio 1
**Enunciado:** Crea dos variables numéricas, súmalas y muestra el resultado.

**Solución**
```python
a = 10
b = 7
resultado = a + b
print(resultado)
```

## Operadores aritméticos
```python
total = 3 * 4 + 2
print(total)
```

### Ejercicio 2
**Enunciado:** Calcula el precio final de un producto de 25 dólares con un 8% de impuesto.

**Solución**
```python
precio = 25
impuesto = precio * 0.08
final = precio + impuesto
print(final)
```

## Entrada de usuario y conversión de tipos
```python
nombre = input('¿Cómo te llamas? ')
edad = int(input('Ingresa tu edad: '))
print(nombre, edad)
```

### Ejercicio 3
**Enunciado:** Pide al usuario una temperatura en Celsius y conviértela a Fahrenheit.

**Solución**
```python
celsius = float(input('Temperatura en °C: '))
fahrenheit = celsius * 1.8 + 32
print(fahrenheit)
```

## Comentarios en el código
Los comentarios comienzan con `#` y sirven para explicar el código.
```python
# Este es un comentario
print('Usando comentarios')
```

### Ejercicio 4
**Enunciado:** Escribe un programa que imprima tu nombre y tu edad en líneas separadas. Incluye un comentario al inicio explicando la tarea.

**Solución**
```python
# Imprime nombre y edad
print('Ana')
print(25)
```

## Conversión de tipos
Se puede convertir un valor con funciones como `int()`, `float()` y `str()`.

### Ejercicio 5
**Enunciado:** Solicita un número entero al usuario, conviértelo a flotante y multiplícalo por 1.5.

**Solución**
```python
num = int(input('Ingresa un entero: '))
resultado = float(num) * 1.5
print(resultado)
```
