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

```{dropdown} **Solução**: 
Para esse caso podemos escrever o vetor inicial igual à transformação e verificar se a métrica assume o mesmo formato apresentado no enunciado. Vamos mudar a notaçõ para evitar confusão:

$$\begin{pmatrix}
 x^{0}\\ 
 x^{1}
\end{pmatrix} \mapsto \begin{pmatrix}
\cosh{\theta} & \sinh{\theta}\\ 
\sinh{\theta} & \cosh{\theta}
\end{pmatrix}\begin{pmatrix}
 y^{0}\\ 
 y^{1}
\end{pmatrix}.$$

Então devemos calcular os diferenciais $dx^{0}$ e $dx^{1}$ para calcular o tensor métrico após a transformação.

$$x^{0} = \cosh{\theta}\ y^{0} + \sinh{\theta}\ y^{1}, \text{ e } x^{1} = \sinh{\theta}\ y^{0} + \cosh{\theta}\ y^{1},$$

e

$$dx^{0} = \cosh{\theta}\ dy^{0} + \sinh{\theta}\ dy^{1}, \text{ e } dx^{1} = \sinh{\theta}\ dy^{0} + \cosh{\theta}\ dy^{1}.$$

Lembre que $\cosh{\theta}$ é constante, por isso o diferencial possui o mesmo formato dos vetores iniciais. Agora fazemos:

$$dx^{0} \otimes dx^{0} = \cosh^{2}{\theta}\ dy^{0}dy^{0} + \sinh^{2}{\theta}\ dy^{1}dy^{1} + \cosh{\theta}\ \sinh{\theta}\ dy^{0}dy^{1} + \sinh{\theta}\ \cosh{\theta}\ dy^{1}dy^{0},$$

$$dx^{1} \otimes dx^{1} = \sinh^{2}{\theta}\ dy^{0}dy^{0} + \cosh^{2}{\theta}\ dy^{1}dy^{1} + \sinh{\theta}\ \cosh{\theta}\ dy^{0}dy^{1} + \cosh{\theta}\ \sinh{\theta}\ dy^{1}dy^{0}.$$

Por fim,

$$\begin{align*}
 g &= dx^{0} \otimes dx^{0} - dx^{1} \otimes dx^{1}\\ 
 &= \left(\cosh^{2}{\theta}\ - \sinh^{2}{\theta}\right) dy^{0}dy^{0} + \left(\sinh^{2}{\theta}\ - \cosh^{2}{\theta}\right) dy^{1}dy^{1} \\
 &= dy^{0}dy^{0} - dy^{1}dy^{1}
\end{align*},$$

onde usamos $\cosh^{2}{\theta}\ - \sinh^{2}{\theta} = 1$ (isso pode ser verificado usando as formas exponenciais: $\cosh{\theta} = \frac{e^{\theta} + e^{-\theta}}{2}$ e $\sinh{\theta} = \frac{e^{\theta} - e^{-\theta}}{2}$).

Desta maneira podemos ver que o tensor métrico apresentou o mesmo formato diante dessa tansformação. Devemos ainda citar aqui que esse tensor métrico coincide com o tensor de Minkowski para a relatividade especial (se usarmos apenas uma dimensão para o tempo e outra para o espaço), ou seja,

$$g = \begin{pmatrix}
1 & 0\\ 
0 & -1
\end{pmatrix}.$$

e por fim, a matriz de transformação usada nesse problema tem a mesma forma da Transformação de Lorentz, onde o parâmetro $\theta$ é dependente da velocidade relativa entre os referenciais e da velocidade da luz.
```

<br/>

3 - Seja a 1-forma diferencial $\theta = \left( 2 y^{1}y^{2} + (y^{1})^{2} +1 \right)dy^{1} + \left((y^{1})^{2} - y^{2} \right)dy^{2}$ no $\mathbb{R}^{2}$. Seja o mapa $f: \mathbb{R}^{3} \rightarrow \mathbb{R}^{2}$, definido por $(x^{1},x^{2},x^{3} ) \mapsto (y^{1},y^{2}) = (x^{1}-x^{2}, (x^{2})^{2} + x^{3})$. Encontre o pullback de $f$ sobre $\theta$, ou seja, $f^{*} \theta$.

