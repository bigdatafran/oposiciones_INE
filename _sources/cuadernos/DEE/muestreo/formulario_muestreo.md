
# Formulario Muestreo


# Tipos de muestreo.

::: center
                    Con reposición                  Sin Reposición
  ---------- ----------------------------- --------------------------------
   Si orden        $VR_{N,n}=N^{n}$         $V_{N,n}=\binom{N}{n}\cdot n!$
   No orden   $CR_{N,n}=\binom{N-n-1}{n}$       $C_{N,n}=\binom{N}{n}$
:::

(\*) Todas las muestras son equiprobables, salvo en el caso de No
importar orden y con reposición.

# Muestreo aleatorio simple.

$$\hat{X}=N\overline{x};\quad\hat{\overline{X}}=\overline{x};\quad\hat{P}=p;\quad\hat{A}=N\hat{P}$$

## Muestreo sin reposición.

::: center
        $V(\hat{X})=N^{2}(1-f)\frac{S^{2}}{n}$        $V(\hat{\overline{X}})=(1-f)\frac{S^{2}}{n}$
  -------------------------------------------------- ----------------------------------------------
   $V(\hat{A})=\frac{N^{3}}{N-1}\frac{1}{n}(1-f)PQ$   $V(\hat{P})=\frac{N}{N-1}\frac{1}{n}(1-f)PQ$
:::

Para el caso de proporciones, se tiene: $S^{2}=\frac{N}{N-1}PQ$ y
$\hat{S}^{2}=\frac{n}{n-1}\hat{P}\hat{Q}$

### Estimación de varianzas.

::: center
      $\hat{V}(\hat{X})=N^{2}(1-f)\frac{\hat{S}^{2}}{n}$      $\hat{V}(\hat{\overline{X}})=(1-f)\frac{\hat{S}^{2}}{n}$
  ---------------------------------------------------------- ----------------------------------------------------------
   $\hat{V}(\hat{A})=N^{2}(1-f)\frac{1}{n-1}\hat{P}\hat{Q}$     $\hat{V}(\hat{P})=(1-f)\frac{1}{n-1}\hat{P}\hat{Q}$
:::

### Tamaño de la muestra.

#### Para un error de muestreo dado.

-Para la media

$$n=\frac{S^{2}}{e^{2}+\frac{S^{2}}{N}}=\frac{NS^{2}}{Ne^{2}+S^{2}}$$

-Para el total

$$n=\frac{N^{2}\cdot S^{2}}{e^{2}+\frac{N^{2}\cdot S^{2}}{N}}$$

\- Para la proporción.

$$n=\frac{NPQ}{e^{2}(N-1)+PQ}$$

-Para total de clase.

$$n=\frac{N^{3}PQ}{e^{2}(N-1)+N^{2}PQ}$$

#### Para un error relativo de muestreo dado.

$$e_{r}(\hat{\theta})=CV(\hat{\theta})=\frac{\sigma(\hat{\theta})}{E(\hat{\theta})}$$

-Para la media:

$$n=\frac{C_{1,x}^{2}}{e_{r}^{2}+\frac{C_{1,x}^{2}}{N}}=\frac{NC_{1,x}^{2}}{Ne_{r}^{2}+C_{1,x}};\qquad C_{1,x}^{2}=\left(\frac{S}{\overline{X}}\right)^{2}$$

-Para total
$$n=\frac{C_{1,x}^{2}}{e_{r}^{2}+\frac{C_{1,x}^{2}}{N}}=\frac{NC_{1,x}^{2}}{Ne_{r}^{2}+C_{1,x}}$$

-Proporción y total de clase

$$n=\frac{NQ}{P(N-1)e_{r}^{2}+Q}$$

## Muestreo con reposición.

Los estimadores nsesgados son los mismos que para el caso de muestreo
sin reposición.

::: center
   $V(\hat{X})=N^{2}\frac{\sigma^{2}}{n}$   $V(\hat{\overline{X}})=\frac{\sigma^{2}}{n}$
  ---------------------------------------- ----------------------------------------------
       $V(\hat{A})=N^{2}\frac{PQ}{n}$                $V(\hat{P})=\frac{PQ}{n}$
:::

### Estimación de varianzas.

::: center
      $\hat{V}(\hat{X})=N^{2}\frac{\hat{S}^{2}}{n}$      $\hat{V}(\hat{\overline{X}})=\frac{\hat{S}^{2}}{n}$
  ----------------------------------------------------- -----------------------------------------------------
   $\hat{V}(\hat{A})=N^{2}\frac{1}{n-1}\hat{P}\hat{Q}$     $\hat{V}(\hat{P})=\frac{1}{n-1}\hat{P}\hat{Q}$
:::

### Tamaño de la muestra.

#### Para un error de muestreo dado.$e=\sigma(\hat{\theta}).$

::: center
              media                             total                      proproción               total clase
  ------------------------------ ----------------------------------- ---------------------- ---------------------------
   $n=\frac{\sigma^{2}}{e^{2}}$   $n=\frac{\sigma^{2}N^{2}}{e^{2}}$   $n=\frac{PQ}{e^{2}}$   $n=\frac{N^{2}PQ}{e^{2}}$
:::

#### Error relativo de muestreo dado. $e_{r}=CV(\hat{\theta})$

::: center
                             media                                                        total                                     proproción                total clase
  ------------------------------------------------------------ ------------------------------------------------------------ -------------------------- -------------------------
   $n=\frac{\left(\sigma/\overline{X}\right)^{2}}{e_{r}^{2}}$   $n=\frac{\left(\sigma/\overline{X}\right)^{2}}{e_{r}^{2}}$   $n=\frac{Q}{Pe_{r}^{2}}$   $n=\frac{Q}{e_{r}^{2}}$
