# Formulario estadística 

## Tema 1 

**Leyes de Morgan:**
$\overline{A\cup B}= \overline{A}\cap \overline{B}$;
$\overline{A\cap B} = \overline{A} \cup \overline{B}$.\
**Probabilidad condicionada:** $P(A|B)=\frac{P(A\cap B)}{P(B)}$.\
**Ley Multiplicativa para probabilidades condicionadas:**
$P(A\cap B)= P(B)P(A|B)=P(A)P(B|A)$.\
**Sucesos independientes:** $P(A|B)=P(A)$; $P(A\cap B)=P(A)P(B)$.

## Tema 2 

Para variables aleatorias discretas se define la **función de
probabilidad** $P_i= P(X=i), i\in I$, que satisface 1)
$P_i= P(X=i)\geq 0, i\in I$ y 2)
$\sum_{i \in I} P_i= \sum_{i \in I} P(X=i) = P(\Omega)=1$.\
Para variables aleatorias continuas cuando su **función de
distribución** $F(x)$ es continua. En ese caso, existe una función de
desidad $f(x)$ tal que $\forall x \in  \mathbb{R}$
$F(x)= \int_{-\infty}^x f(s)ds \Leftrightarrow \frac{\partial}{\partial x}F(x)=f(x)$
y verifica 1)$f(x)\geq 0$, $\forall x \in  \mathbb{R}$ y
2)$\int_{-\infty}^{\infty} f(x)dx =1$.

## Tema 3 

**Esperanza de una distribución discreta:**
$E(X)=\sum_{i \in I} iP(X=i)$.\
**Esperanza de una distribución continua:**
$E(X)= \int_{-\infty}^{\infty}xf(x)dx$.\
Propiedades de la esperanza: 1)Sea $Y=aX+b$ entonces $E(Y)=aE(X)+b$ y
2)$E(XY)\neq E(X)E(Y)$, a excepción de que X e Y sean independientes.\
**Varianza:** $Var(X)=E(X^2)-E^2(X)$\
Propiedades de la varianza: 1)$Var(X)=0\Leftrightarrow$ existe una
constante $c$ tal que $P(X=c)=1$, 2)sea $Y=aX+b$ entonces
$Var(Y)=a^2Var(X)$ y 3)$Var(-X)=Var(X)$.\
**Función generatriz:** considerando una variable aleatoria X, para cada
número real $t$ se define $\Psi (t)=E(e^{tX})$. Donde $\Psi'(0)=E(X)$,
$\Psi''(0)=E(X^2)$, \...\
**Función característica:** considerando una variable aleatoria X, para
cada número real $t$ se define la función compleja
$\varphi_X (t)=E(e^{itX})$.\
Saber que la función característica es función generatriz de momentos:
$EX^n= \frac{\varphi^{n)}_X(0)}{i^n}$.

## Tema 4 

**Función de probabilidad conjunta:**
$P_{i,j}=P(X=i, Y=j),  i\in I, j\in J$.\
Propiedades de la función de probabilidad conjunta: 1)
$P_{i,j}=P(X=i, Y=j)\geq 0,  i\in I, j\in J$ y 2)
$\sum_{i\in I}\sum_{j\in J}P(X=i, Y=j)=1$.\
Probabilidades marginales: $P(X=i)=\sum_{j\in J}P(X=i, Y=j)$ si
$i \in I$ y $P(Y=j)=\sum_{i\in I}P(X=i, Y=j)$ si $j \in J$.\
Distribución condicionada:
$P(X=i|Y=j_0)=\frac{P(X=i, Y=j_0)}{P(Y=j_0)}$.\
**Independencia de X e Y:** X e Y son independientes si y solo si
$\forall i \in I, \forall j \in J, P(X=i, Y=j)=P(X=i)P(Y=j)$.\
**Función de densidad/distribución conjunta:**
$F(x,y)= \int_{-\infty}^x \int_{-\infty}^y f(s,t)dsdt \Leftrightarrow \frac{\partial^2}{\partial x \partial y}F(x,y)=f(x,y)$.\
Propiedades: 1) $f(x,y)\geq 0,  \forall x,y \in \mathbb{R}$ y 2)
$\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} f(x,y)dxdy=1$.\
Probabilidades marginales: $f(x)=\int_{-\infty}^{\infty} f(x,y)dy$ y
$f(y)=\int_{-\infty}^{\infty} f(x,y)dx$.\
Distribución condicionada: $f_{X|Y=y_0}(x)=\frac{f(x,y_0)}{f(y_0)}$.\
**Independencia de X e Y:** X e Y son independientes si y solo si
$\forall x,y \in \mathbb{R}, F(x,y)=F(x)F(y)$ y $f(x,y)=f(x)f(y)$.\

## Tema 5 

