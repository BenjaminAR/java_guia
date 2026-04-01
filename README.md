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
| Array | Objetos | tipo[ ] | { 1, 2 ,3 } |
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

---

## Métodos / Funciones
En java, la funcionalidad está encapsulada en métodos (funciones) dentro de clases. La librería estándar proporciona calses con métodos  
muy útiles para tareas comunes, desde la manipulación de texto como `String` hasta operaciones matemáticas con `Math` o la iteracción con la consola a através de `System`

| NOMBRE | CLASE | OPERACIÓN |
| :--- | :--- | :--- |
| println() | `System.out` | Muestra texto o variables en la consola con un salto de línea. |
| equals() | Objetc | Compara si un objeto es igual a otro (A nivel de contenido). |
| toString() | Object | Devuelve una representación en texto del objeto. | 
| hashCode() | Object | Devuelve un código hash del objeto |
| length() | String | Devuelve la cantidad de caracteres de una cadena |
| charAt() | String | Devuelve el carácter en una posición específica. |
| substring() | String | Extrae una parte de una cadena. |
| toUpperCase() | String | Convierte una cadena en mayúsculas. |
| toLowerCase() | String | Convierte una cadena en minúsculas. |
| trim() | String | Divide una cadena en un array de subcadenas. |
| contains() | String | Comprueba si una cadena contiene una subcadena. |
| valueOf() | String | Convierte un tipo primitivo a su representación en String. |
| abs() | Math | Retorna el valor absoluto de un número. |
| sqrt() | Math | Calcula la raíz cuadrada. |
| pow() | Math | Calcula la potencia. |
| random() | Math | Genera un número aleatorio entre 0.0 y 1.0. |
| max() | Math | Devuelve el valor máximo entre dos números. |
| min() | Math | Devuelve el valor mínimo entre dos números. |
| round() | Math | Redondea al entero más cercano. |
| parseInt() | Math | Convierte una cadena a un doble |
| now() | LocalDate / LocalDataTime | Obtienela fecha o fecha y hora actual |
| of() | LocalDate / LocalTime | Crea una fecha/hora a partir de valores. |
| format() | DataTimeFormatter | Formatea una fecha/hora a una cadena. |

---

## Estructuras de datos.

En Java collections Framework (JCF) provee un conjunto de estructuras de datos. Las listas, conjunto y mapas son las interfaces principales, con implementaciones como _ArrayList, HashMap y HashSet_ que ofrecen distintas garantías de rendimiento y orden. Támbien existen el _Arrey_ como estructura primitiva.

| NOMBRE | OPERACIÓN | SINTAXIS |
| :--- | :--- | :--- |
| **---------** | **Arrays** | **---------** |
| length() | Obtiene el tamaño (propiedad) | array.length |
| **---------** | **Listas (Arrays)** | **---------** |
| add() | Agrege múltiples elementos | lista.add(valor) |
| add() | Inserta en una posición | lista.add(índice, valor) |
| get() | Obtiene un elemento por índice | lista.get(índice, valor) |
| set() | Modifica un elemento por índice | lista.set(índice, nuevo) |
| remove() | Elimina un elemento por índice | lista.remove(índice) |
| remove() | Eliminala primera ocurrencia | lista.remove(valor) |
| size() | Devuelve el tamaño | lista.size() |
| indexOf() | Devuelve el índice de un valor | lista.indexOf(valor) |
| clear() | Elimina todos los elementos | lista.clear() |
| contains() | Comprueba si existe el valor | lista.contains(valor) |
| **---------** | **Colecciones** | **---------** |
| sort() | Ordena un array o una lista | lista.sort() |
| filter() | filtra elementos según condición | lista.filter() |
| map() | Transforma cada elemento | lista.map() |
| **---------** | **Conjuntos (HashSet)** | **---------** |
| add() | Agrega un elemento (si no existe) | set.add(valor) |
| remove() | Elimina un elemento | set.remove(valor) |
| contains() | Comprueba si existe el valor | set.contains(valor) |
| size() | Devuelve el número de elementos | set.size() |
| isEmpty() | Commprueba si está vacío | set.isEmpty() |
| clear() | Elimina todos los elementos | set.clear() |
| **---------** | **Mapas (HashMap)** | **---------** |
| put() | Inserta/actualiza un par clave-valor | mapa.put(clave, valor) |
| get() | Obtiene el valor de una clave | mapa.get(clave) |
| remove() | Elimina el par de una clave | mapa.remove(clave) |
| constainsKey() | Comprueba si existe la clave | mapa.constainsKey(clave) |
| KeySet() | Devuelve un `set` de las claves | mapa.keySet() |
| values() | Devuelve una colleccion de valores | mapa.values() |
| entrySet() | Devuelve un set de pares clave-valor | mapa.entrySet() |
| size() | Devuelve el número de pares | mapa.size() |
| clear() | Elimina todos los pares | mapa.clear() |

