# <p align="center"> TEST DE JAVASCRIPT ✌️👽🦖🦖</p>
> ### **¡Es hora de poner a prueba cuánto sabes sobre JavaScript!**
> Esta lectura es una prueba de JavaScript. A diferencia de un examen, nadie te obligará a nada. Puedes hacer trampa y saltar a la siguiente clase, ese es el camino fácil. Pero tengo mucha fe en ti, confío en que seguirás mis consejos y no avanzarás a la siguiente clase hasta superar esta prueba.
> ## Instrucciones para tomar esta prueba
> - Evalúa muy críticamente tu conocimiento.
> - Si logras resolver la prueba, no importa cuánto te cueste, puedo asegurarte que tienes todo para continuar a las siguientes clases y tomar el resto del curso.
> - Si no lo logras, no te preocupes, absolutamente nadie puede juzgarte, solo tú. Vuelve al Curso Básico de JavaScript, anota los temas clave donde puedes mejorar, ubica las clases donde puedes aprenderlos y estudia vigorosamente.
> - Es completamente válido hacer búsquedas en Google, cursos y tutoriales de Platzi, incluso usar tu cuaderno de notas sin importar si es físico o virtual.
> ### Recuerda que el éxito no se mide por cuánto tiempo te toma aprender, esa métrica es relativamente inútil.
> ### Mejor concéntrate en completar los cursos de tu ruta de aprendizaje profesional y desarrollar los proyectos que realmente demuestran que dominas cada tecnología.



## *<p align="center"> Variables y Operaciones </p>*


###  1️⃣ Responde las siguientes preguntas en la seccion de comentarios
1. ¿Que es una variable y para que sirve?

    Una variable es un espacio de almacenamiento identificado por un nombre (identificador) y asociado con un valor o información.
    Pueden contener diferentes tipos de información, como números, cadenas de texto, booleanos, objetos, entre otros.

2. ¿Cuál es la diferencia entre declarar e inicializar una variable?

    Declarar variable: Es especificar su existencia y su nombre, pero aun no se le asigna un valor.
    Inicializar: Es asignarle un valor por primera vez despues de declarla

3. ¿Cuál es la diferencia entre sumar números y concatenar strings?

    Sumar números: La suma se realiza cuando se tienen variables o valores numéricos, y el operador + se utiliza para agregar sus valores.
	  Concatenar strings: La concatenación se realiza cuando se tienen variables o valores de tipo cadena (string), y el operador + se utiliza para unir (concatenar) las cadenas.

4. ¿Cuál operador me permite sumar o concatenar?

    El operador utilizado es el signo +

### 2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

```jsx
// Nombre
	nombre = String

// Apellido
	apellido = String

// Nombre de usuario en Platzi
  usuarioPlatzi = String

// Edad
	edad = number

// Correo electrónico
	email = String

// Mayor de edad
	mayorEdad = boolean

// Dinero ahorrado
	ahorro = number

// Deudas
	deudas = number
```


### 3️⃣ Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.
	
```jsx
// Nombre
let nombre = "Fernando";

// Apellido
let apellido = "Montoya";

// Nombre de usuario en Platzi
let usuarioPlatzi = "fernandoMontoya_1506";

// Edad
let edad = 26; //

// Correo electrónico
let correoElectronico = "ferguapo@gmail.com";

// Mayor de edad
let esMayorDeEdad = true;

// Dinero ahorrado
let dineroAhorrado = 20;

// Deudas
let deudas = 1200;
```


### 4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

- Nombre completo (nombre y apellido)

```jsx
	let nombre = prompt("Digita tu nombre");
	let apellido = prompt("Digita tu apellido");

	console.log(`Tu nombre completo es ${nombre} ${apellido}`);
```

- Dinero real (dinero ahorrado menos deudas)

```jsx
  let ahorro = Number(prompt("¿Cuanto dinero tienes ahorrado?"));
  let deudaTotal = Number(prompt("¿Cuanto dinero debes actualmente?"));

  let dineroDisponible = ahorro - deudaTotal;
  if(dineroDisponible < 0 ) {
      alert("No tienes suficiente dinero para pagar tus deudas pronto seras embargado, lo lamento")
  } else {
      alert("Felicidades con lo que tienes ahorra te puedes quitar tus dedudas")
  }
```


