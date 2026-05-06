# Propriedades comuns às ondas tridimensionais

A particularidade da natureza eletromagnética vai ser usada na parte seguinte, que é a obtenção das amplitudes refletida e transmitida. Como antecipado, não abriremos as contas aqui. Obtém-se para a refletividade:

\begin{equation}\label{eq:rperp}
r_{\perp} = \frac{\sin^2(\theta_1-\theta_2)}{\sin^2(\theta_1+ \theta_2)}
\end{equation}
e, para a polarização perpendicular ao plano de incidência:

\begin{equation}\label{eq:parallel}
r_{\parallel} = \frac{\tan^2(\theta_1-\theta_2)}{\tan^2(\theta_1+ \theta_2)}
\end{equation}

Os gráficos de $r_{\parallel}$ e $r_{\perp}$ para a interface ar/vidro são mostrados a seguir:

% 
:::{figure} ./figures/refletividade.png
---
width: 200px
name: fig_refletividade
---
:::

Note que $r_{\perp} \geq r_{\parallel}$. Portanto, se a luz incidente não é polarizada, a luz refletida tem polarização (a direção de saída é a mesma, mas a amplitude, não). Dizemos que há polarização por reflexão. Em particular, quando $\theta_1 + \theta_2 = \pi/2$ (o que implica em $\tan \theta_1 = n$), não há onda refletida com polarização paralela (a onda com polarização paralela é toda transmitida). A luz refletida é completamente polarizada. Este é chamado de ângulo de Brewster. Para a interface ar-vidro, o ângulo de Brewster é cerca de $57^\circ$.

Observe também que as equações \ref{eq:rperp} e {eq}`eq:rparallel` são simétricas se trocarmos a ordem dos meios. Isso implica que a interface  de forma igual em ambos os lados.

Para $n_2 < n_1$, há um ângulo de incidência $\theta_c$ para o qual $\sin(\theta_c) = n_2/n_1$. 
