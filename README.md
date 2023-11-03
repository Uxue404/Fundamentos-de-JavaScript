# Fundamento de JavaScript

![Banner JavaScript](/images/javascript-logo-banner.jpg)
---
## Contenido
 * ***En Proceso ...***
---

## Que es JavaScript

JavaScript es un lenguaje de programación multiplataforma orientado a objetos que se utiliza para hacer que las páginas web sean interactivas. Tambien hay versiones de JavaScript de lado del servidor más avanzadas, como Node.js que te permiten agregar más funcionalidad a un sitio web que simplemente descargar archivos. 

Usos de JavaScript: 
+ Frontend
+ Backend
+ Aplicaciones de Escritorio  

JavaScript es un lenguaje orientado a objetos (utiliza clases y objetos).

## Lenguajes Compilados vs Interpretados

- Un lenguajes compilado son convertidos en su totalidad a código maquina, y asi la computadora ejecuta el código.

- El lenguaje interpretado ejecuta línea a línea el programa. 


| Compilado | Interpretado |  
| --- |---|
|![Compilado](/images/Compilado.png) | ![Interpretado](/images/Interpretado.png) |  

Ejemplos de lenguajes Compilados vs interpretados:  
| Compilados | Interpretados |  
| --- | --- |  
| C | JavaScript|  
| C++ | Python |  
| Java | Ruby |


Hola mundo de JS:   
```js
console.log("Hola Mundo,soy Uxue y estoy aprendiendo JS");
```

## ¿Qué es una variable?

Una variable nos permite almacenar los datos de nuestros programas, las variables son volatiles osea se guardan y usan en la ram.  
Las variables se crean al instante abrir nuestro programa pero se destruyen al momento de cerrarlo.

Las variables se componen de:  
1. Nombre
2. Valor almacenado (Tipo de dato)
3. Dirección de memoria

Ejemplo: 

```js
var miVariables; // Ya no se usa "var"
let miOtraVariable = 100;
```

### Reglas para definir variables

 Debe de comenzar con: 
 * Una letra ( A - Z o a - z )
 * Un signo de dolar ( $ )
 * Con un guión bajo ( _ )

 Los caracteres siguientes pueden ser: 
 * Letras ( A - Z o a - z )
 * Dígitos ( 0 - 9 )
 * Guiones bajos ( _ ) 
 * Signo de dolar ( $ )

 Ejemplo 
 ```js
 let nombre;
 let miVariable1;
 ```
---
 La notación que se usa para nombrar variables en JS es la "`Camel Case`".  

**Camel Case:**
Camel Case combina las palabras directamente, sin usar ningún símbolo, estableciendo que la primera letra de cada palabra esté en mayúscula a excepción de la primera palabra, estando el resto de letras en minúsculas. Este tipo de notación está muy extendida, siendo su uso muy común tanto en la declaración de variables como en el nombre de funciones y métodos.

Ejemplo: 
- La sintaxis de contar palabras en notación Camel Case sería ***contarPalabras***.
---

JavaScript es sensible a mayúsculas y minúsculas.

Ejemplo: **miNombre** ≠ **minombre**


---
## Constantes

Una constante es una variable que una vez definido su valor, ya no se puede modificar.

Como buena práctica, el nombre de una constante se define en mayúsculas, y si tiene más palabras se separan con guión bajo ( _ ).
```js
const MI_CONSTANTE = 10;
console.log(MI_CONSTANTE); // 10

MI_CONSTANTE = 20; // Assigment to constant variable
```

---
## Comentarios en JavaScript

Los comentarios son ignorados en la ejecución del programa.

Se utilizan para explicar el código o para evitar ejecutar código.

Ejemplo: 
```js
// Comentario de una sola línea

/*
    Comentario de múltiples líneas
*/
```
---
## Tipos de datos

* number
* string
* boolean
* null
* undefined
* symbol
* bigint
---
### Números

Los números (tipo ***Number***) son los datos más básicos que podemos representar en JS,, no hay una diferencia entre números enteros y números decimales, todos los numero son de tip ***number***: 

```js
7
3.14
2.999e8
-122
-12.34
```

#### Operadores aritméticos

Con los números, puedes usar los **operadores aritmeticos** para realizar operaciones matemáticas. Te mostramos los siguientes operadores: 

* +: suma
* -: resta
* *: multipicación
* /: división
* %: módulo (reciduo de la división)
* **: exponente

Te mostramos un ejemplos del uso de operadores: 

```js 
2 + 2 // 4
4 - 2 // 2
3 * 2 // 6
2 / 2 // 1
2 % 2 // 0
3 ** 3 // 27
```

