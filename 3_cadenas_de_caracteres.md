Las cadenas de caracteres o **Strings**, son como su propio nombre indica una secuencia de caracteres, que pueden ser letras, números, espacios ó signos de puntuación.

Las cadenas de caracteresm siempre van envueltas entre ```comillas```simples o dobles, es indiferente, pero siempre tiene que empezar y acabar con el mismmo tipo de comillas.

```
// formatos correctos
var nombre = 'Ivan';
nombre = "Ivan José";

// formato incorrecto
var nombre = "Ivan';
var artista = 'Sinead o'Connor';
```

Algunas operaciones con Strings
----
```
var saludo = "Hola mundo!!";
console.log(saludo);
```

Concatenar strings
----
```
saludo = "¡¡ Hola" + " mundo !!";
console.log(saludo);

var hola = "Hola";
var mundo = "mundo";
saludo = hola + mundo;
console.log(saludo);

saludo = hola + ' ' + mundo;
console.log(saludo);
```

Obtener la logitud de un String
----
```
// length
// devuelve la cantidad de caracteres del string
console.log( saludo.length );
```

Todos los caracteres a Mayúsculas
----
```
// toUpperCase()
// devuelve un nuevo string con string original en mayúsculas
var saludo_mayusculas = saludo.toUpperCase();
console.log( "toUpperCase: " + saludo_mayusculas );
```

Todos los caracteres a Minúsculas
----
```
// toLowerCase()
// devuelve un nuevo string con string original en minusculas
var saludo_minusculas = saludo.toLowerCase();
console.log( "toLowerCase: " + saludo_minusculas );
```

Sustituir una cadena de caracteres por otra
----
```
// replace([cadena a reemplazar],[cadena de reeplazo])
// devuelve un nuevo string reemplazando 'mundo' por 'Javascript'
var nuevo_saludo = saludo.replace('mundo', 'Javascript');
console.log( "replace: " + nuevo_saludo );
```

Extracción de caracteres de un String
----
```
// substr([indice de la cadena a extraer],[numero de caracteres a extraer])
// devuelve un nuevo string extrayendo 4 caracteres empezando por el caracter con indice 0 
var saludo_hola = saludo.substr(0,4);
console.log( "substr: " + saludo_hola );
// si el primer número es negativo comienza por el final del string
console.log( "substr (negativo): " + saludo.substr(-7,5) )	
```

Separar caracteres y devolver un array
----
```
// split([patron de separacion])
// devuelve un Array separando el string original por el patron (' ')
var saludo_array = saludo.split(' ');
console.log( "split: " + saludo_array );
```
