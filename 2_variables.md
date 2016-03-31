Como indicamos al principio, la programacion es la manipulacion o la transformacion de datos, pero los datos pueden ser volátiles y perder información por el camino.

Las variables son la forma en la que podemos **guardar los valores de esos datos, y acceder a ellos en cualquier momento**, asignandoles un nombre personalizado a dicho valor.

Para crear variables utilizamos un palabra clave ```var´´ seguida del nombre con el que queramos nombrar a ese valor:

```
var nombre;
// undefined
```

En este caso hemos creado una variable llamada ```nombre```, la consola nos devuelve "undefined", no es un error, es simplemente que la consola siempre imprime el valor devuelto por la expresion y en este caso la declaración de la variable no devuelve ningun valor.

Vamos a asignar un valor a la variable:
```
var nombre;
nombre = "Ivan";
console.log( nombre );
```

Mediante la igualación por asignación con el signo ```=``` lo que hacemos es asignarle al operador de la izquierda el valor de la derecha, de tal manera que ahora siempre que escriba en la consola ```nombre``` devolverá su valor, en éste caso "Ivan", podemos modificar ese valor tantas veces como queramos.

```
nombre = "Ana";
nombre = "Victoria";
nombre = "Miguel";
```

Incluso podemos cambiar el tipo de dato:

```
nombre = ["Ivan","Mejias"];
nombre = false;
```

Siempre conservará el ultimo valor que le hayamos asignado, y en la escritura de su valor ya no utilizamos la palabra reservada ```var```porque ya la hemos declarado anteriormente.

Reglas de las variables
----

- La variables son 'case sensitives', significa que son sensibles a mayusculas y minusculas de tal forma que si queremos acceder al valor de una variable que hayamos declarado anteriormente, tiene que ser con la misma nomenclarura con la que lo declaramos. Siguiendo el ejemplo anterior:

```
nombre = "Ivan";
console.log(Nombre) // undefined
console.log(nombre) // Ivan
```
- No podemos utilizar palabras reservadas o claves, por ejemplo:
for
var
do
in
if
else
break
continue
...

```
var continue = 1 // Error de sintaxis
```

- No puden comenzar por numero:
```
var 1nombre = "Ivan" // Error de sintaxis
```

Algunos ejemplos:
```
/**
 * Cuantos segundos hay en 3 horas?
 */
var segundos_por_minuto = 60;
var minutos_por_hora = 60;
var horas = 3;

var resultado_segundos = horas * minutos_por_hora * segundos_por_minuto;
console.log( "Hay " + resultado_segundos + " segundos en " + horas + " horas" );

/**
 * Cuantas horas son 86400 segundos?
 */

var segundos = 86400;
var resultado_horas = segundos / minutos_por_hora / segundos_por_minuto;
console.log( "Hay " + resultado_horas + " horas en " + segundos + " segundos" );
```



