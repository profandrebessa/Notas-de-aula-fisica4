
# Óptica geométrica

Nesta seção iremos estudar espelhos e superfícies refratoras. Para os espelhos vamos utilizar simplesmente que o ângulo de reflexão é igual ao ângulo de incidência. Para as superfícies refratoras, vamos usar a Lei de Snell:
```{math}
n_1\,\sin \theta_1 = n_2\,\sin\theta_2
\label{eq:leidesnell2}
```

## Espelhos planos

As propriedades da formação das imagens dos espelhos dependem de relações geométricas. O estudo dos espelhos é uma oportunidade de revisar e aplicar os conceitos da Geometria Euclideana.

#### Formação de uma imagem perfeita

Considere uma fonte luminosa pontual. Nas figuras, essa fonte será denotada pela letra $P$. Raios são emitidos em todas as direções e serão refletidos no espelho. É importante compreender que a reflexão será tal que todos os raios refletidos parecerão ser emitidos de um mesmo ponto $P'$, localizado atrás do espelho. Como não chegam (e, portanto, não emanam) raios em $P'$, essa convergência do prolongamento dos raios não pode ser captada por um anteparo atrás do espelho. Dizemos que a imagem é virtual.

A demonstração de que todos os raios refletidos parecem ser emitidos de $P'$ é simples. Considere um raio qualquer que atinge o espelho formando um ângulo $\theta$ com a normal. Além disso, considere um raio que atinge o espelho em ângulo zero. Os prolongamentos dos dois raios se encontram em um ponto $P'$. A questão é esse ponto $P'$ depende de $\theta$? 

:::{figure} ./figures/espelhoplano1.png
---
width: 300px
name: fig_espelhoplano1
---
:::

Por semelhança de triângulos, vemos que a distância $s'$ de $P'$ ao espelho deve ser igual à distância $s$ de $P$ ao espelho. O fato de que essa conclusão não depende do valor de $\theta$ garante que todos os prolongamentos de raios se encontrarão em $P'$: teremos uma imagem perfeita do ponto $P$ atrás do espelho.

#### Orientação tridimensional invertida

A transformação que um espelho (com normal na direção $\hat{k}$) faz é tal que a base $\hat{i},\hat{j},\hat{k}$ aparece como $\hat{i},\hat{j},-\hat{k}$. Na Álgebra Linear, diríamos que o determinante da transformação é $-1$.

:::{figure} ./figures/espelhoplano2.png
---
width: 300px
name: fig_espelhoplano2
---
:::

#### Múltiplos espelhos. 

:::{figure} ./figures/multiplosespelhos.png
---
width: 300px
name: fig_multiplosespelhos
---
:::

#### Exercício

Na configuração mostrada, demonstre que o ângulo do raio refletido final será sempre igual ao ângulo incidente.
:::{figure} ./figures/cuboLua.png
---
width: 300px
name: fig_cuboLua
---
:::

## Espelhos esféricos

A superfície refletora é esférica. 

### Espelho côncavo

Quando manipulamos um espelho côncavo, percebemos uma série de efeitos, a depender da distância do objeto ao espelho. A imagem pode ficar maior ou menor, direita (ereta) ou invertida. Vamos caracterizar todas essas situações neste seção.


#### Geometria do espelho:
    - Vértice (V)
    - Centro de curvatura (C)
    - Raio de curvatura (r)

:::{figure} ./figures/espelhoesfericogeometria1.png
---
width: 700px
name: fig_espelhoesfericogeometria1
---
:::

A seguir, obteremos relações geométricas que caracterizarão a formação da imagem. As deduções utilzarão a geometria indica na figura acima, na qual o objeto está à esquerda do centro de curvatura. Porém, as deduções se aplicarão a todas as posições do objeto.

#### Formação da imagem: aproximação paraxial

