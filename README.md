# Front-End-M5-EP0
P1. Preguntas Teóricas sobre TypeScript (2 puntos)

1.1. ¿Qué es TypeScript y para qué se utiliza?
TypeScript es un superconjunto de JavaScript que añade tipado estático opcional. Esto significa que se pueden definir tipos de datos para las variables y funciones, lo que ayuda a detectar errores durante la compilación y mejora la legibilidad y mantenibilidad del código. 

1.2 ¿Cuáles son las principales diferencias entre TypeScript y JavaScript?
i. Tipado:
JavaScript: Es un lenguaje de tipado dinámico. Esto significa que el tipo de una variable se verifica en tiempo de ejecución. Una misma variable puede almacenar diferentes tipos de datos a lo largo del programa. Esto ofrece flexibilidad, pero también puede dar lugar a errores difíciles de rastrear.
TypeScript: Es un lenguaje de tipado estático. Los tipos de las variables se declaran explícitamente (o se infieren) y se verifican en tiempo de compilación. Esto ayuda a detectar errores antes de que lleguen a la fase de ejecución, mejorando la calidad del código y facilitando el mantenimiento.

ii. Detección de errores:
JavaScript: Los errores de tipo se detectan en tiempo de ejecución, lo que significa que pueden aparecer una vez que la aplicación está en producción y siendo utilizada por los usuarios.
TypeScript: Los errores de tipo se detectan en tiempo de compilación, lo que permite corregirlos durante el desarrollo y evitar sorpresas desagradables en producción.

iii. Escalabilidad:
JavaScript: Puede ser desafiante mantener y escalar proyectos grandes con JavaScript puro, especialmente cuando trabajan varios desarrolladores en el mismo proyecto, debido a la falta de tipado estático y la dificultad para refactorizar código sin introducir errores.
TypeScript: Facilita la creación y el mantenimiento de proyectos grandes y complejos gracias al tipado estático, las interfaces, las clases y otras características que mejoran la organización y la modularidad del código.

iv. Soporte de IDE:
JavaScript: Los IDEs ofrecen un soporte básico para JavaScript, con autocompletado y resaltado de sintaxis.
TypeScript: Los IDEs ofrecen un soporte mucho mejor para TypeScript, con autocompletado más preciso, navegación por el código, refactorización segura y detección temprana de errores.

v. Curva de aprendizaje:
JavaScript: Tiene una curva de aprendizaje inicial más suave, ya que es un lenguaje más sencillo.
TypeScript: Tiene una curva de aprendizaje inicial más pronunciada, ya que requiere aprender conceptos como tipado estático, interfaces, genéricos, etc. Sin embargo, a largo plazo, el esfuerzo se ve recompensado con un código más robusto y fácil de mantener.

vi. Compilación:
JavaScript: Se ejecuta directamente en el navegador o en un entorno de ejecución como Node.js.
TypeScript: Requiere un proceso de compilación para convertir el código TypeScript a JavaScript, que es el lenguaje que entienden los navegadores.

vii. Caracteristicas del proyecto:
JavaScript: Es recomendable para un proyecto pequeño y sencillo, que requiere prototipos rápidos y con importantes restricciones de tiempo para finalizar.
TypeScript: Es recomendable para un proyecto grande y complejo, que requiere un código más robusto y mantenible, el que se trabaja con un equipo grande y se valora la detección temprana de errores.


1.3. ¿Por qué es útil TypeScript en el desarrollo de aplicaciones ReactJS?
En el desarrollo de aplicaciones ReactJS, TypeScript ofrece las siguientes ventajas:
i. Detección temprana de errores: TypeScript ayuda a identificar errores de tipo durante el desarrollo, lo que reduce la probabilidad de encontrar errores en tiempo de ejecución.
ii. Mejora la legibilidad del código: La sintaxis de TypeScript, con la definición de tipos, facilita la comprensión del código y su mantenimiento.
iii. Mayor productividad: La detección temprana de errores y la mejora en la legibilidad del código contribuyen a un desarrollo más eficiente.
iv. Mejor autocompletado: Los IDEs ofrecen un mejor autocompletado con TypeScript, lo que agiliza el desarrollo.
v. Refactorización más segura: Los cambios en el código son más seguros con TypeScript, ya que el compilador ayuda a identificar posibles errores.
TypeScript es una herramienta muy útil para el desarrollo de aplicaciones ReactJS, ya que ayuda a mejorar la calidad del código, la productividad y la mantenibilidad.


