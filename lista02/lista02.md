# Lista 02 
- João Henrique Schmidt de Carvalho
- 119050097

## Questão 1
**Um barco que está amarrado a um cabo puxado por um carro que se move
na margem de um trecho retilíneo de um canal. A tensão no cabo é igual a
$T$ e o cabo forma um ângulo $α$ com a direção na qual o barco se move. Qual
a força com a qual o barco está sendo puxado?**

Supondo a velocidade distância entre a margem e o barco é mantida, 
i.e, a força resultante é 0, então a única força resultante é paralela à margem
com módulo $T*\cos(\theta)$

## Questão 2
**Quatro partículas de massa $m$ estão situadas nos vértices de um tetraedro
regular cuja aresta mede $a$. Qual a intensidade da força gravitacional exercida
sobre uma das partículas pelas outras três?**

É sabido que ângulo entre os átomos de moléculas tetraedricas é $\arccos(-1/3) \approx 109.5$.
Portanto, visto de dos vertices, o ângulo entre o centro do tetraedro e outro vértice é 
$\alpha = \frac{\pi - \arccos(-1/3)}{2}$. É possível achar isso graças à soma internas 
de triângulos $\pi = \arccos(-1/3) + 2\alpha$

Pela Lei da Gravitação Universal, a força entre duas particulas é $F = \frac{Gm^2}{a^2}$

Portanto, o valor do modulo da força é $F_{res} = 3\cos(\frac{\pi - \arccos(-1/3)}{2})*\frac{Gm^2}{2}$

## Questão 3
**O movimento de uma partícula de massa m, no plano xy, é descrito por
$x = a(αt − \sin(αt))$ e $y = a(1 − \cos(αt))$.**

**$(a)$ Use um computador para desenhar a trajetória da partícula.**

Primeiramente, pode-se escrever $\alpha t$ em função de $y$.

$\alpha t = \arccos(a - y)$

$x = a(\arccos(a-y) - \sin (\arccos(a-y)))$

**$(b)$ Determine o vetor que descreve a força que está agindo sobre a partícula para produzir a trajetória dada.**

Para isso pode-se derivar duas vezes para achar o vetor de aceleração:

$x = a(αt − \sin(αt))$ e $y = a(1 − \cos(αt))$

$\therefore x' = a(α − \cos(αt)α)$ e $y' = a\sin(αt)α$

$\therefore x'' = a\sin(αt)α^2$ e $y'' = a\cos(αt)α^2$

Assim, a força resultante é dado pelo vetor:

$F = m*(a\sin(\alpha t)\alpha^2,a\cos(\alpha t)\alpha^2)$

Isolando os termos:

$F = m*a*\alpha^2(\sin(\alpha t),\cos(\alpha t))$

## Questão 4
**Uma bola de massa $m$ está amarrada em um barbante de comprimento $l$, que
suporta uma tensão máxima igual a $T$. Qual a velocidade máxima com que a
bola pode ser girada em um círculo horizontal sem que o barbante se parta?**

Circulo Horizontal é equivalente a uma mesa ou superficie qualquer, isso é, sem a ação da gravidade.

Pode-se usar a fórmula da força centripeda, que precisa ser igual a Tensão máxima.

A fórmula da força centrípeta: $f_c = T = m * \frac{v^2}{l}$

Assim, $v_{máx} = \sqrt{\frac{l*T}{m}}$

## Questão 5
**Um carrinho de brinquedo é solto do repouso, no ponto mais alto $P$ de uma
rampa de altura $h$. Determine a velocidade mínima que o carrinho deve ter
no ponto $A$ para continuar tocando na superfície do círculo de raio $R$.**

A força mínima necessário é quando a Normal chega a 0, fazendo com que a
força centrípeta seja apenas influência da força gravitacional $mg$, 
ou também que a pseudoforça seja resultante da força gravitacional apenas.

Como no ponto $A$: $f_{cp} = \frac{mv_A^2}{R} = mg$

$\implies v_A^2 = gR$ (1)

Supondo que não haja perda de energia por atrito, tem-se a fórmula de conservação de energia:

$hmg + \frac{mv_P^2}{2} = 2Rmg + \frac{mv_A^2}{2}$

Usando (1):

$hmg + \frac{mv_P^2}{2} = 2Rmg + \frac{mgR}{2}$

Somando $-hmg$:

$\frac{mv_P^2}{2} = 2Rmg + \frac{mgR}{2} - hmg$

m. $2$ e dividindo por $m$:

$v_P^2 = 4Rg + gR - 2hg$

$\therefore v_P = \sqrt{(5R-2h)g}$


## Questão 6 (Versão antiga)

**Uma partícula de massa $m$ move-se ao longo da elipse**

**$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$**

**A aceleração da partícula é paralela ao eixo $y$. Quando $t = 0$, as coordenadas
da partícula são $(0, b)$ e sua velocidade escalar é $v_0$.**

**(a) Determine a velocidade horizontal da partícula em um tempo $t$**

> OBS: Supondo afirmação "A aceleração da partícula é paralela ao eixo $y$" verdadeira apenas no $t=0$

Usando trigonometria:

Como $1  > \frac{x^2}{a^2},\frac{y^2}{b^2} > 0$, pode-se escolher uma 
função trigonométrica que satisfaça a equação.

Pela identidade: $\sin^2(t) + \cos^2(t)= 1$

