# Introducción a la Nomenclatura

|Modelos para señales| SVID | SVIC |
|:-| :-: | :-: |
|Señal determinística| $x[n]$ | $x(t)$ |
|Señal aleatoria| $X[n]$ | $X(t)$ |

## Modelo Determinístico

### Valor Medio
| | |
|-|-|
|SVID|$\overline{x[n]}=<x[n]>=\lim_{N\to\infty}\frac{1}{2N+1}\sum_{n=-N}^{N}x[n]$|
|SVIC|$\overline{x(t)}=<x(t)>=\lim_{T\to\infty}\frac{1}{2T}\int_{-T}^{T}x(t)dt$|

* Notar que a $\lim_{T\to\infty}\frac{1}{2T}\int_{-T}^{T}$ se lo conoce como *Operador de Promedio Temporal* (análogo para SVID)

Propiedades:
* Si la señal es periódica, calcular el promedio en un periodo es igual que calcularlo para $(-\infty,\infty)$

### Energía y Potencia

||Energía|Potencia|
|-|-|-|
|SVID|$\varepsilon_x=\sum_{n=-\infty}^{\infty}\lvert x^{2}[n] \rvert$|$P_x=\lim_{N\to\infty}\frac{1}{2N+1}\sum_{n=-N}^{N}\lvert x^{2}[n] \rvert=<\lvert x^{2}[n]\rvert>$|
|SVIC|$\varepsilon_x=\int_{\infty}^{\infty}\lvert x^{2}(t) \rvert dt$|$P_x=\lim_{T\to\infty}\frac{1}{2T}\int_{-T}^{T}\lvert x(t)^{2} \rvert dt=<\lvert x^{2}(t)\rvert>$|

Definiciones:
* Se llama a $\lvert x^2(t) \rvert$ a la **potencia instantanea**
* Se llama a $P_x$ a la **potencia media normalizada**

Propiedades:
* La señal es de energía si $\varepsilon_x<\infty$, análogo para la potencia.
* Si la señal tiene valor medio no nulo, nunca podrá ser de energía.
  * Si la señal es periódica, $\varepsilon = \infty$
* Si $\varepsilon_x<\infty\Rightarrow P_x=0$
* Si $P_x<\infty\Rightarrow \varepsilon_x=\infty$ (corolario de lo anterior)
* Si la señal es de potencia, en el contenido en frecuencia de la misma (espectro o transformada de fourier de la señal) aparecerán $\delta(t)$.

<details><summary>Análisis de la potencia de una <b>señal truncada</b></summary>

<br>

Siendo $x_T(t)$ una señal *truncada* en el intervalo temporal $[-T,T]$, esta se encuentra definida por: 

$$ x_T(t) = x(t) ⊓(\frac{1}{2T}t) $$

* El cajón tiene soporte/largo $2T$.
* También es válido para SVID con sus correspondientes cambios en su definición.

| | |
|-|-|
|SVID| $$ P_x= \lim_{N\to\infty}\frac{1}{2N+1}\sum_{n=-\infty}^{\infty}\lvert x^{2}_N[n] \rvert=\lim_{N\to\infty}\frac{\varepsilon_{x_{N}}}{2N+1} $$ |
|SVIC| $$ P_x= \lim_{T\to\infty}\frac{1}{2T}\int_{-\infty}^{\infty}\lvert x^{2}_T(t) \rvert=\lim_{T\to\infty}\frac{\varepsilon_{x_{T}}}{2T} $$ |

</details>

<!-- TODO: hacer un summary de señales de potencias periódicas, ayudarse con el ejercicio P1-Ej. 1 a) I. -->

$$ \underset{a}{\underbrace{1111111111111111111}} $$