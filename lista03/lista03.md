# lista03
- João Henrique Schmidt
- 119050097

## Questão 1
**1. Sejam $w_1$ e $w_2$ dois vetores do $\mathbb{R}3$. Mostre que**

$\frac{d}{dt} (w_1 \times w_2) = \dot{w}_1 \times w_2 + w_1 \times \dot{w}_2$

Tem-se que para dois vetores quaisquer $a$ e $b$, o produto vetorial $a\times b$ (eq 1) é:

$\begin{vmatrix}
i & j & k \\
a_i & a_j & a_k \\
b_i & b_j & b_k \\
\end{vmatrix} =
\begin{bmatrix}
a_jb_k - a_kb_j\\
a_kb_i - a_ib_k\\
a_ib_j  -a_jb_i
\end{bmatrix}$

Já a equação 2, $<a,\dot{b}>$ é:

$\begin{vmatrix}
i & j & k \\
a_i & a_j & a_k \\
\dot{b}_i & \dot{b}_j & \dot{b}_k \\
\end{vmatrix} =
\begin{bmatrix}
a_j\dot{b_k} - a_k\dot{b_j}\\
a_k\dot{b_i} - a_i\dot{b_k}\\
a_i\dot{b_j}  -a_j\dot{b_i}
\end{bmatrix}$

E finalmente a equação 3, $<\dot{a},b>$ é:

$\begin{vmatrix}
i & j & k \\
\dot{a}_i & \dot{a}_j & \dot{a}_k \\
b_i & b_j & b_k \\
\end{vmatrix} =
\begin{bmatrix}
\dot{a_j}b_k - \dot{a_k}b_j\\
\dot{a_k}b_i - \dot{a_i}b_k\\
\dot{a_i}b_j  -\dot{a_j}b_i
\end{bmatrix}$

---
Separando em duas diferenças da equação (1):

$
\begin{bmatrix}
a_jb_k - a_kb_j\\
a_kb_i - a_ib_k\\
a_ib_j  -a_jb_i
\end{bmatrix}=
\begin{bmatrix}
a_jb_k \\ 
a_kb_i \\ 
a_ib_j 
\end{bmatrix}-
\begin{bmatrix}
a_kb_j\\
a_ib_k\\
a_jb_i
\end{bmatrix}$

Derivando em função do tempo usando regra do produto:

$
\begin{bmatrix}
a_j\dot{b_k} + \dot{a_j}b_k  \\ 
a_k\dot{b_i} + \dot{a_k}b_i \\ 
a_j\dot{b_i} + \dot{a_j}b_i 
\end{bmatrix}-
\begin{bmatrix}
a_k\dot{b_j} + \dot{a_k}b_j\\
a_i\dot{b_k} + \dot{a_i}b_k\\
a_j\dot{b_i} + \dot{a_j}b_i
\end{bmatrix}=
\begin{bmatrix}
a_j\dot{b_k} \\
a_k\dot{b_i} \\
a_j\dot{b_i} 
\end{bmatrix}+
\begin{bmatrix}
\dot{a_j}b_k  \\ 
\dot{a_k}b_i \\ 
\dot{a_j}b_i 
\end{bmatrix}-
\begin{bmatrix}
a_k\dot{b_j} \\
a_i\dot{b_k} \\
a_j\dot{b_i} \\
\end{bmatrix}-
\begin{bmatrix}
\dot{a_k}b_j\\
\dot{a_i}b_k\\
\dot{a_j}b_i
\end{bmatrix}
$

Reorganizando:

$
\begin{bmatrix}
a_j\dot{b_k} \\
a_k\dot{b_i} \\
a_j\dot{b_i} 
\end{bmatrix}+
\begin{bmatrix}
a_k\dot{b_j} \\
a_i\dot{b_k} \\
a_j\dot{b_i} \\
\end{bmatrix}-
\begin{bmatrix}
\dot{a_j}b_k  \\ 
\dot{a_k}b_i \\ 
\dot{a_j}b_i 
\end{bmatrix}-
\begin{bmatrix}
\dot{a_k}b_j\\
\dot{a_i}b_k\\
\dot{a_j}b_i
\end{bmatrix}=
\begin{bmatrix}
a_j\dot{b_k} + a_k\dot{b_j} \\
a_k\dot{b_i} + a_i\dot{b_k} \\
a_j\dot{b_i} + a_j\dot{b_i} \\
\end{bmatrix}-
\begin{bmatrix}
\dot{a_j}b_k +\dot{a_k}b_j\\
\dot{a_k}b_i +\dot{a_i}b_k\\
\dot{a_j}b_i +\dot{a_j}b_i
\end{bmatrix}
$

