
# Interferência e Difração

Quando duas ou mais fontes de luz estão presentes, a onda resultante envolverá a superposição de todas as ondas. Matematicamente, isso corresponde à soma algébrica das funções de onda, uma para cada fonte. Utilizaremos as palavras "superposição", "soma" e "interferência" para indicar essa situação.

Em princípio, as funções de onda que serão consideradas corresponderão a ondas com periodicidade espacial e temporal. Serão ondas harmônicas, planas ou esféricas, com certo comprimento de onda e frequência. Em cada ponto do espaço, as funções de onda oscilarão como um seno ou cosseno, admitindo valores positivos ou negativos. Assim, a soma de várias funções de onda podem levar ao reforço ou ao cancelamento da oscilação local. Teremos, portanto, situações em que a interferência de duas fontes de luz levam à ausência de luz em certos pontos do espaço, ou mesmo em toda uma região.

As múltiplas fontes que serão consideradas podem corresponder, de fato, a diferentes fontes de ondas eletromagnéticas, ou podem ser as inúmeras frentes de ondas esféricas utilizadas no Princípio de Huygens para compreender a evolução temporal (propgação) de uma onda. A figura abaixo ilustra o Princípio de Huygens:
:::{figure} ./figures/interferenciaHuygens.png
---
width: 300px
name: interferenciaHuygens
---
Foto do comportamento de uma onda plana na água quando atinge um anteparo com uma pequena fenda.
:::

Neste contexto, o estudo da interferência abrange uma grande gama de fenômenos, incluindo os efeitos conhecidos como difração. Além disso, sua aplicação não está restrita às ondas eletromagnéticas, aplicando-se, por exemplo, para o som. As particularidades da natureza ondulatória serão relevantes quando os comportamentos dependerem da frequência, seja pela geometria do problema, seja pela dependência da velocidade de propagação na frequência (dispersão).

Os assuntos aqui tratados não podem ser abordados pela óptica geométrica. Isso ocorre porque a óptica geométrica se ocupa apenas da direção de propagação de raios. Efeitos que envolvem a fase da onda, bem como os desvios da propagação retilínea, precisam de outra abordagem.


## Interferência e diferença de fase

Considere duas ondas que se propagam em uma direção $x$. Vamos analisar como muda a interferência das duas ondas ao longo do eixo $x$. Para simplificar, vamos considerar duas ondas harmônicas de mesma amplitude, frequência $(\omega)$ e comprimento de onda
$\lambda = 2\pi/k$. O que distingue as ondas? Será apenas a constante de fase. Em termos de funções de onda, temos:
\begin{equation}
y_1(x,t) = A \,\sin(kx -\omega t)
\end{equation}
e
\begin{equation}
y_2(x,t) = A \,\sin (kx -\omega t + \delta)
\end{equation}

O que distingue $y_1$ de $y_2$ é apenas a constante de fase $\delta$. Que fenômenos essa situação modela? Modela a interferência de ondas provenientes de fontes idênticas, mas que acumularam uma defasagem. Essa defasagem pode ter várias origens, dentre elas:

1) **As fontes são idênticas, mas têm defasagem na geração**. 

Considere as duas fontes da figura abaixo. Enquanto a onda da fonte 1 está numa crista, a da fonte 2 está quase em um vale. Consequentemente, um ponto no meio do caminho irá observar uma defasagem entre as ondas, correspondendo a uma interferência parcialmente destrutiva.

:::{figure} ./figures/interferenciadiferencafase.png
---
width: 700px
name: interferenciadiferencafase
---
Duas fontes são emitidas fora de fase. Um observador no meio do caminho entre as fontes irá observar a diferença de fase.
:::

2) **A defasagem surgiu por que os percursos das ondas tiveram tamanhos distintos**.

Perceba que, agora, as duas fontes estão em fase: no mesmo instante, a onda da fonte 1 está numa crista e da fonte 2, também. Porém, pela diferença de caminho percorrido, as ondas chegarão ao observador com fases distintas, em geral. 