Al igual que las matemáticas, **las operaciones siguen un orden de precedencia.** Por ejemplo, si queremos sacar el resultado de ***2 + 2 * 3***, primero se multiplica ***2 * 3*** y luego se sumará ***2 + 6*** y su resultado sera ***8***. Pero tambien se puede usar paréntesis para cambiar el orden de las operaciones.

```js
2 + 2 * 3 // 8
(2 + 2) * 3 // 12
```
---
### Cadenas de texto

Las cadenas de texto (tipo **String**) es otro tipo de dato muy común. Las cadenas de texto se representan entre comillas simples, dobles o acentos graves.
 ```js
 "Esta es una cadena de texto con doble comilla"
 'Esta es una cadena de texto con comilla simple'
 ```

 Las comillas simples y dobles funcionan igual, pero al usar los acentos graves, se pueden escribir cadena de texto que ocupen varias lineas.

 ```js
 `Esto es una cadena de texto
 donde se ocupan varias linea, 
 y la cantidad de lineas que uses
 son a tu gusto`
 ```

##### Concatenación
Para poder unir dos o mas cadenas de texto, se usa el operador **+**: 
```js
"Hola, estamos aprendiendo " + "JavaScript !!" // Hola, estamos aprendiendo JavaScript !!
```

***Como puedes notar el operador `+` funciona de forma diferente dependiendo del tipo de dato que estemos usando***

___
### Booleanos
Los booleanos represneta sólo dos valores: `true` (verdadero) o `false` (falso). Por ejemplo: 
* ¿Está lloviendo (`true`) o no está lloviendo (`false`)?

### null y undefined

La particularidad de estos dos datos es que cada uno sólo tiene un valor. El tipo `null` sólo puede tener el valor `null` y el tipo `undefined` solo puede tener ese valor.

#### La diferencia entre estos dos

Mientras que `null` es un valor que significa que algo no tiene valor, `undefined` significa que algo no ha sido definido. Por ejemplo, si creamos una variable sin asignarle ningún valor, su valor sera `undefined`:
```js
let botella; // --> undefined
//Tambien se le puede asignar el valor undefined directamente
let botella1 = undefined; // --> undefined
``` 

En cambio, para que el valro de una variable sea `null` solo lo conseguiremos si lo asignamos directamente a la variable.

```js
let caguama = null;
```

Ejemplo visual para entender la diferencia entre ambas:

![ejemploNullUndefined](/images/null-undefined.jpg)

---
## Operadores de comparación

Estos tipos de operadores nos **nos permiten comparar dos valores**. Y estos siempren devuelven un valor booleano (`true` o `false`).

Por ejemplo podemos comparar siun numero es mayor que otro con el operador `>`, o si un numero es menor que otro con el operador `<`.

```js
5 > 3 // true
5 < 3 // false
```
Tambien tenemos los operadores `>=` y `<=` que nos permiten comparar si un número es mayor o igual que otro o viceversa.

```js
5 >= 3 // true
5 >= 5 // true
5 <= 3 // false
5 <= 5 // true
```
Para saber si dos valores son iguales se usa el operador `==`
```js
4 == 4 // true 
3 == 4 //false
'JavaScript' === "JavaScript" // true
'JavaScript' === `Java` // false
```

> Fíjate que puedes comparar cadenas de texto que usan comillas simples, dobles o acentos graves. Al final, siguen siendo cadenas de texto y lo importante es que sean iguales.

Para saber si los datos comparados son iguales en cuanto a contenido y a tipo de dato se usa el operador de estrictamente igual `===`. 
```js
5 === '5' // false
4 === 4 // true
"3" === '3' // true
```

Y para saber si los datos son desiguales se usa `!=` y `!==` para saber si es estrictamente desigual.
```js
console.log(5 !== 2); // true
console.log(2!='3'); // true
console.log(2 !== 2); // false
```

## Operadores lógicos

Los operadores lógicos en JavaScript ( y en otros lenguajes de programación) se utilizan para evaluar expresiones lógicas.

En JavaScript, hay tres operadores lógicos: AND (`&&`), OR (`||`) y NOT (`!`).

### Operador AND ( `&&` )

El operador *AND* se indica con `&&`. Devuelve `true` cuando ambos valores que conceca son `true`.

```js
true && true // → true
true && false // → false
false && false // → false
```

### Operador OR ( `||` )

El operador lógico *OR* se indica con `||` y devuelve `true` cuando cualquiera de los valores que conecta es`true`.

```js
true || true // → true
true || false // → true
false || false // → false
```

### Operador NOT ( `!` )

El operador lógico *NOT* se indica con `!` e invierte el valor de un valor booleano. Se pone delante del valor que queremos invertir.

```js
!true // → false
!false // → true
```

## Combinando operadores lógicos, aritméticos y de comparación

