(algebras)=
# Álgebras

1 - Considere o conjunto de funções do tipo $f: \mathbb{R} \rightarrow \mathbb{R}$ e denotado por $\mathcal{F}$ dotado de um produto $(fg) = f g$ (a multiplicação convencional), onde $f,g \in \mathcal{F}$, formam uma álgebra.

```{dropdown} **Solução**:

Observamos que o produto sde duas funções é também uma funcão, portanto o produto é um mapa $\mathcal{F} \times \mathcal{F} \rightarrow \mathcal{F}$.

Verificamos as leis distributivas usando $\alpha,\beta \in \mathbb{R}$ e $f,g,h \in \mathcal{F}$:

$$\begin{align*}
f(\alpha g+\beta h) &= (f \alpha g + f \beta h)\\
 &= (\alpha fg + \beta fh)\\
 \text{e}\\
(\alpha g+\beta h)f &= (\alpha gf + \beta hf).\\
\end{align*}$$

As leis são obedecidas, pois a multiplicação de escalares por funções é comutativa.

Por fim definimos o "vetor zero" como a função $o \in \mathcal{F}$ definida por $(x) \mapsto (0)$ e o escalar zero como $0 \in \mathbb{R}$. Verificamos que

$$of = (0f)f = 0(ff) = o \\ 
fo = f(0f) = 0ff = o,
$$

ou seja, o produto de uma função com a $o$ sempre resulta em $o$.

Sendo atendidas todas as exigências, vemos que esta construção forma uma álgebra.
```
<br/>

2 - Sejam $f,g \in \mathcal{F}$ definidas respectivamente por $(x) \mapsto (x^{2})$ e $(x) \mapsto (x+1)$. Mostre que o mapa $\frac{d}{dx}: \mathcal{F} \rightarrow \mathcal{F}$ é uma derivação na álgebra $\mathcal{F}$. Cálcule sua ação sobre $(fg)$.

```{dropdown} **Solução:**

Esse mapa é uma derivação nesta álgebra, pois atende a regra de Leibniz:

$$\frac{d}{dx}(fg) = \frac{df}{dx}g + f\frac{dg}{dx}$$

resultando em:

$$\begin{align*}
\frac{d}{dx}(fg) =& \frac{d}{dx}(x^{2}(x+1))\\
 &= \left(\frac{d}{dx} x^{2}\right)(x+1) + x^{2} \left(\frac{d}{dx}(x+1)\right)\\
 &= (2x^{2}+2x) + (x^{2})\\
 &= 3x^{2} +2x.
\end{align*}$$
```
<br/>

3 - Considere a álgebra formada pelo conjunto de matrizes quadradas $\mathcal{M}_{n}(\mathbb{R})$ e pelo produto de matrizes. Mostre o determinante $det: \mathcal{M}_{n}(\mathbb{R}) \rightarrow \mathbb{R}$ é um homomorfismo desta álgebra.

```{dropdown} **Solução**:
Dadas duas matrizes $A,B \in \mathcal{M}_{n}(\mathbb{R})$ o determinante  respeita a regra

$det(AB) = det(A)det(B)$

logo o determinante é um homomorfismo dest álgebra.
```
<br/>

4 - Construa a derivação do homomorfismo do problema anterior usando o mapa $\frac{d}{dx}: \mathcal{M}_{n}(\mathbb{R}) \rightarrow \mathcal{M}_{n}(\mathbb{R})$, sendo que os elementos das matrizes que compõem $\mathcal{M}_{n}(\mathbb{R})$ são funções de $x$.

```{dropdown} **Solução**:
$$\begin{align*}
\frac{d}{dx}(AB) =& \frac{d}{dx}(A)det(B) + det(A)\frac{d}{dx}(B)\\
\end{align*}$$

onde os termos $det(B)$ e $det(A)$ são escalares multiplicando as matrizes resultantes de $\frac{d}{dx}(A)$ e $\frac{d}{dx}(B)$ Respectivamente.
```
<br/>

5 - Sejam $A,B \in \mathcal{M}_{2}(\mathbb{R})$ definidas por 

$$A = \begin{pmatrix}
\cos{x}& -r \sin{x}\\
\sin{x}& r \cos{x}\\
\end{pmatrix}\ \ \ B = \begin{pmatrix}
1& 0\\
0& r^{2}\\
\end{pmatrix}$$