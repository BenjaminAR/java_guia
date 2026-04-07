# Programación orientada a objetos (POO)
La programación orientada a objetos no solo es una forma de escribir código, es una arquitectura para modelar la realidad (En un sistema de softare).

## Objeto
Es la unidad básica de la POO. si la clase es el molde para hacer el pan, el objeto seria el pan. En práctica un objeto es la instancia de una clase.
### Caracteristicas
- identidad: Cada objeto es único, incluso si sus atributos son iguales a otros; ejemplo: choche("Morado", "4 puertas") y otro igual choche("Morado", "4 puertas") estos dos tienen asignado un espacio de memoria diferente.
- Ciclo de vida: Un objeto nace (Se instancia con la palabra reservada `new`, vive mientras tenga un uso y muere (Trabajo automatico de *Garbage Collector* da java) cuadno ya no hay referencias a el.
- Interacción: Los objetos se cominican entre si invocando métodos unos de otros. 

---
## Pilares de POO.

| PILAR  | DEFINICION | PALABRA(S) RESERVADA |
| :--- | :--- | :---: | 
| Abtracción | Poceso de identificar las caracteristicas y comportamientos esenciales de un objeto SEGÚN EL CONTEXTO.  | `abstract` <br> `interface` |
| Encapsulamiento | Proteje los datos usando modificadores de acceso ( `private`, `protected`, `public` ).  | `Get` <br> `Set` |
| Herencia | Permite a un objeto padre heredar sus caracteristicas y comportamientos a una clase hijo  | `extends` <br> `super` |
| Polimorfiso | La capacidad de un objeto de tomar varias formas.  | `abstract` <br> `interface` |