:::

#### Error de muestreo y coeficientes de confianza dados. $e_{\alpha}=z_{\alpha/2}\sigma(\hat{\theta})$

::: center
                           media                                                     total                                               proproción                                        total clase
  ------------------------------------------------------- ------------------------------------------------------------ ----------------------------------------------- ----------------------------------------------------
   $n=\frac{z_{\alpha/2}^{2}\sigma^{2}}{e_{\alpha}^{2}}$   $n=\frac{z_{\alpha/2}^{2}\sigma^{2}N^{2}}{e_{\alpha}^{2}}$   $n=\frac{z_{\alpha/2}^{2}PQ}{e_{\alpha}^{2}}$   $n=\frac{z_{\alpha/2}^{2}PQN^{2}}{e_{\alpha}^{2}}$
:::

#### Error relativo de muestreo y coeficiente de confianza dados.$e_{r\alpha}=z_{\alpha/2}CV(\hat{\theta})$

::: center
                                        media                                                                              total                                                           proproción                                      total clase
  ---------------------------------------------------------------------------------- ---------------------------------------------------------------------------------- ------------------------------------------------ ------------------------------------------------
   $n=\frac{z_{\alpha/2}^{2}\left(\sigma/\overline{X}\right)^{2}}{e_{r\alpha}^{2}}$   $n=\frac{z_{\alpha/2}^{2}\left(\sigma/\overline{X}\right)^{2}}{e_{r\alpha}^{2}}$   $n=\frac{z_{\alpha/2}^{2}Q}{e_{r\alpha}^{2}P}$   $n=\frac{z_{\alpha/2}^{2}Q}{e_{r\alpha}^{2}P}$
:::

## Notas.

-   El muestreo sin reposición es más preciso que el muestreo con
    reposición.

-   Con el muestreo sin reposición se necesita menos tamaño de muestra
    para cometer el mismo error que en el caso del muestreo con
    reposición.

# Muestreo conglomerados.

$$\hat{X_{st}}=\sum_{h=1}^{L}\hat{X}_{h};\quad\hat{\overline{X}}_{st}=\sum_{h=1}^{l}W_{h}\overline{x}_{h};\quad\hat{A}_{st}=\sum_{h=1}^{l}\hat{A}_{h};\quad\hat{P}_{st}=\sum_{h=1}^{L}W_{h}\hat{P}_{h}$$

## Varianzas.

::: center
            $V(\hat{X}_{st})=\sum_{h}N_{h}^{2}(1-f_{h})\frac{S_{h}^{2}}{n_{h}}$                     $V(\overline{x}_{st})=\sum_{h}W_{h}^{2}(1-f_{h})\frac{S_{h}^{2}}{n_{h}}$
  ---------------------------------------------------------------------------------------- -------------------------------------------------------------------------------------------
   $V(\hat{A}_{st})=\sum N_{h}^{2}(1-f_{h})\frac{N_{h}}{N_{h}-1}\frac{P_{h}Q_{h}}{n_{h}}$   $V(\hat{P}_{st})=\sum_{h}W_{h}^{2}(1-f_{h})\frac{N_{h}}{N_{h}-1}\frac{P_{h}Q_{h}}{n_{h}}$
:::

## Estimación de varianzas.

::: center
      $\hat{V}(\hat{X}_{st})=\sum_{h}N_{h}^{2}(1-f_{h})\frac{\hat{S}{}_{h}^{2}}{n_{h}}$        $\hat{V}(\overline{x}_{st})=\sum_{h}W_{h}^{2}(1-f_{h})\frac{\hat{S}{}_{h}^{2}}{n_{h}}$
  ------------------------------------------------------------------------------------------ ------------------------------------------------------------------------------------------
   $\hat{V}(\hat{A}_{st})=\sum_{h}N_{h}^{2}(1-f_{h})\frac{\hat{P}_{h}\hat{Q}_{h}}{n_{h}-1}$   $\hat{V}(\hat{P}_{st})=\sum_{h}W_{h}^{2}(1-f_{h})\frac{\hat{P}_{h}\hat{Q}_{h}}{n_{h}-1}$
:::

## Afijación de la muestra.

### Afijación uniforme.

$$n_{h}=k$$

::: center
              $V(\hat{X}_{st})=\sum_{h}N_{h}^{2}(1-\frac{k}{N_{h}})\frac{S_{h}^{2}}{k}$              $V(\overline{x}_{st})=\sum_{h}W_{h}^{2}(1-\frac{k}{N_{h}})\frac{S_{h}^{2}}{k}$
  ------------------------------------------------------------------------------------------------- --------------------------------------------------------------------------------
   $V(\hat{A}_{st})=\sum_{h}N_{h}^{2}(1-\frac{k}{N_{h}})\frac{N_{h}}{N_{h}-1}\frac{P_{h}Q_{h}}{k}$     $V(\hat{P}_{st})=\sum_{h}W_{h}^{2}(1-\frac{k}{N_{h}})\frac{P_{h}Q_{h}}{k}$
:::

### Afijación proporcional.

$$\frac{n_{h}}{N_{h}}=k;\ k=\frac{n}{N}=f;\ f_{h}=f;\ W_{h}=\frac{N_{h}}{N}=\frac{n_{h}}{n}$$

$$\hat{X_{st}}=\frac{x}{f}=\frac{Total\ muestral}{Fracci\acute{o}n\ muestreo};\ \hat{\overline{X}_{st}}=\frac{Total\ muestral}{Tama\tilde{n}o\ muestra}$$

