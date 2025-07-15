# Día 2 - Condicionales y Bucles

Continuamos con estructuras de control y repetición.
A cada concepto le sigue un ejercicio práctico y su solución.

## Condicionales
```python
edad = 20
if edad >= 18:
    print('Mayor de edad')
else:
    print('Menor de edad')
```

### Ejercicio 1
**Enunciado:** Pedir al usuario su edad y mostrar si puede conducir (mayor o igual a 18).

**Solución**
```python
edad = int(input('Edad: '))
if edad >= 18:
    print('Puedes conducir')
else:
    print('No puedes conducir')
```

## Bucle while
```python
contador = 1
while contador <= 3:
    print('Vuelta', contador)
    contador += 1
```

### Ejercicio 2
**Enunciado:** Juego de adivinar un número entre 1 y 5.

**Solución**
```python
secreto = 3
numero = int(input('Adivina: '))
while numero != secreto:
    numero = int(input('Intenta otra vez: '))
print('¡Acertaste!')
```

## Bucle for y listas
```python
frutas = ['manzana', 'pera', 'naranja']
for fruta in frutas:
    print(fruta)
```

### Ejercicio 3
**Enunciado:** Imprimir cada nombre de una lista precedido de "Hola".

**Solución**
```python
nombres = ['Ana', 'Luis', 'Marta']
for n in nombres:
    print('Hola', n)
```

## Condicional ternario
Permite expresar condiciones simples en una sola línea.
```python
edad = 20
resultado = 'Mayor' if edad >= 18 else 'Menor'
print(resultado)
```

### Ejercicio 4
**Enunciado:** Determina si un número es par o impar usando una expresión condicional.

**Solución**
```python
num = int(input('Numero: '))
print('Par' if num % 2 == 0 else 'Impar')
```

## For con range
La función `range()` facilita generar secuencias de números.
```python
for i in range(3):
    print('Iteración', i)
```

### Ejercicio 5
**Enunciado:** Calcula la suma de los números del 1 al 100 usando un bucle for.

**Solución**
```python
suma = 0
for i in range(1, 101):
    suma += i
print(suma)
```

## Break y continue
Palabras clave para controlar la ejecución de bucles.

### Ejercicio 6
**Enunciado:** Imprime los números del 1 al 10 pero detén el bucle al llegar a 7.

**Solución**
```python
for i in range(1, 11):
    if i == 7:
        break
    print(i)
```
