# Día 2 - Condicionales y Bucles

Continuamos con estructuras de control y repetición.
A cada concepto le sigue un ejercicio práctico y su solución.

## Condicionales
Permiten que el programa tome decisiones. Es como preguntar "¿puedo entrar?" y
actuar según la respuesta.
```python
edad = 20
if edad >= 18:
    print('Mayor de edad')
else:
    print('Menor de edad')
```

### Ejercicio 1
**Enunciado:** En un juego de carreras necesitas saber si el jugador puede condu­dr. Pide su edad y muestra si tiene permiso (18 o más).

Pasos sugeridos:
1. Solicita la edad con `input()`.
2. Usa `if` para comparar con 18.
3. Muestra el mensaje correspondiente.

**Solución**
```python
edad = int(input('Edad: '))
if edad >= 18:
    print('Puedes conducir')
else:
    print('No puedes conducir')
```

## Bucle while
Repite instrucciones mientras una condición sea verdadera, como seguir
dando vueltas a la manzana hasta que te canses.
```python
contador = 1
while contador <= 3:
    print('Vuelta', contador)
    contador += 1
```

### Ejercicio 2
**Enunciado:** Has escondido un tesoro en un número secreto entre 1 y 5. Pide
al jugador que adivine hasta acertar.

Divide la solución en pasos:
1. Define el número secreto.
2. Pide un número con `input()`.
3. Mientras sea distinto al secreto, vuelve a preguntar.

**Solución**
```python
secreto = 3
numero = int(input('Adivina: '))
while numero != secreto:
    numero = int(input('Intenta otra vez: '))
print('¡Acertaste!')
```

## Bucle for y listas
Permite recorrer una secuencia elemento por elemento, como revisar una lista de
compras y leer cada producto.
```python
frutas = ['manzana', 'pera', 'naranja']
for fruta in frutas:
    print(fruta)
```

### Ejercicio 3
**Enunciado:** Tienes una lista de invitados a una fiesta. Saluda a cada uno
mostrando su nombre precedido de "Hola".

Sigue estos pasos:
1. Recorre la lista de invitados con un `for`.
2. Muestra el saludo para cada nombre.

**Solución**
```python
nombres = ['Ana', 'Luis', 'Marta']
for n in nombres:
    print('Hola', n)
```

## Condicional ternario
Permite escribir una decisión corta en una sola línea, como escoger rápidamente
entre dos opciones.
```python
edad = 20
resultado = 'Mayor' if edad >= 18 else 'Menor'
print(resultado)
```

### Ejercicio 4
**Enunciado:** Imagina un robot que debe decidir si gira a la izquierda o a la
derecha según si el número es par o impar. Usa una expresión condicional para
mostrar "Par" o "Impar".

Pasos:
1. Pide un número.
2. Usa el operador módulo (`%`) para comprobar si es par.
3. Muestra el resultado con el condicional ternario.

**Solución**
```python
num = int(input('Numero: '))
print('Par' if num % 2 == 0 else 'Impar')
```

## For con range
La función `range()` facilita generar secuencias de números. Es como tener
una cinta métrica que marca cuántas veces repetirás una acción.
```python
for i in range(3):
    print('Iteración', i)
```

### Ejercicio 5
**Enunciado:** Imagina que estás contando monedas desde el 1 hasta el 100. Usa
un bucle `for` para obtener el total.

Pasos sugeridos:
1. Inicia una variable para acumular la suma.
2. Recorre los números del 1 al 100 con `range()`.
3. Ve sumando cada valor.

**Solución**
```python
suma = 0
for i in range(1, 101):
    suma += i
print(suma)
```

## Break y continue
Palabras clave para controlar la ejecución de bucles: `break` detiene la
repetición y `continue` pasa a la siguiente vuelta.

### Ejercicio 6
**Enunciado:** Estás subiendo escalones numerados del 1 al 10, pero te detienes en
el escalón 7. Imprime cada número hasta ese punto.

Plan de solución:
1. Recorre los números del 1 al 10 con un `for`.
2. Usa `break` para salir cuando el contador llegue a 7.

**Solución**
```python
for i in range(1, 11):
    if i == 7:
        break
    print(i)
```
