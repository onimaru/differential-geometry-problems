(vector-spaces)=
# Espaços Vetoriais

1 - Usando os axiomas de espaços vetoriais, mostre que é possível definir um espaço vetorial $V(2,\mathbb{R})$. Deixe claro quais são os elementos nulo, unitário e inverso.

```{dropdown} **Solução**:

 Definimos os vetores, $\textbf{u},\textbf{v},\textbf{w},\textbf{0} \in V(2,\mathbb{R})$:

$$\begin{align*}
\textbf{u} &= u^{1}e_{1}+u^{2}e_{2} = (u^{1}, u^{2})\\
\textbf{v} &= v^{1}e_{1}+v^{2}e_{2} = (v^{1}, v^{2})\\
\textbf{w} &= w^{1}e_{1}+w^{2}e_{2} = (w^{1}, w^{2})\\
\end{align*}$$

onde $e_{1}$ e $e_{2}$ são as bases de $V(2,\mathbb{R})$ e $u^{1},u^{2}v^{1},v^{2}w^{1},w^{2},0,1$ são escalares pertencentes ao corpo dos reais. Agora mostramos que esses vetores o obedecem os axiomas de formação de um espaço vetorial.

(i) - 

$$\begin{align*}
\textbf{u} + \textbf{v} &= \textbf{v} + \textbf{u}\\
(u^{1}+v^{1},u^{2}+v^{2}) &= (v^{1}+u^{1},v^{2}+u^{2})
\end{align*}$$

Como os escalares são reais, sua soma é comutativa.

(ii) - 

$$\begin{align*}
(\textbf{u} + \textbf{v}) + \textbf{w} &= \textbf{u} + (\textbf{v} + \textbf{w})\\
(u^{1}+v^{1},u^{2}+v^{2}) + (w^{1},w^{2}) &= (u^{1},u^{2}) + (v^{1}+w^{1},v^{2}+w^{2})\\
(u^{1}+v^{1}+w^{1},u^{2}+v^{2}+w^{2}) &= (u^{1}+v^{1}+w^{1},u^{1}+v^{2}+w^{2})\\
\end{align*}$$

Novamente a comutatividade da soma dos reais garante a associatividade da soma vetorial.

(iii) - seja o elemento nulo: $\textbf{0} = 0e_{1}+0e_{2} = (0, 0)$

$$\begin{align*}
\textbf{0} + \textbf{u} &= (0,0) + (u^{1},u^{2})\\
 &= (0+u^{1},0+u^{2}) \\
 &= (u^{1},u^{2})\\
 &= \textbf{u}
\end{align*}$$

(iv) - 

$$\begin{align*}
\textbf{u} + (-\textbf{u}) &= (u^{1},u^{2}) + (-u^{1},-u^{2})\\
 &= (u^{1}-u^{1},u^{2}-u^{2})\\
 &= (0,0)\\
 &= \textbf{0}
\end{align*}$$

(v) - seja $a \in \mathbb{R}$,

$$\begin{align*}
a(\textbf{u}+\textbf{v}) &= a\textbf{u}+ a\textbf{v}\\
a(u^{1}+v^{1},u^{2}+v^{2}) &=(au^{1},au^{2}) + (av^{1},av^{2})\\
(a(u^{1}+v^{1}),a(u^{2}+v^{2})) &= (au^{1}+av^{1},au^{2}+av^{2})\\
(au^{1}+av^{1},au^{2}+av^{2}) &= (au^{1}+av^{1},au^{2}+av^{2})
\end{align*}$$

(vi) - sejam $a,b \in \mathbb{R}$,

$$\begin{align*}
(a+b)\textbf{u} &= a\textbf{u}+ b\textbf{u}\\
 &= a(u^{1},u^{2}) + b(u^{1},u^{2})\\
 &=(au^{1},au^{2}) + (bu^{1},bu^{2})\\
 &= (au^{1}+bu^{1},au^{2}+bu^{2})\\
 &= ((a+b)u^{1},(a+b)u^{2})\\
 &= (a+b)\textbf{u}
\end{align*}$$

(vii) - sejam $a,b \in \mathbb{R}$,

$$\begin{align*}
(ab)\textbf{u} &= a(b\textbf{u})\\
 &= a(bu^{1},bu^{2})\\
 &=(abu^{1},abu^{2})\\
 &= (ab)(u^{1},u^{2})\\
 &= (ab)\textbf{u}
\end{align*}$$

Como o produto $ab$ é apenas um novo escalar $c \in \mathbb{R}$, não importa a ordem de atuação dos escalares.

(viii) - seja $1 \in \mathbb{R}$ o elemento unitário de $\mathbb{R}$,

$$\begin{align*}
1\textbf{u} &= 1(u^{1},u^{2})\\
 &= (1u^{1},1u^{2}) \\
 &= (u^{1},u^{2})\\
 &= \textbf{u}
\end{align*}$$
```

<br/>

2 - Seja o mapa $f: V \rightarrow W$, definido por $(x,y) \mapsto (r \cos{\theta}, r \sin{\theta})$, ou seja, $V$ é um espaço vetorial euclidiano "convencional" (com coordenadas cartesianas) e $W$ o seu correspondente em coordenadas polares. Sejam $v^{i} \in V$ e $w^{i} \in W$, encontre os mapas $\eta: V \rightarrow V^{*}$ e $g: W \rightarrow W^{*}$, ou seja, os mapas que levam cada elemento dos espaços $V$ e $W$ para seua correspondentes elementos nos espaços duais $V^{*}$ e $W^{*}$.

