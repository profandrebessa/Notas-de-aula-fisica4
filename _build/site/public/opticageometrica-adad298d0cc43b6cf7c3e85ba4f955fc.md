
# Óptica geométrica

## Espelhos planos

- Imagem sempre virtual: os raios de luz não chegam atrás do espelho.

:::{figure} ./figures/espelhoplano1.png
---
width: 300px
name: fig_espelhoplano1
---
:::


- Orientação invertida

:::{figure} ./figures/espelhoplano2.png
---
width: 300px
name: fig_espelhoplano2
---
:::

- Múltiplos espelhos. 

:::{figure} ./figures/multiplosespelhos.png
---
width: 300px
name: fig_multiplosespelhos
---
:::

- Cubo da Lua. Na configuração mostrada, demonstre que o ângulo do raio refletido final será sempre igual ao ângulo incidente.
:::{figure} ./figures/cuboLua.png
---
width: 300px
name: fig_cuboLua
---
:::
## Espelhos esféricos

A superfície refletora é esférica. 

### Espelho côncavo

- Imagem real longe e imagem virtual perto. O que é longe e perto?

- Geometria do espelho:
    - Vértice (V)
    - Centro de curvatura (C)
    - Raio de curvatura (r)

:::{figure} ./figures/espelhoesfericogeometria1.png
---
width: 700px
name: fig_espelhoesfericogeometria1
---
:::

- Formação da imagem: aproximação paraxial

:::{figure} ./figures/espelhoesfericoparaxial0.png
---
width: 350px
name: fig_espelhoesfericoparaxial0
---
:::


:::{figure} ./figures/espelhoesfericoparaxial1.png
---
width: 300px
name: fig_espelhoesfericoparaxial0
---
:::

:::{figure} ./figures/espelhoesfericoparaxial2.png
---
width: 500px
name: fig_espelhoesfericoparaxial0
---
:::

Para um objeto puntiforme no eixo, qual é a relação entre a distância $s$ do objeto ao espelho e a distância $s'$ entre a imagem e o espelho?

Geometria, lei dos senos. Na aproximação paraxial: 

- Distância objeto e distância imagem

```{math}
\frac{1}{s} + \frac{1}{s'} = \frac{2}{r}\;.
\label{eq:espelhoesferico1}
```

Para um objeto puntiforme fora do eixo, qual é a relação entre a distância $y$ do objeto ao eixo e a distância $y'$ da imagem ao eixo?

```{math}
\frac{y'}{y} \;=\;-\;\frac{s'}{s}\;.
\label{eq:espelhoesferico2}
```

- O plano focal do espelho esférico

:::{figure} ./figures/espelhoesfericofoco.png
---
width: 500px
name: fig_espelhoesfericofoco
---
:::

Obtemnos a chamada **equação dos espelhos esféricos**:
```{math}
f = \frac{r}{2}\;\;\;\Rightarrow\;\;\;\frac{1}{s} + \frac{1}{s'} = \frac{1}{f}\;.
\label{eq:espelhoesferico3}
```

:::{figure} ./figures/espelhoesfericofoco2.png
---
width: 500px
name: fig_espelhoesfericofoco2
---
:::

- **Exercício**: uma fonte puntiforme está a 12 cm de um espelho côncavo e 3,0 cm acima do eixo do espelho. O raio de curvatura do espelho é 6,0 cm. Encontre: (a) a distância focal do espelho e (b) a distância imagem. (c) Encontre a posição da imagem relativa ao eixo.

:::{figure} ./figures/espelhoesfericoexerciciofoco.png
---
width: 500px
name: fig_espelhoesfericoexerciciofoco
---
:::

- Raios principais: para encontrar a imagem formada, trace os seguintes raios:
    - Raio paralelo ao eixo: é refletido no foco.
    - Raio apontando ou partindo do foco: reflete paralelamente ao eixo.
    - Raio apontando ou partindo do centro: reflete sobre si mesmo.

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

- **Aumento (magnificação) lateral**

O aumento lateral do espelho é a razão $y'/y$. Ele dá a razão entre o tamanho da imagem e o tamanho do objeto, além da orientação (sinal positivo, mesma orientação; sinal negativo: orientação invertida).

- **Convenção de sinais**

1) $s>0$ se o objeto está do mesmo lado que a luz incidente.
2) $s'>0$ se a imagem está do mesmo lado que a luz refletida.
3) $r>0$ se $C$ está do lado da luz incidente. 

Portanto, $r>0$ para espelho côncavo e $r<0$ para o espelho convexo.
 
### Espelho convexo

Para espelhos convexos valem as mesmas expressões, desde que consideremos $r<0$. 

Pela equação dos espelhos esféricos, temos necessariamente que $s'<0$, isto é, a imagem é sempre virtual.

:::{figure} ./figures/espelhoesfericoconvexo.png
---
width: 350px
name: fig_espelhoesfericoconvexo
---
:::