:::{figure} ./figures/interferenciadiferencafase2.png
---
width: 700px
name: interferenciadiferencafase2
---
Duas fontes emitem em fase. Porém pela diferença de caminho, as ondas chegam defasadas em um observador.
:::
Pode acontecer de as ondas chegarem em fase. Isso acontece, por exemplo, se a diferença de caminho é igual a exatamente 1 comprimento de onda: uma onda estará $2\pi$ à frente da outra; mas, pela periodicidade da função seno, as ondas estarão em fase. Em geral, se a diferença de caminho é $\Delta r$, a diferença de fase correspondente é
\begin{equation}\label{eq:deltaigualkdeltar}
\delta \;=\;2\pi\,\frac{\Delta r}{\lambda}\, = k\,\Delta r,
\end{equation}
sendo $k$ o módulo do vetor de onda. Como a fase de uma onda harmônica é o argumento do seno, ou seja, é: 
\begin{equation}
\hbox{fase } = kx -\omega t + \delta_0\,,
\end{equation}
é esperado que a defasagem entre duas ondas idênticas envolva o produto de $k$ pela diferença de caminho.

3) **A defasagem surgiu devido à mudança de velocidade da onda**.

Neste caso, as duas fontes estão em fase e os caminhos até o observador têm o mesmo tamanho. Porém, uma das ondas viajou uma parte do caminho em um meio mais refringente, onde se propagou com velocidade diferente, gerando uma defasagem. Note que na mudança de meio, a frequência se mantém e o comprimento de onda muda. 
:::{figure} ./figures/interferenciadiferencafase3.png
---
width: 700px
name: interferenciadiferencafase3
---
Duas fontes emitem em fase. Porém pela diferença de caminho, as ondas chegam defasadas em um observador.
:::

Este caso e o caso anterior são agrupados com o conceito de **caminho óptico**, que leva em conta o produto do deslocamento $\delta r$ e o índice de refração. O caminho óptico acumulado é, em geral, uma integral ao longo da direção de propagação:
\begin{equation}
\hbox{diferença de caminho óptico }\;=\;\;\;\int n(r)dr\;.
\end{equation}

\begin{equation}
\delta \;=\;2\pi\,\frac{(\hbox{diferença de caminho óptico })}{\lambda_0}\;,
\end{equation}
onde $\lambda_0$ é o comprimento de onda da luz no vácuo.


4) **A defasagem foi gerada pela reflexão da onda**.

Quando a onda passa de um meio em que a velocidade é maior (menos refringente) para um meio em que a velocidade é menor (mais refringente), a onda é refletida de forma invertida. Vimos isso para a corda com extremidade fixa e é um comportamento comum. Inverter a função seno é o mesmo que deslocar seu argumento (fase) por $\pi$, pois $\sin(\theta + \pi) = -\sin(\theta)$. 
:::{figure} ./figures/interferenciaaragua180.png
---
width: 400px
name: interferenciaaragua180
---
O desenho não mostra, mas quando uma onda passa de um meio menos refringente para um meio menos refringente, a onda refletida volta invertida em relação à onda incidente. 
:::
Nas aplicações, uma fase de $\pi$ pode ser considerada uma diferença de caminho óptico de meio comprimento de onda, pois, pela equação [](eq:deltaigualkdeltar), $\pi = 2\pi\,\Delta r/\lambda$ para $\Delta r = \lambda/2$.

Vamos retornar agora à análise da interferência de duas ondas harmônicas defasadas. Algebricamente, temos que a superposição de $y_1$ com $y_2$ é a onda
\begin{equation}
y(x,t) = y_1(x,t) + y_2(x,t) =  A \,\sin (kx -\omega t) +  A \,\sin (kx -\omega t + \delta)\;.
\end{equation}
Mostraremos agora que $y(x,t)$ é também uma onda harmônica de mesmo comprimento de onda e frequência
que as ondas originais, mas com amplitude e constante de fase diferentes daquelas das ondas originais. Para isso, vamos usar a identidade trigonométrica:
\begin{equation}\label{idtrigonometrica1}
sin \alpha + \sin \beta = 2 \cos\frac{1}{2}(\alpha-\beta)\,\sin\frac{1}{2}(\alpha + \beta)\;.
\end{equation} 
Obtemos:
\begin{equation}\label{auxsomaseno3}
y(x,t) = 2A \,\cos (\delta/2)\,\sin (kx -\omega t + \delta/2)\;,
\end{equation} 
A equação [](auxsomaseno3) está indicando que $y(x,t)$ é uma onda harmônica com amplitude $2A\,\cos(\delta/2)$ e constante de fase $\delta/2$. 