**Covarianza:** Cov(X,Y)=EXY-EXEY.\
Propiedades de la covarianza: 1)es simétrica $Cov(X,Y)=Cov(Y,X)$, 2)si X
e Y son independientes $Cov(X,Y)=0$ (su recíproco no es cierto), 3)la
covarianza es bilineal
$Cov(aX_1+bX_2+c, dX_3+eX_4+f)=adCov(X1,X3)+aeCov(X_1,X_4)+bdCov(X_2,X_3)+beCov(X_2,X_4)$,
4)$Cov(X,X)=Var(X)$,
5)$Var(aX+bY)=Cov(aX+bY,aX+bY)=a^2Var(X)+b^2Var(Y)+2abCov(X,Y)$ y
6)$Cov(X,Y)$ toma valores positivos, negativos y nulos.\
**Coeficiente de correlación:**
$\rho (X,Y)=\frac{Cov(X,Y)}{\sqrt{Var(x)}\sqrt{Var(Y)}}$.\
Propiedades de la correlación: 1)$|\rho(aX+b, cY+d)|=\rho(X,Y)$,
positiva si $ac>0$ y negativa si $ac<0$, 2)$\rho(X,Y) \in [-1,1]$ y 3)si
X e Y son independientes $\rho(X,Y)=0$ (su recíproco no es cierto).\
**Razón de correlación:**
$\eta^2=\frac{b^2}{S^2}=\frac{\sum_{i=1}^n (\bar{y}_i-\bar{y})^2}{\sum_{i=1}^n(y_i-\bar{y})^2}$.\
Propiedades: 1) $\eta^2 \in (0,1)$, 2) $\eta_{Y|X}^2=0$ si y solo si la
curva de regresión $Y$ sobre $X$ es $y=E(Y)$, 3) $\eta_{Y|X}^2=1$ si y
solo si $Y$ depende funcionalmente de $X$ y 4)
$\eta_{Y|X}^2=\eta_{x|Y}^2$ si y solo si hay dependencia funcional
recíproca entre $X$ e $Y$.\
Relación con el coeficiente de correlación lineal:
1)$0\leq\rho^2_{x,y}\leq\eta^2_{Y|X}\leq1$ y 2) si
$\rho^2_{y,x}=\eta^2_{Y|X}$ entonces la curva de regresión $Y$ sobre $X$
y recta de regresión $Y$ sobre $X$.\
\*NOTA: lo mismo ocurre, tanto en las propiedades como en la relación,
con la curva $X$ sobre $Y$.

## Tema 6 

Reproductividad de una distribución:
$\varphi_{X-1+X_2+...+X_n}(t)=E(e^{it(X_1+X_2+...+X_n)})=\prod_{j=1}^n E(e^{itx_j})=\prod_{j=1}^n \varphi _{X_j}(t)$.\
**Distribución $\chi^2$:** Si $X \rightarrow  N(0,1)$ e $Y=X^2$ entonces
$Y \rightarrow \chi^2_1 \equiv \Gamma(\frac{1}{2},\frac{1}{2})$.
Generalizando la última equivalencia, si $Y=\sum_{i=1}^n X_i^2$ entonces
$Y \rightarrow  \chi ^2_n \equiv \Gamma(\frac{n}{2}, \frac{1}{2})$.\
**Distribución T de Student:** si $X \rightarrow  N(0,1)$ e
$Y \rightarrow \chi^2_n$ se puede contruir
$T=\frac{X}{\sqrt{\frac{Y}{n}}}$ que por definición $T\rightarrow t_n$.\
**Distribución F de Snedecor:** si $X_1 \rightarrow \chi^2_n$ y
$X_2 \rightarrow \chi^2_m$ se puede construir
$F=\frac{\frac{X_1}{n}}{\frac{X_2}{m}}$ que por definición
$F \rightarrow F_{m,n}$. Saber que si $T \rightarrow t_n$ entonces
$T^2 \rightarrow F_{1,n}$.

## Tema 7 

**Estadístico suficiente, criterio de factorización:** sea $X_1...X_n$
una muestra aleatoria simple con $f(x,\theta)$ con $\theta \in \Theta$ y
desconocida, $T=T(X_1...X_n)$ es un estadistico suficiente para $\theta$
si $f(x_1...x_n,\theta)=h(x_1...x_n)g(x_1...x_n,\theta)$.\
Estadísticos conjuntamente suficientes: $T_1...T_k$ son estadísticos
suficientes para $\theta$ si, y solo sí,
$f(x_1...x_n,\theta)=h(x_1...x_n)g[T_1(x_1...x_n)...T_k(x_1...x_n),\theta]$.\
Estadístico suficiente minimal: T es un estadístico minimal suficiente
si es un estadístico suficiente y es una función de cualquier otro
estadístico suficiente.

## Tema 8 

Propiedades de los estimadores: 1) sesgo, 2)consistencia y 3)
eficiencia.\
Estimador invariante: $\hat{f(\theta)}=f(\hat{\theta})$.\
**Estimación máximo verosímil, ecuación de verosimilitud:**
$\frac{\partial}{\partial\theta}ln f(x_1...x_n, \theta)=0$. En el caso
de la invarianza del EMV podemos decir que el EMV de $g(\theta)$ es $g$
del EMV de $\theta$.

## Tema 9 