Se a luz atinge o espelho longe do vértice, ocorre aberração esférica:
:::{figure} ./figures/espelhoesfericoparaxial1.png
---
width: 320px
name: fig_espelhoesfericoparaxial1
---
:::
Os raios refletidos não convergem todos para o mesmo ponto e a imagem não se forma perfeitamente, ficando borrada. Para evitar essa situação, vamos trabalhar na chamada **aproximação paraxial**. Nela, os raios chegam ao espelho junto ao vértice (ângulos pequenos). Mostraremos que, na aproximação paraxial, todos os raios que emanam de um ponto convergem para o mesmo ponto: forma-se a imagem.

:::{figure} ./figures/espelhoesfericoparaxial0.png
---
width: 350px
name: fig_espelhoesfericoparaxial0
---
:::

:::{figure} ./figures/espelhoesfericoparaxial2.png
---
width: 500px
name: fig_espelhoesfericoparaxial0
---
:::


#### Distância objeto e distância imagem
Para um objeto puntiforme no eixo, qual é a relação entre a distância $s$ do objeto ao espelho e a distância $s'$ entre a imagem e o espelho?

Considere a figura que usamos para apresentear a [geometria do espelho côncavo](#fig_espelhoesfericogeometria1). Da análise do triângulo $\Delta$PAC, obtemos que $\beta = \alpha  + \theta$. Do triângulo $\Delta$PAP', obtemos: $\gamma = \alpha + 2\theta$. Portanto, obtemos:
\begin{equation}\label{eq:espelhoesferico0}
2\beta\,=\,\gamma\,+\,\alpha\;.
\end{equation}
Na aproximação paraxial, podemos escrever os àngulos em termos de arcos de circunferência aproximados. Teremos que $\alpha \approx \ell/s$, $\beta \approx \ell/r$ e $\gamma \approx \ell/s'$. Substituindo isso na relação acima, obtemos:
\begin{equation}\label{eq:espelhoesferico1}
2\frac{\ell}{r} = \frac{\ell}{s} + \frac{\ell}{s'}\;,
\end{equation}
e, portanto:
\begin{equation}\label{eq:espelhoesferico2}
\frac{1}{s} + \frac{1}{s'} = \frac{2}{r}\;.
\end{equation}

#### O plano focal do espelho esférico

Quando a fonte de luz está muito distante $(s \gg r$), os raios que atingem o espelho devem emanar da fonte com ângulos muito próximos, como sugere a figura abaixo:
:::{figure} ./figures/espelhoesfericoraiosparalelos.png
---
width: 500px
name: fig_espelhoesfericoraiosparalelos
---
:::
Em outras palavras, os raios chegam ao espelho paralelamente entre si. Como $1/s \ll 1/r$, podemos desprezar esse termo na equação [](#eq:espelhoesferico2), obtendo:
\begin{equation}\label{eq:espelhoesfericofoco}
\frac{1}{s'} = \frac{2}{r}\;, \hbox{ de modo que } \, s' = r/2.
\end{equation}
Assim, raios paralelos vindos de direções diferentes convergem para um ponto imagem a uma mesma distância $s'=r/2$ do vértice, a chamada **distância focal**:
\begin{equation}
f\,=\,\frac{r}{2}\,.
\end{equation}
:::{figure} ./figures/espelhoesfericofoco.png
---
width: 500px
name: fig_espelhoesfericofoco
---
:::
Portanto, raios paralelos oriundos de diferentes direções são refletidos em um plano, denominado **plano focal**.
:::{figure} ./figures/espelhoesfericoplanofocal.png
---
width: 400px
name: fig_espelhoesfericoplanofocal
---
:::

Em termos da distância focal obtemos a chamada **equação dos espelhos esféricos**:
```{math}
f = \frac{r}{2}\;\;\;\Rightarrow\;\;\;\frac{1}{s} + \frac{1}{s'} = \frac{1}{f}\;.
\label{eq:espelhoesferico3}
```

#### Raios principais (notáveis)

Para encontrar a imagem formada, trace os seguintes raios:
    - Raio paralelo ao eixo: é refletido no foco.
    - Raio apontando ou partindo do foco: reflete paralelamente ao eixo.
    - Raio apontando ou partindo do centro: reflete sobre si mesmo.
    - Raio que atinge o vértice: reflete simetricamente em relação ao eixo.

:::{figure} ./figures/espelhoesfericocomportamentoimagem1.png
---
width: 400px
name: fig_espelhoesfericocomportamentoimagem1
---
:::

:::{figure} ./figures/espelhoesfericocomportamentoimagem3.png
---
width: 350px
name: fig_espelhoesfericocomportamentoimagem3
---
:::

#### Exercício

Uma fonte puntiforme está a 12 cm de um espelho côncavo e 3,0 cm acima do eixo do espelho. O raio de curvatura do espelho é 6,0 cm. Encontre: (a) a distância focal do espelho e (b) a distância imagem. (c) Encontre a distância da imagem ao eixo.

:::{figure} ./figures/espelhoesfericoexerciciofoco.png
---
width: 400px
name: fig_espelhoesfericoexerciciofoco
---
:::

#### Convenção de sinais

As equações [](#eq:espelhoesferico2) e [](#eq:espelhoesferico3) são válidas para todas distâncias objeto, observada a seguinte convenção de sinais:

1) $s>0$ se o objeto está do mesmo lado que a luz incidente.
2) $s'>0$ se a imagem está do mesmo lado que a luz refletida.
3) $r>0$ e $f>0$ se $C$ está do lado da luz incidente. 

Observe que as relações continuam válidas para espelho convexos, desde que consideremos $r<0$ e $f<0$. 

#### Aumento (magnificação) lateral

O aumento lateral do espelho é a razão $y'/y$. Ele dá a razão entre o tamanho da imagem e o tamanho do objeto.

Para um objeto puntiforme fora do eixo, qual é a relação entre a distância $y$ do objeto ao eixo e a distância $y'$ da imagem ao eixo?
:::{figure} ./figures/espelhoesfericomagnificacao.png
---
width: 700px
name: fig_espelhoesfericomagnificacao
---
:::
A figura acima exibe dois raios notáveis que tornam muito direta a demonstração da relação:
```{math}
\frac{y'}{y} \;=\;-\;\frac{s'}{s}\;.
\label{eq:espelhoesferico2}
```
O sinal $-$ foi colocado à mão para indicar que, nesta configuração específica, a imagem é invertida. Assim, além do fator de amplificação, a razão $y'/y" dá a orientação da imagem em relação ao objeto: sinal positivo, mesma orientação; sinal negativo: orientação invertida. 


### Espelho convexo

Para espelhos convexos valem as mesmas expressões, desde que consideremos $r<0$. 

Pela equação dos espelhos esféricos, temos necessariamente que $s'<0$, isto é, a imagem é sempre virtual.

:::{figure} ./figures/espelhoesfericoconvexo.png
---
width: 350px
name: fig_espelhoesfericoconvexo
---
:::

#### Exercício

Um  objeto de 2,0 cm de altura está a 10,0 cm de um espelho convexo cujo raio de curvatura é 10 cm. (a) Localize a imagem e (b) encontre a altura da imagem.

:::{figure} ./figures/espelhoesfericoconvexo2.png
---
width: 500px
name: fig_espelhoesfericoconvexo2
---
:::

## Refração através de superfície esférica

Agora, os raios irão incidir e refratar através da superfície esférica. O resultado será uma combinação da geometria e da refração ao mudar de meio.

A geometria do problema está ilustrada na figura:
:::{figure} ./figures/refracaoesfera1.png
---
width: 600px
name: fig_refracaoesfera1
---
:::

As convenções que utilizaremos são:
1) $s>0$ se o objeto está do mesmo lado que a luz incidente.
2) $s'>0$ se a imagem está do lado refratado.
3) $r>0$ se $C$ está do lado da luz refratada. 

