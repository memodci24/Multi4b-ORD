<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

Multiplicador binario de 4x4 bits, diseñado para tomar dos números de 4 bits (A0-A3 y B0-B3) para generar un resultado de 8 bits (P0-P7). Su funcionamiento se basa en tres etapas principales. Primero, se generan los productos parciales mediante compuertas AND, multiplicando cada bit del número A con cada bit del número B. Luego, estos productos parciales se organizan en filas escalonadas y se suman utilizando compuertas XOR y AND para manejar los acarreos intermedios. Finalmente, el resultado se muestra a través de LEDs o un display de 7 segmentos. Este método sigue el mismo principio de la multiplicación binaria manual, donde cada fila representa un desplazamiento de los productos parciales y se suman adecuadamente.

El ordenador de datos comienza a funcionar mientras el botón RESET esté presionado. El ordenamiento será siempre el número mayor en la salida de P0-P3
y el número menor de P4-P7.

## How to test

Primero se configuran los valores de entrada A0-A3 y B0-B3 mediante interruptores. Luego, se verifica que los productos parciales se generen correctamente observando las señales en los nodos internos del circuito. A continuación, se comprueba que las sumas intermedias se realicen correctamente, asegurando que los acarreos sean procesados adecuadamente. Finalmente, se analiza la salida en los LEDs, comparando el resultado con la multiplicación esperada en binario o decimal para confirmar su correcto funcionamiento.

El ordenador unicamente ordena los datos de entrada, colocando el numero mayor primero, y el número menor después.

## External hardware

List external hardware used in your project (e.g. PMOD, LED display, etc), if any