Assim, utiliando a equação 2 e 3 nas duas últimas matrizes:

$= a \times \dot{b} - \dot{a} \times b$ 

## Questão 2

Pela fórmula da força gravitacional e força centrípeta:

$\frac{GM_Tm}{r^2} = mg = \frac{mv^2}{r}$

Assim, mult. r e  div. m:

$v^2= \frac{GM_T}{r}$

$\therefore v = \sqrt{\frac{GM_T}{r}}$

## Questão 3

**Uma partícula de massa $m$ move-se de modo que o vetor $r(t)$ satisfaz as
equações**

$\langle r(0) \vert c \rangle = 0 \quad \text{e} \quad \dot{r} = c \times r$

**para um certo vetor constante não nulo $c$. Seja $H$ o plano ortogonal a $c$ que
contém a origem.**

**(a) Mostre que a derivada de $⟨r | c⟩$ em relação ao tempo é nula**

$\frac{d}{dt} r \cdot c = r'c + rc'$

Como $c$ é constante, sua derivada é nula, assim:

$\frac{d}{dt} (r \cdot c) = r'c$

$r' = c \times r \implies$ $c \perp r'$ e $r \perp r'$

**(b) Mostre que r ∈ H e conclua que o movimento é plano**


Sabe-se que $c$ é normal à $H$, e $r(0)$ é perpendicular à normal pelo enunciado,
tornando-o paralelo ao plano.

Como $r' = c \times r$, então $c$ é perpendicular a $r'$

Portanto o vetor inicial e qualquer variação do vetor ocorre sempre perpendicular à $c$, id est, ao plano $H$

**\(c\) Use $r' = c × r$ e a representação $r(t) = r(t) u_r$ na base {$u_r, u_θ$}, para
mostrar que**

**$r' = 0$ e $r' = r θ'u_θ.$**

A base proposta é equivalente a olhar para o problema em relação a particula, isto é,
colocar um observador na particula, que observa o eixo $y$ em direção ao centro de
rotação e eixo $x$ como tangente da rotação.

$r(t) = r(t)u_r + 0u_θ$

$r' = c \times r$

Fazendo em relação a essa base:

$\begin{vmatrix}
u_r & u_θ & u_k \\
0 & 0 & c \\
r & 0 & 0
\end{vmatrix}= 
rcu_θ
$

Pode-se renomear a constante $c$ conforme precisa. Como ele é a velocidade angular,
normlamente usa-se $\omega$, mas precisamos provar usando $\theta'$:

$=r\omega u_\theta = r\theta' u_\theta$

**(d) Mostre que $m$ move-se com velocidade escalar constante em uma órbita
circular.**

Pela matriz de mudança de base:
$\begin{bmatrix}
\cos{θ} && -\sin(θ) \\
\sin{θ} && \cos(θ)
\end{bmatrix}$

Assim:

$\begin{cases}
u_r = u_x\cos(θ) - u_y\sin(θ) \\
u_θ = u_x\sin(θ) + u_y\cos(θ)
\end{cases}$

A equação de posição dada em **\(c\)**

$r(t) = r(t)u_r + 0u_θ =r(t)[u_x\cos(\theta) - u_y\sin(\theta)]$

$r'(t) = r\theta' u_\theta = r\theta'[u_x\sin(\theta) + u_y\cos(\theta)]$

Isto é, na forma vetorial simplificada:

$r(t) = r(\cos(\theta), - \sin(\theta))$

$r'(t) = r\theta'(\sin(\theta),\cos(\theta))$

Pode-se trocar o sinal de $\theta$ para o sentido mais comfortável:

$r(t) = r(\cos(\theta), \sin(\theta))$

$r'(t) = r\theta'(-\sin(\theta),\cos(\theta))$

Portanto, é possível observar que o movimento é de órbita circular

## Questão 4
**Uma bola é chutada com velocidade escalar $v$, do alto de um penhasco de
altura $h$, em uma direção que forma um ângulo $θ$ relativamente à horizontal. Determine:**

**(a) a distância horizontal $x$ e a distância vertical y percorrida pela bola em
função de h, da aceleração da gravidade g, do tempo t e do ângulo θ;**

Usando o Taylor:

$y = y_0 + y't + \frac{y''}{2}t^2 \implies y = h + \sin(\theta)vt - \frac{g}{2}t^2$ (.eq 0)

$x = x_0 + x't + \frac{x''}{2}t^2 \implies x = \cos(\theta)vt$ (.eq 1)

