8 - Funcional: é uma regra que associa um número a um conjunto de funções: $f_{1}, f_{2}, ... \rightarrow F[f_{1}, f_{2}]$

Variação de um funcional: $\delta F = F[f + \delta f] - F[f]$, onde $\delta f(\vec{x}) = \epsilon \eta(\vec{x})$,onde $\epsilon$ é infinitesimal e $\eta$ é uma função arbitrária.

Derivada de primeira ordem:

$$\frac{d F}{d \epsilon}[f + \epsilon \eta] \vert_{\epsilon = 0} \equiv \int dx_{1} \frac{\delta F[f]}{\delta f(x_{1})} \eta(x_{1}),$$

onde $\frac{\delta F[f]}{\delta f(x_{1})}$ é a derivada funcional de primeira ordem.



**Categoria**: uma categoria é composta de três coisas:

1. uma classe $\mathcal{O}$, cujos elementos são chamados de objetos;
2. um conjunto $Mor(A,B)$, cujos elementos são chamados de morfismos de $A$ para $B$, onde $A$ e $B$ são dois objetos (ou seja, atribui para cada elemento de $A$ algum elemento de $B$);
3. uma regras que atribui, dados quaisquer objetos $A$, $B$ e $C$, morfismos, $\phi$ de $A$ para $B$ e $\psi$ de $B$ para $C$, um morfismo, escrito $\psi \circ \phi$ ou $\psi \phi$ de $A$ para $C$, chamado de composição de $\phi$ com $\psi$ sujeitos as seguintes condições:
- Associatividade: dados os objetos $A$, $B$, $C$ e $D$, os morfismos $\phi: A \rightarrow B$, $\psi: B \rightarrow C$ e $\lambda: C \rightarrow D$, então $\left( \lambda \circ \psi \right) \circ \phi = \lambda \circ \left( \psi \circ \phi \right)$;
- Existência da identidade: para cada objeto $A$ existe um morfismo $i_{A}$ de $A$ para $A$ (chamado de morfismo de identidade sobre $A$) com a propriedadeL se $\phi: A \rightarrow B \Rightarrow \phi \circ i_{A} = \phi$; se $\mu : C \rightarrow A \Rightarrow i_{A} \circ \mu = \mu$.

Seja $\phi$ um morfismo de $A$ para $B$:

**Monomorfismo**: $\phi$ é um monomorfismo se: dado qualquer objeto $X$ e quaisquer dois morfismos $\alpha$ e $\alpha'$, de $X$ para $A$ tal que $\phi \circ \alpha = \phi \circ \alpha'$, segue que $\alpha = \alpha'$.

**Epimorfismo**: ...