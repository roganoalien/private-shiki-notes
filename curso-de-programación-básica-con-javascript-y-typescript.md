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
En todo lenguaje de programación, o al menos los relativamente modernos o que siguen siendo actualizados y mejorados tienen paquetes, librerías y frameworks escritos en ese lenguaje y por lo tanto tienen algún tipo de manejador de paquetes, en el caso específico de JavaScript npm que significa Node Package Manager, ya que venía incluído en NodeJS, y estos manejadores de paquetes se encargar de administrar y permitir la instalación de paquetes al igual que manejar las versiones de cada uno y una que otra actividad más. Actualmente existen varios manejadores de paquetes para javascript como bun, pnpm, yarn, etc.

Y qué es un manejador de paquetes? Pues fácilmente es una tecnología que se encarga de varias actividades entre las que están la resolución y gestión de dependencias, ejecución de scripts y tareas, gestión de espacio y caché, publicación y distribución y auditoría y seguridad de los paquetes. En otras palabras qué significa? se encarga de manejar cada paquete que necesitas, mantener seguros a los usuarios que lo utilizan o al menos avisar y pedir que instalen nuevas versiones, eliminar las versiones con vulnerabilidades, aprovechar cache, ayudarte con la ejecución y actividades como builds y ejecuciones necesarias para trabajar localmente y de mantener gestionadas todas las dependencias de esos paquetes. Por ejemplo: si tuvieramos un camión que reparte pan bimbo, como dependencia tiene a la gasolina y las llantas por lo que el paquete se encarga de que esas dependencias se mantengan disponibles y no dejen de trabajar. 

Y ya que saben que es un manejador de paquetes, qué es un paquete, una librería y un framework? bueno pues un paquete se podría decir que es el formato de distribución. Código empaquetado (con su metadata) listo para ser instalado, transportado y compartido mediante un manejador de paquetes. Puede contener una librería, un framework completo o simplemente una función "suelta". 

Una librería es código reutilizable con funciones específicas. Tu tienes el control ya que la llamas únicamente cuando la necesitas para resolver un problema puntual.

Y un Framework es una estructura base o esqueleto arquitectónico. Dicta cómo debes de organizar tu proyecto y cómo debe de fluir tu código y aplicación. El framework invierte el papel y es quien "te llama a ti", de cierta forma dicha, dictando un ciclo de vida y las reglas. Básicamente un framework bajo sus reglas y ciclo de vida muchas cosas suceden afuera del escenario que no ves y el mismo framework llama tu código en el momento que lo necesita. De estos existen muchos en JavaScript como React, Angular, Vuejs, Svelte, NextJS, Adonis, Express, Elysia, Hono, etc. 

