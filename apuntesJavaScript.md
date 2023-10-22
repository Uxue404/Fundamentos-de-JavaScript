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

- el lenguajes interpretado ejecuta línea a línea el programa. 


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

* Number: Almacena valores numericos.  
Ej. 10, -40, 3.9, -15.9
* String: Almacena cadenas de caracteres  
Ej. "Hola", 'Adios', \`Saludos`

* Boolean: Almacena un valor logico  
Ej. **true** o **false**

* Null: Ausencia de la referecnia de un objeto  
Ej. ***Null***

* Undefined: Ausencia de valor  
Ej. ***undefined***






