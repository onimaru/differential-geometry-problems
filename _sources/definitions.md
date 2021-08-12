# Definições

**Mapa**: um mapa $\phi$ é uma regra que atribui para cada $y \in Y$ um $x \in X$, denotado por $\phi: X \rightarrow Y$.
O conjunto $Y$ é chamado de **alcance** (range) do mapa, o conjunto $X$ é chamado de **domínio** de $\phi$ e a **imagem** de $\phi$ é o conjunto $\phi(x) = \lbrace y \in Y | \phi(x) = y, \forall x \in X \rbrace$.

**Um-a-um**: um mapa é chamado de um-a-um (1-1) se para cada $y \in Y$ existe somente um $x \in X$ tal que para $x, x' \in X, x \ne x' \Longrightarrow f(x) \ne f(x')$.


**Sobrejetivo**: um mapa é chamado de sobrejetivo se para cada $y \in Y$ existe pelo menos um $x \in X$. É comum
dizer apenas ”$\phi$ é um mapa de $X$ sobre $Y$.”

**Bijetivo**: um mapa é dito bijetivo ou que é uma bijeção se é tanto 1-1 quanto sobrejetivo.

**Correspondência 1-1**: se existe uma bijeção entre dois conjuntos é dito que estes possuem uma correnpondência 1-1.

**Mapa constante**: um mapa é chamado de constante se existe um $y_{0} \in Y$ ﬁxo para um $x \in X$ arbitrário, $\phi(x) = y_{0}$.


**Categoria**: uma categoria é composta de três coisas:

1. uma classe $\mathcal{O}$, cujos elementos são chamados de objetos;
2. um conjunto $Mor(A,B)$, cujos elementos são chamados de morfismos de $A$ para $B$, onde $A$ e $B$ são dois objetos (ou seja, atribui para cada elemento de $A$ algum elemento de $B$);
3. uma regras que atribui, dados quaisquer objetos $A$, $B$ e $C$, morfismos, $\phi$ de $A$ para $B$ e $\psi$ de $B$ para $C$, um morfismo, escrito $\psi \circ \phi$ ou $\psi \phi$ de $A$ para $C$, chamado de composição de $\phi$ com $\psi$ sujeitos as seguintes condições:
- Associatividade: dados os objetos $A$, $B$, $C$ e $D$, os morfismos $\phi: A \rightarrow B$, $\psi: B \rightarrow C$ e $\lambda: C \rightarrow D$, então $\left( \lambda \circ \psi \right) \circ \phi = \lambda \circ \left( \psi \circ \phi \right)$;
- Existência da identidade: para cada objeto $A$ existe um morfismo $i_{A}$ de $A$ para $A$ (chamado de morfismo de identidade sobre $A$) com a propriedadeL se $\phi: A \rightarrow B \Rightarrow \phi \circ i_{A} = \phi$; se $\mu : C \rightarrow A \Rightarrow i_{A} \circ \mu = \mu$.

Seja $\phi$ um morfismo de $A$ para $B$:

**Monomorfismo**: $\phi$ é um monomorfismo se: dado qualquer objeto $X$ e quaisquer dois morfismos $\alpha$ e $\alpha'$, de $X$ para $A$ tal que $\phi \circ \alpha = \phi \circ \alpha'$, segue que $\alpha = \alpha'$.

**Epimorfismo**: ...