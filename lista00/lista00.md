# Questão 1
Seja R uma rotação de eixo $l$ em $R^3$ e $v = (1, 1, 1)$ um vetor ortogonal a $l$.
Sabendo-se que $Rv = (1, −1, 1)$, determine:

#### (a) o \cosseno do ângulo de rotação de $R$;

O angulo de rotação pode ser determinado pelo produto vetorial entre dois vetores:

$<Rv,v> = ||Rv||*||v||*\cos(\theta) => \cos(\theta) = \frac{<Rv,v>}{||Rv||*||v||}$

$\therefore$

$\cos(\theta) = \frac{1*1 + 1*(-1) + 1*1}{\sqrt{1^2+(-1)^2 + 1^2} * \sqrt{1^2+1^2+1^2}} = \frac{1}{\sqrt{3}*\sqrt{3}} = 1/3$

#### (b) o eixo da rotação $R$;
$l = (a,b,c)$

O eixo $l$ é perpendicular a $v$ e $Rv$, portanto.

$<l,v> = a*1 + b*1 + c*1 = 0 => a+b+c =0$

$<l,Rv> = a*1 + b*(-1) + c*1 = 0 => a-b+c =0$

$\therefore$

$b = 0$ e $a = -c => l = (a,0,-a)$
#### \(c\) a matriz de $R$ na base canônica

$Rv = \begin{bmatrix}
a & b & c\\
d & e & f\\
g & h & i
\end{bmatrix} * v = (1,-1,1)$

$\therefore$

$\begin{cases}
a + b + c = 1\\
d + e + f = -1\\
g + h + i = 1 
\end{cases}$

Pular.

## Questão 2
Seja ρ a rotação do $R^3$ cujo eixo é a reta $⟨(1, 0, −1)⟩$ e que leva
o vetor $(1, 0, 1)$ no vetor $(−7, 8, −7)/9$

#### (a) 
Determine uma base ortonormal β do $R^3$ formada por um vetor ao longo do eixo e dois vetores sobre o plano perpendicular ao eixo.

Se os dois vetores no plano são perpendiculares ao eixo, então o eixo $(1,0,-1)$ é normal ao plano.

Portanto podemos usar a fórmula do plano $ax + by + cz + d = 0$ para normal $n = (a,b,c)$

Portanto para o eixo $(1,0,-1)$, temos $x - z + d = 0$

#### (b) Determine o ângulo de rotação.

Usando a mesma justificativa da questão 1a, temos:

$<(1,0,1),(-7/9,8/9,-7/9)> = ||(1,0,1)||*||(-7/9,8/9,-7/9)||*\cos(\theta)$

$-7/9 -7/9 = \sqrt{2} * \sqrt{\frac{49+49+64}{81}}*\cos(\theta)$

$=> \cos(\theta) = \frac{-14*\sqrt{81}}{9*\sqrt{162*2}} = \frac{-14}{18}$

$=> \theta = \arccos(-7/9)$

#### \(c\) Determine as matrizes $(ρ)_β , M_{βε}, M_{εβ}$ e $(ρ)_ε$.

Pular.

## Questão 3

// TODO: Revisar dps

#### (a) $\int \exp(x)*\sin(\exp(x))dx$
$u = \exp(x) => du = d(\exp(x)) = \exp(x)dx$

$\int \sin(u)*du = -\cos(u) + c = -\cos(\exp(x)) + c$

#### (b) $\int x*\exp(-x^2)dx$
$u = \exp(-x^2) => du = \exp(-x^2)(-2x)dx$

$\int x * \exp(-x^2)dx = -1/2 \int -2x*\exp(-x^2)dx$

$= -1/2 \int du = -1/2 *(u +c) = -1/2(\exp(-x^2) + c)$

$\therefore \int x*\exp(-x^2)dx = -\exp(-x^2)/2 + c$ 

#### \(c\) $\int x*\sqrt{1-x^2}dx$

$\sin(\theta) = x => \sin(\theta)*d\theta = dx$

$\int \sin(\theta)*\sqrt{1 - \sin(\theta)^2}d\theta=\int \sin(\theta)*\sqrt{\cos(\theta)^2}d\theta = \int \sin(\theta)\cos(\theta)d\theta = \int \sin(2\theta)d\theta/2$

