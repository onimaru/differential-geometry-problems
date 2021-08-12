# Definições

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

**Categoria**: uma categoria é composta de três coisas:

1. uma classe $\mathcal{O}$, cujos elementos são chamados de objetos;
2. um conjunto $Mor(A,B)$, cujos elementos são chamados de morfismos de $A$ para $B$, onde $A$ e $B$ são dois objetos (ou seja, atribui para cada elemento de $A$ algum elemento de $B$);
3. uma regras que atribui, dados quaisquer objetos $A$, $B$ e $C$, morfismos, $\phi$ de $A$ para $B$ e $\psi$ de $B$ para $C$, um morfismo, escrito $\psi \circ \phi$ ou $\psi \phi$ de $A$ para $C$, chamado de composição de $\phi$ com $\psi$ sujeitos as seguintes condições:
- Associatividade: dados os objetos $A$, $B$, $C$ e $D$, os morfismos $\phi: A \rightarrow B$, $\psi: B \rightarrow C$ e $\lambda: C \rightarrow D$, então $\left( \lambda \circ \psi \right) \circ \phi = \lambda \circ \left( \psi \circ \phi \right)$;
- Existência da identidade: para cada objeto $A$ existe um morfismo $i_{A}$ de $A$ para $A$ (chamado de morfismo de identidade sobre $A$) com a propriedadeL se $\phi: A \rightarrow B \Rightarrow \phi \circ i_{A} = \phi$; se $\mu : C \rightarrow A \Rightarrow i_{A} \circ \mu = \mu$.

Seja $\phi$ um morfismo de $A$ para $B$:

**Monomorfismo**: $\phi$ é um monomorfismo se: dado qualquer objeto $X$ e quaisquer dois morfismos $\alpha$ e $\alpha'$, de $X$ para $A$ tal que $\phi \circ \alpha = \phi \circ \alpha'$, segue que $\alpha = \alpha'$.

**Epimorfismo**: ...