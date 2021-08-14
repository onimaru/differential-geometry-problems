(matric-tensor-fields)=
# Campos Tensoriais Métricos

1 - Considere o tensor métrico 

$$g = dx^{1} \otimes dx^{1} + dx^{2} \otimes dx^{2}$$

para o espaço Euclidiano bi-dimensional $\mathbb{E}^{2}$ e a 2-forma diferencial $dx^{1} \wedge dx^{2}$. (i) Expresse o tensor métrico e a 2-forma diferencial em coordenadas polares: $x^{1}(r,\theta) = r \cos{\theta},\ x^{2}(r,\theta) = r \sin{\theta}$. (ii) Por fim expresse a integral $\int \int f(x^{1},x^{2})dx^{1}dx^{2}$ em coordenadas polares.  

```{dropdown} **Solução**: 
(i) Para calcular os componentes do tensor métrico precisamos primeiro calcular os diferenciais.

$$dx^{1} = \frac{\partial x^{1}}{\partial r}dr + \frac{\partial x^{1}}{\partial \theta}d\theta, \text{ e } dx^{2} = \frac{\partial x^{2}}{\partial r}dr + \frac{\partial x^{2}}{\partial \theta}d\theta.$$
$$dx^{1} = \cos{\theta} dr - r \sin{\theta} d \theta, \text{ e } dx^{2} = \sin{\theta} dr + r \cos{\theta} d \theta.$$

Agora calculamos os produtos tensoriais descritos no tensor métrico:

$$dx^{1} \otimes dx^{1} = \cos^{2}{\theta} dr \otimes dr -r \cos{\theta} \sin{\theta} dr \otimes d\theta -r \cos{\theta} \sin{\theta} d\theta \otimes dr + r^{2} \sin^{2}{\theta} d\theta \otimes d\theta$$
$$dx^{2} \otimes dx^{2} = \sin^{2}{\theta} dr \otimes dr +r \cos{\theta} \sin{\theta} dr \otimes d\theta +r \cos{\theta} \sin{\theta} d\theta \otimes dr + r^{2} \cos^{2}{\theta} d\theta \otimes d\theta$$

Assim, temos $g = dr \otimes dr + r^{2} d \theta \otimes d \theta$ ou na forma matricial, $g_{ij} = \begin{pmatrix}
1 & 0\\ 
0 & r^{2}
\end{pmatrix}.$
Para calcular a 2-forma devemos lembrar da antissimetria, $dx^{1} \wedge dx^{2} = - dx^{2} \wedge dx^{1}$ e $dx^{1} \wedge dx^{1} = dx^{2} \wedge dx^{2} = 0$. Essas propriedades são preservadas com a mudanças de coordenadas. Então,

$$dx^{1} \wedge dx^{2} = r \cos^{2}{\theta}dr \wedge d \theta - r \sin^{2}{\theta} d \theta \wedge dr = r dr \wedge d \theta,$$

onde usamos o $\cos^{2}{\theta} + \sin^{2}{\theta}=1$ e $dr \wedge d \theta = - d \theta \wedge dr.$

(ii) Seja qual for a função $f(x^{1},x^{2})$ reexpressamos ela com as variáveis $r$ e $\theta$ e os termos $dx^{1}dx^{2}$ representam a 2-forma $dx^{1} \wedge dx^{2}$. Portanto a integral pode ser expressa em coordenadas polares da seguinte forma:

$$\int \int f(x^{1}(r,\theta),x^{2}(r,\theta)) r dr \wedge d \theta.$$

Para o caso de uma integral definida devemos também redefinir os limites de integração em coordenadas polares.
```
<br/>

2 - Considere o tensor métrico 

$$g = dx^{0} \otimes dx^{0} - dx^{1} \otimes dx^{1}.$$

Mostre que $g$ é invariante sob a transformação

$$\begin{pmatrix}
 x^{0}\\ 
 x^{1}
\end{pmatrix} \mapsto \begin{pmatrix}
\cosh{\theta} & \sinh{\theta}\\ 
\sinh{\theta} & \cosh{\theta}
\end{pmatrix}\begin{pmatrix}
 x^{0}\\ 
 x^{1}
\end{pmatrix},$$

onde $\theta \in \mathbb{R}$.  

**Solução**:
Para esse caso podemos escrever o vetor inicial igual à transformação e verificar se a métrica assume o mesmo formato apresentado no enunciado.

```{dropdown} **Solução**: 

```