**Estimador insesgado**: sea T un estimador de $\theta$, este será
insesgado si $ET=\theta$.\
Error cuadrático medio: $ECM(T)= E(T-\theta)^2$\
Estimador suficiente, Criterio de factorización de Neyman y Fisher: sea
$X_1...X_n$ mas de $X$ con distribución $f(X,\theta)$,
$\theta desconocido$. T es es un estadístico suficiente para estimar
$\theta$ si $f(x_1..x_n, \theta)=g(t, \theta)h(x_1..x_n, \theta)$.\
**Cota de Cramèr-Rao**: $VarT \geq \frac{(1+b'(\theta))^2}{I_n(\theta)}$
donde
$I_n(\theta)=-E[\frac{\partial^2}{\partial^2 \theta}lnL(x, \theta)]$.

## Tema 10 

**Contraste de hipótesis simple:**
$H_0: \theta=\theta_0; H_1: \theta=\theta_1$.\
Sea una regla de decisión para este contraste y C la correspondiente
región crítica se tiene:\
Error de tipo I: rechazar $H_0$ siendo cierta $\alpha=p_{H_0}(C)$.\
Error de tipo II: rechazar $H_1$ siendo cierta
$\beta=p_{H_1}(\bar{C})$.\
**Contrastes de hipótesis compuestos: unilaterales y no unilaterales.**\
Contraste unilateral: $H_0: \theta<\theta_0; H_1: \theta>\theta_0$ o
bien $H_0: \theta>\theta_0; H_1: \theta<\theta_0$.\
Sea una regla de decisión para este contraste y C la correspondiente
región crítica se tiene:\
Potencia del test: $\pi(\theta)=1-\beta(\theta)$.\
Contraste no unilateral:
$H_0: \theta \in \Theta_0; H_1: \theta \in \Theta_1$.\
**Principales contrastes de hipótesis**:\
$H_0: \mu=\mu_0$ con $\sigma$ conocida:
$C=\{| \bar{X}-\mu_0|>z_\frac{\alpha}{2}\frac{\sigma}{\sqrt{n}}\}$.\
$H_0: \mu=\mu_0$ con $\sigma$ desconocida:
$C=\{| \bar{X}-\mu_0|>t_{n-1;\frac{\alpha}{2}}\frac{S}{\sqrt{n}}\}$.\
$H_0: \mu\leq \mu_0$ con $\sigma$ conocida:
$C=\{\bar{X}-\mu_0>z_\frac{\alpha}{2}\frac{\sigma}{\sqrt{n}}\}$.\
$H_0: \mu\leq\mu_0$ con $\sigma$ desconocida:
$C=\{\bar{X}-\mu_0>t_{n-1;\frac{\alpha}{2}}\frac{S}{\sqrt{n}}\}$.\
$H_0: \mu\geq \mu_0$ con $\sigma$ conocida:
$C=\{\bar{X}-\mu_0<z_\frac{\alpha}{2}\frac{\sigma}{\sqrt{n}}\}$.\
$H_0: \mu\geq\mu_0$ con $\sigma$ desconocida:
$C=\{\bar{X}-\mu_0<t_{n-1;\frac{\alpha}{2}}\frac{S}{\sqrt{n}}\}$.\
$H_0: \sigma= \sigma_0$:
$C=\{\frac{n-1}{\sigma^2_0}S^2 \notin (\chi^2_{n-1; 1-\frac{\alpha}{2}}, \chi^2_{n-1;\frac{\alpha}{2}})\}$.\
$H_0: \sigma \leq \sigma_0$:
$C=\{\frac{n-1}{\sigma^2_0}S^2 > \chi^2_{n-1; \alpha}\}$.\
$H_0: \sigma \geq \sigma_0$:
$C=\{\frac{n-1}{\sigma^2_0}S^2 < \chi^2_{n-1; 1-\alpha}\}$.\
Poblaciones normales independientes: $H_0: \mu_1=\mu_2$ con
$\sigma_1, \sigma_2$ conocidas:
$C=\{|\bar{X}-\bar{Y}|>z_\frac{\alpha}{2}\sqrt{\frac{\sigma^2_1}{n_1}+\frac{\sigma^2_2}{n_2}}\}$.\
$H_0: \mu_1=\mu_2$ con $\sigma_1= \sigma_2$:
$C=\{|\bar{X}-\bar{Y}|>t_{n_1+n_2-2;\frac{\alpha}{2}}s_p\sqrt{\frac{1}{n_1}+\frac{1}{n_2}}\}$
con $s_p=\frac{(n_1-1)s^2_1+(n_2-1)s^2_2}{n_1+n_2-2}$.\
$H_0: \mu_1=\mu_2$ con $\sigma_1 \neq \sigma_2$:
$C=\{|\bar{X}-\bar{Y}|>t_{f;\frac{\alpha}{2}}\sqrt{\frac{s^2_1}{n_1}+\frac{s^2_2}{n_2}}\}$
con f=entero mas cercano a
$\frac{(\frac{s^2_1}{n_1}+\frac{s^2_2}{n_2})^2}{\frac{(\frac{s^2_1}{n_1})^2}{n_1-1}+\frac{(\frac{s^2_2}{n_2})^2}{n_2-1}}$.\
$H_0: \sigma_1=\sigma_2$:
$C=\{ \frac{s^2_1}{s^2_2} \notin (F_{n_1-1, n_2-1,1-\frac{\alpha}{2}}, F_{n_1-1, n_2-1,\frac{\alpha}{2}})\}$.\
$H_0: \sigma_1\leq \sigma_2$:
$C=\{ \frac{s^2_1}{s^2_2} > F_{n_1-1, n_2-1,\alpha}\}$.\
$H_0: \sigma_1\geq \sigma_2$:
$C=\{ \frac{s^2_1}{s^2_2} < F_{n_1-1, n_2-1,1-\alpha}\}$.\
Comparación de proporciones.\
$H_0: p_1=p_2$:
$C=\{|\bar{X}-\bar{Y}|> z_\frac{\alpha}{2}\sqrt{\bar{p}(1-\bar{p})(\frac{1}{n_1}+\frac{1}{n_2})}\}$.

## Tema 11 

**Intervalos de confianza para $\mu$**.\
Con $\sigma$ conocida:
$I=(\bar{x}\pm z_\frac{\alpha}{2} \frac{\sigma}{\sqrt{n}})$.\
Con $\sigma$ desconocida:
$I=(\bar{x}\pm t_{n-1;\frac{\alpha}{2}} \frac{s}{\sqrt{n}})$.\
**Intervalo de confianza para $\sigma^2$**.\
Con $\mu$ conocida:
$I=(\frac{\sum_{i=1}^n (X_i-\mu_0)^2}{\chi_{n; \frac{\alpha}{2}}}, \frac{\sum_{i=1}^n (X_i-\mu_0)^2}{\chi_{n;1- \frac{\alpha}{2}}})$\
Con $\mu$ desconocida:
$I=(\frac{(n-1)s^2}{\chi^2_{n-1; \frac{\alpha}{2}}}, \frac{(n-1)s^2}{\chi^2_{n-1; 1- \frac{\alpha}{2}}})$.\
**Intervalo de confianza para $\mu_1=\mu_2$**.\
Con $\sigma_1, \sigma_2$ conocidas:
$I=(\bar{x}-\bar{y} \pm z_\frac{\alpha}{2}\sqrt{\frac{\sigma^2_1}{n_1}+\frac{\sigma^2_2}{n_2}})$.\
Con $\sigma_1, \sigma_2$ desconocidas e iguales:
$I=(\bar{x}-\bar{y} \pm t_{n_1+n_2-2;\frac{\alpha}{2}}s_p\sqrt{\frac{1}{n_1}+\frac{1}{n_2}})$.\
Con $\sigma_1, \sigma_2$ desconocidas y diferntes:
$I=(\bar{x}-\bar{y} \pm t_{f;\frac{\alpha}{2}}\sqrt{\frac{s^2_1}{n_1}+\frac{s^2_2}{n_2}})$.\
**Intervalo de confianza para $\frac{\sigma_1^2}{\sigma_2^2}$**:
$I=(\frac{\frac{s^2_1}{s^2_2}}{F_{n_1-1;n_2-1;\frac{\alpha}{2}}}, \frac{\frac{s^2_1}{s^2_2}}{F_{n_1-1;n_2-1;1-\frac{\alpha}{2}}})$.\
**Intervalo de confianza para $p_1-p_2$**:
$I=(\hat{p_1}-\hat{p_2}\pm z_\frac{\alpha}{2}\sqrt{\frac{\hat{p_1}(1-\hat{p_1})}{n_1}+{\frac{\hat{p_2}(1-\hat{p_2})}{n_2}}})$.

## Tema 12 

**Variable cualitativa:** toman valores de $x$ que no se pueden ordenar
de forma lógica o natural.\
**Variable cuantitativa:** representa cantidades que se pueden medir, se
pueden ordenar de forma lógica y natural.\
**Escala nominal:** los valores de una variable nominal no se pueden
ordenar. Por ejemplo: sexo (H/M)\
**Escala ordinal:** los valores de una variable ordinal sí se pueden
ordenar. Por ejemplo: nivel educativo (ninguno, Primaria, ESO,
Bachillerato, Universidad).\
**Elementos de una distribución de frecuencias**\
Frecuencia absoluta $n_j$: nº de observaciones en una categoría.
($n_1+...+n_i=n$)\
Frecuencia relativa $f_j$: peso de la categoría. ($f_i=n_i/n$)\
Frecuencia acumulada $F_j$: suma sucesiva de frecuencia absoluta o
relativa, desde el menor al mayor de sus valores.\
**Función de distribución para variables continuas:**
$F(x)= \left\{ \begin{array}{lcc}
             0 &   si  & x < e_0 \\
             \\ F(e_j)+\frac{f_j}{d_j}(x-e_{j-1}) &  si  & x \in [e_{j-1}, e_j) \\
             \\ 1 &  si  & x \geq e_k
             \end{array}
   \right.$ Donde $d_j=e_j-e_{j-1}$ es la amplitud del intervalo y,
$e_{j-1}$ y $e_j$ son los límites inferior y superior respectivamente.\
**Representación gráfica**\
1. Gráfico de barras. Herramienta sencilla para la visualización de
frecuencias absolutas o relativas. Se puede usar tanto para variables
nominales como ordinales, siempre y cuando el nº de categorías no sea
muy grande.\
2. Gráfico de sectores. Visualización de frecuencias absolutas o
relativas de variables nominales y ordinales. El tamaño del sector viene
dado por $f_j*360$º. Tener en cuenta que cada sector no es proporcional
a la frecuencia absoluta de cada sector, pero el ángulo sí.\
3. Histograma. Usado especialmente en la discretización de variables
continuas, ya que el número de categorías resultantes probablemente sea
muy alto y el gráfico de barras no sea la mejor opción. La altura de
cada barra viene dada por $h_j=\frac{n_j}{d_j}$.

## Tema 13 

**Medidas de posición**\
1. Media aritmética. $\bar{x}=\frac{\sum_{i=1}^n x_i}{n}$.\
Media aritmética ponderada (tabla de distribución de frecuencias).
$\bar{x}=\frac{\sum_{i=1}^n n_im_i}{n}=\sum_{i=1}^n f_im_i$ donde $m_i$
es el valor medio de clase $m_i=\frac{e_j-e_{j-1}}{2}$.\
2. Media geométrica.
$\bar{x}_G= \sqrt[n]{\prod_{i=1}^n x_i}= (\prod_{i=1}^n x_i)^{\frac{1}{n}}=\sqrt[n]{x_1*x_2*...*x_n}$.
Tener cuidado con si alguna observación es 0.\
Usos: formalización de porcentajes, por ejemplo rentabilidad de una
empresa, factor de crecimiento, tasa de crecimiento.\
3. Media armónica. $\bar{x}_H= \frac{n}{\sum_{i=1}^n \frac{1}{x_i}}$.\
Uso: típicamente cuando hay diferentes valores $x_i$ que contribuyan a
la media cada uno de ellos con diferentes pesos $w_i$.

## Tema 14 

**Medidas de posición robustas**\
1. Mediana. Es aquel número tal que, ordenados los datos de forma
creciente, la mitad son inferiores a dicho valor y la otra mitad son
superiores.

-   Distribución de frecuencias unitarias. Si N es par Me será
    $X_{(N/2)}$, si N es impar entonces Me será la media aritmética de
    los valores centrales.

-   Distribución de frecuencias no unitarias. Si $N_i$ es la primera
    frecuencia absoluta acumulada igual o superior a N/2, entonces:
    $\left\{\begin{array}{lcc}
        Me=x_i & si & N_{i-1}<\frac{N}{2}<N_i\\
        \\ Me= \frac{x_i+x_{i+1}}{2} & si & N_i=N/2
        \end{array}
    \right.$

-   Distribución de frecuencias agrupadas.
    $Me= L_{i-1}+c_i\frac{\frac{N}{2}-N_{i-1}}{n_i}$.

2\. Moda. Es el valor de la variable con mayor frecuencia.

-   Distribución de frecuencias sin agrupar. Se calcula la moda
    fijándose en el valor de la variable que más se repite (es decir, el
    de mayor frecuencia).

-   Distribución de frecuencias agrupadas.
    $Mo= L_{i-1}+c_i\frac{h_{i+1}}{h_{i-1}+h_{i+1}}$ siendo
    $h_j=\frac{n_j}{c_j}$.

3\. Cuantiles. Son aquellos valores de la disrbución que dividen la
distribución en $k$ partes, conteniendo en cada uno de ellas la misma
proporción de observaciones, habiendo sido previamente ordenadas las
observaciones.

-   Distribución de frecuencias sin agrupar. $\left\{\begin{array}{lcc}
        C_\frac{s}{k}=x_i & si & N_{i-1}<\frac{sN}{k}<N_i\\
        \\ C_\frac{s}{k}= \frac{x_i+x_{i+1}}{2} & si & N_i=\frac{sN}{k}
        \end{array}
    \right.$

-   Distribución de frecuencias agrupadas.
    $C_\frac{s}{k}=L_{i-1}+c_i\frac{\frac{sN}{k}-N_{i-1}}{n_i}$.\
    Los cuantiles maás usados son los
    cuartiles($Q_1=25\%, Q_2=50\%, Q_3=75\%$), los deciles
    ($D_1=10\%, D_2=20\%,...,D_9=90\%$) y los percentiles
    ($P_10=10\%, P_20=20\%,...,P_90=90\%$).

## Tema 15 

**Medidas de dispersión absoluta**\
- Rango/ recorrido. Diferencia entre los valores máximo y mínimo de la
variable, $Re=x_{max}-x_{min}$.\
- Varianza. media aritmética de los cuadrados de las desviaciones de los
datos respecto a su media aritmética,
$S^2=\frac{\sum_{i=1}^n (x_i-\bar{x})^2*n_i}{N}= \frac{\sum_{i=1}^n x_i^2*n_i}{N}-\bar{x}^2$.
En el caso de que todos los valores sean únicos $n_i$ por lo que la
fórmula se simplifica.\
- Cusivarianza. $S^{*2}=\frac{\sum_{i=1}^n (x_i-\bar{x})^2*n_i}{N-1}$ y
$S^{*2}\geq S^2$.\
- Desviación típica: $S=+\sqrt{S^2}$.\
- Cuasidesviación típica:
$S^{*}= +\sqrt{S^{*2}}=+\sqrt{\frac{N}{N-1}S^2}$ y $S^{*}\geq S$.\
**Medidas de dispersión relativas**\
- Coeficiente de variación. Es una medida que sirve para comparar el
grado de dispersión de dos distribuciones que no vienen medidas en las
mismas unidades, $CV=\frac{S}{|\bar{x}|}$. Valores cercanos a 0 indican
baja dispersión (relativa) y por tanto, mejor representatividad de la
media.\
- Tipificación de variables. Una variable tipificada es una nueva
variable que se obtiene mediante una transformación lineal,
$Z=\frac{X-\bar{x}}{S}$. La nueva variable tendrá media 0 y desviación
típica 1.\
**Transformaciones de escala y origen**

         Estadístico                   $Y=X\pm a$                  $Y=b*X$                  $Y=X/b$                          $Y=b*X\pm a$
  -------------------------- ------------------------------ --------------------- ---------------------------- -----------------------------------------
           Varianza                      Igual                $S^2_Y=b^2*S^2_X$     $S^2_Y=\frac{S^2X}{b^2}$              $S^2_Y= b^2*S^2_X$
   Coeficiente de variación   $CV_Y=\frac{S_X}{|X \pm a|}$          Igual                    Igual              $CV_Y=\frac{|b|*S_x}{|b*\bar{x}\pm a|}$
          Recorrido                      Igual               $Re(Y)= |b|* Re(X)$   $Re(Y)= \frac{Re(X)}{|b|}$              $Re(Y)=|b|*Re(X)$

## Tema 16 

**Coeficiente de asimetría de Fisher**.
$g_1(X)=\frac{m_3(X)}{S^3}=\frac{\frac{\sum^k_{i=1}(x_i-\bar{x})^3}{N}}{S^3}$.\
Tipos de asimetría: 1)Negativa($g_1(X)<0$, se concetran a la derecha),
2)simétrica($g_1(X)=0$) y 3)positiva($g_1(X)>0$, se concentran a la
izquierda).\
**Curtosis o medida de apuntamiento**.
$g_2(X)=\frac{m_4(X)}{S^4}-3=\frac{\frac{\sum_{i=1}^k (x_i-\bar{x})^4}{N}}{S^4}-3$.\
Tipos de curtosis: 1)leptocúrtica ($g_2(X)>0$, más apuntada que la
normal), 2)mesocúrtica($g_2(X)=0$, igual de apuntada que la normal) y
3)platicúrtica ($g_2(X)<0$, menos apuntada que la normal).\
**Índice de Gini**(medida de concentración).
$IG=\frac{\sum^{k-1}_{i=1} (p_i-q_i)}{\sum^{k-1}_{i=1} p_i}$ con
$p_i=\frac{N_i}{N}*100$ y
$q_i=\frac{\sum_{j=1}^i x_jn_j}{\sum_{j=1}^k x_jn_j}*100$.\
Interpretación: 1)IG=0, concentración mínima y 2) IG=1, concentración
máxima.

