---
title: learning python
date: 2026-08-29
tags: []
notebook: private-shiki-notes
links: []
template: null
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