$=-\cos(2\theta)/4 + c = 1/4 - 2\sin^2(\theta)/4 + c = 1/4 - x^2/2 + c$

## Questão 4
#### (a) $∫ x^2 e^xdx$

$\begin{cases}
u = x^2 \implies du = 2xdx\\
dv = e^x dx \implies v = e^x
\end{cases}$

$\therefore \int x^2 e^xdx = x^2e^x - 2\int e^x xdx$

$\begin{cases}
u = x \implies du = dx\\
dv = e^x dx \implies v = e^x
\end{cases}$

$\therefore x^2e^x - 2\int e^x xdx = x^2e^x - 2[e^xx - \int e^xdx] = x^2e^x - 2e^xx + e^x$


#### (b) igual a (a)
#### \(c\) $∫ x^2 \sin(x)dx$

$\begin{cases}
u = x^2 \implies du = 2xdx\\
dv = \sin(x) dx \implies v = - \cos(x)
\end{cases}$

$\therefore \int x^2 \sin(x) dx = x^2(-\cos(x)) + 2\int \cos(x)xdx$

$\begin{cases}
u = x \implies du = dx\\
dv = \cos(x) dx \implies v = \sin(x)
\end{cases}$

$\therefore -x^2\cos(x) + 2\int \cos(x)xdx = -x^2\cos(x) + 2[x\sin(x) - \int \sin(x)dx]$

$= -x^2\cos(x) + 2x\sin(x) + \cos(x)$

## Questão 5
#### (a) $\int \frac{dx}{a^2+x^2}$
Pular

$u^2=a^2 + x^2 \implies x = \sqrt{u^2-a^2} \implies dx = \frac{1}{2}(u^2-a^2)*2u*du$

$\therefore \int \frac{dx}{a^2+x^2} = \int \frac{(u^2-a^2)*u*du}{u} = \int (u^2 -a^2)du = \int u^2du - \int a^2 du = \frac{u^3}{3} - ua^2$

#### (b) $\int \frac{dx}{\sqrt{a^2-x^2}}$

$\int \frac{dx}{\sqrt{a^2-x^2}} = \int \frac{dx}{a^2\sqrt{1-x^2/a^2}} = \frac{1}{a^2} \int \frac{dx}{\sqrt{1-x^2/a^2}}$

$\sqrt{a^2-x^2} \ge 0 \implies a^2 \ge x^2 \implies \exists \theta : \sin^2(\theta) = x^2/a^2$

$\sin^2(\theta) = x^2/a^2 \implies \sin(\theta) = x/a$ ou $\sin(-\theta) = x/a$

$\sin(\theta) = x/a \implies a*\cos(\theta)d\theta = dx$

$\therefore \frac{1}{a^2} \int \frac{dx}{\sqrt{1-\sin^2(\theta)}} =\frac{1}{a^2} \int \frac{a*\cos(\theta)*dx}{\cos(\theta)} = \frac{1}{a^2}\int adx = \frac{1}{a^2}*ax + c = \frac{x}{a} + c$

## Questão 6
Use integração por partes duas vezes para mostrar que

$\int \sin^2(x)dx = \frac{x - \sin(x)\cos(x)}{2}$

$\begin{cases}
u = \sin^2(x) \implies du = 2\sin(x)\cos(x)dx\\
dv = dx \implies v = x
\end{cases}$

$\int \sin^2(x)dx = x*\sin^2(x) - \int x*2\sin(x)\cos(x)dx=x\sin^2(x) - \int x\sin(2x)dx$

$\begin{cases}
u = x \implies du = dx\\
dv = \sin(2x)dx \implies v = -\cos(2x)/2
\end{cases}$

$\int  \sin^2(x)dx =x\sin^2(x) - \int x\sin(2x)$

$=x\sin^2(x) - [-x\cos(2x)/2 - \int -\cos(2x)/2 dx]$

$= x\sin^2(x) + x\cos(2x)/2 -\frac{1}{2} \int \cos(2x) dx = x\sin^2(x) + x\cos(2x) - \frac{1}{4} \sin(2x)$

## Questão 7
Pular

Use a substituição $u = h\sin^2(r)$ para mostrar que

$\int \left(\sqrt{\frac{r}{h - r}}\right) dr = h \left( \arcsin\left(\sqrt{\frac{r}{h}}\right) - \sqrt{\frac{r}{h}} \cdot \sqrt{1 - \frac{r}{h}} \right)$