---

## Manejo de archivos
Java ofrece un potente sistema de **manejo de archivos** a través de los paquetes java.io (clásico , basadi eb streams) y java.nio (moderno, más eficiente) Es recomendable usar el bloque _try-with-resourse_ para asegurar que los ficheros se cierren automáticamente.

| NOMBRE | REPRESENTACIÓN | SINTAXIS |
| :--- | :--- | :--- |
| **---------** | **Moderno (java.nio)** | **---------** |
| readString() | Lee todo el contenido a un String | Files.readString(path) |
| readAllLines() | Lee todas las líneas a una List | Files.writeString(path) |
| writeString() | Escribe un string en un archivo | Files.writeString(path) |
| exist() | Comprueba si un archivo existe | Files.exist(path) |
| creteDirectory() | Crea un directorio | Files.createDirectory(p) |
| delate() | Elimina | Files.delete(path) |
| **---------** | **Clásico (java.io)** | **---------** |
| FileReader | Lee un archivo de texto | new FileReader(File) |
| BufferedReader | Lee texto en una forma eficiente | new BufferedReader(reader) |
| readLine() | Lee una línea | BufferedReader.readLine() |
| FileWriter | Escribe en un archivo | new FileWriter(file) |
| BufferedWriter | Escribe texto de forma eficiente | new BufferedWriter(writer) |
| write() | Escribe una cadena | bufferedWriter.write(text) |

---
## Paquetes estándar
Java cuenta con una **Biblioteca de cales estándar (API)** muy extensa, organizada en paquetes (_packages_). Estos paquetes proveen funcionalidades listas para usar sin necesidad de instalar librerias externas, desde colecciones y concurrencia hasta redes y acceso a base de datos, Algunaos aquí :arrow_down:

| NOMBRE | DESCRIPCIÓN | 
| :--- | :--- |
| `java.lang` | Paquete fundamental, importado automáticamente. <br> contiene Object, String, System, Math y las clases envortorio (integer, Double). |
| `java.util` | Contiene el collections framework(List, Map, Set), clases de utilidad como Scaner, Random, Optinal y Objects. |
| `java.nio` | Nueva API I/O (NIO), ofrece manejo de archivos y redes de alto rendimiento, con buffers y canales. |
| `java.time` | API moderna y completa para el manejo de fechas, horas, duraciones e instantes. Sustituye a la antigua java.util.Date |
| `java.net` | Proporciona calses para la programación de red, como Socket, URL, URLConnection para crear clientes y servidores. |
| `java.math` | Ofrece clases para cálculos matemáticos. |
| `java.util.stream` | La API de streams, que permite un prosesamiento de datos de estilo funcional (declarativo) sobre colecciones. |
| `java.sql` | API de JDBC para interactuar con base de datos relacionales mediante sentencias SQL. |
| `javax.swing` | Framwork para crear interfaces gráficas de usuario (GUI) de escritorio, Ha sido en gran parte secedido por JavaFX |
| `javafx.*` | Framework moderno para crear aplicaciones de escritorio enriquecidas y multiplataforma. Es el sucesor de Swing |

---

## Librerias y frameworks externos

El ecosistema de Java es inmenso. Para gestionar dependencias y contruir proyetos, se usan herramientas como **Maven** o **Gradle**. Estas permiten incorporar **Librerías** y **frameworks** que extienden las capacidades del lenguaje para todo tipo de aplicaciones.

| NOMBRE | DESCRIPCIÓN | 
| :--- | :--- |
| `Spring` | El framwork más popular para crear aplicaciones empresariales robustas y escolares, especialemente con spring boot para mricroservicios y web |
| `Hibernate` | Framework de mapeo Objeto-relacional (ORM) que simplifica la interacción con base de datos SQL al trabajar con objetos java. |
| `JUnit` | El estándar para realizar pruebas unitarias en java |
| `Apache Commons` | Conjunto de librerias con utilidades reusables para operaciones con cadenas, coleccionesm I/O, etc |
| `Quarkus` ó `Micronaut` | Frameworks modernos y ligeros, optimizados para microservicios, serverless y compilación nativa con GraalVM |
| `SLF4J` ó `Logback`| Fachada de logging(SLF4J) y una implementación (Logback/Log4j2) para un registro de eventos flexible y potente. |
| `Apache` ó `Kafka` | Anuqe es una plataforma de mensajería  y trasmisión de datos, sus clientes java son esenciales para construir sistemas de streaming de eventos en tiempo real. |


