Los booleanos son un tipo de dato simple cuyo valor varía entre verdarero ó falso.
En javascript esos dos valores son ```true```y ```false```.

```
var viernesMolan = true;
var anyoBisiesto = false;
```

Operadores Lógicos
----

De la misma manera que hemos realizado operaciones matemáticas con números podemos realizar operaciones lógicas con Booleanos.

&& -- Operador AND
---

El valor de los dos booleanos debe ser igual a true, es decir deben cumplirse las dos condiciones:
```
var tiene_gafas = true;
var tiene_pelo_largo = true;

tiene_gafas && tiene_pelo_largo
// true
```

|| -- Operador OR
---

Al menos el valor de uno de los dos booleanos debe ser igual a true, es decir debe cumplirse, al menos una de las dos condiciones:
```
var tiene_gafas = true;
var tiene_pelo_corto = false;

tiene_gafas || tiene_pelo_corto
// true
```

! -- Operador NOT
---

Cambia el valor de true a false o de false a true:
```
var tiene_pelo_largo = false;
!tiene_pelo_largo
// true
```

Combinando operadores lógicos
----
Al igual que con los operadores matemáticos podemos combinar los operadores lógicos, teniendo en cuenta que ñestos se agrupan de dos en dos

```
var tiene_pelo_corto = false;
var tiene_gafas = true;
var ensenya_javascript = true;
var ensenya_dibujo = false;
var es_ivan = !tiene_pelo_corto && tiene_gafas && (ensenya_javascript||ensenya_dibujo);
console.log(es_ivan);
```

Operadores de Comparacion
----

> (Mayor que)
< (Menor que)
>= (Mayor o igual que)
<= (Menor o igual que)
== (Igual a)
!= (Distinto a)

podemos realizar operaciones de comparacion sobre números
```
var limite = 100;
var valor = 80;

valor > limite // false
valor < limite // true
valor >= limite // false
valor <= limite // false
valor == valor // true
valor != limite // true
```

podemos realizar operaciones de comparacion sobre strings

```
var saludo = "Hola";
var otro_saludo = "hola";

saludo == otro_saludo; // false
saludo != otro_saludo; // true;
```

Operadores estrictos
---
Cuando comparamos valores de distinto tipo y necesitamos saber si em valor coincide en valor y tipo utilizaremos los comparadores estrictos

=== (igual a)
!== (distinto a)

```
var numero = 22;
var edad = "22";

edad == numero // true
edad === numero // false

```
