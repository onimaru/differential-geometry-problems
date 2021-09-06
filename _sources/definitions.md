(definitions)=
# Definições

## Mapas

**Mapa**: um mapa $\phi$ é uma regra que atribui para cada $y \in Y$ um $x \in X$, denotado por $\phi: X \rightarrow Y$.
O conjunto $Y$ é chamado de **alcance** (range) do mapa, o conjunto $X$ é chamado de **domínio** de $\phi$ e a **imagem** de $\phi$ é o conjunto $\phi(x) = \lbrace y \in Y | \phi(x) = y,\ \forall x \in X \rbrace$.

**Um-a-um** ou **injetivo**: um mapa é chamado de um-a-um (1-1) se para cada $y \in Y$ existe somente um $x \in X$ tal que para $x, x' \in X, x \ne x' \Longrightarrow f(x) \ne f(x')$.


**Sobrejetivo**: um mapa é chamado de sobrejetivo (onto) se para cada $y \in Y$ existe pelo menos um $x \in X$. É comum
dizer apenas ”$\phi$ é um mapa de $X$ sobre $Y$.”

**Bijetivo**: um mapa é dito bijetivo ou que é uma bijeção se é tanto 1-1 quanto sobrejetivo.

**Correspondência 1-1**: se existe uma bijeção entre dois conjuntos é dito que estes possuem uma correnpondência 1-1.

**Mapa constante**: um mapa é chamado de constante se existe um $y_{0} \in Y$ ﬁxo para um $x \in X$ arbitrário, $\phi(x) = y_{0}$.

**Restrição**: dado um subconjunto $A \subset X$, uma restrição de um mapa $\phi: X \rightarrow Y$ é $\phi|_{A}: A \rightarrow Y$ .

**Mapa composto**: dados os mapas $\phi: X \rightarrow Y$ e $\psi: Y \rightarrow Z$, o mapa composto é $\psi \circ \phi : X \rightarrow Z$, também denotado como $\psi(\phi(x)) = z$.

**Diagrama comutativo**: se os mapas $\lambda \circ \phi : X \rightarrow E$ e $\mu \circ \psi : X \rightarrow E$ são equivalentes se existe um mapa
$\rho : X \rightarrow E$, então dizemos que o diagrama representando estes mapeamentos comutam.

**Mapa de inclusão**: dado um subconjunto $A \subset X$, o mapa $i : A \rightarrow X$ deﬁnido como $i(a) = a\ \forall a \in A$ é
chamado de mapa de inclusão, também denotado como $i : A \xhookrightarrow{} X$.

**Mapa identidade**: dado o mapa de inclusão, se $A = X$ o mapa é chamado de mapa identidade (ou mapa de identidade), $id_{X} : X \rightarrow X$.

**Mapa inverso**: se um mapa $\phi : X \rightarrow Y$ é bijetivo existe um mapa inverso, $\phi^{-1} : Y \rightarrow X$, tal que $\phi^{-1} : \phi(x) \rightarrow x$ é também bijetivo. Como consequência $\phi^{-1} \circ \phi = id_{X}$ e $\phi \circ \phi^{-1} = id_{Y}$.

**Mapa n-ário**: é o mapa $\phi : X^{n} \rightarrow Y$, deﬁnido como $\phi : (x_{1}, x_{2}, ..., x_{n}) \rightarrow y$.

**Mapa de projeção**: é um mapa n-ário $pr_{i} : X_{1} \times X_{2} \times ... \times X_{n} \rightarrow X_{i}$ , deﬁnido como $pr_{i} : (x_{1}, ..., x_{n}) \rightarrow x_{i}$.

**Mapa característico**: dado um subconjunto $A \subset X$, um mapa $\chi_{A} : X \rightarrow {0, 1}$ é dito característico de $A$, deﬁnido como $\chi_{A} (x) = 0$ se $x \notin A$ e $\chi_{A} (x) = 1$ se $x \in A$.

## Espaços Vetoriais

**Anel**: [wikipedia](https://pt.wikipedia.org/wiki/Anel_(matem%C3%A1tica))

**Corpo (Field)**: [wikipedia](https://pt.wikipedia.org/wiki/Corpo_(matem%C3%A1tica))

**Espaço vetorial ou espaço linear**: um espaço vetorial $V$ sobre o campo (ou corpo) $\mathbb{K}$ é um conjunto que possui deﬁnidas as operações de adição e multiplicação por um elemento de $\mathbb{K}$.

**Escalar**: é um elemento de um campo $\mathbb{K}$, usualmente os campos dos $\mathbb{R}$ ou $\mathbb{C}$ são os mais utilizados na física.

**Vetores**: são elementos de um campo vetorial $V$ satisfazendo as seguintes condições:
1. $u + v = v + u$;
2. $(u + v) + w = u + (v + w)$;
3. Existe um vetor nulo $0$ tal que $v + 0 = v$;
4. Para todo $u$ existe a inversa $−u$ tal que $u + (−u) = −u + u = 0$;
5. $c(u + v) = cu + cv$;
6. $(c + d)u = cu + du$;
7. ($cd)u = c(du)$;
8. $1u = u$;  

onde $u, v, w \in V$, $c, d \in K$ e $1$ é o elemento unitário de $\mathbb{K}$.

**Dependência linear**: para $x_{i} \in \mathbb{K}$, $v_{i} \in V$ e $x_{i} v_{i} = 0$. Se existe uma solução não-trivial, $x_{i} \ne 0$, então o conjunto de todos $\lbrace v_{i} \rbrace$ são linearmente independentes. Se existe somente uma solução trivial, $x_{i} = 0$, então o conjunto de todos $\lbrace v_{i} \rbrace$ são linearmente independentes.

**Base**: um conjunto de vetores linearmente independentes $\lbrace e_{i} \rbrace$ é dito ser uma base de um espeço vetorial $V$ se qualquer $v \in V$ pode ser escrito como uma combinação linear de $\lbrace e_{i} \rbrace$, $v = v_{i} e_{i}$.

**Componentes**: dado $v \in V$ e seja $\lbrace e_{i} \rbrace$ a base de $V$. Os elementos $v_{i} \in v$ são ditos ser os componentes de $v$ com respeito a base $\lbrace e_{i} \rbrace$.

**Dimensão**: a dimensão de um espaço vetorial $dimV$ é o número de elementos que compõem a base do espaço vetorial $V$, usualmente denotado como $V = V(n, \mathbb{K})$.

**Mapa linear**: dados dois espaços vetoriais $V$ e $W$ . Um mapa $\phi: V \rightarrow W$ é dito linear se satisfaz:

$$\phi(a_{1} v_{1} + a_{2} v_{2} ) = a_{1} \phi(v_{1} ) + a_{2} \phi(v_{2} ), \forall a_{1} , a_{2} \in \mathbb{K} \text{ e } v_{1} , v_{2} \in V.$$

**Isomorﬁsmo**: um mapa $\phi: V \rightarrow W$ é chamado de isomorﬁsmo se admite inversa.

**Endomorﬁsmo**: um mapa $\phi: V \rightarrow V$ é chamado de endomorﬁsmo.

**Automorﬁsmo**: um isomorﬁsmo de um espaço vetorial sobre si mesmo é chamado de automorﬁsmo, ou seja, é um endomorﬁsmo que admite inversa.

**Imagem**: o subconjunto $\phi(V) \subset W$ é dito ser a imagem de $\phi$, $Im phi$.

**Kernel**: o kernel do mapa $\phi : V → W$, denotado como $ker(\phi)$, é o conjunto $\lbrace v \in V \vert \phi(v) = 0 \rbrace$, onde $0$ é o
elemento neutro de $W$.

**Espaço vetorial dual**: seja $\phi : V \rightarrow \mathbb{K}$, onde $V(n, \mathbb{K})$ tem uma base $\lbrace e_{i} \rbrace$. Temos que para qualquer $v = v^{i} e_{i}$ e $\phi(v^{i} ) = v^{i} \phi(e_{i} )$ devido a linearidade do mapa. O espaço vetorial $\phi(v)$ é chamado de espaço vetorial dual a $V (n, \mathbb{K})$, denotado como $V^{∗} = V^{∗} (n, \mathbb{K})$.

**Base dual**: é a base que gera $V^{∗}$ , denotada como $\lbrace e^{∗i} \rbrace$. É uma função linear de $\lbrace e_{i} \rbrace$, $e^{∗i} (e_{j} ) = \delta_{j}^{i}$.

**Vetor dual**: é o componente de $V^{∗}$, $\phi = \phi_{i} e^{∗i}$.

**Produto interno 1**: a ação de um vetor dual sobre um vetor é chamada de produto interno, $\phi(v) = \phi_{i} e^{∗i} v^{j} e_{j} = \phi_{i} v^{j} (e^{∗i} e_{j}) = \phi_{i} v^{i}$. Este também é denotado como $<,> : V^{∗} \times V \rightarrow \mathbb{K}$.

**Pullback de um mapa**: sejam $\phi$ e $g$ os mapas tais que $\phi : V \rightarrow W$ e $g : W \rightarrow \mathbb{K}$, onde $g \in W^{∗}$. Então o mapa de composição $g \circ \phi = h$, onde $h \in V^{∗}$, ou $h(v) = g(\phi(v))$, onde $v \in V$. Disso temos $\phi^{∗} : W^{∗} \rightarrow V^{∗}$ deﬁnido por $\phi^{∗} : g \mapsto h = \phi^{∗} (g)$. O mapa $h$ é chamado de pullback de $g$ por $\phi^{∗}$.

## Álgebras

**Álgebra**: consiste de um espaço vetorial $\mathcal{A}$ sobre um campo (ou corpo) $\mathbb{K}$ junto com uma lei de composição
ou produto de vetores, $\mathcal{A} \times \mathcal{A} → \mathcal{A}$, denotado por

$$(A, B) \rightarrow AB \in \mathcal{A}\ \ \  (A, B \in \mathcal{A}),$$

que satisfaz um par de leis distributivas:

$$A(aB + bC) = aAB + bAC,\\
(aA + bB)C = aAC + bBC$$

para todos os escalares $a, b \in \mathbb{K}$ e vetores, $A, B$ e $C$. Sendo $O$ o vetor zero e $0$ o zero escalar tem-se

$$OA = (0A)A = 0(AA) = O e AO = A(0A) = 0AA = O.$$

**Derivação em uma álgebra**: uma derivação em uma álgebra $\mathcal{A}$ é um mapa $\theta : \mathcal{A} \rightarrow \mathcal{A}$ satisfazendo

$$\theta(AB) = \theta(A)B + A \theta(B).$$

**Homomorﬁsmo de uma álgebra**: sejam $\mathcal{A}$ e $\mathcal{B}$ qualquer par de álgebras. Um mapa linear $\phi : \mathcal{A} \rightarrow \mathcal{B}$
é chamado de homomorﬁsmo de álgebra se preserva os produtos,

$$\phi(AB) = \phi(A)\phi(B),$$

onde $A,B \in \mathcal{A}$ e $\phi(A), \phi(B) \in \mathcal{B}$.

**Derivação de um homomorﬁsmo**: seja $\phi : \mathcal{A} \rightarrow \mathcal{B}$ um hohomorﬁsmo de álgebras. Então uma
derivação-$\phi$ ou simplesmente $\phi_{∗}$ é um mapa linear $\theta : \mathcal{A} \rightarrow \mathcal{B}$ que satisfaz $\theta(AB) = \theta(A)\phi(B) + \phi(A)\theta(B)$.

**Álgebra graduada**: uma álgebra graduada $\mathcal{A}$ sobre $\mathbb{R}$ é um espaço vetorial graduado $A = \sum_{p \ge 0}A^{p}$ (soma direta), junto com uma estrutura algébrica, tal que $A^{p} \cdot A^{q} \subset A^{p+q}$.

**Álgebra associativa**: se $A(BC) = (AB)C$ para todos $A, B, C \in \mathcal{A}$ a álgebra é dita associativa.

**Álgebra comutativa**: se $AB = BA$ para todos $A, B \in \mathcal{A}$ a álgebra é dita comutativa.

**Álgebra anti-comutativa**: se $u \in A^{p}$, $v \in A^{q}$ e $uv = (−1)^{pq} vu$, então a álgebra $\mathcal{A}$ é dita anti-comutativa.
Se a existe uma identidade e $dim A^{0} = 1$, então $\mathcal{A}$ é chamada de conexa.

**Álgebra dos operadores lineares**: o espaço vetorial $L(V, V)$ dos operadores lineares sobre um espaço vetorial $V$ forma uma álgebra associativa na qual o produto $AB$ é deﬁnido de maneira usual $(AB)u = A(Bu)$. Entretanto esta álgebra não é necessariamente comutativa.

**Álgebra das matrizes n × n reais ou complexas**: o conjunto de todas as matrizes $\mathcal{M}_{n}(\mathbb{K})$, onde o campo pode ser o dos reais ou dos complexos, forma uma álgebra com respeito a multiplicação matricial. Pode-se pensa nesta álgebra como $L(\mathbb{K}_{n}, \mathbb{K}_{n})$ onde $\mathbb{K}_{n}$ é o espaço vetorial dos vetores coluna $n \times 1$.

**Constante de estrutura**: se $\mathcal{A}$ é uma álgebra de dimensão ﬁnita e $E_{1}, E_{2}, ..., E{n}$ é qualquer base, então seja $C_{ij}^{k}$ um conjunto de escalares deﬁnido por

$$E_{i} E_{j} = C_{ij}^{k}E_{k}.$$

Os escalares $C_{ij}^{k} \in \mathbb{K}$, unicamente deﬁnidos como os componentes do vetor $E_{i} E_{j}$ com respeito a base dada
são chamados de constantes de estrutura da álgebra com respeito a base {$E_{i}$}.

**Produto tensorial canônico**: se $\mathcal{A}$ e $\mathcal{B}$ são duas álgebras graduadas, então $\mathcal{A} \otimes \mathcal{B}$ pode ser uma álgebra graduada da forma $(u_{1} \otimes v_{1} )(u_{2} \otimes v_{2} ) = u_{1} u_{2} \otimes v_{1} v_{2}$ para $u_{1} , u_{2} \in \mathcal{A}$ e $v_{1}, v_{2} \in \mathcal{B}$. Esta álgebra é chamada de produto tensorial canônico.

**Produto tensorial antissimétrico**: para as mesmas deﬁnições anteriores outra álgebra possível é
$(u_{1} \otimes v_{1} )(u_{2} \otimes v_{2} ) = (−1)^{q_{1} q_{2}} u_{1} u_{2} \otimes v_{1} v_{2}$, chamada produto tensorial antissimétrico.