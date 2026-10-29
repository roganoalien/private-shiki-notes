---
title: Curso de programación básica con JavaScript y TypeScript
date: 2026-10-29
tags: []
notebook: private-shiki-notes
links: []
template: null
---

# Introducción [video 1]
Primero que nada mi nombre es Rodrigo García y bienvenidos al curso básico de programación con JavaScript y TypeScript. Probablemente se preguntarán quién soy y qué o quién me da razón de ser para poder enseñar este curso y pues la respuesta más fácil y sencilla es la experiencia. Llevo más de 12 años como programador, he visto caer y crecer tecnologías, lenguajes de programación, herramientas y demás pero cuando empecé a programar todo era más "sencillo" y difícil a la vez, mi primer lenguaje de programación fue ActionScript 3 que era el lenguaje usado con Flash, el programa donde podías mezclar muy fácil código con animación y tener productos muy visuales. Y por su similitud, después me trasladé a JavaScript en el lado profesional, pero en la universidad aprendí a hacer videojuegos, hacer motodos gráficos con gl3, hice aplicativos, interfaces, emulaciones y demás. Cuando salí de la universidad entendí que no sabía absolutamente nada del mundo real de programación y empecé a aprender por mi cuenta WordPress, CSS, HTML, Php, servidores privados, conexiones ssh, git, jQuery y muchas otras cosas más. Mi prioridad fue el desarrollo frontend ya que yo venía del mundo visual, aunque aprendí sobre programación en la universidad mi carrera fue una licenciatura de Arte y Animación Digital, aunque de animación casi no aprendí nada. Por el momento no se preocupen por los términos que no entiendan, ya iremos resolviendo o viendo eso conforme avancemos. En ese entonces, la programación era la única profesión que se movía más rápido que la medicina, de la cual dicen que NUNCA terminas de estudiar... la programación es así pero comparado al día de hoy, decir que antes se movía rápido era como decir que antes caminabas y ahora tomas un tren para moverte de lugar. Después de varios años de especializarme en frontend mi perspectiva cambió, quería aprender a hacer desarrollos completos y más complejos por lo que empecé a aprender más sobre backend y por ese momento NodeJS ya estaba bien establecido en el mundo de desarrollo y era un lenguaje que ya conocía, con sus diferencias pero corriendo con JavaScript, luego aprendí sobre bases de datos no relacionales como MongoDB y luego me cambié a PostgresQL. Actualmente trabajo como líder de desarrollo para Aeroméxico en el área de Aeropuertos TI donde nos hacemos cargo de software que tiene que ver con la Operación pero específicamente con la operación de Aeropuertos, llevo 7 años trabajando aquí y, aunque llevo bastantes años tratando de hacer este curso, creo que ahora es el mejor momento. Intenté hacerlo antes cuando la IA no estaba tan bien posicionada y luego de la nada empezó a crecer muchísimo y hoy más que nunca creo que es necesario aprender a programar o saber programación básica aunque vayas a utilizar IA para "escribir código", no es lo mismo usar una herramienta de la que desconoces todo a usar una con un conocimiento bien establecido y funcional. Soy fiel creyente que aunque hagas vibe coding, aprender a programar y llevar ese conocimiento a un nivel más alto te llevará a crear herramientas 10 veces más funcionales, con muchos menos errores y sobre todo menos vulnerabilidades que es lo que más tienen todas estas aplicaciones vibe coded. También sabrás cómo darles mantenimiento, resolver errores e incluso darle instrucciones de cómo expandir y mejorar esas herramientas. 

## Bases de programación [video 2]
Todo en la programación es hecho con pensamiento lógico y con matemáticas. Una computadora necesita instrucciones para poder hacer lo que quieres que haga al igual que una IA, sin instrucciones es inservible y el lenguaje universal de las cosas son las matemáticas. Pero espera, no te espantes, no necesitas aprender matemáticas avanzadas o física. Con simples matemáticas y algebra básica puedes hacer casi de todo... los conocimientos avanzados de matemáticas y físicas sirven mucho mejor en investigación de campo, computación visual, videojuegos, creación y mejoras de IA, machine learning y otras áreas más. Para todo lo demás no necesitas matemáticas avanzadas pero sí necesitas mucha lógica. De echo, si decides continuar por este mundo tu forma de ver, pensar y resolver cosas cambiará por completo. Un programador no puede pensar en resolver algo y ya, por ejemplo: Tenemos un carro, al crearlo necesitamos hacer que avance y una vez que logremos hacer que avance no es la meta final sino un programador o ingeniero debe de saber que avanzar solo es el primer paso, también necesitaremos detenernos, ir en reversa, poder dar vuelta, indicarle a otros carros que vamos a dar vuelta o que nos detendremos y todo esto para evitar chocar y así es en la programación... debemos de pensar en que una herramienta podría ser explotada si no le ponemos límites pero esto vendrá con la experiencia y la práctica.