Vamos usar a Lei de Snell na apromação axial em que $\sin\theta\approx \theta$. Obteremos:
```{math}
n_1\,\theta_1 = n_2\,\theta_2
\label{eq:leidesnellparaxial}
```

Os triângulos relevantes são: $ACP'$ e $PAC$. Obtém-se: $\beta = \theta_2 + \gamma$ e $\theta_1 = \alpha + \beta$. Juntando as equações, obtemos:
```{math}
n_1\,\alpha + n_2\,\gamma = (n_2-n_1)\beta\;.
\label{eq:esferarefratoraaux1}
```
Usando que $\alpha\approx \ell/s$, $\gamma \approx \ell/s'$ e $\beta\approx \ell/r$, chegamos à equação::
```{math}
\frac{n_1}{s}+ \frac{n_2}{s'}= \frac{(n_2-n_1)}{r}\;.
\label{eq:equacaoesferarefratora}
```

A magnificação é dada pela relação:
```{math}
\frac{y'}{y}\;=\;\frac{-n_1 s'}{n_2\,s}\;.
\label{eq:magnificacaorefratora}
```
:::{figure} ./figures/refracaoesfera2.png
---
width: 400px
name: fig_refracaoesfera2
---
:::

**Exercício:** Um peixe está em um aquário de borda esférica, com raio de 15,0 cm. Um peixe observa o peixe de modo que seu nariz está a 10,0 cm da superfície do aquário. A luz refletida pelo nariz do gato se refrata através da superfície ar-água e forma uma umagem vista pelo peixe. Encontre: (a) a distância imagem e (b) a magnificação da imagem do nariz do gato. Despreze qualquer efeito óptico do vidro do aquário. Use $n_{agua} = 1,33$.
:::{figure} ./figures/refracaogatopeixe.png
---
width: 500px
name: fig_refracaogatopeixe
---
:::