```{dropdown} **Solução**:

Os mapas $\eta$ e $g$ são os tensores métricos de cada um dos espaços, para o espaço Euclidiano bi-dimensional este se reduz ao delta de Kronecker, então $\eta \equiv \delta_{ij}$ ($\delta_{ij} = 1$ se $i=j$ e $0$ caso contrário). Para encontrar $v^{*} = v_{i}$ utilizamos o delta para "descer" o índice de $v^{i}$:

$$\begin{align*}
v_{i} &= \delta_{ij}v^{j}\\
 &= \delta_{00}v^{0} + \delta_{11}v^{1}
\end{align*}$$

ou ainda

$$\begin{align*}
\begin{pmatrix}v_{0} & v_{1} \end{pmatrix} &= \begin{pmatrix} 1 & 0\\ 0&1 \end{pmatrix}\begin{pmatrix}v^{0} \\ v^{1} \end{pmatrix}\\
&= \begin{pmatrix} v^{0} & v^{1} \end{pmatrix}
\end{align*}$$

Ou seja, o elemento $v^{i}$ é um vetor coluna (ou vetor contravariante) e $v_{i}$, o vetor dual de $v^{i}$, é um vetor linha (ou vetor covariante). Vemos que $v_{i}$ é o tansposto de $v^{i}$.

Para encontrar $g$ podemos verificar como $\delta_{ij}$ se transforma do espaço $V$ para $W$. Para tal precisamos verificar como um tensor se transforma de $V$ para $W$. Denotaremos os elementos de $W$ com o símbolo $'$ para evitar confusão com os elementos de $V$:

$$\begin{align*}
w^{'j} = \frac{\partial x^{'j}}{\partial x^{i}} v^{i} &= \begin{pmatrix} \frac{\partial x^{'0}}{\partial x^{0}} & \frac{\partial x^{'0}}{\partial x^{1}} \\ \frac{\partial x^{'1}}{\partial x^{0}} &\frac{\partial x^{'1}}{\partial x^{1}} \end{pmatrix}\begin{pmatrix}v^{0} \\ v^{1} \end{pmatrix} \\
 &=\begin{pmatrix} \cos{\theta} & \sin{\theta} \\ \frac{-\sin{\theta}}{r} & \frac{\cos{\theta}}{r} \end{pmatrix}\begin{pmatrix}v^{0} \\ v^{1} \end{pmatrix} \\
 &= \begin{pmatrix} v^{0} \cos{\theta} + v^{1} \sin{\theta} \\ v^{0}\frac{-\sin{\theta}}{r} + v^{1} \frac{\cos{\theta}}{r} \end{pmatrix}
\end{align*}$$

onde usamos a inversa de $f$ como $f^{-1}(r,\theta) \mapsto (\sqrt{x^{2}+y^{2}},\tan^{-1}(y/x))$.

A transformação de um vetor dual é dada por:

$$\begin{align*}
w_{j}^{'} = \frac{\partial x^{j}}{\partial x^{'i}} v_{i} &= \begin{pmatrix}v_{0} & v_{1} \end{pmatrix} \begin{pmatrix} \frac{\partial x^{0}}{\partial x^{'0}} & \frac{\partial x^{0}}{\partial x^{'1}} \\ \frac{\partial x^{1}}{\partial x^{'0}} &\frac{\partial x^{1}}{\partial x^{'1}} \end{pmatrix} \\
 &= \begin{pmatrix}v_{0} & v_{1} \end{pmatrix}\begin{pmatrix} \cos{\theta} & -r \sin{\theta} \\ \sin{\theta} & r \cos{\theta} \end{pmatrix}\\
 &= \begin{pmatrix} v^{0} \cos{\theta} + v^{1} \sin{\theta} & -v_{0} r \sin{\theta} + v_{1} r \cos{\theta} \end{pmatrix}
\end{align*}$$

Assim, a matriz de transformação é $\Lambda_{i}^{j} =\begin{pmatrix} \cos{\theta} & -r \sin{\theta} \\ \sin{\theta} & r \cos{\theta} \end{pmatrix}$ e com ela podemos transformar o tensor métrico:

$$\begin{align*}
g_{ij}^{'} &= \frac{\partial x^{l}}{\partial x^{'i}} \frac{\partial x^{m}}{\partial x^{'j}} g_{lm}\\
 &= \Lambda_{i}^{l}\Lambda_{j}^{m} \delta_{lm} \\
 &= \Lambda_{i}^{0}\Lambda_{j}^{0} + \Lambda_{i}^{1}\Lambda_{j}^{1} \\
 &= \begin{pmatrix} \Lambda_{0}^{0}\Lambda_{0}^{0} + \Lambda_{0}^{1}\Lambda_{0}^{1} & \Lambda_{0}^{0}\Lambda_{1}^{0} + \Lambda_{0}^{1}\Lambda_{1}^{1}\\ \Lambda_{1}^{0}\Lambda_{0}^{0} + \Lambda_{1}^{1}\Lambda_{0}^{1} & \Lambda_{1}^{0}\Lambda_{1}^{0} + \Lambda_{1}^{1}\Lambda_{1}^{1} \end{pmatrix}\\
 &= \begin{pmatrix} \cos^{2}{\theta} + \sin^{2}{\theta}& 0 \\ 0 &  r^{2}(\cos^{2}{\theta} + \sin^{2}{\theta})\end{pmatrix}\\
 &= \begin{pmatrix} 1 & 0 \\ 0 & r^{2} \end{pmatrix}
\end{align*}$$

Finalmente podemos fazer a transformação:

$$\begin{align*}
w_{i} &= g_{ij}w^{j} \\
&= \begin{pmatrix} 1 & 0 \\ 0 & r^{2} \end{pmatrix} \begin{pmatrix} w^{0} \\ w^{1} \end{pmatrix} \\
&= \begin{pmatrix} 1 w^{0} & r^{2} w^{1} \end{pmatrix}
\end{align*}$$

```

<br/>