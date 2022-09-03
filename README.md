# poo

![alt text](http://url/to/img.png)

## ¿Qué resuelve la Programación Orientada a Objetos?

De la programacion estructurada tenemos una programación lineal, es decir, paso a paso.

Resuelve el código muy largo

Si algo falla, todo se rompía

Era difíl de mantener

La programacion estructurada causaba codigo espagueti, multiples if else

La POO busca simplificar la programación.

## Paradigma Orientado a Objetos

La orientación a objetos surge cuando tenemos que partir de los problemas que tenemos y necesitamos plasmarlos en codigos

Es decir, analizar un problema en forma d eobjeto para llevarlo a una solución de código

La POO es un paradigma, una forma de pensar, que compone de 4 elementos:

- Clases

- Propiedades

- Metodos

- Objetos

También tenemos:

- Encapsulamiento

- Abstracción

- Herencia

- Polimorfismo

![alt text](https://static.platzi.com/media/user_upload/platzi-ced1193b-4155-4723-a55d-3a346feb60fb.jpg)

![alt text](https://static.platzi.com/media/user_upload/%C2%BFQu%C3%A9%20es%20la%20Programaci%C3%B3n%20orientada%20a%20objetos_-ffb6955d-ae7d-4446-96e2-66f071517a77.jpg)

## Lenguajes Orientados a Objetos

Java

- Orientado a objetos naturalmente
- Android
- Server side
- .java

PHP

- Lenguaje interpretado por el servidor
- Pensado para la web
- .php

Python

- Diseñado para ser fácil de usar
- Multiples usos: Web, Server Side, Análisis de Datos, Machine Learning, etc.
- .py

Javascript

- Lenguaje interpretado
- Orientado a Objetos pero basado en prototipos
- Pensado para la web
- .js

## Diagramas de Modelado

Nos ayudan a entender el problema con ayuda de graficos, sirve de intermediario para entender el problema y aplicar la solución con la poo

Tenemos a OMT y UML

OMT - Object Modeling Techniques
Es una metodología para el analísis orientado a objetos. Luego de atribuir nombres, atributos y metodos a los objetos, deberíamos plasmarlos en un cuadro. Y con conectores definimos las relaciones de un objeto con otro.

UML - Unified Modeling Language
Tiene mas aplicaciones. Ahora cuentas con diagramas de clases, casos de uso, objetos, actividades, iteración, estados, implementación.

Implica:

- Especificar
- Construir
- Visualizar
- Documentar

Guia UML: <https://drive.google.com/file/d/1zLWH_tcEq_SuBHDA39094l4MX59DJKbz/view>

Herramienta UML: <https://www.lucidchart.com/pages/>

![alt text](https://staruml.io/image/screenshot_jumbotron.png)

## Que es UML

Las clases se representan así:

![alt text](https://static.platzi.com/media/user_upload/clase-1897e6cf-84b3-4432-926b-aff4fc4db122.jpg)

En la parte superior se colocan los atributos o propiedades, y debajo las operaciones de la clase. Notarás que el primer caracter con el que empiezan es un símbolo. Este denotará la visibilidad del atributo o método, esto es un término que tiene que ver con Encapsulamiento y veremos más adelante a detalle.

Estos son los niveles de **visibilidad** que puedes tener:

```py
- private
+ public
# protected
~ default
```

Una forma de representar las relaciones que tendrá un elemento con otro es a través de las flechas en UML, y aquí tenemos varios tipos, estos son los más comunes:

### Asociación

![alt text](https://static.platzi.com/media/user_upload/associacion-d2e1b691-b6e9-4854-85e2-d3ffdf0a9049.jpg)

Como su nombre lo dice, notarás que cada vez que esté referenciada este tipo de flecha significará que ese elemento contiene al otro en su definición. La flecha apuntará hacia la dependencia.

![alt text](https://static.platzi.com/media/user_upload/uml-relacion-asociacion-99b916c6-1f80-4b61-889a-ebf6e74f4f23.jpg)

Con esto vemos que la ClaseA está asociada y depende de la ClaseB.

### Herencia

![alt text](https://static.platzi.com/media/user_upload/herencia-2eb98d5e-bcad-4162-b236-aa87eba20e76.jpg)

Siempre que veamos este tipo de flecha se estará expresando la herencia.
La dirección de la flecha irá desde el hijo hasta el padre.

![alt text](https://static.platzi.com/media/user_upload/herencia-clases-53cb3117-def7-433f-adc5-4ad183d6b5e7.jpg)

Con esto vemos que la ClaseB hereda de la ClaseA

### Agregación

![alt text](https://static.platzi.com/media/user_upload/agregacion-6489d946-cc06-4e3c-a976-f6435531b4f2.jpg)

Este se parece a la asociación en que un elemento dependerá del otro, pero en este caso será: Un elemento dependerá de muchos otros. Aquí tomamos como referencia la multiplicidad del elemento. Lo que comúnmente conocerías en Bases de Datos como Relaciones uno a muchos.

![alt text](https://static.platzi.com/media/user_upload/uml-relacion-agregacion-adb20be8-d6c2-41d1-b002-2cfa37639240.jpg)

Con esto decimos que la ClaseA contiene varios elementos de la ClaseB. Estos últimos son comúnmente representados con listas o colecciones de datos.

### Composición

![alt text](https://static.platzi.com/media/user_upload/composicion-1da1dd19-6925-42d9-9727-7fd8cb031b0c.jpg)

Este es similar al anterior solo que su relación es totalmente compenetrada de tal modo que conceptualmente una de estas clases no podría vivir si no existiera la otra.

![alt text](https://static.platzi.com/media/user_upload/uml-relacion-composicion-2d4cb1fa-5422-44e3-849b-3a3e2d276733.jpg)

Con esto terminamos nuestro primer módulo. Vamos al siguiente para entender cómo podemos hacer un análisis y utilizar estos elementos para construir nuestro diagrama de clases de Uber.

![alt text](https://www.ionos.es/digitalguide/fileadmin/DigitalGuide/Screenshots_2019/klassendiagramme-uml-ES-9.png)

En la composición, el elemento Tree depende completamente del elemento Leaf, siendo el caso de que si el elemento Leaf desapareciera también lo haría el elemento Tree.

Mientras que en la agregación si el elemento Book desaparece, o se vuelve 0, (esto me imagino que lo explicarán más adelante) el elemento Book Shop no lo haría.

### Resumen Diagramas de clases

link : <https://www.youtube.com/watch?v=Z0yLerU0g-Q>

Una clase se referencia en un cuadro, en la seccion superior se escribe la clase (el tipo), una clase puede ser animales

A traves de atributos describes cada campos o propiedades de la clase, como nombre, ID, edad

Los atributos deben tener un formato, seaun string o un numero

En la sección inferior colocas los métodos, especificas el comportamiento de la clase. Por ejemplo funciones que cambien el nombre.
O del comportamineto de la propia clase, por ejm la clase animales, tiene una función de -comen()

Tenemos la visibilidad de atributos

```py
- privado
Ninguna otra clase o subclase puede acceder a ellos
+ publico
Cualquier otra clase puede acceder a ellos
# protegido
Solo la misma clase y subclases pueden acceder a eñños
~ paquete/defecto
Significa que el paquete puede usarse distitnas clases que esten en el mismo paquete
```

Los atributos serán privados y protegidos, los métodos serán publicos

En las relaciones se ahorra codigo. De una clase creamos subclases (como de la superclase Animales creamos las subclases tortugas, nutrias, loros)

Estableciendo una relacion de herencia, las subclases cuentan con los atributos de la superclase. Le puedes añadir tambien un atributo en especial a solo una subclase o a la clase derivada y que no las contengan las otras subclases. Pero si quieres añadir un nuevo atributo a todas las subclases, solo debes añadir un nuevo atributo a la superclase

Tenemos la abstraccion, la superclase suele ser una idea abstracta, la clase animal es una forma de simplificar el codigo, normalmente se pone en *cursiva*

Se puedes establecer relaciones especiales entre clases con un nombre. Esto es asociacion.

Agregacion, una clase puede formar parte de otra clase como un conjunto de estas (tortuga a tortugero), pero puede vivir fuera de esta, no depende de la clase grupal.

Composicion, las clases (o subclases) dependen de la clase mayor, no pueden vivir sin el objeto principal

Multiplicidad, definir el numero de clases u objetos por cada objeto mayor, como 1 o 1..*

## Objetos

Ante un problema tenemos que **identificar objetos**

> ⚠️ Un objeto es una instancia de una clase

Los objetos son aquellos que tienen propiedas y comportamientos y serán sustantivos, es decir, tendrán nombre. Podrán ser **físicos** o **conceptuales**. Algunos objetos conceptuales podrán tener comportamiento pero serán simbologías o ideas que no son tangenciales.

Por ejemplo un objeto User es un usuario físico. Pero un objeto conceptual como una sesión de usuario no es tangencial, pero tiene sus comportamientos y atributos. Una cuenta bancaria también es un objeto conceptual pero la tarjeta es uno físico.

Las **propiedades** o **atributos** también serán sustantivos como:

- nombre
- tamaño
- forma
- estado

Los **comportamientos** serán todas las **acciones de ese objeto**, son verbos, o son sustantivos en ocasiones. Por ejemplo:

- login()
- logout()
- makeReport()

Siempre estarán definidos un verbo y a lo máximo un sustantivo

Por ejemplo:

El objeto Perro.

Propiedades:

- nombre
- color
- raza
- altura

Comportamientos

- ladrar
- comer
- dormir
- correr

Analizando el contexto de los objetos. Imaginemos un sistema de adopciones. Con un catalogo de perritos disponibles para ser adoptados.
Ahora las propiedades cambiarían y los comportamientos también. Necesitamos un **id** para el perrito. Y necesitamos un comportamiento para el perrito en el contexto (en el sistema) de ser adoptado. Esta será **serAdoptado()**

Entonces ya no interesan los anteriores comportamientos del perrito, si ladra o come o duerme.

![alt text](https://static.platzi.com/media/user_upload/dog-2833b1ce-4289-447a-8cd0-7ad9b6f0da1a.jpg)

## Abstracción y Clases

Clase: Modelo creado a base de la abstracción de un Objeto

Abstracción: Proceso el cual separamos las caracteristicas de un objeto para generar un molde.

Entonces, una clase es el modelo sobre el cuall se construirá nuestro objeto. Las clases permitirán generar más objetos.

Es decir, analizamos objetos, obtenemos sus atributos y creamos las clases.

Y así las clases serán los modelos sobre los cuales crearemos aún más objetos

![alt text](https://static.platzi.com/media/user_upload/clip_image001-8ad14bdf-1124-4e5f-8815-650c61712dd8.jpg)

## Modularidad

Va acompañado del diseño modular. Es ecir subdividir un sistema en partes mas pequeña, modulos, que funcionarán en partes independientes y formarán un sistema complejo

Los asientos de un sofa pueden ser un modulo por ejemplo, puedes formar de 2 asientos, 3, 4, o hasta 8 asientos

> Divide y vencerás

Empieza a pensar y programar en pequeños trozos.

Una clase será lo que provoque la modularidad que permitirá analizar el problema. Separar objetos y de sus comportamientos y de otros objetos sin que este revuelto.

## Analiizando Uber en Objetos

Todo parte de una necesidad.

1. Usando uber, queremos trasladarnos desde un punto A hasta un punto B.
2. Luego solicitamos el auto en la aplicacion señalando el punta A hasta el punto B.
3. Habrán tipos de autos, Uber X, Uber pool, Uber Black, Uber Van. Y tenemos al driver (conductor).
4. El auto se dirigirá a nosotros y nos llevará del punta A al punto B. Al final de esto, se establecerá un monto o un saldo que será por el viaje.

Tenemos que analizar nuestros objetos. Tenemos:

- user
- route (ruta del punto A hasta el B)
- tipos de autos: uberx, uberpool, uberblack, ubervan
- driver
- pago: card, paypal, cash
- trip (viaje, objeto conceptual): quien ejecuta el viaje, a donde quieres ir, que auto elegiste, y el tipo de pago

Aproximadamente tendremos 11 objetos

## Clases en UML y su sintaxis en código

En UML, las clases se mostraran en un cuadro, conteniendo:

- Identidad
- Estado(atributos o propiedades)
- Comportamiento

Por ejemplo:
Person
name
walk()

Esto en distintos lenguajes se ve de esta manera:

Java:

```java
class Person{
  String name = "";
  void walk(){}
}
```

JavaScript:

```js
class Person {
  constructor() {
    this.name = '';
  }
  walk() {...}
}

//O
functionPerson(name = ''){
this.name = name;
}

Person.prototype.walk() = function(){
  //...
}
```

python

```py
class Person:
  name = ""
  def walk()
```

Java:

```php
class Person{
  $
}
```

## Modelando nuestros objetos Uber
 