# Fundamento de JavaScript

![Banner JavaScript](/images/javascript-logo-banner.jpg)
---
## Contenido
 * ***En Proceso ...***
---

## Que es JavaScript

JavaScript es el lenguaje de programación mas utilizado para el desarrollo web (en conjunto con HTML, CSS).

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
 La notación que se usa para nombrar variables en JS es la "Camel Case".  

**Camel Case:**
Camel Case combina las palabras directamente, sin usar ningún símbolo, estableciendo que la primera letra de cada palabra esté en mayúscula a excepción de la primera palabra, estando el resto de letras en minúsculas. Este tipo de notación está muy extendida, siendo su uso muy común tanto en la declaración de variables como en el nombre de funciones y métodos.

Ejemplo: 
- La sintaxis de contar palabras en notación Camel Case sería ***contarPalabras***.
---

JavaScript es sensible a mayúsculas y minúsculas.

Ejemplo: **miNombre** ≠ **minombre**

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
#### Cadenas de texto

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