Com as convenções adotadas, as equações desta seção se aplicam a superfícies refratoras côncavas ($R< 0$) e para quaisquer sinais de $s$ e $s'$. Em particular, podemos tomar o limite $r\rightarrow \infty$, que corresponde a considerar a superfície plana. Teremos:
```{math}
s'\;=\;\frac{-n_2 s}{n_1}\;.
\label{eq:magnificacaorefratoraRinfty}
```

## Lentes finas

Vamos modelar as lentes como um meio com índice de rafração $n$. A luz incidirá a partir do ar, sofrerá difração ao entrar na lente e ao voltar para o ar. Para simplificar, vamos admitir que cada metade da lente é formada por uma calota esférica ou por uma superfície plana. Os raios de curvatura usados podem ser diferentes, e serão denotados por $r_1$ e $r_2$. A formação final da imagem envolve a aplicação dupla de expressões conhecidas.

Para ilustrar, vamos considerar uma lente biconvexa:
:::{figure} ./figures/lentes1.png
---
width: 700px
name: fig_lentes1
---
:::

A imagem do ponto $P$ para a superfície refratora convexa será virtual e vale a relação:
```{math}
\frac{n_{ar}}{s}+ \frac{n}{s_1'}= \frac{(n-n_{ar})}{r_1}\;.
\label{eq:equacaolenteaux1}
```
A luz refratada através da primeira superfície atinge a segunda, que é uma superfície refratora côncava ($r_2<0$). Tudo se passa como se o raio viesse do ponto $P_1'$, à esquerda de $P$ (na posição $s_1'<0$).  Portanto, podemos considerar esse ponto como objeto para a segunda superfície refratora. Considerando que a maior espessura da lente é menor que as dimensões envolvidas, a distância objeto para a segunda refração é $s_2 = -s_1$. Teremos:
```{math}
\frac{n}{-s_{1'}} + \frac{n_{ar}}{s'}= \frac{{n_{ar}-n}}{r_2}\;.
\label{eq:equacaolenteaux2}
```
Eliminando o parâmetro intermediário $s_1'$, obtemos:
$$
\frac{1}{s}+ \frac{1}{s'}= \left(\frac{n}{n_{ar}}-1\right)\left(\frac{1}{r_1}-\frac{1}{r_2}\right)
$$