::: center
             $V(\hat{X}_{st})=\frac{1-k}{k}\sum_{h}N_{h}S_{h}^{2}$                          $V(\overline{x}_{st})=\frac{1-k}{n}\sum_{h}W_{h}S_{h}^{2}$
  ---------------------------------------------------------------------------- -------------------------------------------------------------------------------------
   $V(\hat{A}_{st})=\frac{1-k}{k}\sum_{h}\frac{N_{h}^{2}}{N_{h}-1}P_{h}Q_{h}$   $V(\text{\ensuremath{\hat{P}_{st})=}}\sum_{h}\frac{N_{h}^{2}/N}{N_{h}-1}P_{h}Q_{h}$
:::

### afijación de mínima varianza ( afijación de Neyman).

$$n_{h}=n\cdot\frac{N_{h}S_{h}}{\sum_{h}N_{h}S_{h}}$$

::: center
   $V(\hat{X}_{st})=\frac{1}{n}\left(\sum_{h=1}^{L}N_{h}S_{h}\right)^{2}-\frac{1}{N}\sum_{h=1}^{L}N_{h}S_{h}^{2}$   $V(\overline{x}_{st})=\frac{1}{n}\left(\sum_{h=1}^{L}W_{h}S_{h}\right)^{2}-\frac{1}{N}\sum_{h=1}^{L}W_{h}S_{h}^{2}$
  ---------------------------------------------------------------------------------------------------------------- ---------------------------------------------------------------------------------------------------------------------
:::

Para obtener la afijación o la expresión de la varianza mínima para la
proporción y el total de clase, en las fórmulas anteriores, se sustituye
$S_{h}^{2}$ por $P_{h}Q_{h}N_{h}/(N_{h}-1)$

### Afijación óptima.

$$n_{h}=n\cdot\frac{N_{h}S_{h}/\sqrt{c_{h}}}{\sum_{h}N_{h}S_{h}/\sqrt{c_{h}}}$$

::: center
     $V(\hat{X}_{st})=\frac{1}{n}\left(\sum_{h=1}^{L}N_{h}S_{h}/\sqrt{c_{h}}\right)\cdot\left(\sum_{h=1}^{L}N_{h}S_{h}\cdot\sqrt{c_{h}}\right)-\frac{1}{N}\sum_{h=1}^{L}N_{h}S_{h}^{2}$
  -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
   $V(\overline{x}_{st})=\frac{1}{n}\left(\sum_{h=1}^{L}W_{h}S_{h}/\sqrt{c_{h}}\right)\cdot\left(\sum_{h=1}^{L}W_{h}S_{h}\cdot\sqrt{c_{h}}\right)-\frac{1}{N}\sum_{h=1}^{L}W_{h}S_{h}^{2}$
:::

Para obtener la afijación o la expresión de la varianza mínima para la
proporción y el total de clase, en las fórmulas anteriores, se sustituye
$S_{h}^{2}$ por $P_{h}Q_{h}N_{h}/(N_{h}-1)$

## Tamaño de la muestra.

### Error de muestreo dado $e=\sigma(\hat{\theta})$.

#### Media, total, proporción y total de clase con afijación proporcional.

\- Para la media.

$$n=\frac{\sum_{h}W_{h}S_{h}^{2}}{e^{2}+\frac{1}{N}\sum_{h}W_{h}S_{h}^{2}}$$

-Para el total:

$$n=\frac{N\sum_{h}N_{h}S_{h}^{2}}{e^{2}+\sum_{h}N_{h}S_{h}^{2}}$$

Los tamaños de la muestra en los casos de la proporción y total de
clase, se calculan sustituyendo $S_{h}^{2}$ por
$\frac{N_{h}}{N_{h}-1}P_{h}Q_{h}$ en las fórmulas del tamaño de la
muestra para la estimación de la media y el total respectivamente.

#### Media, total, proporción y total de clase con afijación de mínima varianza.

-Para la media:

$$n=\frac{\left(\sum_{h}W_{h}S_{h}\right)^{2}}{e^{2}+\frac{1}{N}\sum_{h}W_{h}S_{h}^{2}}$$

-Para el total:

$$n=\frac{\left(\sum_{h}N_{h}S_{h}\right)^{2}}{e^{2}+\sum_{h}N_{h}S_{h}^{2}}$$

Los tamaños de la muestra en los casos de la proporción y total de
clase, se calculan sustituyendo $S_{h}^{2}$ por
$\frac{N_{h}}{N_{h}-1}P_{h}Q_{h}$ en las fórmulas del tamaño de la
muestra para la estimación de la media y el total respectivamente.

### Error de muestreo y coeficiente de confianza dados $e_{\alpha}=z_{\alpha}\sigma(\hat{\theta}).$

#### Media, total, proporción y total de clase con afijación proporcional.

\- Para la media.

$$n=\frac{\sum_{h}W_{h}S_{h}^{2}}{\frac{e^{2}}{z_{\alpha/2}^{2}}+\frac{1}{N}\sum_{h}W_{h}S_{h}^{2}}$$

-Para el total.

$$n=\frac{N\sum_{h}N_{h}S_{h}^{2}}{\frac{e^{2}}{z_{\alpha/2}^{2}}+\sum_{h}N_{h}S_{h}^{2}}$$

Los tamaños de la muestra en los casos de la proporción y total de
clase, se calculan sustituyendo $S_{h}^{2}$ por
$\frac{N_{h}}{N_{h}-1}P_{h}Q_{h}$ en las fórmulas del tamaño de la
muestra para la estimación de la media y el total respectivamente.

