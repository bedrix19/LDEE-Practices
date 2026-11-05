


1.  Cales son as bandas de frecuencia e os límites de emisión conducida que establece
a norma para os dispositivos de clase 2 medida polo método de tensión?

![Frecuencia emisiones](imgs/20260924101531.png)

2. Cal é a tensión media na carga? Cal é a potencia media entregada á carga? Cal é
a frecuencia de conmutación do convertedor?


![[Pasted image imgs/20260910124921.png]]


- Realizar unha transformada rápida de Fourier (FFT) da corrente sobre un intervalo de
500 μs considerando un número de mostras igual a 131 072, co obxectivo de conseguir un
rango aproximado de frecuencias na FFT de 108 MHz. Para obter unha estimación das emisións
conducidas multiplicar o valor da corrente polos seguintes factores de escala:
- √2 para obter valores de amplitude.
- 50 Ω para obter os valores de emisión de tensión correspondentes.
- 106 μV/V para obter o resultado final en dB(μV)

Poner la siguiente línea en la expresión de la FFT de salida del circuito simulado:

$I(V1)*50*1e6*sqrt(2)$

![[Pasted image imgs/20260910125149.png]]


![[Pasted image imgs/20260910125034.png]]


- La frecuencia del primer pico es de 600kHz

- Aquí podemos ver si se cumple la norma (viendo los picos y si son mayores del límite), para ello hay que corregir, porque la simulación da valores en eficaz (multiplica por raíz de 2 para compensar), y pasar de microvoltias

- El valor medio del voltaje: 3.2651V, el de la corriente: -787.83 mA.


- **Frecuencia de conmutador?: **





![[Pasted image imgs/20260924104236.png]]


- Según se ve aquí, la magnitud en el primer (y mayor) pico, es de 153dB, el máximo son 78dB, dando 76dB de atenuación, 50/10^(A/20)=0.0079 Ohms. Cogeremos la resistencia más pequeña para poder cumplir





![[Pasted image imgs/20260924112728.png]]



![[Pasted image imgs/20260924112801.png]]