## Tema 17 

**Distribución de frecuencias absoluta y distribución marginal**\

   Valores X/Y    $y_1$     \...    $y_j$     \...   $y_{J}$     $n_i$
  ------------- ---------- ------ ---------- ------ ---------- ----------
      $x_1$      $n_{11}$   \...   $n_{1j}$   \...   $n_{1J}$   $n_{1.}$
      \...         \...     \...     \...     \...     \...       \...
      $x_i$      $n_{i1}$   \...   $n_{ij}$   \...   $n_{iJ}$   $n_{i.}$
      \...         \...     \...     \...     \...     \...       \...
      $x_I$      $n_{I1}$   \...   $n_{Ij}$   \...   $n_{IJ}$   $n_{I.}$
    $n_{.j}$     $n_{.1}$   \...   $n_{.j}$   \...   $n_{.J}$      N

**Distribución de frecuencias relativas** con
$f_{ij}=\frac{n_{ij}}{N}$.\

   Valores X/Y    $y_1$     \...    $y_j$     \...   $y_{J}$
  ------------- ---------- ------ ---------- ------ ----------
      $x_1$      $f_{11}$   \...   $f_{1j}$   \...   $f_{1J}$
      \...         \...     \...     \...     \...     \...
      $x_i$      $f_{i1}$   \...   $f_{ij}$   \...   $f_{iJ}$
      \...         \...     \...     \...     \...     \...
      $x_I$      $f_{I1}$   \...   $f_{Ij}$   \...   $f_{IJ}$