```{dropdown} **Solução**:
Inicalmente vamos lembrar como calcular o pullback de uma forma diferencial. Para facilitar a notação vamos definir $g_{1} = \left( 2 y^{1}y^{2} + (y^{1})^{2} +1 \right)$ e $g_{2} = \left((y^{1})^{2} - y^{2} \right)$. Então podemos adequar o problema à fórmula:

$$f^{*} \theta = \frac{\partial (y^{i} \circ f)}{\partial x^{j}}(g_{i} \circ f)dx^{j}$$

Podemos escrever explicitamente na forma matricial:

$$f^{*} \theta = \begin{pmatrix} (g_{1} \circ f) & (g_{2} \circ f) \end{pmatrix} \begin{pmatrix}
\frac{\partial (y^{1} \circ f)}{\partial x^{1}} & \frac{\partial (y^{1} \circ f)}{\partial x^{2}} & \frac{\partial (y^{1} \circ f)}{\partial x^{3}}\\ 
\frac{\partial (y^{2} \circ f)}{\partial x^{1}} & \frac{\partial (y^{2} \circ f)}{\partial x^{2}} & \frac{\partial (y^{2} \circ f)}{\partial x^{3}}
\end{pmatrix} \begin{pmatrix} dx^{1} \\ dx^{2} \\ dx^{3} \end{pmatrix}.$$

Por exemplo, $\frac{\partial (y^{1} \circ f)}{\partial x^{1}} = \frac{\partial (x^{1} - x^{2})}{\partial x^{1}} = 1$. Vamos calcular todos os termos: 

$$g_{1} \circ f = 2 (x^{1} - x^{2})((x^{2})^{2} + x^{3}) + (x^{1} - x^{2})^{2} + 1$$

$$g_{2} \circ f = (x^{1} - x^{2})^{2} - (x^{2})^{2} - x^{3}$$

$$\frac{\partial (y^{i} \circ f)}{\partial x^{j}} = \begin{pmatrix}
1 & -1 & 0\\ 
0 & 2x^{2}& 1
\end{pmatrix}$$

Agora basta fazer os produtos:

$$\begin{align*}
f^{*} \theta &= 
\left(2 (x^{1} - x^{2})((x^{2})^{2} + x^{3}) + (x^{1} - x^{2})^{2} + 1 \right)dx^{1} \\ &\ \ \ + \left(2x^{2}(x^{1} - x^{2})^{2} - (x^{2})^{2} - x^{3}  -2 (x^{1} - x^{2})((x^{2})^{2} + x^{3}) - (x^{1} - x^{2})^{2} - 1 \right)dx^{2} \\
&\ \ \ + \left( (x^{1} - x^{2})^{2} - (x^{2})^{2} - x^{3} \right)dx^{3}
\end{align*}.$$

Não nos incomodamos em simplificar os termos, talvez possa ficar um pouco mais curto. Se você entender bem estes passos poderá realizar um cálculo como esse sem usar a multiplicação de matrizes. De todo modo este problema pode ser um guia mais detalhado.
```

<br/>

4 - Sejam $a > 0$ e $b > 0$. Considere o mapa $f: \mathbb{R}^{2} \rightarrow \mathbb{R}^{2}$ definido por 

$$f^{1}(x^{1},x^{2}) = 1 + x^{2} - a (x^{1})^{2},\ f^{2}(x^{1},x^{2}) = b x^{1}$$

com as 1-formas diferenciais $df^{1} = dx^{2} - 2 a x^{1} d x^{1},\ df^{2} = b dx^{1}$.

(i) Seja $\Omega = dx^{1} \wedge dx^{2}$. Encontre o pullback de $f$ sobre $\Omega$, ou seja, $f^{*}(\Omega) = f^{*}(dx^{1} \wedge dx^{2})$.

**Solução**:

(ii) Seja $\alpha = x^{1}dx^{2} - x^{2} dx^{1}$. Encontre $f^{*}(\alpha)$.

**Solução**:

(iii) Considere o tensor métrico de $\mathbb{E}^{2}$, $g = dx^{1} \otimes dx^{1} + dx^{2} \otimes dx^{2}$. Encontre $f^{*}(g)$.


**Solução**:







