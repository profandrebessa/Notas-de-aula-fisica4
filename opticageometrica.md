
# Óptica geométrica

As figuras destas notas de aula são quase todas extraídas do livro: "Física para Cientistas e Engenheiros - Volume 3: Física Moderna", de Paul A. Tipler e Gene Mosca, que é uma referência bastante recomendada pelo professor. A notação utilizada também é a mesma desta referẽncia.

A discussão procura ser particularizada para o interesse de um curso de Licencitura. Uma referência auxiliar importante é o livro "Curso de Física Básica, Volume 4" de H. Moysés Nussenzveig.

Nesta seção iremos estudar espelhos e superfícies refratoras. Para os espelhos vamos utilizar simplesmente que o ângulo de reflexão é igual ao ângulo de incidência. Para as superfícies refratoras, vamos usar a Lei de Snell:
```{math}
n_1\,\sin \theta_1 = n_2\,\sin\theta_2
\label{eq:leidesnell2}
```

## Espelhos planos

As propriedades da formação das imagens dos espelhos dependem de relações geométricas. O estudo dos espelhos é uma oportunidade de revisar e aplicar os conceitos da Geometria Euclideana.

#### Formação de uma imagem perfeita

Considere uma fonte luminosa pontual. Nas figuras, essa fonte será denotada pela letra $P$. Raios são emitidos em todas as direções e serão refletidos no espelho. É importante compreender que a reflexão será tal que todos os raios refletidos parecerão ser emitidos de um mesmo ponto $P'$, localizado atrás do espelho. Como não chegam (e, portanto, não emanam) raios em $P'$, essa convergência do prolongamento dos raios não pode ser captada por um anteparo atrás do espelho. Dizemos que a imagem é virtual.

A demonstração de que todos os raios refletidos parecem ser emitidos de $P'$ é simples. Considere um raio qualquer que atinge o espelho formando um ângulo $\theta$ com a normal. Além disso, considere um raio que atinge o espelho em ângulo zero. Os prolongamentos dos dois raios se encontram em um ponto $P'$. A questão é: esse ponto $P'$ depende de $\theta$? 

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

#### Múltiplos espelhos planos
Quando há N espelhos planos próximos, é possível que um observador perceba mais de N imagens a partir de uma única fonte pontual. Isso acontece por conta das múltiplas reflexões, como sugere a imagem abaixo:
:::{figure} ./figures/multiplosespelhos.png
---
width: 300px
name: fig_multiplosespelhos
---
:::
Perceba que um observador na posição indicada pelo olho recebe os raios de $P_1'$ e $P_2'$ obtidos pelo prolongamento dos raios refletidos uma vez no espelho 1 e no espelho 2, respectivamente. Mas, o observador vê também uma imagem obtida pelo prolongamento de raios que refletiram uma vez no espelho 1 e, em seguida, refletiram novamente no espelho 2. Esses raios parecem ter sido emitidos da posição $P_{12}'$. 

A quantidade de imagens vai depender da quantidade de espelhos, de suas posições e da posição do observador. 

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

