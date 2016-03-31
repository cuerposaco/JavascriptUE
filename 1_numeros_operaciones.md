Números y operaciones.

En javascript podemos realizar todo tipo de operacione matemáticas básicas como la suma, resta, multiplicación y la division.

Podemos usar la consola como una calculadora:

- Suma:
  ```
  1 + 1 + 23 
  // 25
  ```
- Resta:
  ```
  -11 - 11 
  // -22
  ```

- Multiplicación:
  ```
  123 * 987 
  // 121401
  ```

- División: 
  ```
  123 / 23 
  // 5.3478260869565215
  ```

Podemos combinar las operaciones para hacer operaciones más complejas

  ```999 + 997 * 12 - 1000 / 2```
Pero tenemos que tener muy en cuenta el orden en el que Javascript ejecuta esas operaciones porque podemos obtener resultados no deseados:
  ```
  1 + 1 * 2
  // 3
  ```

Este resultado se produce porque javascript procesa primero las operaciones de multiplicación y division, antes que las sumas y restas, en el caso anterior, el proceso sería el siguiente:
  ```
  1 + 1 * 2
  1 + 2
  // 3
  ```

Para priorizar unas operaciones sobre otras podemos envolver entre paréntesis aquellas operaciones que queramos priorizar, en el caso anerior para obtener un resultado correcto, deberiamos de realizar lo siguiente:
  ```
  ( 1 + 1 ) * 2
  // 4
  ```

El proceso seguido sería el siguiente:
  ```
  ( 1 + 1 ) * 2
  2 * 2
  // 4
  ```

- Para operaciones aritméticas más complejas disponemos de la librería "Math", que forma parte del núcleo de Javascript:

```
Math.pow(10,2) // 10 elevado a 2
Math.cos(90) // Coseno de 90
Math.sqrt(4) // Raíz cuadrada de 4

// otras operaciones no matemáticas
Math.max(1,2,100,56,7,34,87) // devuelve el valor maximo de los elementos dados
Math.min(1,2,100,56,7,34,87) // devuelve el valor minimo de los elementos dados
Math.random() // genera un número aleatorio entre el 0 y el 1
Math.random()*99+1 // genera un número aleatorio entre el 1 y el 100
Math.floor(2.51) // redondea a la baja
Math.ceil(2.51) // redondea a la alta
Math.round(2.51) // redondeo más proximo
```


- Documentación:
http://www.w3schools.com/js/js_math.asp









