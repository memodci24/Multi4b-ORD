<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

El proyecto se divide en dos circuitos independientes (A y B) descritos a continuación:

Circuito A:
Multiplicador binario de 4x4 bits, diseñado para tomar dos números de 4 bits (A0-A3 y B0-B3) para generar un resultado de 8 bits (P0-P7). Su funcionamiento se basa en tres etapas principales. Primero, se generan los productos parciales mediante compuertas AND, multiplicando cada bit del número A con cada bit del número B. Luego, estos productos parciales se organizan en filas escalonadas y se suman utilizando compuertas XOR y AND para manejar los acarreos intermedios. Finalmente, el resultado se muestra a través de LEDs o un display de 7 segmentos. Este método sigue el mismo principio de la multiplicación binaria manual, donde cada fila representa un desplazamiento de los productos parciales y se suman adecuadamente.

Circuito B:
Ordenador de datos binario, de 4x4 bits, diseñado para tomar dos números de 4 bits (A0-A3 y B0-B3) y hacer el ordenamiento a la salida, resultando siempre
el numero mayor (max) primero, y el numero menor (min) al final.

La selección entre "Circuito A" - "Circuito B" se realiza mediante el botón RESET. Mientras no se esté pulsando, a la salida veremos la multiplicación de los numeros de
entrada. Cuando se mantiene pulsado el botón, a la salida veremos el ordenamiento de los datos de mayor a menor.

## How to test

Primero se configuran los valores de entrada A0-A3 y B0-B3 mediante interruptores. A la salida, mientras no se mantenga pulsado el botón, veremos la multiplicación de los datos de entrada. Si mantenemos pulsado el botón, entonces se podrá observar a la salida los mismos datos de la entrada, pero ordenados de mayor a menor.
## External hardware

List external hardware used in your project (e.g. PMOD, LED display, etc), if any