X e Y serán independientes si $f_{ij} = f_{i.}* f_{.j} \forall i,j$.\
**Covarianza**. $S_{XY}=\frac{\sum_i x_iy_i}{N}-\bar{x}\bar{y}$.\
Interpretación: 1) si es muy cercana a 0 no existe relación entre las
variables o es marcadamente no lineal, 2) si es positiva hay asociación
lineal positiva y 3) si es negativa hay asociación lineal inversa. Tener
en cuenta que como depende de las unidades de medida no permite
cuantificar el grado de asociación lineal.\
**Coeficiente de correlación de Pearson**.
$\rho=r=\frac{S_{XY}}{S_XS_Y}$.\
Interpretación: 1)$|\rho|<0.25$ no existe relación lineal,
2)$0.25<|\rho|<0.75$ existe correlación lineal débil y 3) $|\rho|>0.75$
existe correlación lineal fuerte.\
La difeencia ente la covarianza y el coeficiente de correlación es que
el seguno no tiene unidades de medida.

## Tema 18 

**Recta de regresión Y sobre X**. $Y=\beta_1X+\beta_0+\epsilon$.\
Se calculará como $\hat{Y}=\bar{y}-\frac{S_{XY}}{S^2_X}(X-\bar{x})$ por
tanto $\beta_1=\frac{S_{XY}}{S^2_X}$ y
$\beta_0= \bar{y}-\beta_1*\bar{x}$.\
**Recta de regresión X sobre Y**. $X=\beta_1Y+\beta_0+\epsilon$.\
Se calculará como $\hat{X}=\bar{x}-\frac{S_{XY}}{S^2_Y}(Y-\bar{y})$ por
tanto $\beta_1=\frac{S_{XY}}{S^2_Y}$ y
$\beta_0= \bar{x}-\beta_1*\bar{y}$.\
**Varianza residual y explicada**\
- Varianza residual: $S_e^2=\frac{\sum_{i=1}^N (y_i-\hat{y})^2}{N}$.\
- Varianza explicada:
$S^2_{\hat{Y}}=\frac{\sum_{i=1}^N(\hat{y}_i-\bar{y})^2}{N}$.\
$S_Y^2= \frac{\sum^{N}_{i=1}(y_i-\bar{y})^2}{N}=\frac{\sum_{i=1}^N(y_i-\hat{y})^2}{N}+\frac{\sum_{i=1}^N(\hat{y}_i-\bar{y})^2}{N}$.\
**Coeficiente de determinación**. Proporción de varianza explicada por
el modelo de regrasión.\
$R^2=\frac{S^2_\hat{Y}}{S^2_Y}=1-\frac{S^2_e}{S^2_Y}$. Aplicandolo a la
regresión lineal obtenemos que $R^2=\rho^2$, además
$R^2=\beta_1*\beta_1^*$ siedo $\beta_1$ el coeficiente de regresión de
la recta Y sobre X y $\beta_1^*$ el coeficiente de regresión de la recta
X sobre y.\
Interpretación: 1) si $R^2$ es próximo a 0 se dirá que el modelo no
ajusta bien, 2) cuanto más próximo a 1 mejor será el modelo y 3) si
$R^2=1$ existe dependencia funcional.

