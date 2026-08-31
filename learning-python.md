---
title: learning python
date: 2026-08-29
tags: []
notebook: private-shiki-notes
links: []
template: null
language: python
learning: 'true'
---

# Learning python

### Using three double commas
Using a triple `"` is used to define a multiline string

#### String
se maneja igual que en otros lenguajes

##### len
Len es el equivalente a `.length` de JavaScript pero se utiliza de otra forma:

```python
nombre_curso = "Ultimate Python"
len(nombre_curso)
```

Parece que las cadenas de texto, Python, las trata como si fuesen un array. Por ejemplo:
```python
nombre_curso = "Ultimate Python"
print(nombre_curso[0]) # devuelve U
print(nombre_curso[0:8]) # nos devuelve digamos que un rango del string 'Ultimate'
print(nombre_curso[9:]) # nos devuelve desde el indice 9 hasta el final pero tambien podemos poner un numero para un rango
print(nombre_curso[:8]) # esto asume el valor por defecto, igual que el anterior y devuelve lo mismo que el segundo print
print(nombre_curso[:]) # nos devuelve el string completo
```

##### Formato de strings
para poder hacer uso de interpolacion de variables en una string se hace de la siguiente forma

```python
nombre = "Rodrigo"
apellido = "Garcia"
nombre_completo = f"{nombre} {apellido}"
```

##### Metodos de strings

```python
animal = "perro feliz"
print(animal.upper()) # PERRO FELIZ
print(animal.lower()) # perro feliz
print(animal.capitalize()) # Perro feliz
print(animal.title()) # Perro Feliz
print(animal.strip()) # es parecido al trim y remueve todos los espacios en blanco al inicio y final del stirng
print(animal.lstrip()) # para quitar los espacios en blanco a la izquierda
print(animal.rstrip()) # igual que el anterior pero lo hace con los espacios de la derecha
print(animal.find("fel")) # buscamos caracteres y nos regresa el indice. Es sensible a si es mayuscula o minuscula. Si no encuentra devuelve un -1
print(animal.replace("perro", "gato")) # remplaza lo que encuentra por lo que pones como segundo argumento
print("fel" in animal) # hace algo similar a lo que hace .find() pero find devuelve el indice de donde lo encontro e IN devuelve un boolean si es que lo encuentra
print("gato" not in animal) # hace lo similar al in pero negando
```

#### Secuencias de escape
Basicamente poner caracteres especiales en un string como poner dobles comillas en un string `"Ultimate \"Python\""` o tambien `'Ultimate "Pyton"'`. Eso aplica como en cualquier otro lenguaje con `\n \\ \" \'`, etc.

#### Numeros
Se tienen dos tipos de numeros en python

```python
entero = 1 # int
decimal = 1.5 # float
imaginario = 2 + 2j # 2 + 2i // i es la raiz cuadrada de -1

print(1 / 3) # 0.3333
print(1 // 3) # 0 - no devuelve los decimales
print(8 % 3) # de la division devuelve el resto
print(2 ** 3) # para poner potencias
entero += 2 # se puede usar este metodo con multiplicacion, resta, division
entero -= 2
entero *= 2
entero /= 2
```

#### Modulo Math
Parecido al Math de JavaScript pero no se necesita usar la palabra reservada `Math`.

```python
print(round(1.3)) # redondear al numero mas cercano
print(abs(-77)) # 77 ... nos devuelve el valor absoluto, siempre devuelve un numero positivo
```

##### Math.py
Es el modulo nativo de Python parecido al de Javascript, los anteriores son las funciones por default sin el modulo. Tiene muchos metodos pero estos son los mas utilizados o "importantes".

```python
import math

print(math.ceil(1.1)) # nos lleva al numero entero hacia arriba
print(math.floor(1.9999)) # nos lleva al numero entero hacia abajo
print(math.isnan(23)) # para validar si es o no un numero, devuelve un boolean
print(math.pow(10, 3)) # nos ayuda a elevar un numero a la potencia de algo, el primer argumento es el numero y el segundo la potencia
print(math.sqrt(9)) # la raiz cuadrada
```

Para buscar todos los metodos de `math` esta en la pagina de documentacion oficial de python https://docs.python.org/3/library/math.html

#### Input de datos
Para obtener datos del usuario desde la terminal y guardarlo en una variable

```python
n1 = input("ingresa primer numero") # nos devuelve un string y habria que transformar a un numero
```

#### Conversion de tipos

```python
# int() - transforma en un numero entero
# str() - transforma en un string
# float() - transforma en un numero decimal
# bool() - transforma en un booleano // falsy nos da con un "", 0 o None
```

#### Comparadores logicos
Basicamente aplican todos en cualquier lenguaje de programacion `> < = != == >= <=`.

#### Condicionales

```python
edad = 22
if edad > 54:
    print("Puedes ver la pelicula con descuento")
elif edad > 17:
    print("Puedes ver la pelicula")
else:
    print("No puedes entrar")

print("Listo!")
```

#### Operador ternario
Como en JavaScript y otros lenguajes

```python
edad = 15

mensaje = "Es mayor de edad" if edad > 17 else "Es menor de edad"

print(mensaje)
```