#### Media, total, proporción y total de clase con afijación de mínima varianza.

-Para la media:

$$n=\frac{\left(\sum_{h}W_{h}S_{h}\right)^{2}}{\frac{e^{2}}{z_{\alpha/2}^{2}}+\frac{1}{N}\sum_{h}W_{h}S_{h}^{2}}$$

-Para el total:

$$n=\frac{\left(\sum_{h}N_{h}S_{h}\right)^{2}}{\frac{e^{2}}{z_{\alpha/2}^{2}}+\sum_{h}N_{h}S_{h}^{2}}$$

Los tamaños de la muestra en los casos de la proporción y total de
clase, se calculan sustituyendo $S_{h}^{2}$ por
$\frac{N_{h}}{N_{h}-1}P_{h}Q_{h}$ en las fórmulas del tamaño de la
muestra para la estimación de la media y el total respectivamente.

### Tamaño de la muestra sin especificar el tipo de afijación.

-Para la media:

$$n=\frac{\sum\frac{W_{h}^{2}}{w_{h}}S_{h}^{2}}{\left(\frac{e^{2}}{z_{\alpha/2}^{2}}+\frac{\sum W_{h}S_{h}^{2}}{N}\right)}$$

-para el total

$$n=\frac{\sum\frac{W_{h}^{2}}{w_{h}}S_{h}^{2}}{\left(\frac{e^{2}}{z_{\alpha/2}^{2}}+\sum N_{h}S_{h}^{2}\right)}$$

## Muestreo estratificado con reposición.

Los estimadores lineales insesgados del total, media, proporción y total
de clase son los mismos que en el caso sin reposición.

### Varianzas de los estimadores.

::: center
   $V(\hat{X}_{st})=\sum_{h}N_{h}^{2}\frac{\sigma_{h}^{2}}{n_{h}}$   $V(\overline{x}_{st})=\sum_{h}W_{h}^{2}\frac{\sigma_{h}^{2}}{n_{h}}$
  ----------------------------------------------------------------- ----------------------------------------------------------------------
      $V(\hat{A}_{st})=\sum N_{h}^{2}\frac{P_{h}Q_{h}}{n_{h}}$           $V(\hat{P}_{st})=\sum_{h}W_{h}^{2}\frac{P_{h}Q_{h}}{n_{h}}$
:::

### Estimación de varianzas.

::: center
      $\hat{V}(\hat{X}_{st})=\sum_{h}N_{h}^{2}\frac{\hat{S}{}_{h}^{2}}{n_{h}}$        $\hat{V}(\overline{x}_{st})=\sum_{h}W_{h}^{2}\frac{\hat{S}{}_{h}^{2}}{n_{h}}$
  --------------------------------------------------------------------------------- ---------------------------------------------------------------------------------
   $\hat{V}(\hat{A}_{st})=\sum_{h}N_{h}^{2}\frac{\hat{P}_{h}\hat{Q}_{h}}{n_{h}-1}$   $\hat{V}(\hat{P}_{st})=\sum_{h}W_{h}^{2}\frac{\hat{P}_{h}\hat{Q}_{h}}{n_{h}-1}$
:::

### Afijación uniforme.

::: center
   $V(\hat{X}_{st})=\sum N_{h}^{2}\frac{\sigma_{h}^{2}}{k}$   $V(\overline{x}_{st})=\sum_{h}W_{h}^{2}\frac{\sigma_{h}^{2}}{k}$
  ---------------------------------------------------------- ------------------------------------------------------------------
   $V(\hat{A}_{st})=\sum_{h}N_{h}^{2}\frac{P_{h}Q_{h}}{k}$        $V(\hat{P}_{st})=\sum_{h}W_{h}^{2}\frac{P_{h}Q_{h}}{k}$
:::

### Afijación proporcional.

::: center
   $V(\hat{X}_{st})=\frac{1}{k}\sum_{h}N_{h}\sigma_{h}^{2}$   $V(\overline{x}_{st})=\frac{1}{n}\sum_{h}W_{h}\sigma_{h}^{2}$
  ---------------------------------------------------------- ----------------------------------------------------------------
     $V(\hat{A}_{st})=\frac{1}{k}\sum_{h}N_{h}P_{h}Q_{h}$     $V(\hat{P}_{st})=\frac{1}{n}\sum_{h}W_{h}\frac{P_{h}Q_{h}}{k}$
:::

### Afijación de mínima varianza o de Neyman.

::: center
                                        media                                                                              total
  ---------------------------------------------------------------------------------- ----------------------------------------------------------------------------------
               $n_{h}=n\frac{N_{h}\sigma_{h}}{\sum_{h}N_{h}\sigma_{h}}$                           $n_{h}=n\frac{W_{h}\sigma_{h}}{\sum_{h}W_{h}\sigma_{h}}$
   $V(\overline{X}_{st})=\frac{1}{n}\left(\sum_{h=1}^{L}W_{h}\sigma_{h}\right)^{2}$   $V(\overline{X}_{st})=\frac{1}{n}\left(\sum_{h=1}^{L}N_{h}\sigma_{h}\right)^{2}$
:::

Si se quiere esta afijación para la proporción y el total de clase, hay
que sustituir $\sigma_{h}$ en la expresión anterior por $P_{h}Q_{h}$

### Afijación óptima. 