## Tema 19 

**Limitaciones del método de mínimos cuadrados**.\
- Variable dependiente truncada, faltan datos de la muestra.\
- Variable dependiente censurada, mediciones incompletas y/o asignación
a un cierto valor un número simbólico.\
- Modelos Tobit, evolución del modelo censurado. Considera la existencia
de una variable indepndiente $Y^*$ no observable y una variable $Y$
observable formada por la parte no censurable de $Y^*$. El objetivo es
estimar $Y^*$ empleando solo la muestra de la parte observable.\
*Conclusión:* solamente si la variable dependiente es continua con
dominio $\mathbb{R}$ el método de mínismos cuadrados es óptimo.\
**Interpretación de los coeficientes de regresión.**\
- $\beta_1$ o coeficiente de regresión, indica el tipo de dependiencia
entre las variables:

-   $\beta_1<0$: dependencia negativa, cuando aumenta Y disminuye X.

-   $\beta_1>0$: dependencia positiva, cuando aumenta Y aumenta X.

-   $\beta_1=0$: indica que la media de Y es constante y por tanto la
    recta de regresión es paralela al eje de abscisas.

**Coeficiente de correlación lineal**.
$\rho=\frac{S_{XY}}{S_XS_Y}\frac{S_X}{S_X}=\frac{S_{XY}S_X}{S^2_XS_Y}=\beta_1\frac{S_x}{S_Y}$.\
Si las variables son independientes entonces $\rho=0$, al contrario no
tiene por qué verificarse. Si $\rho=0$ puede existir dependencia
funcional entre variables, siendo la función que las relaciona no
lineal. Por otro lado, si $\rho\pm 1$ entonces las rectas de regresión X
sobre Y e Y sobre X son coincidentes.\
En el caso de que $\rho \neq \{0,\})$ no serán coincidentes. Cuanto
mayor sea el coeficiente menor será el ángulo entre las rectas.\