**(b) a fórmula para y em função de x, v, h, g e tan(θ);**

Usando equação 1, tem-se: $t = \frac{x}{\cos(\theta)v}$

$\therefore y 
= h + \frac{\sin(\theta)}{\cos(\theta)}x - \frac{g}{2}\frac{x^2}{\cos^2(\theta)v^2}$
$= h + \tan(\theta)x - \frac{g}{2}\frac{x^2}{v^2}(1 + \tan^2(\theta))$


**\(c\) a distância horizontal percorrida pela bola para um dado valor de θ;**

Basta resolver a equação do segundo grau que forma-se quando $y=0$: 

$0 = h + \tan(\theta)x - \frac{g}{2}\frac{x^2}{v^2}(1 + \tan^2(\theta))$

$x = \left[
-\tan(θ) \pm \sqrt{\tan^2(θ) + 4\frac{gh}{2v^2}(1+\tan^2(θ))}
\right] \frac{-v^2\cos^2(\theta)}{g}$

Div. 2 dentro do $\Delta$:

$= \left[
-\tan(θ) \pm \frac{1}{v}\sqrt{\tan^2(θ) + 2ghv^{-2}(1+\tan^2(θ))}
\right] \frac{-v^2\cos^2(\theta)}{g}$


Removendo secante e cortando -1:

$= \left[
\frac{\sin(θ)}{\cos(θ)} \pm \frac{1}{\cos(θ)}\sqrt{\sin^2(θ) + 2ghv^{-2}}
\right] \frac{v^2\cos^2(\theta)}{g}$

mult. $\cos(\theta)$

$= \left( \sin(θ) \pm \sqrt{\sin^2(θ) + 2ghv^{-2}} \right)\frac{v^2\cos(\theta)}{g}$

**(d) a máxima distância do penhasco que a bola pode cair;**


$x = \left( \sin(θ) \pm \sqrt{\sin^2(θ) + 2ghv^{-2}} \right)\frac{v^2\cos(\theta)}{g}$

Para achar o valor de $\theta$ que máximiza a função, podemos descartar os termos constntes,
pois o problema de maximização é equivalente, isto é, $\theta^*$ será o mesmo.

$Maximizar\ x = \left( \sin(θ) \pm \sqrt{\sin^2(θ) + 2ghv^{-2}} \right)\cos(\theta)$

$\implies Maximizar\ x = \sin(θ)\cos(\theta) \pm \cos(\theta)\sqrt{\sin^2(θ) + 2ghv^{-2}}$

Pode-se multiplicar por qualquer constante também... aqui mult. 2:

$\implies Maximizar\ x = 2\sin(θ)\cos(\theta) \pm 2\cos(\theta)\sqrt{\sin^2(θ) + 2ghv^{-2}}$

Usando $2\sin(θ)\cos(\theta) = \sin(2\theta)$

$\implies Maximizar\ x = \sin(2θ) \pm \sqrt{\sin^2(2θ) + 8ghv^{-2}\cos^2(\theta)}$

Para simplificar, renomea-se $ghv^{-2} = k$

$\implies Maximizar\ x = \sin(2θ) \pm \sqrt{\sin^2(2θ) + 8k\cos^2(\theta)}$

Agora é possível derivar e igualar a 0 mais facilmente.

$\implies 0 = 2\cos(2θ) \pm \frac{4\sin(2θ)\cos(2θ)-16k\cos(θ)\sin(θ)}{2\sqrt{\sin^2(2θ) + 8k\cos^2(\theta)}}$

Simplificando e Div 2:

$\implies 0 = \cos(2θ) \pm \frac{\sin(2θ)\cos(2θ)-4k\cos(θ)\sin(θ)}{\sqrt{\sin^2(2θ) + 8k\cos^2(\theta)}}$

Usando a fórmula novamente:

$\implies 0 = \cos(2θ) \pm \frac{\sin(2θ)\cos(2θ)-2k\sin(2θ)}{\sqrt{\sin^2(2θ) + 8k\cos^2(\theta)}}$

Mult $1/\cos(2\theta)$:

$\implies 0 = 1 \pm \frac{\sin(2θ)-2k\tan(2θ)}{\sqrt{\sin^2(2θ) + 8k\cos^2(\theta)}}$

Mult. pela raiz quadrada e organizando um pouco:

$\implies \sqrt{\sin^2(2θ) + 8k\cos^2(\theta)} = \pm (\sin(2θ)-2k\tan(2θ))$

Quadrado:

