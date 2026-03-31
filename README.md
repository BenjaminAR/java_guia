# Guia de JAVA

## Tipos de datos básicos:
Los datos básicos de cualquier lenguaje de programacion son fundamentales para entender la forma correcta de almacenar y manipular la información los valores. Java es un lenguaje fuertemente tipado que distingue entre tipos primitivos (Datos simples) y tipos de referencia (Objetos complejos), Como Strings, Arrays o las propias clases que creamos. Conocerlos es fundamental para escribir código robusto y eficiente. Cada intruccion en JAVA se termina con punto y coma (;).

| NOMBRE | FAMILIA |PALABRA RESERVADA | SINTAXIS |
| :--- | :--- | :---: | :---: |
| Entero | Primitivo | int(32 bits) | 0 |
| Entero (byte) | Primitivo | byte (8 bits) | 0 |
| Entero (short)| Primitivo | short (16 bits) | 0 |
| Entero (long) | Primitivo | long (64 bits) | 0L |
| Flotante | Primitivo | float (32 bits) | 3.1416 |
| Flotante (double) | Primitivo |  doble (64 bits) | 3.1416 |
| Carácter | Primitivo | char | 'A' |
| Booleano | Primitivo | boolean | true/false |
| Cadena de texto | Objetos | String | "Hola" |
| Array | Objetos | tipo[] | { 1, 2 ,3 } |
| Lista | Objetos | List | `new ArrayList<>()` |
| Conjunto | Objetos | Set | `new HashSet<>()` |
| Mapa | Objetos | Map | `new HashMap<>()` |
| Clase (Objeto) | Objetos | NombreClase | `new Object()` |
| Nulo | Objetos | null (Ausencia de objeto) | `null` |

La sintaxis de JAVA es estructurada y orintada a objetos, heredada de gran parte de C++. Aquí encontrarás las estructuras fundamentales del lenguaje, como la definición de clases, condicionales, bucles, y métodos, junto con su respectiva sintaxis para escribir código claro y organizado.

| NOMBRE | PALABRA RESERVADA | SINTAXIS |
| :--- | :--- | :--- |
| Variable | tipo / var | tipo variable = valor <br> var variable = valor |
| Constante | final | final tipo constante = valor  | 
| Condicional if | if | if (condición) { } |
| Condicional else if | else if | else if (otra_condición) { } |
| Condicional else | else | else { } |
| Bucle for | for | for(inicialización; condición; incremento) { } |
| Bucle for each | for | for ( elemento : colección ) { } |
| Bucle while | while | while (condición) { } |
| Bucle do while | do while | do { } while (condición) |
| Switch | switch | switch (variable) { case valor: } |
| Función (método) | void / tipo | public void/tipoRetorno <br> nombreMétodo (parámetros) |
| Método principal | main | public static void main <br>(String[] args) { } |
| Clase | class | public class NombreClase { } |
| Sentencia break | break | break |
| Sentencia continue | continue | continue |
| Retorno | return | return valor |
| Paquete | package | package com.paquete |
| Importar | import | import java.util.List |
| Contructor | NobreClase | public NombreClase() { } |
| Instanciar objeto | new | new MiClase() |
| Excepciones | try, catch | try (...) catch (Exepción) {  } |
| Bloque finally | finally | finally { } |
| Lanzar excepción | throw | trow new Excepción |
| Declarar excepcón | throws | throws Excepción {  } |
| Comprobar instancia | instanceof | variable instanceof tipo |
| Acceder a superclase | super | super.metodoSuperclase() |
| Referencia a instancia | this | this.miVariable |
| ------ | MODIFICADORES DE ACCESO | ----- |
| Public | public | Acesible desde cualquier otra clase en cualquier paquete |
| Private | private | Accecible sólo desde la clase en la que fue declarado |
| protected | protected | Accesible desde el mismo paquete y subclase |
| default | (Sin palabra) | Por defecto. Accesible para las clases del mismo paquete. |

## Operadores:
Los operadores son símbolos que permiten eralizar cálculos y comprobaciones en Java. Se dividen en variascategorías:  
- Aritméticos (suma, resta ...).
- Comparación (mayor, menor, igual).
- Lógicos (&&, \|| , !).
- De asignación (=, +=).
- Bitwise.
- Operador ternario.


| NOMBRE | FAMILIA | SIMBOLO(S) | SINTAXIS |
| :--- | :--- | :---: | :---: |
| Suma | Aritméticos | + | A + B |
| Resta | Aritméticos | - | A - B |
| Multiplicación | Aritméticos | * | A * B |
| División | Aritméticos | / | A / B |
| Módulo (residuo) | Aritméticos | % | A % B |
| Incremento | Aritméticos | ++ | a++ ó ++a |
| Decremento | Aritméticos | -- | a-- ó --a |
| Iugual a | Comparación | == | A == B |
| Distito de | Comparación | != | A != B |
| Mayor que | Comparación | > | A > B |
| Menor que | Comparación | < | A < B |
| Mayor o igual que | Comparación | >= | A >= B |
| Menor o igual que | Comparación | <= | A <= B |
| AND | Operador Lógico | && | a && b |
| OR | Operador Lógico | \|\| | A \|\| B |
| NOT | Operador Lógico | ! | !a |
| Asignar | Asignación | = | x = 5 |
| Asig. con suma | Asignación | += | x += 7 |
| Asig. con resta | Asignación | -= | x -= 10 |
| Asig. con multiplicación | Asignación | *= | x *= 7 |
| Asig. con división | Asignación | /= | x /= 10 |
| AND bit a bit | Bitwise | & | a & b |
| OR bit a bit | Bitwise | \| | a \| b |
| XOR bit a bit | Bitwise | ^ | a ^ b |
| Desplaz. a la izq. | Bitwise | << | a << b |
| Desplaz. a la der. | Bitwise | >> | a >> b |
| Condicional ternario | O. Ternario | ? : | Condición ? <br> valorSiTrue : <br> valorSiFalse |

## Métodos / Funciones
En java, la funcionalidad está encapsulada en métodos (funciones) dentro de clases. La librería estándar proporciona calses con métodos  
muy útiles para tareas comunes, desde la manipulación de texto como `String` hasta operaciones matemáticas con `Math` o la iteracción con la consola a através de `System`