::: center
                                                                          media                                                                                                                                                total
  ------------------------------------------------------------------------------------------------------------------------------------------------------ -------------------------------------------------------------------------------------------------------------------------------------------------
                                   $n_{h}=n\frac{N_{h}\sigma_{h}/\sqrt{c_{h}}}{\sum_{h}(N_{h}\sigma_{h})/\sqrt{c_{h}}}$                                                                $n_{h}=n\frac{W_{h}\sigma_{h}/\sqrt{c_{h}}}{\sum_{h}(W_{h}\sigma_{h})/\sqrt{c_{h}}}$
   $V(\overline{X}_{st})=\frac{1}{n}\left(\sum_{h=1}^{L}W_{h}\sigma_{h}/\sqrt{c_{h}}\left(\sum_{h=1}^{L}W_{h}\sigma_{h}\cdot\sqrt{c_{h}}\right)\right)$   $V(\hat{X}_{st})=\frac{1}{n}\left(\sum_{h=1}^{L}N_{h}\sigma_{h}/\sqrt{c_{h}}\left(\sum_{h=1}^{L}N_{h}\sigma_{h}\cdot\sqrt{c_{h}}\right)\right)$
:::

Si se quiere esta afijación para la proporción y el total de clase, hay
que sustituir $\sigma_{h}$ en la expresión anterior por $P_{h}Q_{h}$

### Tamaño de la muestra.

a\) Error de muestreo dado $e=\sigma(\hat{\theta})$.

\- **Media, Total, proporción y total de clase con afijación
proporcional**.

\- Para la media.

$$n=\frac{\sum_{h}W_{h}\sigma_{h}^{2}}{e^{2}}$$

\- Para el total.

$$n=\frac{N\sum_{h}N_{h}\sigma_{h}^{2}}{e^{2}}$$

Para el caso de la proporción y el total de la clase, se emplean las
fórmulas anteriores sustituyendo $\sigma_{h}^{2}$ por $P_{h}Q_{h}$

\- **Media, Total, proporción y total de clase con afijación de mínima
varianza**.

-Para la media:

$$n=\frac{\left(\sum_{h}W_{h}\sigma_{h}\right)^{2}}{e^{2}}$$

-Para el total.

$$n=\frac{\left(\sum_{h}N_{h}\sigma_{h}\right)^{2}}{e^{2}}$$

Para el caso de la proporción y el total de la clase, se emplean las
fórmulas anteriores sustituyendo $\sigma_{h}^{2}$ por $P_{h}Q_{h}$

b\) Error de muestreo y coeficiente de confianza dados
$e_{\alpha}=z_{\alpha/2}\sigma(\hat{\theta})$.

\- **Media, Total, proporción y total de clase con afijación
proporcional**.

-Para la media.

$$n=\frac{\sum_{h}W_{h}\sigma_{h}^{2}}{e_{\alpha}^{2}/z_{\alpha/2}^{2}}$$

-Para el total

$$n=\frac{N\sum_{h}N_{h}\sigma_{h}^{2}}{e_{\alpha}^{2}/z_{\alpha/2}^{2}}$$

Para el caso de la proporción y el total de la clase, se emplean las
fórmulas anteriores sustituyendo $\sigma_{h}^{2}$ por $P_{h}Q_{h}$.

\- **Media, Total, proporción y total de clase con afijación de mínima
varianza.**

\- para la media.

$$n=\frac{\left(\sum_{h}W_{h}\sigma_{h}\right)^{2}}{e_{\alpha}^{2}/z_{\alpha/2}^{2}}$$

\- Para el total.

$$n=\frac{\left(\sum_{h}N_{h}\sigma_{h}\right)^{2}}{e_{\alpha}^{2}/z_{\alpha/2}^{2}}$$

# Muestreo sistemático.

$$\hat{X}=N\overline{x}_{j},\quad\hat{\overline{X}}=\overline{x}_{j},\quad\hat{P}=\hat{P}_{j},\quad\hat{A}=N\hat{P}_{j}$$

Definiciones:

cuasivarianza
muestral:$S^{2}=\frac{1}{n-1}\sum_{i,j}\left(x_{ij}-\overline{X}\right)^{2}$

cuasivarianza intermuestral:
$S_{bs}^{2}=\frac{1}{k-1}\sum_{i=1}^{n}\sum_{j=1}^{k}\left(\overline{x}_{j}-\overline{X}\right)^{2}$

cuasivarianza intramuestral:
$S_{ws}^{2}=\frac{1}{N-k}\sum_{i=1}^{n}\sum_{j=1}^{k}\left(X_{ij}-\overline{X}\right)^{2}$

Se verifica: $(N-1)S^{2}=(N-k)S_{ws}^{2}+(k-1)S_{bs}^{2}$

## Varianzas en función de $S_{bs}^{2}$.

\- General (para el total)

$$\boxed{V(\hat{X)}=k\sum_{r=1}^{k}\left(\sum_{h\in s_{r}}y_{h}-\frac{1}{k}\cdot Y_{U}\right)^{2}\qquad(*)}$$

\- a partir de cuasivarianza intermuestral

::: center
                   $V(\hat{\overline{X}})=(1-f)\frac{S_{bs}^{2}}{n}$                                  $V(\hat{X})=N^{2}(1-f)\frac{S_{bs}^{2}}{n}$
  ------------------------------------------------------------------------------------ --------------------------------------------------------------------------
   $V(\hat{P})=\frac{1}{N}\sum_{i=1}^{n}\sum_{j=1}^{k}\left(\hat{P}_{j}-P\right)^{2}$   $V(\hat{A})=N\sum_{i=1}^{n}\sum_{j=1}^{k}\left(\hat{P}_{j}-P\right)^{2}$
:::

