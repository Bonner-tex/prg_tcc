# Programas do meu Trabalho de Conclusão de Curso

`Por Willian Bonner`

Este repositório contém os códigos desenvolvidos para meu Trabalho de Conclusão de Curso, que aborda sistemas dinâmicos e suas aplicações em modelagens de sistemas laser. Os códigos geram exemplos e resultados numéricos discutidos no texto.

## Contexto

Sistemas dinâmicos podem ser lineares ou não lineares, dependendo da forma das equações que os descrevem. Para mais detalhes teóricos, consulte o TCC (link a ser adicionado quando disponível).

## Ambiente de desenvolvimento

Todos os códigos foram gerados localmente utilizando Jupyter Notebook em uma máquina com Windows 10. É necessário ter o LaTeX instalado para a execução correta (recomenda-se a instalação do MiKTeX). As configurações específicas ficam a cargo do usuário.

## Estrutura do repositório

### 1. Pasta principal: `src`

#### 1.1. Código de Exemplos: `code_examples`

Neste código estão disponíveis os trechos utilizados para gerar as imagens dos exemplos presentes no TCC. A estrutura é simples e deve ser executada na seguinte ordem:

1. Importação de pacotes e configurações iniciais.
2. Códigos para plotagem de espaços de fase em 2D.
3. Código para o espaço de fase de um sistema unidimensional.
4. Códigos para diagramas de fase.

#### 1.2. Resultados Maxwell-Bloch: `code_results_MB`

Este código realiza a análise numérica de um sistema laser baseado nas equações de Maxwell-Bloch, transformadas no sistema de Lorenz. No TCC, é referenciado como "Código 02". O código recebe parâmetros como σ, b e r; no trabalho, utilizamos os parâmetros do laser de amônia (NH3). Também é analisado um sistema reduzido de Maxwell-Bloch.

#### 1.3. Resultados Equações de Taxa: `code_results_TX`

Este código faz a análise numérica de um sistema laser de três níveis descrito por equações de taxa.

### 2. Modelo do TCC em LaTeX: `tex-model`

O template do texto do TCC, escrito em LaTeX, está disponível nesta pasta para quem desejar utilizá-lo como modelo.