## Tema 20 

**Regresión múltiple** en función del tipo de variable dependiente:\

   **Tipo de variable**         **Modelo**
  ---------------------- -------------------------
         Continua                 Lineal
        Dicotómica            Logit o probit
         Recuento           Poisson o Binomial
     Factor ordenado      Logit o probit ordenado
        Porcentaje         Regresión fraccional

\
**Regresión lineal múltiple**.
$y_i=\beta_0+\beta_1x_{1i}+\beta_2x_{2i}+...+\beta_kx_{ki}+\epsilon_i$\
-$\beta_0$, el valor de la variable dependiente Y cuando todos los
predictores son 0.\
-$\beta_i$, variación media de la variable Y al incrementar una unidad a
variable $X_i$.\
**Coeficiente de correlación parcial**. Suponiendo una regresión lineal
múltiple de 3 variables, se puede calcular la correlación parcial de $Y$
y $X_1$ manteniendo constante $X_2$ como
$r_{YX_1.X_2}=\frac{r_{YX}-r_{YX_2}r_{X_1X_2}}{\sqrt{1-r^2_{YX_2}}\sqrt{1-r^2_{X_1X_2}}}$.
Cuando no exista la correlación entre $Y$ y $X_2$, y tampoco entre $X_1$
y $X_2$ entronces el anterior coeficiente coincidirá con el coeficiente
de correlación de Pearson.\
**Multicolinealidad**. Se produce cuando al menos dos variables $X_i$
son linealmente dependientes.\
- Factor de inflación de la varianza. $FIV=\frac{1}{1-R_j^2}$.\
1) $FIV=1$ no hay problema de multicolinealidad, 2) $FIV \in (1,5)$ se
considera multicolinealidad baja, 3) $FIV \in (5,10)$ se considera
multicolinealidad alta y 4) $FIV>10$ se dice que hay un problema serio
de multicolinealidad.\
- Tolerancia. $T=1-R^2_j$. Se considera que hay problemas serios de
multicolinealidad si $T<0.1$.