#### Operadores logicos
And `and`, Or `or` and not `not`

```python
gas = True
encendido = True

if gas and encendido:
    print("La estufa esta prendida")

if gas or encendido:
    print("Puedes intentar prender la estufa o la estufa ya esta prendida")

if gas and not encedido:
    print("Puedes encender la estufa")
```

#### Operaciones de corto circuito
Basicamente lo que significa esto es que si tienes un if con un and y la primer variable es falsa, lo demas no se evalua y el or es que uno tiene que ser verdadero. 
#### Cadena de operadores

```python
edad = 25

# if edad >= 15 and edad <= 65 # basicamente es tomar esto y convertirlo en... (siguiente linea)
if 15 <= edad <= 65:
    print("puedes entrar")
```

#### For
Basicamente es lo mismo que javascript pero se escribe como un foreach de javascript

```python
for numero in range(5):
    print(numero)
```

##### For else
Sirve para salir del ciclo, para evitar seguir con el mismo usando `break`. El `else` es en caso de que el For o la busqueda de algo en el ciclo fracase.

```python
buscar = 3

for numero in range(5):
    print(numero)
    if numero == buscar:
        print("encontrado", buscar)
        break
else: 
    print("No encontre el numero que buscas")
```

#### While

```python
numero = 1

while numero < 100:
    print(numero)
    numero *= 2
----
comando = ""

while comando != "salir":
    comando = input("$ ")
    print(comando)
```

#### Funciones

```python
def hola():
    print("Hola mundo!")


def name(nombre, apellido):
    print(f"Hola {nombre} {apellido}")


def fecha(mes, dia=False): # parametro opcional
    if mes:
        print("Agosto")
    elif dia:
        print("29")


name(apellido="Garcia", nombre="Rodrigo") 
```

##### XARGS
Cuando necesitas pasar múltiples argumentos a una función, se vuelve el argumento iterable como si recibiese un arreglo.

```python
def suma(**numeros):
    resultado = 0
    for numero in numeros:
        resultado += numero
    print(resultado)


suma(2, 5, 7)
suma(2, 5)
suma(3, 8, 54, 89)
```

#### Return
Funciona exactamente igual que JavaScript y Go. Solo tengo que revisar si puede devolver un objeto o múltiples valores.

#### Variables globales
Se definen igual que en otros lenguajes como una variable normal pero si quieres acceder a ella dentro de una función o algo necesitas escribir la palabra reservada `global`

```python
saludo = "Hola Mundo"

def saludar():
    global saludo
    saludo "Hola Global"


saludar()
print(saludo) # debe de imprimir Hola Global
```

#### Tipos
Estos son los tipos de python:
- float
- int
- string
- boolean
- list (arreglos) [] tambien se pueden crear con la función `list()` dentro se debe de poner un rango o algo que se pueda iterar y crea esa lista. Por ejemplo: `list(range(0,10))` crea un arreglo con números del 0 al 9, siendo 10 elementos en total. `list("hola mundo")` crea un arreglo con cada caracter, incluido el espacio, del string.

##### "Desempaquetar" listas
Una forma rápida de ingresar el valor de cada indice de un arreglo a una variable se puede hacer de la siguiente forma:
```python
numeros = [1, 2, 3]
primero, segundo, tercero = numeros
print(primero, segundo, tercero) # nos dará como resultado 1 2 3

# para acceder al primer elemento de forma "python" se haría así:
primero, *otros = numeros
print(primero) # nos devuelve 1, usa la misma lógica del uso del * en una función para asignarle infinita cantidad de argumentos sin tener que definirlos. Se puede utilizar esto de *otros, de varias formas para obtener diferentes cosas como agregando después de *otros otro nombre de variable y almacenaría el último 
```

##### Iterar listas (arreglos)
```python
mascotas = ["Renato", "Chulita", "Lilo"]
for mascota in mascotas
    print(mascota) # Renato, Chulita, Lilo
```

Para acceder al indice del elemento se debe de hacer de la siguiente forma:
```python
for mascota in enumerate(mascotas):
    print(mascota) # (0, Renato) \n (1, Chulita) \n (2, Lilo) # esto se llama duplas que sería como un tipo de objeto
    print(mascota[0]) # nos devolvería el indice
    print(mascota[1]) # nos devolvería el nombre, por eso la dupla sale como (index, valor) ## (0, Renato)
```

Para utilizar lo de enumerate de una forma más eficiente y profesional se hace de la siguiente forma:
```python
for indice, mascota in enumerate(mascotas):
    print(indice, mascota) # nos devolverá cada elemento con el siguiente formato: 0 Renato
```
Para buscar un elemento dentro de una lista:
```python
print(mascotas.index("Lilo")) # nos devolvería el indice si es que lo encuentra: 2. En caso de no encontrar un elemento, devuelve un error lo que rompe el código  para corregirlo se hace así:

if "firulais" in mascotas:
    print(mascotas.index("firulais")) # para mostrar cuántas veces hace un match de lo que buscamos se debe de hacer como la siguiente línea:

print(mascotas.count("firulais"))
```