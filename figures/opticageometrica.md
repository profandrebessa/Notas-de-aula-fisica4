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

#### Exercício: espelhos perpendiculares

Na configuração mostrada, demonstre que o ângulo do raio refletido final será sempre igual ao ângulo incidente.
:::{figure} ./figures/cuboLua.png
---
width: 300px
name: fig_cuboLua
---
:::

## Espelhos esféricos

Agora, a superfície refletora é esférica. A formação das imagens continua sendo ditada pela lei: o ângulo de reflexão é igual ao de incidência. Porém, como a direção normal será diferente para cada parte do espelho, será preciso analisar com cuidado a formação da imagem. Faremos todas as deduções para a geometria de um espelho côncavo. Porém, as expressões obtidas poderão ser facilmente adaptadas aos espelhos convexos.  

### Espelho côncavo

Quando manipulamos um espelho côncavo, percebemos uma série de efeitos, a depender da distância do objeto ao espelho. A imagem pode ficar maior ou menor, direita (ereta) ou invertida. Vamos caracterizar todas essas situações neste seção.


#### Geometria do espelho:
    - Vértice (ponto V)
    - Centro de curvatura (ponto C)
    - Raio de curvatura (distância r)

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
\frac{1}{s} + \frac{1}{s'} = \frac{1}{f}\;.
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
width: 450px
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

#### Exercício: distante de um espelho côncavo

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

Observe que as relações continuam válidas para espelhos convexos, desde que consideremos $r<0$ e $f<0$. 

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
O sinal $-$ foi colocado à mão para indicar que, nesta configuração específica, a imagem é invertida. Assim, além do fator de amplificação, a razão $y'/y$ dá a orientação da imagem em relação ao objeto: sinal positivo, mesma orientação; sinal negativo: orientação invertida. 

A magnificação lateral relaciona a variação das dimensões perpendiculares ao eixo do espelho. Já para um objeto fino colocado no eixo do espelho, cada parte do objeto estará a uma distância $s$ diferente do vértice, de modo que a situação final da imagem dependerá da geometria do problema.

#### Comportamento da imagem

Conforme dito no início, a imagem formada por um espelho côncavo muda suas características a depender da distância $s$ ao vértice. Estamos em condições de compreender todos os casos possíveis.

- Objeto à esquerda de C ($s>r$): a imagem é real, invertida e menor, como na [](fig_espelhoesfericocomportamentoimagem1)
- Objeto no centro de curvatura ($s=r$): a imagem é real, invertida e de mesmo tamanho.
- Objeto entre C e o foco ($r> s> f$): a imagem é real, invertida e maior, como na [](fig_esfericoentreCeF).
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

#### Exercício: imagem em espelho convexo

Um  objeto de 2,0 cm de altura está a 10,0 cm de um espelho convexo cujo raio de curvatura é 10 cm. (a) Localize a imagem e (b) encontre a altura da imagem.

:::{figure} ./figures/espelhoesfericoconvexo2.png
---
width: 500px
name: fig_espelhoesfericoconvexo2
---
:::

## Refração através de superfície esférica

Agora, os raios irão incidir e refratar através da superfície esférica. O resultado será uma combinação da geometria e da refração ao mudar de meio.

#### Formação da imagem

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
Usando que $\alpha\approx \ell/s$, $\gamma \approx \ell/s'$ e $\beta\approx \ell/r$, chegamos à equação para as superfícies esféricas refratoras: 
\begin{equation}\label{eq:equacaoesferarefratora}
\frac{n_1}{s}+ \frac{n_2}{s'}= \frac{(n_2-n_1)}{r}\;.
\end{equation}
Para raio incidentes paralelos ao eixo $(s \rightarrow \infty)$, a imagem se forma no chamado **foco imagem**. Indicando a distância focal imagem por $f'$, temos:
\begin{equation}\label{eq:equacaoesferarefratorafocoimagem}
\frac{n_2}{f'}= \frac{(n_2-n_1)}{r}\;.
\end{equation}
A imagem se forma no infinito $(s' \rightarrow \infty)$ quando o objeto está localizado no **foco objeto**. Indicando por $f$ a distância focal objeto, temos:
\begin{equation}\label{eq:equacaoesferarefratorafocoobjeto}
\frac{n_1}{f}= \frac{(n_2-n_1)}{r}\;.
\end{equation}
Portanto, diferentemente do caso do espelho esférico, temos dois planos focais e duas distâncias focais diferentes. O sinal de $f$ e o de $f'$ é o mesmo e depende da natureza das superfícies (côncava ou convexa) e de se a luz passa para um meio mais refringente ($f,f' >0$, imagem real) ou menos refringente ($f,f'<0$, imagem virtual e objeto virtual.)
:::{figure} ./figures/refracaofocosconvexoAB.png
---
width: 700px
name: refracaofocosconvexoAB
---
Superfície esférica refratora convexa com $n_1  <n_2$. Os dois focos são reais e têm distância focal diferente.
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
Superfície esférica refratora côncava ($r<0$) com $n_1 < n_2$. Novamente, os dois focos são virtuais. Em relação à situação anterior, a troca de $n_1$ por $n_2$, de $r$ por $-r$ e $f$ por $f'$ leva à mesma situação, como pode ser entendido também pelas equações. 
:::
:::{figure} ./figures/refracaofocosconcavoCD.png
---
width: 700px
name: refracaofocosconcavoCD
---
Superfície esférica refratora côncava com $n_1 > n_2$. 
:::
Em termos de $f$ (ou $f'$), temos a equação:
\begin{equation}
\frac{n_1}{s}+\frac{n_2}{s'} = \frac{n_1}{f} =\frac{n_2}{f'}\,. 
\end{equation}

#### Situação final da imagem: real ou virtual?

Tal como no caso de um espelho esférico, a natureza da imagem vai depender da distância objeto. Porém, agora a natureza da imagem vai depender também da diferença entre os índices de refração. A figura abaixo analisa um raio que parte do ponto P no eixo da superfície convexa refratora, passando de um meio menos refringente ($n_1$) para um meio mais refringente ($n_2$). Nesta situação, o raio refratado irá se aproximar da normal. O desvio, porém, depende de $n_1$ e $n_2$. 

Se o desvio for pequeno (raio refratado desenhado em vermelho, para ilustrar), a imagem será virtual (raios divergem a partir do ponto de incidência, dando a impressão de partir de um ponto à esquerda). 

Para um determinado valor intermediário de $n_2$ o raio refratado (raio azul) sairá paralelo. O ponto $P$ será o foco objeto, e a imagem se formará no infinito, como na situação de baixo da [](refracaofocosconvexoAB).

 Finalmente, aumentando ainda mais $n_2$ (situação ilustrada pelo raio verde), haverá convergência na região refratada, e a imagem será real. É esta a situação detalhada na [](fig_refracaoereflexao).

:::{figure} ./figures/refracaorealvirtualfoco.png
---
width: 800px
name: refracaorealvirtualfoco
---
:::
Ser grande ou pequeno é algo pouco preciso. Para superfícies convexas e na situação em que $n_2>n_1$, a condição precisa para a imagem ser real $(s'>0)$ é $s < f$, ou seja: $s<r/(n_{21}-1)$, onde $n_{21} =n_2/n_1$ é o índice de refração relativo. Perceba que, na aproximação paraxial, essas conclusões não dependem do ângulo $\theta_1$ (ângulo de incidência).


#### Raios principais (notáveis)

Para encontrar a imagem formada, trace os seguintes raios (conhecendo-se as distâncias focais):
- Raio incidente paralelo ao eixo: raio refratado (ou seu prolongamento) passando pelo foco imagem.
- Raio apontando ou partindo do foco objeto: refrata paralelamente.
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

#### Exercício: dentro do aquário
 
 Um peixe está em um aquário de borda esférica, com raio de 15,0 cm. Um gato está nas proximidades, de modo que seu nariz está a 10,0 cm da superfície do aquário. A luz refletida pelo nariz do gato se refrata através da superfície ar-água e forma uma umagem vista pelo peixe. Encontre: (a) a distância imagem e (b) a magnificação da imagem do nariz do gato. Despreze qualquer efeito óptico do vidro do aquário. Use $n_{agua} = 1,33$.
:::{figure} ./figures/refracaogatopeixe.png
---
width: 500px
name: fig_refracaogatopeixe
---
:::

#### Limite $\small R \rightarrow \infty$: superfície plana

Com as convenções adotadas, as equações desta seção se aplicam a superfícies refratoras côncavas ($R< 0$) e para quaisquer sinais de $s$ e $s'$. Em particular, podemos tomar o limite $r\rightarrow \infty$, que corresponde a considerar a superfície plana. Teremos, pela equação [](eq:equacaoesferarefratora):
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

#### Aberração cromática

Vimos que as ondas eletromagnéticas em um meio apresentam dispersão, isto é, têm índice de refração que varia com a frequência. Portanto, a imagem de uma fonte pontual não-monocromática irá se formar em diferentes posições e com diferentes magnificações a depender da frequências. Em termos de cores, a imagem de uma luz branca através de uma superfície esférica refratora será uma mancha levemente colorida.

#### Exercício: desvio cromático

Luz branca incide, a partir do ar, sobre uma superfície esférica convexa de vidro. O raio de curvatura da superfície é 10 cm. O vidro tem índice de refração igual a 1,530 para luz azul e 1,470 para luz vermelha. Encontre a distância focal para cada uma das frequências.

## Lentes delgadas

Vamos modelar as lentes como um meio com índice de refração $n$. A luz incidirá a partir do ar, sofrerá refração ao entrar na lente e ao voltar para o ar. Para simplificar, vamos admitir que cada metade da lente seja formada por uma calota esférica ou por uma superfície plana (limite $\small R\rightarrow \infty$ de uma superfície esférica). 

#### Tipos de lente

A figura abaixo exibe os seguintes tipos de lente: (a) biconvexa; (b) plano-convexa; (c) menisco positivo; (d) bicôncava; (4) plano-côncava; (f) menisco negativo.
:::{figure} ./figures/lentestipos.png
---
width: 400px
name: fig_lentestipos
---
Alguns tipos de lente.
:::
Os raios de curvatura usados podem ser diferentes, e serão denotados por $r_1$ e $r_2$. As lentes serão delgadas, isto é, consideraremos que a maior espessura da lente é menor que as dimensões envolvidas (raios de curvatura, distância objeto e distância imagem).

#### Formação da imagem

A formação final da imagem envolve a aplicação dupla de expressões conhecidas.
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
Vamos admitir que o ponto $P$ esteja entre o foco objeto e o vértice da superfície convexa. Nesta situação (caso do raio vermelho na [](refracaorealvirtualfoco)), os raios atravessam a superfície convexa como se estivem vindo de um ponto $P_1'$, à esquerda de $P$ (na posição $s_1'<0$). A luz refratada através da primeira superfície atinge a segunda, que é uma superfície refratora côncava ($r_2<0$). Podemos considerar o ponto $P'$  como objeto para a segunda superfície refratora. Desprezando a espessura da lente, a distância objeto para a segunda refração é $s_2 = -s_1'$. Teremos:
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
que, por coincidência, tem a mesma forma da equação do espelho esférico. Porém, a imagem se forma por mecanismos físicos diferentes, o que fica nítido pelo fato de a distância focal da lente depender dos raios $r_1$ e $r_2$ e do índice de refração relaivo, enquanto que, para o espelho, a distância focal depende apenas do raio. 

Na equação [](eq:focodalente), como $n>n_{ar}$, o sinal de $f$ será determinado por $r_1$ e $r_2$. Na [](fig_lentestipos), as três primeiras lentes têm a metade esquerda convexa ($r_1>0$) e a segunda metade tem raio de curvatura negativo, infinito ou positivo, porém maior que $r_1$. Assim, as três primeiras lentes têm distância focal positiva, ou seja, são lentes convergentes. O oposto se dá com as 3 lentes à direita na [](fig_lentestipos).

:::{note}
:name: regrageraltipolente
Como regra geral, as lentes mais espessas no centro do que nas extremidades são convergentes. As lentes divergentes são menos espessas no centro.
:::

Note que a lente tem dois planos focais, um em cada lado da lente, e que a igualdade das distâncias focais só acontece por termos considerado o mesmo índice de refração dos dois lados da lente. 


#### Exercício: lente biconvexa

Uma lente delgada de vidro, biconvexa, com índice de refração n=1,5 possui raios de curvatura com magnitudes de 10 cm e 15 cm, como mostrado na figura abaixo. Mostre que sua distância focal no ar é 12 cm.
:::{figure} ./figures/lentesexerciciobiconvexa.png
---
width: 500px
name: lentesexerciciosbiconvexa.png
---
:::

Se luz paralela incide sobre a lente do exercício anterior pela esquerda, ela é focalizada em um ponto a 12 cm à direita da lente; enquanto, se luz paralela incide sobre a lente pela direita, ela é focalizada a 12 cm à esquerda da lente. A figura abaixo mostra a formação da imagem no plano focal. Nela, luz paralela incide sobre a lente fazendo um pequeno ângulo com o eixo. A luz é focalizada em um ponto no plano focal a uma distância $f$ da lente. Em particular, raios incidentes paralelos ao eixo emergem em direção a um dos focos, ou afastando-se dele.

:::{figure} ./figures/lentesfocos.png
---
width: 500px
name: lentesfocos.png
---
:::
A figura abaixo mostra o comportamento da luz através da lente quando a luz é emitida por uma fonte em um dos focos da lente:
:::{figure} ./figures/lentesfoco0.png
---
width: 350px
name: lentesfoco0.png
---
:::

Para uma lente convergente, o foco objeto está no lado da luz incidente e o foco imagem está no lado da luz refratada (para uma lente divergente ocorre o contrário). 

O inverso da distância focal é chamado de **poder de convergência** ou **dioptria**  da lente (representada pela letra $D$ e popularmente chamada de **grau** da lente). Quando a distância focal é expressa em metros, a dioptria é dada em $m^{-1}$.

A dioptria de uma lente mede sua capacidade de focalizar luz paralela a uma curta distância da lente. Quanto menor a distância focal, maior a dioptria. Por exemplo, uma lente com distância focal de $25,0$ cm tem dioptria de $4,0$ m$^{-1}$. Uma lente com distância focal de $10,0$ cm tem dioptria de $10,0$ $^{-1}$. Como a distância focal de uma lente divergente é negativa, sua dioptria também é negativa.

#### Exercício: menisco positivo
A lente mostrada na figura abaixo tem índice de refração 1,5 e raios de curvatura de $10,0$ cm e $13,0$ cm. Encontre: (a) sua distância focal e (b) sua dioptria.
:::{figure} ./figures/lentesexerciciomenisco.png
---
width: 500px
name: lentesexerciciomenisco.png
---
:::



#### Raios principais (notáveis)

Uma vez conhecida (ou calculada) a distância focal da lente, para encontrar a imagem formada, trace os seguintes raios:
- Raio incidente paralelo ao eixo: atravessa a lente e passa pelo foco imagem.
- Raio partindo do foco objeto: atravessa a lente e sai paralelo ao eixo da lente.
- Raio apontando ou partindo do centro da lente: atravessa sem desvio.

Veja o traçado dos raios notáveis para uma lente biconvexa:
:::{figure} ./figures/refracaonotaveisbiconvexa.png
---
width: 600px
name: refracaonotaveisbiconvexa
---
:::
e bicôncava:
:::{figure} ./figures/refracaonotaveisbiconcava.png
---
width: 500px
name: refracaonotaveisbiconcava
---
:::
Observe a posição invertida do foco imagem e do foco objeto, quando comparamos a lente biconvexa com a bicôncava.

#### Magnificação lateral
Tomando por base a [](refracaonotaveisbiconvexa), temos que $y/s = \tan \theta = -y'/s'$, pois $y'<0$ (imagem invertida). Portanto:
\begin{equation}
\frac{y'}{y}\;=\;-\frac{-s'}{s}\;.
\end{equation}
A mesma relação é obtida diretamente também pela [](refracaonotaveisbiconcava), onde, no caso, $y'>0$ e $s'<0$ (imagem do mesmo lado que a luz incidente).


#### Exercício: lente biconvexa

Um objeto de 1,2 cm é colocado a 4,0 cm de uma lente biconvexa com distância focal de 12 cm. Localize a imagem graficamente e usando as equações. Determine se a imagem é real ou virtual e encontre a sua altura. Desenhe um olho na figura indicando seu local e orientação para ver a imagem.
:::{figure} ./figures/figexerciciolentebiconvexa.png
---
width: 700px
name: figexerciciolentebiconvexa
---
:::

#### Exercício com duas lentes: situação 1

Uma segunda lente com distância focal de 6,0 cm é colocada 12 cm à direita da lente do exercício anterior. A figura a seguir mostra o caminho dos raios notáveis. Calcule os valores das posições relevantes mostradas no eixo das lentes.
:::{figure} ./figures/lentesexercicioduaslentes.png
---
width: 700px
name: lentesexercicioduaslentes
---
:::

#### Exercício com duas lentes: situação 2    

Duas lentes com distância focal de 10 cm estão a uma distância de 15 cm. Encontre a localização da imagem final para um objeto que está a 15 cm de uma das lentes e a 30 cm da outra lente. Calcule os valores das posições relevantes.
:::{figure} ./figures/lentesexercicioduaslentesB.png
---
width: 700px
name: lentesexercicioduaslentesB
---
:::

#### Composição de lentes

Quando duas lentes de distância focal $f_1$ e $f_2$ são colocadas juntas (desprezando-se a distância entre as lentes), a distância focal efetiva $f_{eq}$ é dada pela relação:
\begin{equation}\label{eq:equacaocomposicaolentes}
\frac{1}{f_{eq}} = \frac{1}{f_1} + \frac{1}{f_2}\;.
\end{equation}
Portanto, o poder de convergência das lentes se somam. 

Para demonstrar a relação acima, aplicamos a [equação das lentes](eq:eqlentefoco) duas vezes e usamos que a distância imagem (negativa) da primeira lente é a distância objeto da segunda lente. Teremos:
\begin{equation}
\frac{1}{f_{1}} = \frac{1}{s_1} + \frac{1}{s_1'}\;
\end{equation}
e
\begin{equation}
\frac{1}{f_{2}} = \frac{1}{-s_1'} + \frac{1}{s_2'}\;.
\end{equation}
Adicionando, membro a membro, as duas equações, obtemos a equação [](eq:equacaocomposicaolentes).


## Noções sobre instrumentos ópticos

### O olho humano e a lupa  

O olho humano contém estruturas imersas em um fluido transparente com índice de refração próximo ao da água. Existem duas lentes: uma fixa, a **córnea**, formada de material duro e transparente; e outra flexível, o **cristalino**, que pode ter sua distância focal ajustada pelo músculo ciliar. A **íris** é um diafragma, isto é, uma estrutura que controla a entrada de luz. A abertura da íris é a **pupila**, que se contrai ou dilata conforme a necessidade de iluminição.

:::{figure} ./figures/olhopartes.png
---
width: 300px
name: olhopartes
---
:::

Em um olho normal, a luz incidente é focalizada em um ponto $P'$ da retina (fundo do olho). Na retina estão as células sensíveis à luz (cones e bastonetes) que transmitem sinais ao nervo óptico, conectado ao cérebro, onde o sinal é processado. Para uma pessoa míope, a luz é focalizada em um ponto à frente da retina. O olho converge os raios mais do que deveria. Assim, raios paralelos (visão de objetos distantes) não são focalizados corretamente. Uma lente divergente corrige o defeito, como mostrado na figura abaixo:
:::{figure} ./figures/olhomiopia.png
---
width: 300px
name: olhomiopia
---
Na **miopia**, a luz incidente  é focalizada em um ponto à frente retina. O problema pode ser corrigido com uma lente divergente.
:::
:::{figure} ./figures/olhohipermetropia.png
---
width: 300px
name: olhohipermetropia
---
Na **hipermetropia**, a luz incidente  é focalizada em um ponto atrás retina. Nesse caso, deve ser usada uma lente convergente.
:::
Um outro defeito geométrico da visão é o **astigmatismo**. Neste caso, a córnea adquire uma forma não esférica, com uma curvatura horizontal e outra vertical. Assim, a distância imagem para raios horizontais é diferente da distância imagem para raios verticais. O defeito pode ser corrigido pelo uso de lentes de formato cilíndrico, em vez de esférico. 
:::{figure} ./figures/olhoastigmatismo.png
---
width: 500px
name: olhoastigmatismo
---
Nesta ilustração do astigmatismo, os raios emitidos por uma fonte pontual emitidos em um plano vertical (raios em vermelho) convergem para um ponto mais à frente que os raios que chegam no plano horizontal. 
:::
Quando o olho focaliza luz distante, o músculo ciliar está completamente relaxado e o sistema de lentes do olho tem sua máxima distância focal (cerca de 2,5 cm, que é a distância da córnea normal até a retina). Quando o objeto é trazido para perto do olho, a convergência da luz na retina depende de um maior poder de convergência (dioptria). Isso é obtido pela ação do músculo ciliar, que aumenta a curvatura do cristalino (redução do raio de curvatura e, portanto, da distância focal). Esse processo é denominado **acomodação**. Se o objeto está muito próximo ao olho, pode não ser possível focalizá-lo. O ponto mais próximo do olho para o qual o olho consegue focalizar a imagem na retina é denominado **ponto próximo**. Para uma criança, a distância do ponto próximo é cerca de 10 cm. Aos 60 anos, essa distância pode ser 200 cm. O valor de referência considerado para o olho humano é 25 cm. O problema do olho cansado (**presbiopia**) é a dificuldade da musculatura em realizar a acomodação do olho para objetos próximos. Não é um problema geométrico. Sua correção é feita por uma lente multifocal, isto é, uma lente com uma curvatura para perto e outra para longe.

É interessante ver a consequência da presbiopia para o olho míope. Como o olho míope tem um excesso de convergência, a acomodação é mais simples e o ponto próximo fica mais perto do olho do que para uma pessoa normal da mesma idade. Então, um adulto míope costuma ter uma visão melhor para perto do que adultos sem miopia. 

Em princípio, a presbiopia pode ser confundidade com a hipermetropia, pois ambos os efeitos causam dificuldade em enxergar objetos próximos. A pessoa com hipermetropia precisa forçar muito para ler de perto. A pessoa com presbiopia perde essa capacidade de acomodação, mesmo com esforço. 
 
#### Tamanho aparente e lentes de aumento

O tamanho aparente de um objeto é determinado pelo tamanho da imagem formada na retina. Quando visto de perto, um objeto produz uma imagem maior na retina, como sugere a figura abaixo:
:::{figure} ./figures/olhotamanhoaparente.png
---
width: 500px
name: olhotamanhoaparente
---
Na figura (b), o ângulo visual $\phi_2$ e a correspondente imagem (tamanho $y_2'$) são maiores que na situação (a) pelo fato de o objeto estar mais próximo.
:::
O tamanho da imagem é proporcional ao ângulo subtendido pelo objeto no olho. Pela figura, temos (para pequenos ângulos):
\begin{equation}
\phi =  \frac{y'}{2,5\,cm}\;\;\;\hbox{e}\;\;\;\theta= \frac{y}{s}.
\end{equation}
O tamanho da imagem na retina é proporcional ao tamanho do objeto e inversamente proporcional à distância do objeto ao olho. Como o ponto próximo é o mais próximo que o olho consegue focalizar na retina, é nele que se consegue o máximo tamanho aparente. Se $d_p$ é a distância do ponto próximo e $y$ é o tamanho do objeto, o ângulo subtendido correspondente é:
\begin{equation}\label{olhoeqpontoproximo}
\theta_{p}\;=\;\frac{y}{d_p}\,.
\end{equation}


#### Exemplo: grau para vista cansada
O ponto próximo de um olho de uma pessoa está a 75 cm da retina. Com a lente do óculos, essa distância cai para o valor de referência,25 cm. Despreze a distância entre a lente e o olho. (a) Qual é a dioptria da lente? (b) Qual é o aumento lateral da lente? 
:::{figure} ./figures/olhoexemplooculos.png
---
width: 500px
name: olhoexemplooculos
---
:::
O fato de a lente trazer o ponto próximo do olho de $75$ cm de distância para $25$ cm de distância significa que uma imagem virtual é formada a $75$ cm da lente se o objeto é colocado a $25$ cm da lente (os raios que entram no olho parecem divergir de um ponto a $75$ cm). Usando a equação [](eq:eqlentefoco) para a lente, obtemos:
\begin{equation}
\frac{1}{f} = \frac{1}{0,25} + \frac{1}{-0,75}\,,
\end{equation}
de modo que a diopria é 1/f = 2,7D. O aumento lateral é $y'/y=-s'/s=0,75/0,25 =3$. 

Uma pessoa com ponto próximo a $75$ cm tem presbiopia. Para ler um livro, ela tem que afastá-lo a 75 cm, o que faz com que a imagem formada na retina seja muito pequena. A lente produz uma imagem também a 75 cm do olho, porém, 3 vezes maior. 

Perceba que o objeto foi colocado antes da distância focal da lente (ponto $F'$ na imagem). Se o objeto fosse colocado no ponto focal da lente, os raios emergiriam dela paralelos e o olho poderia ficar completamente relaxado, pois nessa situação, raios incidentes paralelos são projetados na retina, sem necessidade de acomodação. A desvantagem é que, estando o objeto mais distante da lente, o ângulo subtendido pelo objeto na lente seria menor e, consequentemente, o tamanho aparente da imagem no olho seria menor. 

Objetos como as lupas funcionam assim: o objeto é colocado no plano focal da lente. 
:::{figure} ./figures/lupafocoolho.png
---
width: 500px
name: lupafocoolho
---
:::
Nessa situação o ângulo subtendido pela lente é dado pelo quociente:
\begin{equation}
\theta_{lupa}\;=\;\frac{y}{f}\,.
\end{equation}
Se a distância focal da lente for menor que a distância do ponto próximo da pessoa, $\theta_{lupa} > \theta_p$ (ângulo subtendido no olho pelo objeto, dado pela equação [](olhoeqpontoproximo)). Como o tamanho aparente da imagem é proporcional ao ângulo subtendido, a lente irá aumentar o tamanho aparente do objeto, mesmo com o olho relaxado. Comparando com o ângulo máximo a olho nu (com o objeto localizado no ponto próximo), obtemos que a magnificação proporcionada pela lupa é:
\begin{equation}\label{olhoaumentolupa}
M = \frac{\theta_{lupa}}{\theta_p} = \frac{d_p}{f}\;.
\end{equation}
Aproximando o objeto da lente um pouco mais, ainda será possível formar a imagem, com o auxílio do olho, e a imagem seria ainda maior. 

Pela equação [](olhoaumentolupa), quanto menor a distância focal, maior o aumento. Valores pequenos de $f$ correspondem a lentes com raios pequenos, que geram grandes aberrações esféricas. As aberrações limitam o aumento máximo das lupas para menos de 10 vezes. Lupas comerciais, tipicamente, têm aumento cerca de 3 vezes.

#### Exercício: magnificação da lupa

Uma pessoa com distância do ponto próximo igual a 25 cm usa uma lupa de $20\,D$. Qual é a magnificação obtida?

### O microscópio simples

O microscópio simples consegue aumentos maiores que as lupas por utilizar uma montagem diferente.
:::{figure} ./figures/lentesmicroscopiosimples.png
---
width: 500px
name: lentesmicroscopiosimples
---
:::
 O objeto é colocado um pouco além do foco de uma lente (a **objetiva**) com pequena distância focal. Estando além do foco, a imagem será real e invertida. Estando próximo ao foco, a magnificação da imagem será grande. Podemos entender tudo isso manipulando a equação [](eq:eqlentefoco):
\begin{equation}
\frac{1}{s'} = \frac{1}{f_{ob}}-\frac{1}{s} = \frac{s-f_{ob}}{s\,f_{ob}}.
\end{equation}
Se $s-f_{ob}>0$ e pequeno, $s/s'$ será positivo (imagem real) e grande.

Como $s$ e $s'$ têm papeis simétricos na equação da lente, teremos também:
\begin{equation}
\frac{1}{s} = \frac{1}{f_{ob}}-\frac{1}{s'} = \frac{s'-f_{ob}}{s'\,f_{ob}}.
\end{equation}
A imagem será formada à direita do foco imagem. Vamos denotar a diferença $s'-f_{ob}$ por $L$ (veja na figura).
Em termos de $L$ podemos reescrever a equação anterior como:
\begin{equation}
\frac{s'}{s} = \frac{L}{f_{ob}}.
\end{equation}
A magnificação da objetiva será, portanto, $M_{ob} = -L/f_{ob}$.

Posiciona-se uma segunda lente, a ocular, de forma que a imagem da objetiva caia no plano focal da ocular. A ocular funciona como uma lupa, aumentando o ângulo subtendido no olho pela imagem real produzida pela objetiva. A magnificação da ocular será dada por $M_{oc}=d_{p}/f_{oc}$, sendo $d_p$ a distância do ponto próximo do observador. A magnificação final será o produto da magnificação de cada lente:
\begin{equation}
M= M_{ob}\,M_{oc} =  -\frac{L\,d_p}{f_{ob}\,f_{oc}}.
\end{equation}

#### Exercício: aumento do microscópio

Um microscópio tem uma objetiva com distância focal de 1,2 cm e uma ocular com distância focal de 2,0 cm. As lentes são separadas pela distância de 20,0 cm. (a) Encontre o aumento do microscópio para uma pessoa com distância do ponto próximo igual a 25 cm. (b) Onde o objeto deveria ser colocado se a iamgem final é para ser vista no infinito?

### O telescópio refrator

O telescópio refrator também é formado por uma objetiva e uma ocular. 
:::{figure} ./figures/lentestelescopio.png
---
width: 600px
name: lentestelescopio
---
:::
Porém, diferentemente do microscópio, no telescópio o objeto está muito distante. A luz chega paralelamente e é formada uma pequena imagem do objeto no plano focal da objetiva. A função da objetiva, neste caso, não é ampliar a imagem, mas formar uma imagem que está próxima o suficiente para ser ampliada pela ocular. Mais uma vez, a imagem da objetiva deve se formar no plano focal da ocular.

O ângulo $\theta_0$ é dado pela razão diâmetro/distância do astro. Para a Lua, $\theta_0 \approx 0,5^\circ$. Pela montagem, vemos que $\theta_0 = -y'/f_{ob}$. Da figura, vemos também que $\theta_{oc} = y'/f_{oc}$. A magnificação do telescópio é, portanto:
\begin{equation}
M= \frac{\theta_{oc}}{\theta_{ob}} = -\frac{f_{ob}}{f_{oc}}.
\end{equation}

#### Exercício: aumento do telescópio

O maior telescópio refrator do mundo está no Yerkes Observatory da Universidade de Chicago. A objetiva do telescópio tem uma distância focal de 19,5 m. A distância focal da ocular é 10,0 cm. Qual é o aumento do telescópio? 

O telescópio mencionado no exercício tem um diâmetro de 1,02 m. Quanto maior a objetiva, maior a quantidade de luz captada e, portanto, mais brilhante será a imagem. 

### Lista de exercícios

1) Um telescópio refletor usa um espelho côncavo que tem raio igual a 8,0 m. Encontre a localização e o diâmetro da imagem da Lua formada pelo espelho. A Lua tem diâmetro de $3,5\times 10^6$ m e está a $3,8\times 10^8$ m da Terra.

2) Uma imagem virtual pode ser fotografada? Se sim, dê um exemplo. Se não, explique o porquê.

3) Indique se é verdadeiro ou falso:

    (a) A imagem virtual de uma imagem formada por um espelho côncavo é sempre menor.

    (b) Um espelho côncavo sempre forma uma imagem real.

    (c) Um espelho convexo nunca forma uma imagem real.

    (d) Um espelho côncavo nunca forma uma imagem real maior do que o objeto.

4) Indique se é verdadeiro ou falso:

    (a) Uma imagem virtual não pode ser projetada em uma tela.
    
    (b) Uma distância imagem negativa implica que a imagem é virtual.   
    
    (c) Todos os raios paralelos ao eixo de um espelho esférico são refletidos para um mesmo ponto.
    
    (d) Uma lente divergente não pode formar uma imagtem real de um objeto.
    
    (e) A distância imagem para uma lente convergente é sempre positiva.

5) A imagem de uma fonte pontual colocada no ponto $P$ na frente de um espelho plano é vista por um observador, como mostra a figura. 
:::{figure} ./figures/exercicioolhoespelho.png
---
width: 200px
name: exercícioolhoespelho
---
:::
- (a) Desenhe dois raios a partir do objeto que reflitam e cheguem ao observador. 
    
- (b) Mantendo a posição do espelho e da fonte mostrada na figura, indique a região espacial em que o observador consegue ver a imagem do objeto através do espelho.

6) Quando dois espelhos planos estão paralelos, um de frente para o outro (como em uma barbearia) múltiplas imagens se formam porque cada imagem em um espelho funciona como fonte (objeto) para o outro espelho. Se a separação entre os espelhos é de 3 m e um objeto está posicionado a 1 m do espelho A (e, portanto, a 2 m do espeho B), encontre a distância das primeiras 4 imagens formadas no espelho A. Explique por que motivo as imagens vão ficando menos intensas.

7) No que consiste a aproximação paraxial?


