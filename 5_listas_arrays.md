Son una lista de datos, pudiendo ser estos cualquier tipo de dato (String, Number, Boolean, null, incluso Array)

Se delara entre corchetes ([]), se separan los elementos que lo van a formar por comas (,)

```
[1,3,5,7,9]
["Lunes","Martes","Miercoles",4,null]
```

A cada elemento se le asigna un indice que se corresponde con el orden que ocupa en el Array, empezando a contar por el 0. El indice es siempre un número.

Accedemos a un elemento del array poniendo entre corchetes ([]) el indice (orden) que ocupa dentro del Array (Siempre empezando desde 0)
```
var elementos = ["H","Li","Na","K","Rb","Cs","Fr"];
elementos[0] // H
elementos[2] // Na

var indice_francio = 6;
elementos[indice_francio] // Fr
```

Algunas operaciones con Arrays
----

Logitud de un Array
---
```
elementos.length // 7
elementos[elementos.length-1] // Fr
```

Modificar el valor de un elemento del array
---
```
elementos[0] = "Hidrógeno";
```

Añadir Elementos al final de un Array
---
```
elementos.push('He');
elementos.push('Ne','Ar','Kr');
```

Extraer el ultimo elemento de un Array
---
```
elementos.pop();
// Kr
```

Añadir Elementos al inicio de un Array
---
```
var elementos = ["Rb","Cs","Fr"];
elementos.unshift("Li","Na","K");
elementos.unshift("H");
```

Extraer el primer elemento de un Array
---
```
var elementos = ["H","Li","Na","K","Rb","Cs","Fr"];
elementos.shift();
// H
```

Añadir / Extraer elementos de un Array en posiciones determinadas (modificando el array original)
---
```
// Añadir elementos 
var elementos = ["H","K","Rb","Cs","Fr"];
elementos.splice( 1, 0, "Li","Na");
// 1 -- Elemento donde se hará la insercion
// 0 -- Elementos a eliminar
// "Li","Na" -- Elementos a insertar

// Eliminar extrayendo elementos
var elementos = ["H","Li","Na","K","Rb","Cs","Fr"];
elementos.splice( 1, 2 );

```

Extraer elementos de un Array en posiciones determinadas (sin modificar el array original)
---
```
var elementos = ["H","Li","Na","K","Rb","Cs","Fr"];
elementos.slice(3);
// ["K", "Rb", "Cs", "Fr"]
elementos.slice(1,3);
// ["Li", "Na"]

// 1 -- es el elemento donde empieza la extraccion
// 3 (opcional) -- es el elemento donde acabará la extracción sin incluirlo
```

Juntar varios arrays
---
```
var elementos_1 = ["H","Li","Na"];
var elementos_2 = ["K","Rb","Cs"];
var elementos_3 = ["Fr"]
elementos_1.concat( elementos_2, elementos_3 );
```

Buscar la posicion de un elemento en el array por valor
---
```
var elementos = ["H","Li","Na","K","Rb","Cs","Fr"];
elementos.indexOf('Rb'); // 4
elementos.indexOf('Kr'); // -1

```