Assim pode-se reescrever usando as equações iniciais:

$\begin{cases}
\frac{y^2}{b^2} = \cos^2(t) \\
0 = a\sin(0) \\
b = b\cos(0) \\
\end{cases}$

Para achar a velocidade, basta derivar a primeira equação em função do tempo:
$\frac{dx}{dt} = a\cos(t)$

**(b) Use derivação implícita para calcular a velocidade vertical da partícula 
em função de $v_0, x$ e $y$.**

Derivando implicitamente pelo tempo:
$\frac{2x}{a^2}\frac{dx}{dt} + \frac{2y}{b^2}\frac{dy}{dt} = 0$

div. 2 e renomeando as derivadas:

$\frac{x}{a^2}x' + \frac{y}{b^2}y' = 0$

No instante $t=0$, $\frac{b}{b^2}v_y= 0 \implies v_y = 0$

Derivando novamente:

$\frac{x'^2}{a^2} +\frac{x}{a^2}x'' + \frac{y'^2}{b^2} + \frac{y}{b^2}y'' = 0$

Pela questão anterior, é sabido que $y' = -b\sin(t)$

$\therefore y' = \frac{-bx}{a}$

## Questão 6 (Versão nova)

Uma partícula de massa m move-se ao longo da parábola

$y^2 = 2\sqrt{v_0}*x + b$

**A aceleração da partícula é paralela ao eixo y. Quando t = 0, as coordenadas
da partícula são (0, b) e sua velocidade escalar é v0.**

**(a) Determine a velocidade horizontal da partícula em um tempo t.**

Derivando implicitamente:

$2y*\frac{dy}{dx} = 2\sqrt{v_0} \implies \frac{dy}{dx} = \frac{\sqrt{v_0}}{y}$

Explicação da regra da cadeia:

Supondo um valor $y$ em função de $x$: $y=y(x)$. Por sua vez, $x$ é uma função 
do tempo $x=x(t)$. Então podemos dizer que $y$ também pode ser vista como indireta
do tempo, via dependência de $x$: $y(t) = y(x(t))$

Derivando os dois lados e utilizando a regra da cadeia:

$\frac{dy}{dt} = \frac{dy}{dx}\frac{dx}{dt} \implies v_y = \frac{dy}{dx} * v_x
\implies \frac{v_y}{v_x} = \frac{dy}{dx}$

Mas $\frac{dy}{dx} = \frac{\sqrt{v_0}}{y} \implies \frac{\sqrt{v_0}}{y} = \frac{v_y}{v_x}$

No instante $t=0$:

$\frac{\sqrt{v_0}}{b} = \frac{v_y(0)}{v_x(0)}$

Mas pelo pitágoras: $v_0^2 = v_x(0)^2 + v_y(0)^2 \implies v_0^2 - v_x(0)^2 = v_y(0)^2$

Substituindo pela equação elevada ao quadrado:

$\frac{v_0}{b^2} = \frac{v_0^2 - v_x(0)^2}{v_x(0)^2}$

$\implies v_0*v_x(0)^2 = b^2(v_0^2 - v_x(0)^2)$

Dist $b^2$:

$\implies v_0*v_x(0)^2 = b^2*v_0^2 - b^2*v_x(0)^2$

Add $b^2*v_x(0)^2$ 

$\implies v_0*v_x(0)^2 + b^2*v_x(0)^2= b^2*v_0^2$

Isolando:

$\implies v_x(0)^2(v_0 + b^2) = b^2*v_0^2$

Finalmente:

$\implies v_x(0)^2 = \frac{b^2*v_0^2}{v_0 + b^2}$

**(b) Use derivação implícita para calcular a velocidade vertical da partícula
em função de v0 e y.**

Pela questão anterior, podemos chegar a mesma conclusão fora do instante $t=0$

Mas $\frac{dy}{dx} = \frac{\sqrt{v_0}}{y} \implies \frac{\sqrt{v_0}}{y} = \frac{v_y}{v_x}$

Sabemos que a aceleração é paralela ao eixo $y$, isto é $v_x$ é constante.

Portanto o resultado da questão anterior também vale pra outros instantes:

$\implies v_x^2 = \frac{b^2*v_0^2}{v_0 + b^2}$

Substituindo:

$v_y=\frac{\sqrt{v_0}}{y}\sqrt{\frac{b^2*v_0^2}{v_0 + b^2}}$

**\(c\) Use derivação implícita para calcular a velocidade vertical da partícula
em função de v0 e y.**

Pela equação da questão **(a)**:

$v_y= v_x\frac{\sqrt{v_0}}{y}$

Derivando implicitamente:

$a_y = -\frac{1}{y^2}\sqrt{v_0}v_x + \frac{1}{y}\sqrt{v_0}a_x$

Como aceleração é paralela a $y$, então $a_x = 0$

$\implies a_y = -\frac{1}{y^2}\sqrt{v_0}v_x$

Pela letra **(b)**: $v_x^2 = \frac{b^2*v_0^2}{v_0 + b^2}$

$\implies a_y = -\frac{\sqrt{v_0}}{y^2}\sqrt{\frac{b^2*v_0^2}{v_0 + b^2}}$

**(d) Determine a intensidade da força que age sob a partícula em cada ponto
de sua trajetória.**

$F_y = -m\frac{\sqrt{v_0}}{y^2}\sqrt{\frac{b^2*v_0^2}{v_0 + b^2}}$
