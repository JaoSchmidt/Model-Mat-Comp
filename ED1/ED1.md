#### 1. 
$R = (r*\cos(\theta),r*\sin(\theta))$

#### 2. (a) Derivando expressão:

Aplicando a regra do produto nas duas dimensões:

$Vel_x = \frac{dr}{dt}*\cos(\theta) - r*\sin(\theta)\frac{d\theta}{dt}$

$Vel_y = \frac{dr}{dt}*\sin(\theta) + r*\cos(\theta)\frac{d\theta}{dt}$

$\therefore Vel = (\frac{dr}{dt}*\cos(\theta) - r*\sin(\theta)\frac{d\theta}{dt},\frac{dr}{dt}*\sin(\theta) + r*\cos(\theta)\frac{d\theta}{dt})$

#### 2. (b) Dados do problema:

$Vel_x = u - \cos(\theta)*v$

$Vel_y = -\sin(\theta)*v$

$Vel = (u - \cos(\theta)*v, -\sin(\theta)*v)$

#### 3.
Usando as duas expressões obtidas no eixo x:

$Vel_x = \frac{dr}{dt}*\cos(\theta) - r*\sin(\theta)\frac{d\theta}{dt} = u - \cos(\theta)*v$

Simplificando $\frac{dr}{dt} = r'$ e $\frac{d\theta}{dt} = \theta'$:

$Vel_x = r'\cos(\theta) - r\sin(\theta)\theta' = u - v\cos(\theta)$

Usando as duas expressões obtidas no eixo y e simplificando:

$Vel_y = r'\sin(\theta) + r\cos(\theta)\theta' = -v\sin(\theta)$

#### 4.

Têm-se que:

$r' = \frac{dr}{d\theta}*\theta' \implies \frac{r'}{\theta'} = \frac{dr}{d\theta}$

Substituindo na equação de velocidade do eixo x e y:

$\begin{cases}
r'\cos(\theta) - r\sin(\theta)\theta' = u - v\cos(\theta) \\
r'\sin(\theta) + r\cos(\theta)\theta' = -v\sin(\theta)
\end{cases}$

Para tentar isolar o $\theta'$, multiplica por $\sin(\theta)$ e $\cos(\theta)$, respectivamente:

$\begin{cases}
r'\sin(\theta)\cos(\theta) - r\sin^2(\theta)\theta' = u\sin(\theta) - v\sin(\theta)\cos(\theta) \\
r'\sin(\theta)\cos(\theta) + r\cos^2(\theta)\theta' = -v\sin(\theta)\cos(\theta)
\end{cases}$

Ao subtrair as duas equações, tem-se:

1. $r\theta' = -u\sin(\theta) \implies \theta' = \frac{-u\sin(\theta)}{r}$

Para tentar isolar o $r'$, multiplica por $\cos(\theta)$ e $\sin(\theta)$, respectivamente:

$\begin{cases}
r'\cos^2(\theta) - r\sin(\theta)\cos(\theta)\theta' = u\cos(\theta) - v\cos^2(\theta) \\
r'\sin^2(\theta) + r\sin(\theta)\cos(\theta)\theta' = -v\sin^2(\theta)
\end{cases}$

Ao somar as duas equações e usar a identidade trigonométrica, tem-se:

2. $r' = u\cos(\theta) - v$

Ao dividir (2) por (1), tem-se:

$\frac{r'}{\theta'} = \frac{(u\cos(\theta) - v)*r}{-u\sin(\theta)}$

Multiplicando por $\frac{-1}{-1}$:

$= \frac{(v - u\cos(\theta))*r}{u\sin(\theta)}$

$= \frac{v}{u\sin(\theta)} - \frac{u\cos(\theta)*r}{u\sin(\theta)}$

$\therefore \frac{r'}{\theta'} = \frac{dr}{d\theta}= \frac{v}{u}\csc(\theta) - \cot(\theta)*r$

#### 5.

$\frac{dr}{d\theta}+ r\cot(\theta)= \frac{v}{u}\csc(\theta)$

Método do Fator integrante:

$\frac{dr}{d\theta} + r*P(\theta)=Q(\theta)$

Onde $P(\theta) = cot(\theta)$ e $Q(\theta) = \frac{v}{u}\csc(\theta)$:

Fator Integrante:

$FI = e^{\int P(x)dx} \implies FI = e^{\int cot(\theta)d\theta} = e^{\ln(|\sin(\theta)|) + c} = sin(\theta)*C$

Multiplicando $IF = \sin(\theta)*C$ na equação:

$\sin(\theta)\frac{dr}{d\theta}+ r\sin(\theta)\cot(\theta) = \frac{v}{u}\sin(\theta)\csc(\theta)$

$\implies \sin(\theta)\frac{dr}{d\theta}+ r\cos(\theta) = \frac{v}{u}$

Mas pela regra do produto:

$\frac{d(IF*r)}{d\theta} = IF\frac{dr}{d\theta} + \frac{d(IF)}{d\theta}r$

Assim:

$\sin(\theta)\frac{dr}{d\theta}+ r\cos(\theta) = \frac{d(r\sin(\theta))}{d\theta}$

$\implies \frac{d(r\sin(\theta))}{d\theta} = \frac{v}{u}$

Integrando ambos os lados com relação a $\theta$

$\int \frac{d(r\sin(\theta))}{d\theta}d\theta = \int \frac{v}{u}d\theta$

$\implies r\sin(\theta) = \frac{v}{u}\theta$