\- a partir de cuasivarianza intramuestral

::: center
    $V(\hat{\overline{X}})=\sigma^{2}-\frac{n-1}{n}S_{ws}^{2}$                        $V(\hat{X})=N(N-1)S^{2}-N(N-k)S_{ws}^{2}$
  --------------------------------------------------------------- ---------------------------------------------------------------------------------
   $V(\hat{P})=PQ-\frac{1}{k}\sum_{j}^{k}\hat{P}_{j}\hat{Q}_{j}$   $V(\hat{A})=N^{2}\left(PQ-\frac{1}{k}\sum_{j}^{k}\hat{P}_{j}\hat{Q}_{j}\right)$
:::

## Coeficiente de correlación intramuestral.

$$\rho_{w}=\frac{2\sum_{j=1}^{k}\sum_{i<z}^{n}(X_{ij}-\overline{X})(X_{zj}-\overline{X)}}{N(n-1)\sigma^{2}}\ ,con\ \ \sigma^{2}=\frac{1}{nk}\sum_{j=1}^{k}\sum_{i=1}^{n}(X_{ij}-\overline{X})^{2}$$

$$\rho_{w}=1-\frac{n}{n-1}\cdot\frac{SSW}{SST}$$

$$\boxed{V(\overline{x}_{j})=\frac{N-1}{N}\cdot\frac{S^{2}}{n}\left[1+(n-1)\rho_{w}\right]}$$

Una medida de homogeneidad entre los elementos de una misma muestra
sistemática es:

$$\delta=1-\frac{N-1}{N-k}\cdot\frac{SSW}{SST}\Rightarrow\rho=1-\frac{N}{N-1}\cdot(1-\delta)$$

## Muestreo estratificado vs sistemático.

\- cuasivarianza interestratal
$S_{bst}^{2}=\frac{1}{n-1}\sum_{i=1}^{n}\sum_{j=1}^{k}\left(\overline{X}_{i}-\overline{X}\right)^{2}$

-cuasivarianza intraestratal:
$S_{wst}^{2}=\frac{1}{N-n}\sum_{i,j}\left(X_{ij}-\overline{X}\right)^{2}$

$$\boxed{(N-1)S^{2}=(N-n)S_{wst}^{2}+(n-1)S_{bst}^{2}}$$

$\rho_{wst}$ es el coeficiente de correlación lineal entre las
desviaciones de las medias de los estratos de todos los pares de valores
que están en la misma muestra sistemática.

$$\rho_{wst}=\frac{2\sum_{j=1}^{k}\sum_{i<z}(X_{ij}-\overline{X}_{i})(X_{zj}-\overline{X}_{z})}{n(n-1)(k-1)S_{wst}^{2}}$$

## Estimación de la varianza.

No hay método directo. Estudiamos los siguientes casos.

\- $\rho_{w}$ próximo a cero:

$$\hat{V}(\overline{x})=(1-f)\cdot\frac{\hat{S}^{2}}{n}\quad\hat{S}^{2}\ cuasivarainaza\ muestra\ sistem\acute{a}tica$$

\- $\rho_{wst}$ próximo a cero.

$$\hat{V}(\overline{x}_{st})=\frac{1-f}{n^{2}}\sum_{h=1}^{n/2}(x_{h1}-x_{h2})^{2}$$

\- ninguno de los coeficientes de correlación anteriores están próximo a
cero.

Se utilizaría método muestras interpenetrantes.

# Métodos de estimación indirecta.

## Método de la razón

En general el estimador $\hat{R}$ es sesgado de
$R=\frac{\overline{X}}{\overline{Y}}$. Se tiene:
$B(\hat{R})=-\rho_{(\hat{R},\overline{y})}\sigma_{\hat{R}}Cv(\overline{y}).\text{\ensuremath{\hat{R}}}$
será insegado si:

1.  $\hat{R}$ e $\overline{y}$ son incorreladas, ó

2.  .-
    $\left|\frac{B(\hat{R})}{\sigma_{\hat{R}}}\right|\le Cv(\overline{y})<0.1$

Para conseguir que $\hat{R}$ sea más o menos insesgado, se debe tomar n:
$n>\frac{100N\frac{S_{Y}^{2}}{\overline{y}^{2}}}{N+100\frac{S_{Y}^{2}}{\overline{y}^{2}}}$
(muestreo sin reposición). Para muestreo con reposición:
$n>100\frac{\sigma_{y}^{2}}{\overline{Y}^{2}}$

\- Si la recta de regresión de Y/X ( o X/Y) pasa por el origen de
coordenadas entonces $\hat{R}$ es insesgado.

### Estimador de Hartley y Ross.

Va a ser siempre insesgado de R. Se construye así:

$$\hat{R}_{HR}=\hat{R}_{1}+\frac{N-1}{N\overline{Y}}\cdot\frac{n}{n-1}\left(\overline{x}-\hat{R}_{1}\overline{y}\right)\quad con\quad\hat{R}_{1}=\frac{1}{n}\sum_{i=1}^{n}\frac{X_{i}}{Y_{i}}$$

### Sesgo aproximado.

::: center
                                                            valor                                                                                   estimación
  ------------------- ---------------------------------------------------------------------------------- ------------------------------------------------------------------------------------------------
   Muest. sin repos.           $B(\hat{R})=\frac{(1-f)}{n\overline{Y}^{2}}(RS_{Y}^{2}-S_{XY})$               $\hat{B}(\hat{R})=\frac{(1-f)}{n\overline{Y}^{2}}(\hat{R}\hat{S}_{Y}^{2}-\hat{S}_{XY})$
   Muest. con repos.   $B(\hat{R})=\frac{1}{n\overline{Y}^{2}}\left(R\sigma_{Y}^{2}-\sigma_{XY}\right)$   $\hat{B}(\hat{R})=\frac{1}{n\overline{Y}^{2}}\left(\hat{R}\hat{S}_{Y}^{2}-\hat{S}_{XY}\right)$