## Tema 21 

**Índices simples**: $\frac{Y_t}{Y_0}*100$.\
Tasa de variación o variación porcentual:
$Ta_{t_1}^{t_2}(Y)=\frac{Y_t_2-Y_t_1}{Y_t_1}*100=I_{t_1}^{t_2}-100$.\
Propiedades: 1) Existencia, 2)Identidad, 3)Circular, 4)Inversión, 5)
Encadenamiento, 6)Adición, 7)Multiplicaicón y 8)homogeneidad.\
**Índices complejos**: ponderados y no ponderados.\
No ponderados:\
1) Índice de Bradstreet y Dûtot:
$I_1^t=\frac{\sum_{j=1}^n y_{ij}}{\sum_{j=1}^n y_{1j}}$\
2) Índice de Sauerbek: $I_0^t=\frac{\sum_{j=1} ^n I_0^t(Y_j)}{n}$.\
Ponderados:\
3) Índice de Laspeyres:
$IPL_0^t=\frac{\sum_{i=1}^n p_{it}q_{i0}}{\sum_{i=1}^n p_{i0}q_{i0}}*100$\
4)Índice de Paasche:
$IPP_0^t=\frac{\sum_{i=1}^n p_{it}q_{it}}{\sum_{i=1}^n p_{i0}q_{it}}*100$\
5)Índice de Edgemorth:
$IPE_0^t=\frac{\sum_{i=1}^n p_{it}q_{i0}+\sum_{i=1}^n p_{it}q_{it}}{\sum_{i=1}^n p_{i0}q_{i0}+\sum_{i=1}^n p_{i0}q_{it}}*100$\
6)índice de Fisher: $\sqrt{IPL_0^t+IPP_0^t}$\
Propiedades: 1) cumple las 8 anteriores; 2), 3) y 4) no cumplen
inversión y la circular; 5) y 6) no cumplen la circular.\

## Tema 22 

**Componentes de una serie temporal**\
- Tendencia. Se puede determinar de manera visual, por medias móviles o
de ajuste analítico

-   Medias móviles de amplitud q. Es un proceso por el cual la tendencia
    $Y_t$ se calcula ajustando la serie obtenida como la media
    aritmética de q valores consecutivos de $Y_t$.

-   Ajuste analítico. Se tratará de obtener una función que sea capaz de
    explicar con una buena aproximación a largo tiempo el comportamiento
    de la serie en función de la variable tiempo.

\- Variabilidad. Variaciones cíclicas, estacionales o residuales.\
Si clasificamos la serie en función de la tendencia y las variaciones
estacionales nos encontramos con series estacionarias y no estacinarias.
Es decir, son series con media y varianza constantes en el tiempo.\
**Modelos**\
-Modelo aditivo. Incremento debido a la estacionaridad siempre es el
mismo, aunque la tencencia sea creciente o decreciente.\
-Modelo multiplicativo. Incremento debido a la estacionaridad aumenta o
disminuye conforme la tendencia crece o decrece.\
Una manera simple de establecer el modelo es calcular el coeficiente de
variación pues si $CV(\frac{Y_{i,k+1}}{Y_{i,k}})>CV(Y_{i,k+1}-Y_{i,k})$
entonces presenta un esquema aditivio, en caso contrario un modelo
multiplicativo.