$\implies \sin^2(2θ) + 8k\cos^2(\theta) = \sin^2(2θ)+4k^2\tan^2(2θ) - 2k\tan(2θ)\sin(2θ)$

Subt. $sin(2\theta)$

$\implies 8k\cos^2(\theta) = 4(k)^2\tan^2(2θ) - 2k\tan(2θ)\sin(2θ)$

Removendo k e div 2:

$\implies 4\cos^2(\theta) = 2\tan^2(2θ) - \tan(2θ)\sin(2θ)$

Fazendo magia:

$\implies 2\cos^2(\theta) + 2\cos^2(\theta) = 2\tan^2(2θ) - \tan(2θ)\sin(2θ)$
 
Identidade:

$\implies 2 + 2\cos^2(\theta) - 2\sin^2(\theta) = 2\tan^2(2θ) - \tan(2θ)\sin(2θ)$

Usando  formula $\cos^2(x) - \sin^2(x) = cos(2x)$

$\implies 2 + 2\cos(2\theta) = 2\tan^2(2θ) - \tan(2θ)\sin(2θ)$

Fazendo $a = 2\theta$

$\implies 2 + 2\cos(a) = 2\tan^2(a) - \tan(a)\sin(a)$

Mult. $\cos(a)$

$\implies 2\cos(a) + 2\cos^2(a) = 2\tan(a)\sin(a) - \sin^2(a)$

Identidade

$\implies 2\cos(a) + \cos^2(a) + 1 = 2\tan(a)\sin(a)$

Mult. $cos(a)$

$\implies 2\cos^2(a) + \cos^3(a) + \cos(a) = 2\sin^2(a)$

Identidade

$\implies 2\cos^2(a) + \cos^3(a) + \cos(a) = 2 - 2\cos^2(a)$

Organizando

$\implies \cos^3(a) +4\cos^2(a) +\cos(a) - 2=0$

Isolando raiz -1:

$\implies (\cos(a) + 1)(\cos^2(a) +3\cos(a)-2)=0$

Têm-se as reaizes $a = \pi$, $a = arccos(\frac{-3 \pm \sqrt{17}}{4})$

Com isso, temos $\theta = \pi/2$, $\theta = \arccos(\frac{-3\pm\sqrt{17}}{2})/2$ como $\theta^*$

O ângulo $\pi/2$ é minimizador, ele representa a menor distância possível de x.

Já o ângulo $\arccos(\frac{-3-\sqrt{17}}{2})/2$ é negativo e não é desejável

Portanto, o ângulo  $\arccos(\frac{-3+\sqrt{17}}{2})/2$ é o maximizador da função.

Por fim basta substituir na função:

$x = \left( \sin(θ) \pm \sqrt{\sin^2(θ) + 2ghv^{-2}} \right)\frac{v^2\cos(\theta)}{g}$

Mas primeiro, vamos reorganizar um pouco:

$\implies xgv^{-2} = \left( \sin(θ)\cos(θ) \pm \cos(θ)\sqrt{\sin^2(θ) + 2ghv^{-2}} \right)$

Mult. 2:

$\implies 2xgv^{-2} = \left( 2\sin(θ)\cos(θ) \pm 2\cos(θ)\sqrt{\sin^2(θ) + 2ghv^{-2}} \right)$

Usando a fórmula de novo:

$\implies 2xgv^{-2} = \left( \sin(2θ) \pm \sqrt{\sin^2(2θ) + 8ghv^{-2}\cos^2(θ)} \right)$

Sabendo-se que $\cos(2θ) = \frac{-3 +\sqrt{17}}{2}$:

$\implies \cos^2(2θ) = \frac{9+17-6\sqrt{17}}{4} = \frac{13-3\sqrt{17}}{2}$:

$\implies \sin^2(2θ) = \frac{-13+3\sqrt{17}}{2} -1 = \frac{-13+3\sqrt{17}-2}{2} = \frac{-15+3\sqrt{17}}{2}$:

**(e) a tangente do ângulo em que a bola deve ser chutada para que caia o
mais longe possível do penhasco**


## Questão 05

**Suponha que um campo radial varia com o inverso do cubo da distância, de
modo que $F(r) = −(1/r^3)u_r$, em $u_r$ é o vetor radial unitário.**

**(a) Ache a equação que descreve a trajetória de uma partícula que se move
sob este campo tendo $L = (0, 0, 1)$ como momento angular.**

Tem-se: $L = r \times p$ 

$F(r) = \frac{dp}{dt} \implies \frac{-1}{r^3} = \frac{dp}{dt}$

$\implies $
