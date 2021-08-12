# Mapas


Fonte: nakahara2018geometry

1. Seja $f: \mathbb{R} \rightarrow \mathbb{R}$ dado por $f(x) = \sin{x}$ ou $f: x \Rightarrow \sin{x}$. Determine o domínio, alcance, imagem e imagem inversa de $0$.  
**Solução**: O domínio e a imagem são $\mathbb{R}$, já a imagem é $f(\mathbb{R}) = \left[-1,1 \right]$. Para a imagem inversa de $0$ vemos que existem diversos valores de $x$ que produzem $\sin{x}=0$, todos esses valores são múltiplos inteiros de $\pi$. Então escrevemos $f^{-1}(0) = \lbrace n \pi \vert n \in \mathbb{Z} \rbrace$.

<br/>

2. Classifique os mapas a seguir como injetivos, sobrejetivos ou bijetivo:
   1. $f: \mathbb{R} \rightarrow \mathbb{R}$ definido como $f: x \mapsto ax$, onde $a \in \mathbb{R} - \lbrace 0\rbrace$.  
   **Solução**: como $a \ne 0$, $ax$ é sempre um múltiplo de $x$. Isso é definido para todo $Dom = \mathbb{R}$ e $Img = \mathbb{R}$. Atende às condições para ser injetivo e sobrejetivo. é portanto, bijetivo.

   2. $f: \mathbb{R} \rightarrow \mathbb{R}$ definido como $f: x \mapsto x^{2}$.  
   **Solução**: Não é injetivo pois, por exemplo: $x = 1$ e $x = -1$ são ambos mapeados para $f(x) = 1$. Não é sobrejetivo pois não há pelo menos um $x$ que seja mapeado para $f(x) < 0$.

   3. $f: \mathbb{R} \rightarrow \mathbb{R}$ definido como $f: x \mapsto e^{x}$.  
   **Solução**: É injetivo, pois para cada $x$ há apenas um $f(x)$.  Não é sobrejetivo pois não há pelo menos um $x$ que seja mapeado para $f(x) < 0$.

   4. Seja $M$ um elemento do grupo linear geral $GL(n,\mathbb{R})$ cujas representação matricial é dada por matrizes $n \times n$ com determinante não nulo, ou seja, $M: \mathbb{R}^{n} \rightarrow \mathbb{R}^{n}$, $x \mapsto Mx$.  
   **Solução**: Com a garantia do determinante não nulo, cada $x$ á mapeado para um $Mx$ único e existe a função inversa $M^{-1}x \mapsto x$ que também é injetiva. Esse mapa é portanto, bijetivo.

<br/>

3. Seja o mapa $f: \mathbb{R} \rightarrow \mathbb{R}$ definido como $f: x \mapsto \sin{x}$. Defina restrições no domínio e no alcance para que $f$ seja bijetivo.  
**Solução**: Restringindo o domínio ao subconjunto $\left[ -\frac{\pi}{2},\frac{\pi}{2} \right] \subset \mathbb{R}$ garantimos que o mapa injetivo e restringindo o alcance para o subconjunto $\left[-1,1 \right]$ garantimos que para todo $f(x)$ exista pelo menos um $x$, sendo assim sobrejetivo. Com as duas restrições $f: \left[ -\frac{\pi}{2},\frac{\pi}{2} \right] \rightarrow \left[-1,1 \right]$ o mapa $f(x) = \sin{x}$ é bijetivo.

<br/>

4. Seja $f: \mathbb{R} \rightarrow \mathbb{R}$ definido por $f: x \mapsto x^{2}$ e $g: \mathbb{R} \rightarrow \mathbb{R}$ por $g: x \mapsto e^{x}$. Quais são os mapas $g \circ f:\mathbb{R} \rightarrow \mathbb{R}$ e $f \circ g:\mathbb{R} \rightarrow \mathbb{R}$?  
**Solução**: $g \circ f = e^{f(x)} = e^{x^{2}}$, enquanto $f \circ g = \left(g(x) \right)^{2} = \left(e^{x}\right)^{2} = e^{2x}$.

<br/>

5. O grupo Euclidiano n-dimensional $E^{n}$ é feito de uma translação n-dimensional $a: x \rightarrow x + a$, onde $x,a \in \mathbb{R}^{n}$, e uma rotation, $O(n)$, $R: x \rightarrow Rx$, onde $R \in O(n)$. Um elemento geral $(R,a)$ de $E^{n}$ atua sobre $x$ pelo mapa $(R,a): x \mapsto Rx + a$. O produto é definido por $(R_{2},a_{2}) \times (R_{1},a_{1}): x \mapsto R_{2}\left( R_{1}x + a_{1}\right) + a_{2}$, que é $(R_{2},a_{2}) \circ (R_{1},a_{1}) = \left( R_{2}R_{1}, R_{2}a_{1} + a_{2} \right)$. Mostre que os mapas $a, R$ e $(R,a)$ são bijeções e encontre seus mapas inversos.