Primeiramente, perceba na [figura acima](#fig_espelhoesfericogeometria1) que, diferentemente do espelo plano, o espelho côncavo pode convergir os raios e formar uma imagem real, que pode ser projetada em um anteparo. Mais à frente, veremos que, quando o objeto está mais próximo do vértice, os raios deixam de convergir e uma imagem é formada atrás do espelho pelo prolongamento dos raios (imagem virtual). 

Outra diferença em relação aos espelhos planos é a seguinte: se a luz atinge o espelho longe do vértice ocorre aberração esférica:
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
\frac{2}{r} = \frac{1}{s} + \frac{1}{s'}\;.
\end{equation}
O fato de a distância $s'$ não depender de $\theta$ é a expressão matemática da formação perfeita da imagem do ponto $P$ em $P'$. Como já foi dito, esse resultado só é válido na aproximação paraxial.

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
Exemplo de traçado de raios principais.
:::

:::{figure} ./figures/esfericoentreCeF.png
---
width: 350px
name: fig_esfericoentreCeF
---
Traçado de raios principais: segunda situação.
:::

:::{figure} ./figures/espelhoesfericocomportamentoimagem3.png
---
width: 350px
name: fig_espelhoesfericocomportamentoimagem3
---
Traçado de raios principais: terceira situação.
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

A magnificação lateral relaciona a variação das dimensões perpendiculares ao eixo do espelho. Já para um objeto fino colocado no eixo do espelho, cada parte do objeto estará a uma distância $s$ diferente do vértice, de modo que a situação final da imagem dependerá da geometria do problema.

#### Comportamento da imagem

Conforme dito no início, a imagem formada por um espelho côncavo muda suas características a depender da distância $s$ ao vértice. Estamos em condições de compreender todos os casos possíveis.

- Objeto à esquerda de C ($s>r$): a imagem é real, invertida e menor, como na [](fig_espelhoesfericocomportamentoimagem1)
- Objeto no centro de curvatura ($s=r$): a imagem é real, invertida e de mesmo tamanho.
- Objeto entre C e o foco ($r> s> f$): a imagem é real, invertida e maior.
- Objeto no foco ($s = f$): a imagem se forma no infinito (raios saem paralelamente ao eixo).
- Objeto entre o foco e o vértice ($f > s$): a imagem é virtual, direita e maior, como na [](fig_espelhoesfericocomportamentoimagem3).

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

### Formação da imagem

A próxima figura ilustra a diferença entre as direções dos raios na reflexão e na refração quando o **meio 2 é mais refringente que o meio 1**:
:::{figure} ./figures/refracaoereflexao.png
---
width: 500px
name: fig_refracaoereflexao
---
:::
Note que o raio relevante agora é o raio transmitido. Ele sofre um desvio na direção, se aproximando da normal (no caso em que $n_2>n_1$). Vimos que, em geral, uma fração da energia incidente é refletida e o restante é transmitido. No estudo da óptica de superfícies refratoras, vamos considerar que não haja reflexão, assim como no estudo dos espelhos ignoramos a refração.

A geometria do problema está ilustrada na figura a seguir, para o caso de um raio incidente paralelo ao eixo da superfície esférica:
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
Note que, por essas convenções, $r>0$ para uma superfície refratora convexa.

Vamos usar a **Lei de Snell na apromação axial** em que $\sin\theta\approx \theta$. Obteremos:
```{math}
n_1\,\theta_1 = n_2\,\theta_2
\label{eq:leidesnellparaxial}
```

Os triângulos relevantes são: $\Delta$ACP' e $\Delta$PAC. Obtém-se: $\beta = \theta_2 + \gamma$ e $\theta_1 = \alpha + \beta$. Juntando as equações, obtemos:
```{math}
n_1\,\alpha + n_2\,\gamma = (n_2-n_1)\beta\;.
\label{eq:esferarefratoraaux1}
```
Usando que $\alpha\approx \ell/s$, $\gamma \approx \ell/s'$ e $\beta\approx \ell/r$, chegamos à equação::Conhecendo-se as distâncias focais, 
```{math}
\frac{n_1}{s}+ \frac{n_2}{s'}= \frac{(n_2-n_1)}{r}\;.
\label{eq:equacaoesferarefratora}
```

Para raio incidentes paralelos ao eixo $(s \rightarrow \infty)$, a imagem se forma no chamado **foco imagem**. Indicando a distância focal imagem por $f'$, temos:
\begin{equation}\label{eq:equacaoesferarefratorafocoimagem}
\frac{n_2}{f'}= \frac{(n_2-n_1)}{r}\;.
\end{equation}
A imagem se forma no infinito $(s' \rightarrow \infty)$ quando o objeto está localizado no **foco objeto**. Indicando por $f$ a distância focal objeto, temos:
\begin{equation}\label{eq:equacaoesferarefratorafocoobjeto}
\frac{n_1}{f}= \frac{(n_2-n_1)}{r}\;.
\end{equation}
Portanto, diferentemente do caso do espelho esférico, temos dois planos focais e duas distâncias focais diferentes. O sinal de $f$ e $f'$ é o mesmo e depende da natureza das superfícies (côncava ou convexa) e de se a luz passa para um meio mais refringente ($f,f' >0$, imagem real) ou menos refringente ($f,f'<0$, imagem virtual e objeto virtual.)
:::{figure} ./figures/refracaofocosconvexoAB.png
---
width: 700px
name: refracaofocosconvexoAB
---
Superfície esférica refratora convexa com $n_1 <> n_2$. Os dois focos são reais e têm distância focal diferente.
:::
:::{figure} ./figures/refracaofocosconvexoCD.png
---
width: 700px
name: refracaofocosconvexoCD
---
Superfície esférica refratora convexa com $n_1 > n_2$. Os dois focos são virtuais. "Objeto virtual" não corresponde a um objeto, mas à condição incomum em que a luz incidente apresenta raios convergentes, em direção à posção objeto negativa (virtual). Essa condição é produzida, no primeiro gráfico da Figura [](refracaofocosconvexoAB) ou em lentes convergentes.
:::
:::{figure} ./figures/refracaofocosconcavoAB.png
---
width: 700px
name: refracaofocosconcavoAB
---
Superfície esférica refratora côncava ($r<0$) com $n_1 <> n_2$. Novamente, os dois focos são virtuais. Em relação à situação anterior, a troca de $n_1$ por $n_2$, de $r$ por $-r$ e $f$ por $f'$ leva à mesma situação, como pode ser entendido também pelas equações. 
:::
:::{figure} ./figures/refracaofocosconcavoCD.png
---
width: 700px
name: refracaofocosconcavoCD
---
Superfície esférica refratora côncava com $n_1 > n_2$. 
:::

#### Raios principais (notáveis)

Para encontrar a imagem formada, trace os seguintes raios (conhecendo-se as distâncias focais):
- Raio incidente paralelo ao eixo: raio refratado (ou seu prolongamento) passando pelo foco imagem.
- Raio partindo do foco objeto: refrata paralelamente.
- Raio apontando ou partindo do centro: refrata sem desvio.

O raio que atinge o vértice, tal como todos os outros, refrata seguindo a Lei de Snell. Sua particularidade é que a normal ao espelho no vértice é o eixo do espelho.

#### Magnificação lateral

A magnificação $y'/y$ pode ser facilmente obtida traçando-se um raio incidente dirigido ao vértice:
:::{figure} ./figures/refracaoesfera2.png
---
width: 400px
name: fig_refracaoesfera2
---
:::
Teremos:
\begin{equation}
\tan \theta_1 = \frac{y}{s}\;\;\;\hbox{e}\;\;\;\tan \theta_2 = \frac{-y'}{s'}. 
\end{equation}
Perceba que $y'<0$ (imagem invertida). 

Na aproximação paraxial, temos $\tan \theta \approx \theta$, de modo que:
\begin{equation}
\frac{y'}{y} = -\frac{s'\,\tan \theta_2}{s\,\tan\theta_1} = -\frac{s'\,\theta_2 }{s\,\theta_1}\,. 
\end{equation}
Usando a [Lei de Snell na aproximação paraxial](eq:leidesnellparaxial), chegamos em:
\begin{equation}\label{eqrefracaoaumentolateral}
\frac{y'}{y}\;=\;\frac{-n_1 s'}{n_2\,s}\;.
\end{equation}
É essa magnifação lateral que explica por que os objetos parecem mais espessos dentro da água. 

#### Exercício
 
 Um peixe está em um aquário de borda esférica, com raio de 15,0 cm. Um gato observa o peixe de modo que seu nariz está a 10,0 cm da superfície do aquário. A luz refletida pelo nariz do gato se refrata através da superfície ar-água e forma uma umagem vista pelo peixe. Encontre: (a) a distância imagem e (b) a magnificação da imagem do nariz do gato. Despreze qualquer efeito óptico do vidro do aquário. Use $n_{agua} = 1,33$.
:::{figure} ./figures/refracaogatopeixe.png
---
width: 500px
name: fig_refracaogatopeixe
---
:::

Com as convenções adotadas, as equações desta seção se aplicam a superfícies refratoras côncavas ($R< 0$) e para quaisquer sinais de $s$ e $s'$. Em particular, podemos tomar o limite $r\rightarrow \infty$, que corresponde a considerar a superfície plana. Teremos:
```{math}
s'\;=\;\frac{-n_2\,s}{n_1}\;.
\label{eq:magnificacaorefratoraRinfty}
```
Assim, para superfícies refratoras planas, $s'$ terá o sinal oposto ao de $s$: a imagem será virtual. Além disso, terá o mesmo tamanho, como vemos ao aplicar a equação [](eqrefracaoaumentolateral). Quando a luz passa da água para o ar, a imagem parece se aproximar da interface plana. Lembre que, como $n_2<n_1$, desta vez na refração o raio irá se afastar da normal ao ir para o ar. Tente entender o traçado de raios mostrado na figura abaixo. 
:::{figure} ./figures/refracaoaguaarvertical.png
---
width: 250px
name: refracaoaguaarvertical
---
:::
Esse comportamento explica por que o fundo de uma piscina, quando visto de cima, parece menos profundo. Para a água, $n \approx 4/3$, de forma que a profundidade aparente da água na piscina quando vista de cima é $3/4$ da real. Por experiência, os indígenas miram suas flexas abaixo da imagem do peixe que querem capturar.
:::{figure} ./figures/refracaoindigena.png
---
width: 300px
name: refracaoindigena
---
:::

    i
### Aberração cromática

Vimos que as ondas eletromagnéticas em um meio apresentam dispersão, isto é, têm índice de refração que varia com a frequência. Portanto, a imagem de uma fonte pontual não-monocromática irá se formar em diferentes posições e com diferentes magnificações a depender da frequências. Em termos de cores, a imagem de uma luz branca através de uma superfície esférica refratora será uma mancha levemente colorida.


## Lentes delgadas

Vamos modelar as lentes como um meio com índice de refração $n$. A luz incidirá a partir do ar, sofrerá difração ao entrar na lente e ao voltar para o ar. Para simplificar, vamos admitir que cada metade da lente é formada por uma calota esférica ou por uma superfície plana. A figura abaixo exibe os seguintes tipos de lente: (a) biconvexa; (b) plano-convexa; (c) menisco positivo; (d) bicôncava; (4) plano-côncava; (f) menisco negativo.
:::{figure} ./figures/lentestipos.png
---
width: 400px
name: fig_lentestipos
---
:::

Os raios de curvatura usados podem ser diferentes, e serão denotados por $r_1$ e $r_2$. A formação final da imagem envolve a aplicação dupla de expressões conhecidas.

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
A luz refratada através da primeira superfície atinge a segunda, que é uma superfície refratora côncava ($r_2<0$). Tudo se passa como se o raio viesse do ponto $P_1'$, à esquerda de $P$ (na posição $s_1'<0$).  Portanto, podemos considerar esse ponto como objeto para a segunda superfície refratora. Considerando que a maior espessura da lente é menor que as dimensões envolvidas, a distância objeto para a segunda refração é $s_2 = -s_1'$. Teremos:
```{math}
\frac{n}{-s_{1'}} + \frac{n_{ar}}{s'}= \frac{{n_{ar}-n}}{r_2}\;.
\label{eq:equacaolenteaux2}
```
Eliminando o parâmetro intermediário $s_1'$, obtemos:
\begin{equation}\label{eq:eqlente}
\frac{1}{s}+ \frac{1}{s'}= \left(\frac{n}{n_{ar}}-1\right)\left(\frac{1}{r_1}-\frac{1}{r_2}\right)
\end{equation}

A equação deduzida vale para todos os tipos de lente, se adotarmos a seguinte convenção de sinais:
1) $s>0$ se o objeto está do mesmo lado que a luz incidente.
2) $s'>0$ se a imagem está do lado oposto ao incidente.
3) O raio de curvatura de cada superfície esférica é positivo se o respectivo $C$ está do lado da luz refratada na superfície. 

Vemos que o a distância focal objeto é igual à distância focal imagem, dadas por:
\begin{equation}\label{eq:focodalente}
\frac{1}{f}= \left(\frac{n}{n_{ar}}-1\right)\left(\frac{1}{r_1}-\frac{1}{r_2}\right)
\end{equation}
de modo que a [equação da lente](eq:eqlente) pode ser escrita como:
\begin{equation}\label{eq:eqlentefoco}
\frac{1}{s}+ \frac{1}{s'}= \frac{1}{f}\;,
\end{equation}
que, por coincidência, tem a mesma forma da equação do espelho esférico. Porém, a imagem se forma por mecanismos físicos diferentes, o que fica nítido pelo fato de a  a distância focal da lente depender dos raios $r_1$ e $r_2$ e do índice de refração relaivo, enquanto que, para o espelho, a distância focal depende apenas do raio. 

Note que a lente tem dois planos focais, um em cada lado da lente, e que a igualdade das distâncias focais só acontece por termos considerado o mesmo índice de refração dos dois lados da lente. 

#### Exercício:

Uma lente delgada de vidro, biconvexa, com índice de refração n=1,5 possui raios de curvatura com magnitudes de 10 cm e 15 cm, como mostrado na figura abaixo. Mostre que sua distância focal no ar é 12 cm.
:::{figure} ./figures/lentesexerciciobiconvexa.png
---
width: 500px
name: lentesexerciciosbiconvexa.png
---
:::

Se luz paralela incide sobre a lente do exercício anterior pela esquerda, ela é focalizada em um ponto a 12 cm à direita da lente; enquanto, se luz paralela incide sobre a lente pela direita, ela é focalizada a 12 cm à esquerda da lente. 
:::{figure} ./figures/lentesfoco0.png
---
width: 350px
name: lentesfoco0.png
---
:::
Usando a propriedade de reversibilidade dos raios de luz, podemos ver que a luz que diverge de um foco e incide sobre uma lente emerge dela como um feixe paralelo, como mostrado na figura abaixo.
:::{figure} ./figures/lentesfocos.png
---
width: 500px
name: lentesfocos.png
---
:::

Raios incidentes paralelos ao eixo emergem em direção a um dos focos, ou afastando-se dele. Reciprocamente, raios incidentes dirigidos para um dos focos, ou afastando-se dele, emergem paralelos ao eixo.

Para uma lente convergente, o foco objeto está no lado da luz incidente e o foco imagem está no lado da luz refratada (para uma lente divergente ocorre o contrário). Se luz paralela incide sobre a lente fazendo um pequeno ângulo com o eixo, ela é focalizada em um ponto no plano focal a uma distância $f$ da lente.

O inverso da distância focal é chamado de **dioptria** (representada pela letra $D$ e popularmente chamada de **grau** da lente). Quando a distância focal é expressa em metros, a dioptria é dada em $m^{-1}$

A dioptria de uma lente mede sua capacidade de focalizar luz paralela a uma curta distância da lente. Quanto menor a distância focal, maior a dioptria. Por exemplo, uma lente com distância focal de $25,0$ cm tem dioptria de $4,0$ D. Uma lente com distância focal de $10,0$ cm tem potência de $10,0$ D. Como a distância focal de uma lente divergente é negativa, sua dioptria também é negativa.

#### Exercício
:::{figure} ./figures/lentesexerciciomenisco.png
---
width: 500px
name: lentesexerciciomenisco.png
---
:::

A lente mostrada na figura abaixo tem índice de refração 1,5 e raios de curvatura de $10,0$ cm e $13,0$ cm. Encontre: (a) sua distância focal e (b) sua dioptria.


#### Raios principais (notáveis)

Uma vez calculada a distância focal da lente, para encontrar a imagem formada, trace os seguintes raios:
- Raio incidente paralelo ao eixo: atravessa a lente e passa pelo foco imagem.
- Raio partindo do foco objeto: atravessa a lente e sai paralelo ao eixo da lente.
- Raio apontando ou partindo do centro da lente: atravessa sem desvio.

Veja o traçado dos raios notáveis para uma lente biconvexa:
:::{figure} ./figures/refracaonotaveisbiconvexa.png
---
width: 600px
name: refracaonotaveisbiconvexa.png
---
:::
e bicôncava:
:::{figure} ./figures/refracaonotaveisbiconcava.png
---
width: 500px
name: refracaonotaveisbiconcava.png
---
:::
Observe a posição invertida do foco imagem e do foco objeto, quando comparamos a lente biconvexa com a bicôncava.
