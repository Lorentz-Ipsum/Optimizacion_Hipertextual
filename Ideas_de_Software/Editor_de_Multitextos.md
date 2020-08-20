
A veces cuando estoy escribiendo el índice detallado de una asignatura también quiero poder añadir el contenido en el archivo de resumen sin alterar el índice.
Sería ideal un plugin de Atom o Vim que permitiera tener dos archivos abiertos lado a lado y poder escribir en ambos de golpe, luego con un atajo de teclado cambiar de uno a otro y escribir detalles, y cuando haya acabado con otro atajo de teclado volver a escribir en los dos a la vez, justo despues del texto recien editado.

(Digamos que el cursor está en [|])
Archivo A           |    Archivo B
  |

[Escribo en ambos a la vez:]
1. Alpha            |  1. Alpha
2. Beta             |  2. Beta
3. Gamma[|]         |  3. Gamma[|]

[Cambio y escribo sólo en B:]
1. Alpha            |  1. Alpha
2. Beta             |  2. Beta
3. Gamma            |  3. Gamma
                    |       - Gamma es la tercera letra del alfabeto griego[|]

[Cambio y escribo en ambos otra vez:]
1. Alpha            |  1. Alpha
2. Beta             |  2. Beta
3. Gamma            |  3. Gamma
4. Delta[|]         |       - Gamma es la tercera letra del alfabeto griego  |
                    |  4. Delta[|]