## Lenguaje de programación, qué es, para qué sirve y cuáles hay? y por qué hay tantos [video 3]
Antes de pasar a escribir código creo que es importante saber qué es un lenguaje de programación, sus funcionalidades y el por qué existen tantos. Al igual que un lenguaje como puede ser el español, inglés, alemán, japonés, etc. todos sirven para poder comunicarnos con alguien y ese alguien es el que cambia cuál lenguaje de programación necesitamos. Últimamente esta barrera de usar un lenguaje para algo en específico ha cambiado por completo, siendo el primero en ser de los más universales posibles JavaScript, sigue siendo verdad que usar el lenguaje correcto o ideoneo es el mejor camino para crear algo que corra rápido, sea más fácil de escribir y tenga más posibilidades. Puede no ser cierto en todos los casos pero en la mayoría es así. No necesitaremos aprender a escribir código binario que son 0s y 1nos, ese es el lenguaje de las computadores, el lenguaje de programación es como nos comunicamos con la computadora/tecnología o programa y este lo interpreta o en algunos casos el lenguaje necesita un proceso llamado build para ser traducido y empaquetado como un ejecutable o código binario. 

Cuáles son los lenguajes de programación más famosos y más utilizados:
1. Javascript / TypeScript
2. Python
3. Java
4. Php
5. Rust
6. C#
7. C++
8. Go
9. etc

Hay muchos más pero de estos escucharán más. Cada uno tiene sus fortalezas y debilidades e incluso enfoque pero nosotros nos enfocaremos en uno de los lenguajes más versátiles que hay que es JavaScript, mucha gente lo odia ya que al inicio era un lenguaje con mucha libertad, no era muy exigente o estricto, no necesita tipado (ya lo veremos más adelante), no exisían constantes y tampoco necesitabas importar muchas librerías o paquetes para hacer ciertas funcinalidades. TypeScript es un super set encima de JavaScript que necesita ser compilado el código para ejecutarse ya que JavaScript fue creado para funcionar especificamente en el navegador y como no necesitamos instalar nada en nuestras computadoras para poder ejecutar el código es en el lenguaje que nos enfocaremos... bueno sí necesitaremos instalar NodeJS para poder llevar nuestro conocimiento más allá pero en un inicio no lo necesitaremos.

## Types o Tipos | Primitivos [video 4]
Ahora veremos que son los types o tipos de contenido que podemos tener en los lenguajes de programación. Específicamente los que tiene JavaScript ya que dependiendo del lenguaje pueden cambiar el nombre y formato de estos. 

Pero para empezar qué son los primitivos? son los datos más básicos que no son objetos y no tienen métodos ni propiedades propias. Estos primitivos, en JavaScript, son: string (cadena de texto), number (número), boolean, undefined (no definido), null (nulo o ausente de valor), symbol son identificadores únicos que evita que choquen con otras propiedades de objetos, bigint (números enteros gigantescos).

También tenemos objetos que son una estructura mutable, que puede cambiar, de colección de datos basada en pares clave-valor. Las claves son siempre string o symbol. Los valores pueden ser de cualquier tipo (primitivo, función, array u otro objeto). Los array o arreglos son objetos especiales que tiene múltiples valores.

## Variables qué son y qué tipo de variables hay [video 5]
Las variables son formas de almacenar temporalmente, podemos imaginarla como una caja con nombre ( o una etiqueta) que creas en la memoria para guardar un valor y puedes consultar, usar o cambiar ese valor más adelante en tu código.