Como $h \ne 0$, é equivalente a provar:

$\int \left(\sqrt{\frac{1}{h^2}\frac{r}{h - r}}\right) dr = \arcsin\left(\sqrt{\frac{r}{h}}\right) -\sqrt{\frac{r(h-r)}{h^2}}$

ou

$\frac{1}{h} \int \left(\sqrt{\frac{r}{h - r}}\right) dr = \arcsin\left(\sqrt{\frac{r}{h}}\right) -\frac{1}{h}\sqrt{r(h-r)}$

Na integral, temos a seguinte restrição que nos dá duas alternativas

$\frac{r}{h-r} \ge 0 \implies$ 

Alternativa 1. $h-r,r \ge 0$

$\implies h>r$ 

$\begin{cases}
u = \sqrt{r} \implies du = \frac{1}{2}r\sqrt{r}dr\\
dv = \frac{1}{\sqrt{h-r}}dr \implies v = 2(h-r)^{1/2}
\end{cases}$

$\int \left(\sqrt{\frac{r}{h - r}}\right) dr =\sqrt{r}*2\sqrt{h-r} - \int 2\sqrt{h-r}*r\sqrt{r}dr$

$=2\sqrt{r(h-r)}- 2\int r\sqrt{r(h-r)}dr$

$sin^2(\theta) = r/h$

Alternativa 2. $h-r,r \le 0$

## Questão 8
Use o método de separação de variáveis para resolver as seguintes equações diferenciais:
#### (a) ẏ = (1 + y)/(1 + t);

$\frac{dy}{dt} = \frac{1+y}{1+t}$

Supondo $y \ne 1$:

$\frac{dy}{1+y} = \frac{dt}{1+t}$

Aplicando integral e resolvendo:

$\int \frac{dy}{1+y} = \int \frac{dt}{1+t}$

$ln|1+y| = ln|1+t| + C$

Exponencial:

$1+y=(1+t)*e^C \implies y = (1+t)*e^C -1$

#### (b) ẏ − 2ty = t;

$\frac{dy}{dt} - 2ty = t$

$\frac{dy}{dt} = t(1-2y)$

$\frac{dy}{1-2y} = t*dt$

$\int \frac{dy}{1-2y} = \int t*dt$

$ln|1-2y| = t^2/2 + C$

Aplicando Exponencial:

$1-2y = e^{t^2/2 + C}$

$y = \frac{1 - e^{t^2/2}}{2}*C'$

#### \(c\) ẏ − tan(t)y = cos(t).
Pular

Para a letra \(c\) use $u = \cos(t)*y$.

$\frac{dy}{dt} - \tan(t)*y = \cos(t)$

$\frac{dy}{dt} = \frac{\sin(t)}{\cos(t)}*y + \cos(t)$

$\frac{dy(\cos(t))}{dt} = \sin(t)*y + \cos^2(t)$

## Questão 9

Determine a solução geral para as seguintes equações:

#### (a) ẍ − 5ẋ + 6x = 0;

Supodo $x(t) = e^{rt} \gt 0$:

$\frac{d^2x}{dt^2} - 5\frac{dx}{dt} + 6x =0 \implies r^2e^{rt} - 5re^{rt} + 6e^{rt} = 0$

$\therefore r^2 - 5r + 6 = (r-3)(r-2) = 0$

Na solução geral:

$x(t) = C_1*e^{2t} + C_2*e^{3t}$


#### (b) ẍ − 4ẋ + 4x = 0;

$\frac{d^2x}{dt^2} - 4\frac{dx}{dt} + 4x =0 \implies r^2e^{rt} - 4re^{rt} + 4e^{rt} = 0$

$\therefore r^2 - 4r + 4 = (r-2)^2 = 0$

Na solução geral:

$x(t) = (C_1+C_2t)e^{2t}$

#### \(c\) ẍ + 2ẋ + 5x = 0

Pular

$\frac{d^2x}{dt^2} + 2\frac{dx}{dt} + 5x =0 \implies r^2e^{rt} + 2re^{rt} + 5e^{rt} = 0$

$\therefore r^2 + 2r + 5 = (r) = 0$

## Questão 10
Ache soluções particulares para as seguintes equações:

$\frac{d^2x}{dt^2} + 2\frac{dx}{dt} + 3x = t^2 + 4t$ 