Uma quantidede importante nas medidas de fenômenos ondulatórios é a **intensidade**. Ela corresponde à energia média por unidade de área. Vamos relacionar a intensidade da onda resultante ($I$) com a intensidade das ondas individuais ($I_0$). Como a intensidade é proporcional ao quadrado da amplitude, teremos o seguinte resultado:
\begin{equation}\label{auxsomaseno3}
\frac{I}{I_0} = 4\,\cos^2 (\delta/2);.
\end{equation} 

A intensidade da superposição depende da defasagem $\delta$ entre as ondas originais. Se $\delta$ é igual a $\pi$, teremos
$2A\,\cos(\delta/2) = 0$, pois $\cos (\pi/2) = 0$. Neste caso, teremos:
\begin{equation}\label{auxsomaseno3}
y(x,t) = y_1(x,t) + y_2(x,t) \;=\;0\;,\;\;\; \forall x,t.
\end{equation} 
Essa é uma característica marcante dos fenômenos ondulatórios: a superposição
de duas ondas pode resultar na ausência de ondas! Assim, a superposição de dois sons pode resultar em silêncio e a superposição de
duas luzes pode resultar em escuridão! Esse fenômeno é denominado **interferência destrutiva** e dizemos que as ondas estão em **oposição de fase**.

O caso em que $\delta = \pi$ dá origem a uma interferência destrutiva total. O mesmo se dá quando $\delta = -\pi, \pm 3\pi, \pm 5\pi$, etc, pois em todos esses casos $\cos(\delta/2)$ se anula. 
:::{note}
Defasagem: $\delta = (2 n+1)\pi\;,\; n=0,\pm 1, \pm 2, \ldots\;\;\;\;$ (interferência destrutiva)\
Intensidade = 0.
:::

Quando $\delta$ é diferente desses valores, mas ainda é próximo a um deles, temos que $\cos (\delta/2)$ não será zero, mas um número bem menor que 1. Por exemplo, para $\delta = 0,9\pi$, temos que $\cos (\delta/2) \approx 0,16$. Nesse caso, dizemos que ainda há interferência destrutiva, embora as ondas não se aniquilem totalmente.

Por outro lado, quando a constante de fase é igual a $0$ (ou $\pm 2\pi, \pm 4\pi,\pm 6\pi$, etc), temos que $\cos(\delta/2)$ vale 1 ou -1 e a amplitude da onda resultante fica o dobro da amplitude das ondas originais. Nesse caso, dizemos que há **interferência totalmentne construtiva**. Perceba que a intensidade é 4 vezes a intensidade original de cada onda. 
:::{note}
Defasagem: $\delta = 2 n\pi\;,\; n=0,\pm 1, \pm 2, \ldots\;\;\;\;$ (interferência construtiva)\
Intensidade = 4$I_0$.
:::

Quando $\cos(\delta/2)$ for diferente de 1 ou -1, mas ainda próximo a esses valores, haverá uma intensificação parcial da onda resultante. Embora sua amplitude não chegue a dobrar, ela certamente irá aumentar e diremos que há interferência construtiva.

Na sequência, vamos explorar situações físicas importantes com diferentes origens para a diferença de fase e, portanto, diferentes padrões de interferência.

### Experimento da dupla fenda (Young)

Neste experimento, luz de uma fonte distante atinge um anteparo em que foram feitas duas fendas idênticas separadas pela distância $d$. As fendas devem ser estreitas e longas, isto é, a espessura das fendas deve ser menor que o comprimento de onda da luz incidente. Já a largura da fenda, deve ser maior. A luz que atravessa as fendas gera um padrão de interferência em uma tela colocada à distância $L$ das fendas, como indica a figura.

:::{figure} ./figures/interferenciaduplafendayoung.png
---
width: 350px
name: interferenciaduplafendayoung
---
Perceba as ondas planas chegando e as ondas esféricas interferindo, gerando um padrão de interferência com franjas na tela.
:::

Pela distância da fonte, a onda atige o anteparo com frentes de onda praticamente planas. Pelo Princípio de Huygens, cada fenda fará com que o comportamento da onda seja equivalente à sobreposição (interferência) de muitas fontes pontuais diminutas, distribuidas ao longo da fenda. Como a frente de onda que atinge as fendas é tipo onda plana, todas as fontes diminutas nas duas fendas estarão em fase. A diferença de fase que se observará na sequência será devida à diferença de caminho.

