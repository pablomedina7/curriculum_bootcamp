# Día 3 - Funciones y Proyecto

El último día se enfoca en funciones, estructuras de datos y un mini proyecto final.

## Funciones con retorno
Una función es como una máquina: recibe datos, los procesa y devuelve un
resultado usando `return`.
```python
def saludar(nombre):
    return f'Hola {nombre}'
print(saludar('Ana'))
```

### Ejercicio 1
**Enunciado:** Quieres saber cuánta cartulina necesitas para recortar un triángulo.
Crea una función que reciba la base y la altura y devuelva el área.

Pauta para resolverlo:
1. Declara la función con dos parámetros.
2. Calcula el área (base por altura dividido entre 2).
3. Retorna el resultado con `return`.

**Solución**
```python
def area_triangulo(base, altura):
    return base * altura / 2

print(area_triangulo(3, 4))
```

## Listas y bucles
Las listas almacenan varios valores en orden. Con los bucles podemos recorrerlas
de principio a fin, como leer página tras página de un cuaderno.
```python
palabras = ['hola', 'mundo']
for p in palabras:
    print(p.upper())
```

### Ejercicio 2
**Enunciado:** Tienes un conjunto de palabras secretas y quieres gritarlas. Crea
otra lista con cada palabra en mayúsculas.

Pasos:
1. Crea una lista vacía para el resultado.
2. Recorre las palabras originales con un `for`.
3. Agrega cada palabra en mayúsculas a la nueva lista.

**Solución**
```python
datos = ['python', 'bootcamp', 'penguin']
mayusculas = []
for d in datos:
    mayusculas.append(d.upper())
print(mayusculas)
```

## Mini proyecto: intento sencillo de Wordle
Un pequeño juego para adivinar una palabra de cuatro letras, inspirado en el
popular Wordle.
```python
secreta = 'casa'
intento = input('Adivina la palabra de 4 letras: ')
if intento == secreta:
    print('¡Ganaste!')
else:
    print('Sigue intentando')
```

## Diccionarios básicos
Estructuras que guardan pares clave-valor. Son como una agenda en la que 
buscas un nombre (clave) para obtener el teléfono (valor).
```python
persona = {'nombre': 'Ana', 'edad': 25}
print(persona['nombre'])
```

### Ejercicio 3
**Enunciado:** Para un juego de sopa de letras necesitas saber cuántas veces se
repite cada letra. Escribe una función que reciba una palabra y devuelva un
diccionario con el conteo de letras.

Guía de pasos:
1. Crea un diccionario vacío.
2. Recorre cada letra de la palabra.
3. Usa `get()` para incrementar el conteo.
4. Devuelve el diccionario al final.

**Solución**
```python
def contar_letras(palabra):
    conteo = {}
    for letra in palabra:
        conteo[letra] = conteo.get(letra, 0) + 1
    return conteo

print(contar_letras('banana'))
```

## Mini proyecto adicional: generador de contraseñas sencillas
Este pequeño script crea contraseñas al azar combinando letras y números.
```python
import random
caracteres = 'abc123'
clave = ''.join(random.choice(caracteres) for _ in range(6))
print('Contraseña:', clave)
```