:::

### Varianza aproximada.

::: center
   Muest. sin rep. (valor)            $V(\hat{R})=\frac{1-f}{\overline{Y}^{2}n(N-1)}\left[\sum_{1}^{N}X_{i}^{2}+R^{2}\sum_{1}^{N}Y_{i}^{2}-2R\sum_{1}^{N}X_{i}Y_{i}\right]$
  ------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------
   Muest. sin rep. (esti.)   $\hat{V}(\hat{R})=\frac{1-f}{\overline{Y}^{2}n(n-1)}\left[\sum_{1}^{n}X_{i}^{2}+\hat{R}^{2}\sum_{1}^{n}Y_{i}^{2}-2\hat{R}\sum_{1}^{n}X_{i}Y_{i}\right]$
   Muest. con rep. (valor)              $V(\hat{R})=\frac{1-f}{\overline{Y}^{2}nN}\left[\sum_{1}^{N}X_{i}^{2}+R^{2}\sum_{1}^{N}Y_{i}^{2}-2R\sum_{1}^{N}X_{i}Y_{i}\right]$
   Muest. con rep. (esti.)         $\hat{V}(\hat{R})=\frac{1-f}{\overline{Y}^{2}n(n-1)}\left[\sum_{1}^{n}X_{i}^{2}+R^{2}\sum_{1}^{n}Y_{i}^{2}-2R\sum_{1}^{n}X_{i}Y_{i}\right]$
:::

## Estimación de parámetros.

::: center
              Total                                  Media                               Proporción                    Total clase
  ------------------------------ ---------------------------------------------- ----------------------------- -----------------------------
   $\hat{X}_{R}=\hat{R}\cdot Y$   $\hat{\overline{X}_{R}}=\hat{R}\overline{Y}$   $\hat{P}_{RX}=\hat{R}P_{Y}$   $\hat{A}_{RX}=\hat{R}A_{Y}$
:::

Estos estimadores son insesgados si lo es el estimador de la razón.

## Varianzas de los estimadores.

::: center
   Muest. sin rep.      $V(\hat{X}_{R})=N^{2}\frac{1-f}{n(N-1)}\left[\sum_{1}^{N}X_{i}^{2}+R^{2}\sum_{1}^{N}Y_{i}^{2}-2R\sum_{1}^{N}X_{i}Y_{i}\right]$
  ----------------- --------------------------------------------------------------------------------------------------------------------------------------
         2-2         $V(\hat{\overline{X}}_{R})=\frac{1-f}{n(N-1)}\left[\sum_{1}^{N}X_{i}^{2}+R^{2}\sum_{1}^{N}Y_{i}^{2}-2R\sum_{1}^{N}X_{i}Y_{i}\right]$
         2-2                                    $V(\hat{P})=\frac{N}{N-1}\frac{1-f}{n}\left(P_{X}+R^{2}P_{Y}-2RP_{XY}\right)$
         2-2                                  $V(\hat{A})=\frac{N^{3}}{N-1}\frac{1-f}{n}\left(P_{X}+R^{2}P_{Y}-2RP_{XY}\right)$
   Muest. con rep.            $V(\hat{X}_{R})=\frac{N}{n}\left[\sum_{1}^{N}X_{i}^{2}+R^{2}\sum_{1}^{N}Y_{i}^{2}-2R\sum_{1}^{N}X_{i}Y_{i}\right]$
                        $V(\hat{\overline{X}}_{R})=\frac{1}{nN}\left[\sum_{1}^{N}X_{i}^{2}+R^{2}\sum_{1}^{N}Y_{i}^{2}-2R\sum_{1}^{N}X_{i}Y_{i}\right]$
                                                        $V(\hat{P})=\frac{1}{n}\left(P_{X}+R^{2}P_{Y}-2RP_{XY}\right)$
                                                      $V(\hat{A})=\frac{N^{2}}{n}\left(P_{X}+R^{2}P_{Y}-2RP_{XY}\right)$
:::

## Estimación varianzas

::: center
   Muest. sin rep.   $\hat{V}(\hat{X}_{R})=N^{2}\frac{1-f}{n(n-1)}\left[\sum_{1}^{n}X_{i}^{2}+\hat{R}^{2}\sum_{1}^{n}Y_{i}^{2}-2\hat{R}\sum_{1}^{n}X_{i}Y_{i}\right]$
  ----------------- --------------------------------------------------------------------------------------------------------------------------------------------------
         2-2         $V(\hat{\overline{X}}_{R})=\frac{1-f}{n(n-1)}\left[\sum_{1}^{n}X_{i}^{2}+\hat{R}^{2}\sum_{1}^{n}Y_{i}^{2}-2\hat{R}\sum_{1}^{n}X_{i}Y_{i}\right]$
         2-2                            $\hat{V}(\hat{P}_{R})=\frac{1-f}{n-1}\left(\hat{P}_{X}+\hat{R}^{2}\hat{P}_{Y}-2\hat{R}\hat{P}_{XY}\right)$
         2-2                         $\hat{V}(\hat{A}_{R})=N^{2}\frac{1-f}{n-1}\left(\hat{P}_{X}+\hat{R}^{2}\hat{P}_{Y}-2\hat{R}\hat{P}_{XY}\right)$
   Muest. con rep.    $\hat{V}(\hat{X}_{R})=N^{2}\frac{1}{n(n-1)}\left[\sum_{1}^{n}X_{i}^{2}+\hat{R}^{2}\sum_{1}^{n}Y_{i}^{2}-2\hat{R}\sum_{1}^{n}X_{i}Y_{i}\right]$
                      $V(\hat{\overline{X}}_{R})=\frac{1}{n(n-1)}\left[\sum_{1}^{n}X_{i}^{2}+\hat{R}^{2}\sum_{1}^{n}Y_{i}^{2}-2\hat{R}\sum_{1}^{n}X_{i}Y_{i}\right]$
                                        $\hat{V}(\hat{P}_{R})=\frac{1}{(n-1)}\left(\hat{P}_{X}+\hat{R}^{2}\hat{P}_{Y}-2\hat{R}\hat{P}_{XY}\right)$
                                      $\hat{V}(\hat{A}_{R})=N^{2}\frac{1}{n-1}\left(\hat{P}_{X}+\hat{R}^{2}\hat{P}_{Y}-2\hat{R}\hat{P}_{XY}\right)$