Los operadores lógicos y los operadores de comparación se pueden combinar para crear expresiones más complejas. Por ejemplo, podemos preguntar si un número está entre dos valores.
```js
2 < 3 && 3 < 4 // → true
```

## Operador typeof

Este operador `typeof` devuelve una cadena de texto que indica el tipo de un operando. Puede ser usado con cualquier tipo de operando, esto incluye a las variables y literales.

```js
let numero = 7
console.log(typeof numero); // "number"
```

El `typeof` tambien puede ser usado con los valores que quieras (booleanos, undifined, number, string).

Sin embargo, existe un valor especial en JavaScript, `null`, que es considerado un bug dentro del lenguaje. Si usamos **typeof** en un valor **null** no devolvera **"object"**.

```js
typeof null // "object"
```
Lo correcto seria que nos devolviera **null**, pero es un [error histórico que no se puede corregir sin romper el código existente.](https://2ality.com/2013/10/typeof-null.html)

Te doy algunos ejemplos de comparacion con el typeof:

```js
let age = 22;
console.log(typeof age == "number"); // true
```

## Estructuras de control

Las estructuras de control en programación son herramientas que te permiten dirigir el flujo de ejecución de un programa. Son como las instrucciones que le das a la computadora para que tome decisiones o realice acciones específicas basadas en ciertas condiciones.

### Código condcional con ***if***

El codigo condicional es un bloque de código que se ejecuta sólo si se cumple una condición. En JS la palabra reservada para crear un bloque condicional es el ***if***

Diagrama de flujo

![DF_IF](/images/If.png)

Sintaxis 

```js 
if (condición) {
  // código que se ejecuta si la condición es verdadera
}
```
Como vez en caso de que la condición se cumpla se ejecutara el bloque de códgio correspondiente, pero ¿Qué pasa si la condición es falsa? Para esto tenemos la siguiente palabra clave ***else***. La cual nos ayudara a ejecutar un bloque de código si la condición es falsa.

```js
const edad = 17
if (edad >= 18) {
  console.log('Eres mayor de edad')
} else {
  console.log('Eres menor de edad') // En este caso se ejecuta este bloque de código.
}
```

También podemos utilizar la palabra clave else if para comprobar más de una condición:

```js
let edad = 17

if (edad >= 18) {
  console.log('Eres mayor de edad')
} else if (edad >= 16) {
  console.log('Eres casi mayor de edad')
} else {
  console.log('Eres menor de edad')
}
```

El programa comprueba la primera condición. Si es true, ejecuta el código dentro del bloque ***if***. Si es ***false***, comprueba la siguiente condición. Si es ***true***, ejecuta el código dentro del bloque else ***if***. Si es ***false***, ejecuta el código dentro del bloque ***else***.

Dicho de otra forma, entrará en el primer bloque que cumpla la condición y no entrará en los demás. Si no cumple ninguna, entonces entrará en el bloque else.

#### Anidación de condicionales

Con todo lo anterior, es posible anidar condicionales dentro de otros condicionales. Te doy un ejemplo:

```js
const edad = 17
const tieneCarnet = true

if (edad >= 18) {
  if (tieneCarnet) {
    console.log('Puedes conducir')
  } else {
    console.log('No puedes conducir')
  }
} else {
  console.log('No puedes conducir')
}
```

Muchas veces vas a querer evitar la anidación inncesesario de caondicionales. ya que se hacen díficiñes de leer e incluso de mantener. Para estos casos es mejor usar operadores lógicos para crear la condición: 

```js
const edad = 17
const tieneCarnet = true

// si es mayor de edad y tiene carnet entonces...
if (edad >= 18 && tieneCarnet) {
  console.log('Puedes conducir')
} else {
  console.log('No puedes conducir')
}
```

La otra técnica que se usa es guadar el resultado de la condicion en una variable. 

```js 
const edad = 17
const tieneCarnet = true
const puedeConducir = edad >= 18 && tieneCarnet

if (puedeConducir) {
  console.log('Puedes conducir')
} else {
  console.log('No puedes conducir')
}
```

> Con esto podemos mejorar la lectura de nuestro código, a esta técnica se le conoce como ***refactorización*** y consiste en mejorar el código sin cambiar su comportamiento. 


### Ciclos

Un ciclo o un bucle nos permite repetir un bloque de código mientra la condicion sea verdadera.

* While
* Do while
* For

#### Ciclo `while`

```js
while (condicion){
  // Instrucciones a cumplir
}
```

Ejemplo, imprimir 5 veces mi nombre

```js 
let cont = 0;

while (cont < 5)
  {
    console.log("Hola Uxue");
    cont ++; // En este caso necesitamo incrementar cont para que cumpla la condicion si no permanecera en 0 y se hara un ciclo infinito.
  } 
```