1.4. ¿Qué es el sistema de tipos en TypeScript y cómo ayuda a evitar errores en tiempo de desarrollo?
El sistema de tipos de TypeScript es la característica central que lo diferencia de JavaScript. Se basa en la idea de añadir anotaciones de tipo al código JavaScript, permitiendo definir explícitamente el tipo de datos que se espera que contengan las variables, los parámetros de las funciones y los valores de retorno. Esta información sobre los tipos se utiliza durante el desarrollo para verificar la corrección del código y detectar errores antes de la ejecución.
i. Tipado estático:
TypeScript introduce el tipado estático, lo que significa que los tipos se verifican en tiempo de compilación, no en tiempo de ejecución como en JavaScript. Esto permite identificar errores de tipo antes de que la aplicación se ejecute en el navegador o en Node.js.

ii. Anotaciones de tipo:
Se utilizan las anotaciones de tipo para declarar el tipo de una variable. Por ejemplo:

let nombre: string = "Juan";
let edad: number = 30;
let esMayorDeEdad: boolean = true;

Donde,
-nombre: string indica que la variable nombre debe contener un valor de tipo cadena (string).
-edad: number indica que la variable edad debe contener un valor de tipo número (number).
-esMayorDeEdad: boolean indica que la variable esMayorDeEdad debe contener un valor de tipo booleano (true o false).

iii. Inferencia de tipos:
TypeScript también ofrece inferencia de tipos. Si no se declara explícitamente el tipo de una variable, TypeScript intenta inferirlo a partir del valor inicial que se le asigna. Por ejemplo:

let mensaje = "Hola mundo"; // TypeScript infiere que 'mensaje' es de tipo string
let contador = 0; // TypeScript infiere que 'contador' es de tipo number

iv. Tipos básicos:
-TypeScript soporta los tipos básicos de JavaScript:
-string: Cadenas de texto.
-number: Números (enteros y decimales).
-boolean: Valores lógicos (true o false).
-null: Valor nulo.
-undefined: Valor indefinido.
-symbol: Símbolos (introducidos en ES6).
-bigint: Enteros arbitrariamente grandes (introducidos en ES11).

Además, introduce tipos adicionales:
-any: Representa cualquier tipo. Se debe evitar su uso en la medida de lo posible, ya que anula las ventajas del tipado estático.
-void: Se utiliza para funciones que no devuelven ningún valor.
-never: Representa un tipo que nunca ocurre (por ejemplo, el tipo de una función que siempre lanza una excepción).
-unknown: Representa un valor desconocido. A diferencia de any, obliga a realizar comprobaciones de tipo antes de utilizar el valor.

v. Tipos más avanzados:
TypeScript también permite definir tipos más complejos:
-Interfaces: Definen la forma de un objeto.
-Clases: Permiten la programación orientada a objetos.
-Arrays: Arrays de un tipo específico.
-Tuplas: Arrays con un número fijo de elementos y tipos específicos para cada elemento.
-Enums: Conjuntos de valores con nombre.
-Genéricos: Permiten escribir código que puede funcionar con diferentes tipos.
-Tipos de unión: Permiten que una variable pueda tener uno de varios tipos posibles.
-Tipos de intersección: Combinan varios tipos en uno solo.

vi. ¿Cómo ayuda a evitar errores?
El sistema de tipos de TypeScript ayuda a evitar errores de las siguientes maneras:
-Detección temprana de errores: Al verificar los tipos en tiempo de compilación, TypeScript puede identificar errores como:
-Intentar sumar un número con una cadena.
-Llamar a un método que no existe en un objeto.
-Pasar un número a una función que espera una cadena.
-Mejora la legibilidad y el mantenimiento del código: La declaración explícita de tipos facilita la comprensión del código y su posterior mantenimiento.
-Facilita la refactorización: Al realizar cambios en el código, el compilador de TypeScript ayuda a identificar posibles errores que se hayan introducido.
-Mejora la experiencia de desarrollo: Los IDEs ofrecen un mejor autocompletado y sugerencias gracias a la información de tipos.

En resumen, el sistema de tipos de TypeScript es una herramienta poderosa que ayuda a escribir código más robusto, mantenible y con menos errores, mejorando significativamente la experiencia de desarrollo, especialmente en proyectos grandes y complejos.


---------------------------------
npm create vite@latest
cd m5-ep0
npm install
npm install typescript ts-loader webpack webpack-cli --save-dev
npm run dev

---------------------------------

Pregunta 2  -> archivo /services/DoctorAPI.ts
            -> página Equipo Médico
---------------------------------
Pregunta 3  -> archivo /objects/Doctor.ts
            -> página Equipo Médico

---------------------------------
Pregunta 4  -> app/EquipoMedicoPage.tsx
            -> components/Doctor*.tsx
            -> página Equipo Médico

---------------------------------
Pregunta 5 -> El resultado final es una version depurada de muchos errores que con Javascript pasan desapercibidos y con Typescript obligan a parchar y mejorar la implementacion. 
Por ejemplo en Equipo Médico Page, me encontre con errores con la variable data. En javascript si no parcho la posibilidad de que la variable este vacia, el codigo funciona bien, mientras la API responda. Esto decantó en esta version final en typescript sin alertas de potenciales errores.