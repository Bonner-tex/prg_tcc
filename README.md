# <center> Programas do meu Trabalho de Conclusão de Curso

`Por Willian Bonner`

Meu trabalho de conclusão de curso foi basicamente estudar Sistemas Dinâmicos e utilizar modelagens matemáticas de sistemas lasers para mostrar algumas dessas características. Resumidamente, para quem não leu o TCC, sistemas dinâmicos são sistemas de equações diferenciais que são escritos da forma de campos vetoriais. Separamos em dois tipos principais para facilidar os estudos:

1. **Sistemas lineares:** São dados por $$\dot{x}_i = \sum_{j=1}^{n} a_{ij}x_j + b_i,$$
onde $b_i$ é um vetor constante. Esse sistema completo pode escrito como um campo vetorial da seguinte forma:$$\dot{\mathbf{x}} = \big(\dot{x}_1, \dot{x}_2, \dots, \dot{x}_n \big).$$

2. **Sistemas não lineares:** São sistemas dados por$$\dot{\mathbf{x}} = \mathbf{F}(x_1, x_2, \dots, x_n),$$
onde $\mathbf{F}(x_1, x_2, \dots, x_n)$ é um campo vetorial mais geral, do tipo $\mathbf{F}: \mathbb{R}^n \to \mathbb{R}^n$. 
Para maiores detalhes, o leitor pode consultar meu TCC (linkar o tcc aqui quando estiver no site da UFS).

Todos os códigos foram gerados localmente utilizando o *Jupyter Notebook* em uma máquina rodando windowns 10. Além disso, é necessário ter o Latex instalado para que os códigos rodem corretamente: isso pode ser feito com um comando próprio no *Jupyter* ou com a instalação do MikTex. Essas configurações ficam a cargo do leitor.

## **1.** Pasta principal: `src`

### **1.1.** Código de Exemplos: `code_examples`

Neste código, estão disponíveis todos os snippets que utilizamos para gerar as imagens dos exemplos no TCC. A estrutura do código é simples, e é importante que seja executado na ordem:

1. **Importação de pacotes:** aqui estão os principais pacotes e configurações deste notebook.
2. **Códigos que plotam espaços de fase 2D**
3. **Código para o espaço de fase do sistema $\dot{x} = \sin{x}$**
4. **Códigos para plotar diagramas de fase**

### **1.2.** Resultados Maxwell-Bloch: `code_results_MB`

O codigo disponível nessa pasta gera análise numérica para o seguinte sistema dinâmico:

$$\begin{array}{l}
		\dot{X} = \sigma (Y - X),\\[.4cm]
		\dot{Y} = X(r - Z) - Y,\\[.4cm]
		\dot{Z} = XY - bZ.
	\end{array}$$

As equações acima descrevem um sistema laser a partir das equações de Maxwell-Bloch transformadas no sistema de Lorenz conforme demonstrou (HAKEN, 1975). No TCC, esse código está referenciado como *"Código 02"*. O código recebe os parâmetros $\sigma$, $b$ e $r$. No TCC, utilizamos os parâmetros do laser de amônia (NH3) para gerar as análises numéricas, os parâmetros são:

$$
	\begin{array}{l}
        \sigma = 2.0,\\[.4cm]
        r = 15,\\[.4cm]
		b = 0.25.
	\end{array}$$

Também estudamos o sistema,

$$\dot{\mathcal{E}} = \mathcal{E} \left(-\kappa_c + \dfrac{g_0\kappa w_0}{\gamma_2}\bigg( 1 + \dfrac{\kappa^2}{\gamma_1\gamma_2}\mathcal{E}^2 \bigg)^{-1}  \right),$$

que chamei de **sistema de Maxwell-Bloch reduzido**.

### **1.3.** Resultados Equações de Taxa: `code_results_TX`

Este código faz a análise numérica do sistema dinâmico:

$$\left\{\begin{array}{l}
    \dot{N}_1 = W_p(N_3 - N_1) + W_l(N_2 - N_1) + T_{21 }N_2\\[.4cm]
	\dot{N}_2 = W_l(N_1 - N_2) + T_{32}N_3 - T_{21} N_2\\[.4cm]
	\dot{N}_3 = W_p(N_1 - N_3) - T_{32}N_3
    \end{array}\right.$$
As equações acima descrevem um sistema laser de três níveis a partir das equações de taxa. 

## **2.** Modelo do TCC em Latex: `tex-model`

O latex dispensa apresentações para pessoas da área das ciências exatas. Caso você queira usar meu modelo de TCC, o template está disponível aqui também.