:::

# Muestreo por conglomerados.

## Conglomerados mismo tamaño sin submuestreo.

$\overline{M}$ Número de unidades elementales en el conglomerado. $n$ :
Número de conglomerado en la muestra. $N$ número de conglorados en la
población

### Muestreo sin remplazamiento en primera etapa.

$\hat{X}=N\overline{M}\overline{\overline{x}}\qquad\hat{\overline{X}}=\overline{\overline{x}}\qquad\hat{P}=\frac{1}{n}\sum_{i=1}^{n}P_{i}\qquad\hat{A}=N\overline{M}\hat{P}\ con\ \overline{\overline{x}}=\frac{1}{n}\sum_{i=1}^{n}\overline{X}_{i}$

$V(\overline{\overline{x}})=(1-f)\frac{S_{b}^{2}}{n\overline{M}}\quad S_{b}^{2}=\frac{\sum_{i=1}^{N}\sum_{j=1}^{\overline{M}}\left(\overline{X}_{i}-\overline{X}\right)^{2}}{N-1};\ V(\hat{X})=N^{2}\overline{M}^{2}(1-f)\frac{S_{b}^{2}}{n\overline{M}}$

$V(\hat{P})=(1-f)\frac{\sum_{i=1}^{N}(P_{i}-P)^{2}}{n(N-1)};\ V(\hat{A})=N^{2}\overline{M}^{2}(1-f)\frac{\sum_{i=1}^{N}(P_{i}-P)^{2}}{n(N-1)}$

$\delta$= coeficiente de correlación intraconglomerados.
$V(\overline{\overline{x}})=(1-f)\frac{S^{2}}{n\overline{M}}\left[1+(\overline{M}-1)\delta\right]$

$\hat{V}(\overline{\overline{x}})=(1-f)\frac{\hat{S}_{0}^{2}}{n\overline{M}}\left[1+(\overline{M}-1)\hat{\delta}\right]=(1-f)\frac{\hat{S}_{b}^{2}}{n\overline{M}}$

siendo:$\hat{S_{0}}^{2}=\frac{N-1}{N\overline{M}-1}\hat{S}_{b}^{2}+\frac{N\left(\overline{M}-1\right)}{N\overline{M}-1}\hat{S}_{w}^{2}$

$\hat{V}(\hat{X})=N^{2}\overline{M}^{2}\hat{V}(\overline{\overline{x}})$

$\hat{V}(\hat{P})=(1-f)\frac{\hat{S}_{0}^{2}}{n\overline{M}}\left[1+(\overline{M}-1)\hat{\delta}\right]=(1-f)\frac{\hat{S}_{b}^{2}}{n\overline{M}}$

$\hat{V}(\hat{A})=N^{2}\overline{M}^{2}\hat{V}(\hat{P})$

### Muestreo con remplazamiento en primera etapa.

Los estimadors son iguales que en el caso sin remplazamiento

$V\left(\overline{\overline{X}}\right)=\frac{\sigma_{b}^{2}}{n\overline{M}}$
con
$\sigma_{b}^{2}=\frac{1}{N}\sum_{i=1}^{N}\sum_{J=1}^{\overline{M}}\left(\overline{X}_{i}-\overline{X}\right)^{2}$

$V(\overline{\overline{X}})=\frac{\sigma^{2}}{n\overline{M}}\left[1+\left(\overline{M}-1\right)\cdot\delta\right]$
siendo $\delta$ el coeficiente de correlación intraconglomerados

$V(\hat{X})=N^{2}\overline{M}^{2}\frac{\sigma_{b}^{2}}{n\overline{M}}$

$V(\hat{P})=\frac{\sum_{i=1}^{N}\left(P_{i}-P\right)^{2}}{nN}\ \ \ \text{\ \ V(\ensuremath{\hat{A})=N^{2}\overline{M}^{2}\frac{\sum_{i=1}^{N}\left(P_{i}-P\right)^{2}}{nN}}}$

#### Estimación de varianzas

$\hat{\sigma}'^{2}=\hat{S}_{1,w}^{2}+\frac{\hat{S}_{b}^{2}}{M}$ es un
estimador insesgado de $\sigma^{2}$,
$\hat{S}_{1,w}^{2}=\frac{1}{n\overline{M}}\sum_{i=1}^{n}\sum_{j=1}^{\overline{M}}\left(X_{ij}-\overline{X}_{i}\right)^{2}$