## *<p align="center">Funciones</p>*


### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

1. ¿Qué es una función?

   Una función en programación es un bloque de código que realiza una tarea específica. Puede recibir datos (parámetros), realizar operaciones y devolver un resultado.

3. ¿Cuándo me sirve usar una función en mi código?

   Las funciones son útiles para organizar y reutilizar código. Puedes usar una función cuando necesitas realizar una tarea específica en varios lugares de tu programa. Esto mejora la legibilidad del 	código y facilita su mantenimiento.

4. ¿Cuál es la diferencia entre parámetros y argumentos de una función?
	
    - Parámetros: Son variables que se declaran en la definición de la función y representan los valores que la función espera recibir.
    - Argumentos: Son los valores reales que se pasan a la función cuando se llama. Los argumentos son los valores que se asignan a los parámetros cuando la función se ejecuta.

### 2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:


```jsx
function presentacion(completeName, nickname) {
    console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");
}

let nombre = prompt("Digita tu nombre");
let apellido = prompt("Digita tu apellido");
const completeName = nombre + " " + apellido;
const nickname = prompt("Digita tu nickname");

presentacion(completeName, nickname);
```


## *<p align="center">Condicionales</p>*


1️⃣ Responde las siguientes preguntas en la sección de comentarios:

1. ¿Qué es un condicional?

   Un condicional es una estructura de control en programación que permite ejecutar cierto bloque de código si se cumple una condición especificada. La ejecución del bloque puede variar dependiendo de si 	la condición es verdadera o falsa.
   
3. ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?

    **En JavaScript, hay varios tipos de condicionales:**
    - if: Se utiliza para ejecutar un bloque de código si una condición es verdadera.
    - else: Se combina con un if para ejecutar un bloque de código cuando la condición del if es falsa.
    - else if: Permite evaluar múltiples condiciones en secuencia.
    - switch: Se utiliza para seleccionar un bloque de código a ejecutar entre varios posibles casos.

4. ¿Puedo combinar funciones y condicionales?

    Sí, es posible combinar funciones y condicionales. Puedes llamar a funciones dentro de bloques condicionales o incluso definir funciones que contengan estructuras condicionales. Esto te permite 	modularizar y organizar tu código de manera efectiva.


### 2️⃣ Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

```jsx
const tipoDeSuscripcion = "Free";

if(tipoDeSuscripcion == "Free") {
    console.log("Solo puedes tomar los cursos gratis");
} else if (tipoDeSuscripcion == "Basic") {
    console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
} else if(tipoDeSuscripcion == "Expert") {
    console.log("Puedes tomar casi todos los curso de Platzi durante un año")
} else if(tipoDeSuscripcion == "ExpertPlus") {
    console.log("Tu y alguien mas pueden tomar TODOS los curso de Platzi durante un año")
} else {
    console.log("La maquina virtual no entiende tu respuesta");
}
```


### 3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).

```jsx

// Bonus: si ya eres una experta o experto en el lenguaje, te desafío a comentar cómo replicar este comportamiento con arrays u objetos y un solo condicional.

var suscripciones = [
    {tipo: "Free", mensaje: "Solo puedes tomar los cursos gratis"}, 
    {tipo: "Basic", mensaje: "Puedes tomar casi todos los cursos de Platzi durante un mes"}, 
    {tipo: "Expert", mensaje: "Puedes tomar casi todos los cursos de platzi durante un año"}, 
    {tipo: "ExperPlus", mensaje: "Tu y alguien mas pueden tomar TODOs los curso de Platzi durante una año"}, 
];
var valor = Number(prompt("Cual es tu plan: 1. Free, 2. Basic, 3. Expert, 4. ExperPlus"));
valor -= 1;
console.log(suscripciones[valor].mensaje);
```




## *<p align="center">Ciclos</p>*


### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

1. ¿Qué es un ciclo?

    Un ciclo, también conocido como bucle, es una estructura de control que permite repetir un bloque de código varias veces hasta que se cumple una condición específica.

2. ¿Qué tipos de ciclos existen en JavaScript?

    - for: Se utiliza cuando se conoce de antemano el número de iteraciones que se deben realizar.
    - while: Se ejecuta mientras una condición específica sea verdadera. Puede ejecutarse un número indefinido de veces.
    - do...while: Similar al while, pero garantiza que el bloque de código se ejecute al menos una vez, incluso si la condición es falsa desde el principio.

3. ¿Qué es un ciclo infinito y por qué es un problema?
   
    Un ciclo infinito es un bucle que nunca termina, ya que su condición siempre es verdadera. Esto puede causar que el programa se ejecute indefinidamente, consumiendo recursos y llevando a un rendimiento 	deficiente o incluso a un bloqueo del programa.

4. ¿Puedo mezclar ciclos y condicionales?
   
    Sí, es posible combinar ciclos y condicionales en JavaScript. Puedes utilizar estructuras condicionales dentro de bucles para controlar el flujo del programa según ciertas condiciones en cada iteración.




### 2️⃣ Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

```jsx
var x = 0;
while(x < 5) {
    console.log("El valor de x es: " + x);
    x++;
}

var y = 10;
while(y >= 2) {
    console.log("El valor de y es: " + y);
    y--;
}
```


### 3️⃣ Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

```jsx
var respuesta;
var intento = 1;
while(respuesta != 4){
    respuesta = Number(prompt("Cuanto es 2 + 2 intento numero: " + intento ));
    intento++;
}
console.log("Felicidades tu respuesta es correcta");
```


## *<p align="center">Listas</p>*


### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

1. ¿Qué es un array?

    Un array en JavaScript es una estructura de datos que permite almacenar múltiples valores bajo un solo nombre. Los elementos en un array están indexados numéricamente, comenzando desde cero.

2. ¿Qué es un objeto?

    Un objeto en JavaScript es una estructura de datos que permite almacenar datos de manera más compleja y estructurada. Los datos se almacenan en pares clave-valor, donde cada clave es única.

3. ¿Cuándo es mejor usar objetos o arrays?
    
    - Usa arrays cuando necesites una colección ordenada de elementos con índices numéricos y operaciones de lista, como agregar, eliminar o acceder a elementos por posición.
    - Usa objetos cuando necesites estructurar datos con propiedades identificadas por nombres (claves) y desees realizar operaciones más complejas sobre esos datos.

4. ¿Puedo mezclar arrays con objetos o incluso objetos con arrays?
    
    Sí, puedes mezclar arrays y objetos en JavaScript. Puedes tener arrays que contengan objetos como elementos, o puedes tener objetos que tengan propiedades que son arrays. Esto proporciona flexibilidad 	para representar y manipular datos de manera efectiva.
   

### 2️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

```jsx
var array = [1,2,3,4,5,6];

function retorno(array){
    console.log(array[1]);
}

retorno(array);
```

### 3️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

```jsx
const animales = ["pinguino", "leon", "chango"];

function recorrido(animales){
    for (const animal of animales) {
        console.log(animal);
    }
}

recorrido(animales);
```

### 4️⃣ Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).

```jsx
const persona = {
    nombre: "Fernando", 
    apellido: "Montoya", 
    apodo: "Chimal"
};
function recorrido(persona){
    for (const propiedad in persona) {
        console.log(propiedad + " " + persona[propiedad])
    }
}

recorrido(persona);
```

> ## ¿ Cómo te fue?
> ### ¡Felicidades por completar la prueba de JavaScript! Confío en que hayas completado cada paso y hayas pausado para repasar los temas de los ejercicios que se te complicaron.
> ### Ahora sí, continúa a la siguiente clase, pero recuerda que ya no puedes abandonar el curso, debes completarlo hasta el final. No importa cuánto tiempo te tome. Yo sé que tú puedes. Y tú deberías de saberlo también.





.