Vamos considerar o efeito da interferência de duas fontes diminutas localizadas em um mesmo plano perpendicular às fendas. Qual será a fase da onda em um ponto de altura $y$ (em relação à altura do ponto médio entre as fendas)? Pela figura, vemos que a diferença de caminho é $d\sin\theta$, com $\tan \theta = y/L$. 
:::{figure} ./figures/interferenciaduplafendayoung2.png
---
width: 600px
name: interferenciaduplafendayoung2
---
Detalhe da diferença de caminho entre as ondas provenientes das duas fendas.
:::

Se a diferença de caminho for igual a um número inteiro de comprimentos de onda, a interferência será construtiva:
\begin{equation}
d\,\sin\theta = m\lambda,\;\;\;m=0,1,2,\ldots \;\;\;\;\text{(máximo de intensidade)}
\end{equation}
O caso $m=0$ corresponde a pontos equidistantes das fendas.  

Por outro lado, a intensidade será mínima (zero) quando 
\begin{equation}
d\,\sin\theta = \bigg(m-\frac{1}{2}\bigg)\lambda,\;\;\;m=1,2,\ldots \;\;\;\;\text{(mínimos de intensidade)}
\end{equation}
Vamos denotar por $y_m$ e $\theta_m$ a coordenada e o correspondente ângulo da $m$-ésima raia de intensidade máxima. Considerando pontos próximos à região central, podemos usar a aproximação em que $\tan\theta_m = \sin\theta_m$. Neste caso, podemos escrever a condição de máxima intensidade em termos da coordenada $y_m$:
\begin{equation}
y_m = m\frac{\lambda L}{d},\;\;\;m=0,1,2,\ldots \;\;\;\;\text{(máximos de intensidade),}
\end{equation}
e a quantidade $\lambda L/d$ é a distância entre duas franjas consecutivas.

:::{figure} ./figures/interferenciaduplafendayoung3.png
---
width: 400px
name: interferenciaduplafendayoung3
---
Foto das franjas de interferência de um experimento de Young. Abaixo, o gráfico correspondente da intensidade em função da coordenada local.
:::
#### Exercício: dupla fenda

Um anteparo tem duas fendas estreitas separadas por 1,5 mm. Luz amareala de uma lâmpada de sódio (comprimento de onda de 589 nm) ilumina o anteparo. Encontre o espaçamento das franjas de interferência que se formam em uma tela à distância de 3 m do anteparo. Resposta: 1,8 mm.

Quando se faz o experimento de Young com luz branca, observa-se a franja central branca, mas as demais franjas variam em posição e largura a depender da cor. Portanto, observam-se franjas coloridas.
:::{figure} ./figures/interferenciaduplafendayoung4.jpg
---
width: 400px
name: interferenciaduplafendayoung4
---
Acima, o resultado do experimento da dupla fenda para a luz branca. Observam-se os efeitos da dispersão da luz. Abaixo, as franjas obtidas com três frequências fixas.
:::

### Interferência em lâminas delgadas 