En todos los lenguajes, o casi todos, existen dos tipos de variables: las constantes y las variables. Las constantes son variables cuyo valor o asignación no se puede modificar o es inmutable y las variables cuyo valor puede ser reasignado en algún punto después de su definición y asignación inicial. 

En JavaScript usamos la palabra reservada `const` para definir a las constantes y `let` para las variables cuyo valor puede ser reasignado.

## Funciones y Scope [video 6]
Las funciones son un pequeño, de preferencia, bloque de código con nombre que puedes guardar en una variable o constante que puedes ejecutar y reutilizar las veces que sean necesarias. Pueden recibir parametros y específicamente en JavaScript pueden tener un callback que es otra función y opcionalmente puede devolver un resultado o nada (void). También tienen un contexto en el cual no indagaremos en este curso al menos que nos lleguemos a ver en la necesidad de revisarlo.

El Scope es el alcance que tiene cada bloque de código y que permite el uso de variables globales o temporales y es una de las cosas mas importantes conocer para evitar problemas con tu código.

## Condicionales [video 7]
Las condiciones son una forma de decir en el código que sí esto ocurre quiero que hagas lo siguiente y si no, haz esta otra cosa y se representa con las palabras reservadas `if`, `else` y `else if`. Podemos poner de ejemplo un sitio que vende alcohol, necesitas comprobar la edad del usuario que accede a tu sitio. Entonces le preguntas su edad y si responde que tiene 18 o más años... puede visitar el sitio pero si no los tiene aún entonces restringes su acceso. 

También tenemos lo que se llama un operador ternario y es un if else puesto en una línea `edad > 18 ? "puede ingresar" : "no puede ingresar";`.

Otra forma de ver una condicional es con un switch estatement: el switch es mejor utilizarlo cuando necesitas evaluar muchas posibilidades a la vez, por ejemplo un pokemon puede ser de agua, tierra, electricidad, fuego, etc. Entonces para no estar poniendo muchos if, else if y else usamos el switch statement: 

```javascript
const pokemon = {
    nombre: "Charizard",
    tipo: "fuego",
    ataque: 10,
};

switch (pokemon.tipo) {
    case "agua":
        console.log("Tipo agua");
        break;
    case "fuego":
        console.log("Tipo fuego");
        break;
    default:
        console.log("Tipo desconocido.");
        break;
};
```

## Ciclos [video 8]
Los ciclos son una forma de repetir código ya sea para ejecutar múltiples veces o buscar algo de forma iterante. Tenemos diferentes tipos de ciclos los cuales son:

for, foreach, while, do while.

```javascript
const pokemones = [
  { nombre: "Charizard", tipo: "fuego" },
  { nombre: "Blastoise", tipo: "agua" },
  { nombre: "Pikachu", tipo: "electricidad" }
];

for (let i = 0; i < pokemones.length; i++) {
  console.log(pokemones[i].nombre);
}

for (const pokemon of pokemones) {
  console.log(pokemon.nombre);
}

for (const propiedad in charmander) {
  console.log(`${propiedad}: ${charmander[propiedad]}`);
}

let i = 0;
while (i < pokemones.length) {
  console.log(pokemones[i].nombre);
  i++;
}

let j = 0;
do {
  console.log(pokemones[j].nombre);
  j++;
} while (j < pokemones.length);

// for each no es un loop tradicional sino un método que tiene un array. La diferencia es que no se puede usar un break ni nada para detenerlo ni saltarlo.
pokemones.forEach((pokemon) => {
  console.log(pokemon.nombre);
});
```

## Paquetes, librerías y frameworks [video 9]

## HTML y CSS básico [video 10]

## Qué son los tipos TypeScript [video 11]

## Nuestro primer sitio web [video 12]

## Usando un framework para crear un sitio web [video 13]

## La terminal y funciones básicas [video 14]

## Nuestro primer programa de terminal [video 15] # Creador de notas

## Nuestro primer servidor y qué es un API [video 16]

## Frameworks para el backend, qué es un backend [video 17]

## Nuestra primer API [video 18]

## Pokedex [video 19]

## Nuestra primer aplicación de escritorio con Electron [video 20] # Creador de notas

## Qué es un ORM [video 21]

## Base de datos no relacional [video 22]

## Base de datos relacional [video 23]

## Qué más podemos hacer con JavaScript y TypeScript? [video 24]