Vamos a ver un ejemplo de cada uno y cómo funciona la instalación y demás. Para eso primero deberemos de instalar NodeJS en nuestro equipo. Ya que lo tengamos instalado comprobaremos de la siguiente forma abriendo la terminal de tu equipo. [Hacer pruebas de una librería, un paquete común y un framework. 

## HTML y CSS básico [video 10]
Como ya les mencioné, JavaScript fue hecho para funcionar dentro de un navegador únicamente o al menos así fue al principio. Pero no fue el único lenguaje pensado para funcionar en el navegador aunque sí el único lenguaje de programación disponible en el navegador en un inicio. Si pudieramos hacer referencia del cuerpo humano como el navegador, HTML serían los huesos del cuerpo y estos mantienen todo en su lugar y le da estructura al cuerpo, JavaScript son los músculos y organos que le dan funcionalidad y movimiento al cuerpo y CSS que es la piel y el cabello que le da visibilidad al cuerpo y define "la belleza". El único tema es que HTML y CSS no son lenguajes de programación y estoy hay que dejarlo muy claro... no són lenguajes de programación ya que no necesitan o requieren de una lógica para funciona, no hay funciones, condicionales, ciclos, etc. Hace unos años se inventaron los Pre-procesadores que le daban esa lógica y funcionalidad a CSS pero el CSS moderno dejó de necesitar esas reglas y funcionalidades extra y aún peor con la IA. HTML es el que casi no ha evolucionado desde la creación de HTML 5, lo siguen actualizando y le han agregado etiquetas y atributos de accesibilidad pero no ha tenido cambios tan importantes como JavaScript y CSS. Los 3 son "necesarios" para hacer funcionar un sitio web aunque el único realmente obligatorio es HTML pero los sitios modernos usan los 3 casi todos. 

Proceder a hacer un landing page muy sencillo.

## Qué son los tipos TypeScript [video 11]
Qué es TypeScript? Se define a sí mismo como JavaScript con sintaxis para tipos. Es básicamente una capa encima de JavaScript que necesita compilación de seguridad y organización. No seguridad del tipo que prevenga ataques, errores o intentos de hackeos sino de seguridad al escribir código. 

Imaginen que están construyendo una pared y JavaScript podría ser como agarrar un ladrido de un cuarto oscuro donde no ves qué tipo de ladrillo agarras podrías agarrar uno naranja pequeño o uno de piedra grande, si está hueco o relleno, o si simplemente echas cemento encima de todo. TypeScript es como si iluminaras ese cuarto y organizaras cada ladrillo en una parte del cuarto y le dieras una descripción de qué tipo de ladrillo es y cómo debería de usarse. Para que se lo puedan imaginar mejor hagamos un ejemplo con código.

```javascript
function saludo(nombre, edad) {
    if(edad < 18){
        console.log(`Hola ${nombre}, no tienes la edad para entrar!!`);
    }
    console.log(`Hola ${nombre}! Tienes la edad suficiente para entrar al sitio!`);
};
```

En ese ejemplo cuando llamemos la función y queramos meter los argumentos necesarios para la función cómo podríamos validar cuál argumento va primero o segundo? si el código lo escribió alguien más o es de una librería externa cómo sabrías si el error lo cometiste tú o el código que llamaste está mal? Cómo previenes eso? Pues con TypeScript, ahora hagamos el mismo ejercicio pero con TypeScript y veamos cómo cambia realmente:

```typescript
function saludo(nombre: string, edad: number):void {
    if(edad < 18) {
        console.log(`Hola ${nombre}, no tienes la edad para entrar!!`);
    } else {
        console.log(`Hola ${nombre}, puedes ingresar!`);
    }
}
```

Aparte de esto, añade nuevos tipos fuera de los de JavaScript que si recuerdan son string, boolean, number, bigInt, undefined, null y symbol. TypeScript nos agrega: any, unknown, never, void, tuplas([string, number]), enums e interfaces y types personalizados. 

## Nuestro primer sitio web [video 12]
Antes de iniciar y hacer un sitio de alguna forma moderna, lo haremos de la forma "viejita" que sigue siendo válida hoy en día pero no muy utilizada ya que necesita varias cosas de preparación y no podríamos asegurar la disponibilidad de archivos, no tendríamos algunos beneficios de servidor, forma de tal vez desplegar el código de forma moderna y alguna que otra cosa. Pero no por eso decir que no sirve aprender esto de forma viejita no tiene su utilidad. Así que haremos un sitio muy sencillo y simple como está la imagen que nos muestra dos páginas en su versión móvil y de escritorio y veremos cómo hacer el código responsivo. Trataré de usar cosas modernas de cada lenguaje pero manteniendo las cosas de la forma más clara y sencilla posible. Usaremos javascript para ver cómo entra este lenguaje de programación de forma sencilla en un sitio para darle cierta interacción y después veremos qué es un framework, qué beneficios nos da un framework de frontend, cómo utilizarlo y demás. Así que vamos a eso.

Posiblemente dividir en varias partes, dependiendo de que tan largo termine siendo.

## Usando un framework para crear un sitio web [video 13]
Ahora veremos qué es un framework, más o menos cómo funcionan, qué son los ciclos de vida, hooks, ventajas y desventajas de ciertas tecnologías, qué es un Single Page Application o SPA. Cómo funciona un manejador de paquetes, cómo usar la terminal, instalar paquetes y preparar el código para desplegarlo en línea de forma moderna y un poco al estilo viejo que se sigue aplicando pero no tla cual como lo haremos en esta prueba. Y lo que vamos a desplegar será el mismo sitio que construimos sin el framework y le daremos un poco más de interacción.

Posiblemente dividir en varias partes, dependiendo de que tan largo termine siendo.

## La terminal y funciones básicas [video 14] - Probablemente debería de ir antes del 13
Cómo usar la terminar, cómo navegar a través de ella, qué ventajas tiene, manejador de paquetes para Sistemas Operativos, y un poco de git de control de versiones, lo más básico y uso de dos o tres funciones. 

1. Navegar carpetas y directorios
2. Abrir archivos y carpetas
3. Copiar archivos, mover archivos y eliminar archivos
4. Crear archivos y carpetas
5. Permisos y cambios de permisos // muy leve
6. Uso de manejador de paquetes de sistema operativo y de nodejs
7. Git muy básico, qué es git y cómo inicializar un proyecto con git, revisar cambios y regresar cambios
8. Hacer scripts, ejecutarlos y cortarlos

## Nuestro primer programa de terminal [video 15] # Creador de notas
Crearemos un programa de la terminal para crear notas y acceder a ellos de forma temporal sin meternos a base de datos. Cómo funcionan los programas de terminal o cómo se ejecutan, argumentos, etc. 

## Nuestro primer servidor y qué es un API [video 16]
Sin usar un framework, crearemos un API muy sencillo y cómo funcionan en el navegador y cómo usar herramientas externas para interactuar con API's.

## Frameworks para el backend, qué es un backend [video 17]
Uso de Hono para crear el mismo API 

## Nuestra primer API [video 18]
Backend del Pokedex en forma de API

## Pokedex [video 19]

## Nuestra primer aplicación de escritorio con Electron [video 20] # Creador de notas

## Qué es un ORM [video 21]

## Base de datos no relacional [video 22]

## Base de datos relacional [video 23]

## Qué más podemos hacer con JavaScript y TypeScript? [video 24]