:::{figure} ./figures/interferencialaminadelgada.png
---
width: 500px
name: interferencialaminadelgada
---
Análise de múltiplas reflexões e transmissões em uma lâmina fina. 
:::
Na figura, a diferença de caminho óptico entre o raio refletido 2 e o raio refletido 1 é dada por:
\begin{equation}
[2]-[1] = n\,\overline{AB} + n\,\overline{BA'} + n\,\overline{A'C} -\left(n_0\overline{AC'}+\frac{\lambda_0}{2}\right)\;. 
\end{equation}
O termo $\lambda_0/2$ corresponde à fase de $\pi$ adquirida pelo raio 1 ao passar do meio menos refringente (ar) para o meio mais refringente (material da lâmina). O raio 2 não sofre esse tipo de reflexão.
 
Agora, observe que $n_0\overline{AC'} = n_0\,L\sin \theta_1$ e $n\overline{A'C} = n\,L\,\sin\theta_2$. Pela Lei de Snell, eles são iguais. Agora, note que $\overline{AB} + \overline{BA'} = \overline{A\overline{A}}\,\cos\theta_2=2d\cos\theta_2$. Portanto, a diferença de caminho óptico dos raios refletidos é
\begin{equation}
([2]-[1])_{reflexão}\;=\;2 n d \cos\theta_2 \;-\;\frac{\lambda_0}{2}. 
\end{equation}

Por simetria, podemos escrever diretamente a diferença de caminho entre os raios transmitidos $2'$ e $1'$:
\begin{equation}
([2']-[1'])_{transmissão}\;=\;2 n d \cos\theta_2\,. 
\end{equation}
Como não reflexão do ar para o meio mais refringente, não tem a diferença de fase adicional de meio comprimento de onda.

Observe que os raios refletidos $3,4,\ldots$ têm o mesmo caminho óptico do raio $2$. A inteferência construtiva de $2,3,4,\ldots$ interfere com o raio $1$, que tem mais intensidade. Argumentos análogos valem para a análise dos raios transmitidos. O cálculo completo, que leva em conta a refletividade e a transmissividade pode ser feito.

Finalmente, observam-se as seguintes condições:
\begin{equation*}
2 n d \cos\theta_2 = m\,\lambda_0\;\;\;\;(m=0, 1, 2, \ldots)\;\;\Rightarrow \begin{cases}\hbox{Mínimo de reflexão}\\\hbox{Máximo de transmissão}\end{cases} 
\end{equation*}
\begin{equation*}
2 n d \cos\theta_2 = \left(m+\frac{1}{2}\right)\,\lambda_0\;\;\;\;(m=0, 1, 2, \ldots)\;\;\Rightarrow \begin{cases}\hbox{Máximo de reflexão}\\\hbox{Mínimo de transmissão}\end{cases} 
\end{equation*}
Em particular, no limite $d\rightarrow 0$, teremos interferência destrutiva.

Para observação próxima à normal ($\theta_1=\theta_2 =0$), ao irmos aumentando a espessura da lâmina a partir do zero, o primeiro máximo de reflexão acontece para
\begin{equation}
d = \frac{1}{4}\frac{\lambda_0}{n} = \frac{\lambda}{n}, 
\end{equation}
onde $\lambda$ é o comprimento de onda da luz no meio com índice de refração $n$.

Se tivermos um meio de espessura variável no ar, as condições de interferência construtiva e destrutiva para luz monocromática (uma só frequência) se darão para várias espessuras. É isso que acontece, por exemplo, com bolhas de sabão. Por gravidade, o líquido tem espessura variável, sendo maior embaixo. Na parte de cima, a espessura pode ser tão pequena (menor que $\lambda/4$) que não há luz refletida. Como a formação das faixas de máximos e mínimos de reflexão dependem do comprimento de onda, se a luz incidente envolve várias frequência, vemos bonitos efeitos coloridos. típicos das bolhas de sabão.
:::{figure} ./figures/interferencialaminasdelgadasfoto.jpg
---
width: 400px
name: interferencialaminasdelgadasfoto
---
Interferência em lâmina de sabão.  
:::
É esse efeito que explica também os chamados **anéis de Newton**, mostrados na figura abaixo:
:::{figure} ./figures/interferencialaminasdelgadasaneisnewton.png
---
width: 700px
name: interferencialaminasdelgadasaneisnewton
---
Nos anéis de Newton, as regiões de igual espessura são anéis.
:::
Outros exemplos de interferência de lâminas delgadas são as manchas de óleo sobre o asfalto molhado, a plumagem das asas de beija-flores e das asas das borboletas. As asas desses animais têm 
:::{figure} ./figures/interferencialaminasdelgadasborboleta.png
---
width: 700px
name: interferencialaminasdelgadasborboleta
---
As asas de algumas borboletas têm várias camadas de lâminas que dão a coloração das asas.
:::

### O princípio dos interferômetros

Na seção anterior, para um dado comprimento de onda, estudamos as espessuras de lâminas que correspondiam a interferência construtiva ou destrutiva. Podemos usar as relações obtidas para, a partir de uma lâmina com espessura $d$ conhecida, medir comprimentos de onda ou diferenças de caminho óptico.

A capacidade de um interferômetro em diferenciar dois comprimentos de onda próximos depende da nítida separação entre duas franjas de interferência consecutivas. Usando interferômetros foi possível caracterizar a estrutura fina e hiperfina do espectro dos elementos químicos.  

### Coerência da radiação

## Padrão de difração por uma fenda
