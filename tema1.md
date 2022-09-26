---
"lang": "en",
"title": "Euler's Identity",
"subtitle": "How to combine 5 important math constants to a short formula",
"authors": ["Max Muster<sup>1</sup>", "Lisa Master<sup>2</sup>"],
"adresses": ["<sup>1</sup>Hochschule Gartenstadt","<sup>2</sup>Universität Übersee"],
"date": "May 2021",
"description": "mdmath LaTeX demo site",
"tags": ["markdown+math","VSCode","static page","publication","LaTeX","math"]
---

# Tema 1

## Introducción a la Nomenclatura

<style>
  table {
    margin: 0px 0px 0px 0px;
  }
</style>

<center>

|Modelos para señales| SVID | SVIC |
|:-| :-: | :-: |
|Señal determinística| $x[n]$ | $x(t)$ |
|Señal aleatoria| $X[n]$ | $X(t)$ |

</center>

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
|SVID|$\varepsilon_{x}=\sum_{n=-\infty}^{\infty}\lvert x^{2}[n] \rvert$|$P_{x}=\lim_{N\to\infty}\frac{1}{2N+1}\sum_{n=-N}^{N}\lvert x^{2}[n] \rvert=<\lvert x^{2}[n]\rvert>$|
|SVIC|$\varepsilon_{x}=\int_{\infty}^{\infty}\lvert x^{2}(t) \rvert dt$|$P_{x}=\lim_{T\to\infty}\frac{1}{2T}\int_{-T}^{T}\lvert x(t)^{2} \rvert dt=<\lvert x^{2}(t)\rvert>$|

Definiciones:
* Se llama a $\lvert x^{2}(t) \rvert$ a la **potencia instantanea**
* Se llama a $P_{x}$ a la **potencia media normalizada**

Propiedades:
* La señal es de energía si $\varepsilon_{x}<\infty$, análogo para la potencia.
* Si la señal tiene valor medio no nulo, nunca podrá ser de energía.
  * Si la señal es periódica, $\varepsilon_{x} = \infty$
* Si $\varepsilon_{x}<\infty\Rightarrow P_{x}=0$
* Si $P_{x}<\infty\Rightarrow \varepsilon_{x}=\infty$ (corolario de lo anterior)
* Si la señal es de potencia, en el contenido en frecuencia de la misma (espectro o transformada de fourier de la señal) aparecerán $\delta(t)$.

<details><summary>Análisis de la potencia de una <b>señal truncada</b></summary>

<br>

Siendo $x_{T}(t)$ una señal *truncada* en el intervalo temporal $[-T,T]$, esta se encuentra definida por: 

$$ x_{T}(t) = x(t) ⊓(\frac{1}{2T}t) $$

* El cajón tiene soporte/largo $2T$.
* También es válido para SVID con sus correspondientes cambios en su definición.

| | |
|-|-|
|SVID| $ P_{x}= \lim_{N\to\infty}\frac{1}{2N+1}\sum_{n=-\infty}^{\infty}\lvert x_{N}^{2}[n] \rvert=\lim_{N\to\infty}\frac{\varepsilon_{x_{N}}}{2N+1} $ |
|SVIC| $ P_{x}= \lim_{T\to\infty}\frac{1}{2T}\int_{-\infty}^{\infty}\lvert x_{T}^{2}(t) \rvert=\lim_{T\to\infty}\frac{\varepsilon_{x_{T}}}{2T} $ |

</details>

$\boxed{c_i = \langle\psi|\phi\rangle}$

Search by definition $\eqref{1-1}$ or $\ref{1-1}$.

$$
\begin{aligned} \sin 2\theta = 2\sin \theta \cos \theta \\ = \cfrac{2 \tan \theta}{1+\tan^2 \theta} \end{aligned} \label{1-1}\tag{1-1}
$$

<!-- TODO: hacer un summary de señales de potencias periódicas, ayudarse con el ejercicio P1-Ej. 1 a) I. -->

$$ \underset{\htmlStyle{color: red;}{x}}{\underbrace{1111111111111111111}} $$


