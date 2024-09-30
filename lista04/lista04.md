# Modelagem Matemática e Computacional
João Henrique Schmidt de Carvalho

119050097

## Questão 1

**Duas bolas caem verticalmente, separadas por uma pequena distância, com
a bola grande abaixo da pequena. No momento em que a bola grande acerta
o chão, ambas as bolas têm velocidade $−v0$ relativamente ao eixo vertical
que aponta para cima. Ignorando a resistência do ar e supondo os choques
perfeitamente elásticos:**

**(a) qual a velocidade da bola grande imediatamente após o impacto com o
chão?**


Como o choque é perfeitamente elástico $e=\frac{v_{afastamento}}{v_{aproximação}}=1$

Pela conservação de momento:

$Q_{antes} = Q_{depois}$

$\implies Mv = Mv'$

Assim, em módulo: $|\vec{v}| = v_0$ e $\vec{v} = (0,v_0)$

Pela conservação de momento:

$Q_{antes} = Q_{depois}$

$\implies Mv_M + mv_m = Mv_M' + mv_m'$

Com os valores dados:

$Mv_0 + m(-v_0) = Mv_M' + mv_m'$

$v_0(M-m) = Mv_M'+mv_m'$

Mas pelo coeficiente de restituição:

$e = 1 \implies |v_0 - (-v_0)| = |v_M' - v_m'| \implies 2v_0 = |v_M' - v_m'|$

Assim, supondo $|v_m'| < |v_M'|$:

$\begin{cases}
2v_0 = v_M' - v_m' \\
v_0(M-m) = Mv_M'+mv_m'
\end{cases}$

Substituindo $v_M' = 2v_0 + v_m'$ na segunda equação:

$v_0(M-m) = M(2v_0 + v_m')+mv_m'$

$\implies v_0(M-m) = 2Mv_0 + (M+m)v_m'$

$\implies v_0(-M-m) =(M+m)v_m'$

$\implies (M+m)v_m' = v_0(-M-m)$

$\implies v_m' = \frac{-v_0(M+m)}{M+m} = v_0$

$\implies v_M' = 3v_0$


Supondo $|v_m'| > |v_M'|$:

$\begin{cases}
2v_0 = v_m'- v_M' \\
v_0(M-m) = Mv_M'+mv_m'
\end{cases}$

Substituindo $v_M' = v_m' - 2v_0$ na segunda equação:

$v_0(M-m) = M(v_m' - 2v_0)+mv_m'$

$\implies v_0(M-m) = - 2Mv_0 + (M+m)v_m'$

$\implies v_0(3M-m) =(M+m)v_m'$

$\implies (M+m)v_m' = v_0(3M-m)$

$\implies v_m' = \frac{v_0(3M-m)}{M+m}$

$\implies v_M' = \frac{v_0(3M-m)}{M+m} - 2v_0 = \frac{v_0(3M-m) + v_0(-2M-2m)}{M+m}$

$\implies v_M' = \frac{v_0(M-3m)}{M+m}$


