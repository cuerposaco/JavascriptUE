Variables
==

Una variables es un lugar donde se guardará, en ocasiones un contenido y en otras una referencia que apunta a un contenido.

Las variables se declaran por primera vez con la palabra reservada ```var``` y luego se iguala al valor que se le quiera asignar:

```
var saludo = "Hola Unidad Editorial!!!";
console.log(saludo);
```

Si no se declara con ```var``` la variable ocupara el espacio "global", que es el nivel superior donde se ejecura el código.

```
saludo_global = "Hola desde el espacio global!!!";
console.log(window.saludo_global);
```

Tipos de Variables
==

En javascript todo es un "Objeto", pero de distintos tipos.

```
Object.prototype.toString.call(123)
> "[object Number]"

Object.prototype.toString.call(123.2)
> "[object Number]"

Object.prototype.toString.call("123")
> "[object String]"

Object.prototype.toString.call(true)
> "[object Boolean]"

Object.prototype.toString.call([1,2,3])
> "[object Array]"

Object.prototype.toString.call({})
> "[object Object]"

```
Tipos
==
- **Strings** : Cualquier valor encerrado **entre comillas (dobles o simples). Son literales de texto.
``` 
var string_var = "variable de ejemplo";
var string_var_simple = 'variable de ejemplo';
var string_var_mix = 'Aquí queremos usar "comillas" porque es un texto "destacado"';
```
- **Numbers** : Son valores numéricos, enteros, decimales, ... Al contrario que con los Strings **no se entrecomillan**.
``` 
var entero = 123;
var decimal = 3.1416;
var negativo = -123;
```
- **Boolean** : Sólo tiene dos valores, verdadero o falso **( true / false )**
```
var es_correcto = true;
var usuario_logado = false;
```
- **Arrays** : Es una **colección de objetos** del mismo tipo o de tipos distintos, encerrados entre **corchetes** y separados por **comas**
```
var fibonacci = [0, 1, 1, 2, 3, 5, 8, 13, 21, 34];
var miscelanea = ["Hola", false, 1.2, 1.3, "1.5", true];

// Acceso a un elemento de un array
// array[orden_que_ocupa_el_elemento_en_el_array]
// el orden del array siempre empeza en 0
fibonacci[0]
> 0

// Elementos que hay en un array. metodo: length
fibonacci.length
> 10

// El último elemento del array siempre es: logitud del array - 1
fibonacci[fibonacci.length-1]
> 34
```	
- **Objetos** : Es una asignación {**clave**:**valor**} encerrada entre llaves, cuya clave es un string identificativo de acceso y el valor puede ser cualquier objeto de cualquier tipo, pudiendo ser otro objeto de forma recursiva
```
var deportista = { nombre:"Rafa Nadal", "edad": 29, "palmares":[ {"grand_slam":"Wimbledon","anyos":[2008,2010]},{"grand_slam":"Abierto de EE. UU.","anyos":[2010,2013]} ]};

// acceso a una clave del objecto. Se utiliza la "notacion por punto"
deportista.nombre
> "Rafa Nadal"

deportista.palmares[0].gand_slam
> "Wimbledon"

deportista.palmares[0].anyos[0]
> 2008

deportista.palmares[0].anyos[1]
> 2010
```
