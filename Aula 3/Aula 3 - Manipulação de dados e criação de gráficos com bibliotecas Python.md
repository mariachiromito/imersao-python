
# Objetivos da aula

Nesta aula, vamos continuar a manipulação de dados com Pandas no Colab por meio da transformação da planilha de ações. Além disso, vamos começar a construir gráficos com a biblioteca Plotly.

## Nesta aula, você vai:

- Manipular dados com Pandas;
- Transformar a planilha de ações com funções do Pandas;
- Construir gráficos com a biblioteca Plotly Express;
- Usar o Chat GPT durante o código.

Fique até o final da aula e descubra insights e orientações exclusivas para impulsionar o seu aprendizado de forma eficaz com o uso do ChatGPT.

---
# Aula 

Nesta aula recriamos a planilha feita na primeira aula usando python, recriamos também a planilha de análises feita segunda aula, e fizemos um gráfico com o DataFrame criado com base na tabela das variações por resultado.

[Códigos e mais explicações da aula](aula3_codigo.ipynb)

---
# Desafio proposto

- Pesquise com a documentação da biblioteca Plotly ou GPT como mudar a formatação dos números do gráfico de barras;
- Fazer o gráfico de pizza no df_análise_segmentos com a mesma biblioteca Potly;
- Fazer o GroupBy da categoria de idades e gerar o gráfico de barras.
[Link para saber mais sobre a biblioteca Plotly](https://plotly.com/python/bar-charts/)

[Resolução do desafio](desafio_aula3.ipynb)

---
# Links para saber mais

## Bibliotecas python

Existem diversas bibliotecas em python que servem para nos auxiliar no processo de análise e visualização de dados

### O que é visualização de dados

Também pode ser chamada de Data Visualization ou DataViz, que são um conjunto de técnicas usadas para mostrar os dados e informações de uma forma visual, fazendo com que a análise se torne mais fácil e rápida.

Essa visualização pode ser feita na forma de gráficos, tabelas ou diagramas.

Tudo isso é muito importante pois dessa forma todos os setores do projeto podem entender os resultados que a análise de dados trouxeram.

### Terminologia

| **Termo**   | **Tradução** | **Observações**                                                                                                                                                                                         |
| ----------- | ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Chart       | Gráfico      | Geralmente é acompanhado do tipo do gráfico.  <br>Ex: Pie Chart (Pizza), Bar Chart (Barras), Line Chart (Linhas), Bubble Chart (Bolhas), etc.                                                           |
| Plot        | Plotagem     | Produção de uma imagem por meio de desenhos e linhas. Ação de construir o gráfico.                                                                                                                      |
| Axis / Axes | Eixo         | Eixo dos gráficos.  <br>Ideia análoga à Matemática, na qual temos X e Y para o caso 2D e X, Y, Z para o caso 3D.                                                                                        |
| Label       | Rótulo       | São os rótulos que dão o nome e acompanham cada eixo.  <br>Geralmente aparecem acompanhados do respectivo eixo. Ex: `x_label`, `y_label`, etc.                                                          |
| Grid        | Grade/Malha  | É a estrutura de fundo de um gráfico.  <br>Linhas horizontais e verticais espaçadas que servem de referência para as unidades dos eixos.                                                                |
| Legend      | Legenda      | Caixa de texto descritivo, contendo informações sobre os elementos do gráfico.  <br>Geralmente traz informação sobre o que significa determinada cor ou traçado e/ou quais as variáveis sendo plotadas. |

![[Pastedimage20240330202644.png]]

### Principais bibliotecas

#### Matplotlib

Está é uma das principais bibliotecas para análise de dados em python.

Ela possui uma variedade de gráficos e também permite a personalização dos gráficos. Para os gráficos em imagens, é possível trabalhar com vários tipos de saída, desde os mais comuns PNG, PDF, JPEG, SVG e EPS, sendo este último um formato bastante utilizado para artigos acadêmicos e técnicos. 

##### Galeria de gráficos 

A documentação do Matplotlib disponibiliza dois links interessantes: o **Plot Types** e o **Examples**.

- [Plot types](https://matplotlib.org/stable/plot_types/): página dedicada a mostrar os tipos de visualizações possíveis com Matplotlib. Alguns deles são: _plot_, _scatter_, _bar_, _stem_, _step_ e _fill_between_.

![[Pastedimage20240330203527.png]]

- [Examples](https://matplotlib.org/stable/gallery/): página com exemplos diversos e junção de funções de criação e customização diferentes do matplotlib. Alguns dos exemplos mostrados são: _Bar color demo_, _Bar Label Demo_, _Stacked bar chart_, _Grouped bar chart with labels_, _Horizontal bar chart_ e _Broken Barh_.

![[Pastedimage20240330203813.png]]

Além da grande variedade de gráficos 2D estáticos, a Matplotlib também permite a criação de animações no formato GIF, gráficos em 3D e a junção de vários gráficos em um só (subplots). Tudo isso com o uso de módulos específicos dentro da biblioteca.A documentação do Matplotlib disponibiliza dois links interessantes: o **Plot Types** e o **Examples**.

#### Seaborn

Está é uma biblioteca que é baseada no matplotlib.Ela propõe uma interface de alto nível para trabalhar com gráficos mais atrativos e com informações estatísticas, com a ideia principal que, segundo Waskom, “a Seaborn torna coisas difíceis em coisas muito fáceis de serem feitas”.

A biblioteca é geralmente utilizada em conjunto com outras bibliotecas de análise de dados, das quais tem uma ótima aderência entre os seus objetos, como NumPy e Pandas, nos quais é possível indicar de maneira simples as variáveis que estão sendo utilizadas e gerar rapidamente resultados.

##### Galeria de gráficos da Seaborn

A Seaborn também possui uma [galeria de imagens](https://seaborn.pydata.org/examples/index.html) dos gráficos feitos utilizando a biblioteca.

![[Pastedimage20240330205136.png]]
E uma das características mais importantes da Seaborn é a **facilidade em tratar informações estatísticas** do conjunto de dados durante o processo de _plot_ dos gráficos.

#### Plotly

A Plotly é uma biblioteca para visualização de dados **de forma interativa** em Python e que possui suporte em outras linguagens de programação.
A principal característica da Plotly é a capacidade de criar gráficos que podem ser manipulados em tempo real pelos usuários, permitindo que a exploração dos dados seja dinâmica e imersiva.

A Plotly funciona muito bem com várias plataformas usadas em Ciência de Dados e desenvolvimento de softwares, tais como: [Jupyter Notebook](https://www.alura.com.br/artigos/conhecendo-o-jupyter-notebook), Dash (framework de dashboards web), aplicativos webs, [Streamlit](https://www.alura.com.br/artigos/streamlit-compartilhando-sua-aplicacao-de-dados-sem-dor-de-cabeca) e possui a possibilidade de exportação de HTML para páginas web.
##### Galeria de gráficos da Plotly

A galeria de gráficos da Plotly está disponível na página [Plotly Open Source Graphing Library for Python](https://plotly.com/python/) e conta com diversos exemplos de gráficos básicos, estatísticos, mapas e vários exemplos aplicados.

![[Pastedimage20240330205425.png]]

[Conheça as bibliotecas do Python](https://www.alura.com.br/artigos/data-visualization-conhecendo-bibliotecas-python)

---
## O que é um DataFrame

[[Aula 2 - Gráficos e análises com Google Colab e python pandas#DataFrames]]

 [O que é DataFrame](https://www.alura.com.br/artigos/pandas-o-que-e-para-que-serve-como-instalar#:~:text=DataFrame,Series%20sob%20um%20mesmo%20index.)

---
## ChatGPT e a análise de dados avançada

 [ChatGPT e a análise de dados avançada](https://www.youtube.com/watch?v=u-JoDQ58Dv0)