---
title: On an Equal Volume Cut of Conical Carrots
date: 2018-11-14 00:00:00 Z
categories:
- posts
layout: post
mathjax: true
---

## Abstract
In order to split an idealized conical carrot into two pieces of equal volume, a cut should be made parallel to the base at approximately one fifth of the carrots total length measured up from the bottom. This simple rule of thumb warrants real world testing.
{: style="text-align: justify"}

## Motivation
It is of interest to cut a carrot into two pieces of equal volume. A trivial solution is to make a cut lengthwise from the tip to the base. However, this is often inconvenient because the carrot may be curved, longer than the knife's blade, or both. Therefore, the cut shall be made across the shorter dimension. 
{: style="text-align: justify"}

Fully grown carrots generally taper significantly from one end to the other <a name="ref1"></a>[[citation needed]](#cavalieri). In order to get a rough estimate for the position of the equal volume cut, an idealized model shall be adopted where the carrot is represented as a cone. It should be noted that by invoking Cavalieri's Principle, the following derivation can reasonably be applied to mildly curved carrots <a name="ref1"></a>[[1]](#cavalieri).
{: style="text-align: justify"}

## Derivation

Consider an idealized conical carrot of length $L$ and a circular base of radius \\( r \\) (Figure $\ref{fig:carrot}$). The volume of this carrot is
{: style="text-align: justify"}

$$
	\begin{align}\label{V}
		V = \frac{1}{3}\pi r^2 L.
	\end{align}
$$

<figure class="image">
  <img src="/img/CCFig1.JPG" />
</figure>

A fraction \\( k \\) will define where the cut should be made. The length of the base piece will be \\( kL \\) and the length of the tip piece will be \\( L-kL \\). The circle formed by the cut is defined to have a radius \\( r_k \\) (Figure \ref{fig:cutcarrot}). 
{: style="text-align: justify"}

<figure class="image">
  <img src="/img/CCFig2.JPG" />
</figure>

Since the cut is defined so the volumes of the base piece and the tip piece are equal, it is only necessary to find one of those volumes for this derivation. The tip piece is a cone and its volume is given by 
{: style="text-align: justify"}

$$
	\begin{align}\label{tipVol}
		V_1 = \frac{1}{3}\pi r_k^2 (L-kL).
	\end{align}
$$

In order to find \\( r_k \\) in terms of \\( r \\) and \\( k \\), consider the two right triangles shown in Figure \ref{fig:triangles}. The triangles were formed by drawing a line from the center of the base to the tip of the carrot. Because they share the angle \\( \theta \\), the trigonometric relation
{: style="text-align: justify"}

$$
	\begin{align}\label{bigT}
		\text{tan}(\theta) = \frac{r}{L}
	\end{align}
$$

can be defined for the big triangle and the similar relation
{: style="text-align: justify"}

$$
	\begin{align}\label{lilT}
		\text{tan}(\theta) = \frac{r_k}{L-kL}
	\end{align}
$$

can be defined for the smaller triangle. 
{: style="text-align: justify"}

<figure class="image">
  <img src="/img/CCFig3.JPG" />
</figure>

Setting equations \eqref{bigT} and \eqref{lilT} equal to each other allows for \\( r_k \\) to be found in terms of \\( r \\) and \\( k \\):
{: style="text-align: justify"}

$$
	\begin{align*}
		\frac{r_k}{L-kL} &= \frac{r}{L}
	\end{align*}

$$

$$
	\begin{align*}
		r_k &= \frac{r}{L}(L-kL)\nonumber \\
		r_k &= r(1-k).
	\end{align*}
$$

This may be substituted into equation (\ref{tipVol}) to redefine the tip piece's volume:
{: style="text-align: justify"}

$$
	\begin{align}
		V_1 &= \frac{1}{3}\pi [r(1-k)]^2 (L-kL)\nonumber\\
		V_1 &= \frac{1}{3}\pi r^2 (1-k)^2 L(1-k)\nonumber\\
		V_1 &= \frac{1}{3}\pi r^2 (1-k)^3 L \label{tipVol2}
	\end{align}
$$

Because the tip and base pieces are of equal volume, the total volume \\( V \\) will be equal to twice the tip piece's volume.
{: style="text-align: justify"}

$$
	\begin{align*}
		V = 2\cdot V_1
	\end{align*}
$$

Substituting equations (\ref{V}) and (\ref{tipVol2}) into the above expression gives
{: style="text-align: justify"}

$$
	\begin{align*}
		 \frac{1}{3}\pi r^2 L &= 2\cdot \frac{1}{3}\pi r^2(1-k)^3 L.
	\end{align*}
$$

Canceling common factors from both sides leaves a relatively simple expression for \\( k \\).
{: style="text-align: justify"}

$$
	\begin{align}
		1 &= 2(1-k)^3\nonumber\\
		\left(\frac{1}{2}\right)^{1/3} &= 1-k\nonumber\\
		k &= 1 - \left(\frac{1}{2}\right)^{1/3}
	\end{align}
$$

Evaluated numerically, \\( k = 0.2063 \\) which is reasonably close to a fifth.
{: style="text-align: justify"}

$$
	\begin{equation}
		\boxed{k \approx \frac{1}{5}}
	\end{equation}
$$
	
## Conclusion

The equal volume cut of a conical carrot is approximately one fifth of the carrot's total length from the base. This simple rule warrants testing, most likely using the water displacement method to measure the volume of real, irregularly shaped carrots.
{: style="text-align: justify"}



## References

<a name="cavalieri"></a>
[[1]](#ref1) "Cavalier's Principle." *Wikipedia,* 7 November 2018. [Web Link.](https://en.wikipedia.org/wiki/Cavalieri%27s_principle)