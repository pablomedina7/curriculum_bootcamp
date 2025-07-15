# Día 3 - Funciones y Proyecto

El último día se enfoca en funciones, estructuras de datos y un mini proyecto final.

## Funciones con retorno
```python
def saludar(nombre):
    return f'Hola {nombre}'
print(saludar('Ana'))
```

### Ejercicio 1
**Enunciado:** Crear una función que reciba base y altura y retorne el área de un triángulo.

**Solución**
```python
def area_triangulo(base, altura):
    return base * altura / 2

print(area_triangulo(3, 4))
```

## Listas y bucles
```python
palabras = ['hola', 'mundo']
for p in palabras:
    print(p.upper())
```

### Ejercicio 2
**Enunciado:** Dada una lista de palabras, crear otra lista con cada palabra en mayúsculas.

**Solución**
```python
datos = ['python', 'bootcamp', 'penguin']
mayusculas = []
for d in datos:
    mayusculas.append(d.upper())
print(mayusculas)
```

## Mini proyecto: intento sencillo de Wordle
```python
secreta = 'casa'
intento = input('Adivina la palabra de 4 letras: ')
if intento == secreta:
    print('¡Ganaste!')
else:
    print('Sigue intentando')
```

## Diccionarios básicos
Estructuras para almacenar pares clave-valor.
```python
persona = {'nombre': 'Ana', 'edad': 25}
print(persona['nombre'])
```

### Ejercicio 3
**Enunciado:** Crea una función que cuente la aparición de cada letra en una palabra y retorne un diccionario.

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
```python
import random
caracteres = 'abc123'
clave = ''.join(random.choice(caracteres) for _ in range(6))
print('Contraseña:', clave)
```
