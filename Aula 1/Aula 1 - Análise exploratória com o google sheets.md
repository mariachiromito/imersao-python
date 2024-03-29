# Objetivos da aula

Nesta aula, vamos começar a nossa análise da base da bolsa de valores explorando o Google Sheets, com VLOOKUP, SUMIF e muitas outras fórmulas, além de usarmos o Chat GPT durante a aula.

**Nesta aula, você vai:**
- Analisar as bases de variações na B3;
- Fazer análises exploratórias pelo Google Sheets com fórmulas
- Usar o Chat GPT;
- Gerar tabelas e cálculos de estatísticas como Máximo, Mínimo e Média. Nesta aula, vamos começar a nossa análise da base da bolsa de valores explorando o Google Sheets, com VLOOKUP, SUMIF e muitas outras fórmulas, além de usarmos o Chat GPT durante a aula.

[Tabela de ações utilizada na aula](https://docs.google.com/spreadsheets/d/1J49LTDP9wJEE9YydKgNd3mQjLPHQLXwGN0bDAbD92IE/edit?usp=sharing)

---
# Definições 

**Ativo**: nome da ação
	**Tickers**: nome da ação / código
**Ultimo**: valor que fechou a ação
**Variação dia:** iniciou em XX terminou em XX e variou em YY%
**Variação anual:** a partir do inicio daquele ano
**Variação 12 meses:** sempre 12 meses antes 
**Volume:** volume de operações

>**Análise exploratória**: Extrair informações de uma base de dados

---
# Tabela

**Cálculos**
*Variação percentual* - $variaçao / 100$

*Valor inicial*  $x = valor final / (1 + variação)$

*Valor final* = $valor inicial * (1 + variação)$ *pode ser usado para conferir*

> **Quantidade teórica** - pq tem mais de uma opção por ação / quantidade de ações que aquela empresa emitiu

*Quantidade de ações* - fórmulas: PROCV ou VLOOKUP

*Calcular a variação do montante*: $x = (valorFinal - valorInicial) * quantidade de ações$

*Resultado*: se o valor da ação subiu ou desceu

*Nome da empresa:* utiliza o PROCV ou VLOOKUP também

**Calculados com o ChatGPT**
*Segmento*: segmento em que aquela empresa atua 
*idade da empresa*:

---
# Desafio proposto

- Fazer os cálculos com as colunas de porcentagem (variação semanal; mensal; anual e 12 meses);
- Pegar via Chat GPT as faixas de idade;
- Pedir para o GPT gerar a fórmula IF para as faixas de idade.

[Planilha com o desafio concluído](https://docs.google.com/spreadsheets/d/1BVAoLD2UMz0aGgmZa_YCQvvxvJMHHZdi/edit?usp=drive_link)
# Conteúdo Extra (I.A.)

Breve introdução ao ChatGPT e Gemini (google)

---
# Links para saber mais

Esta é uma seção que faz um resumo dos artigos e outros links fornecidos pela imersão.

---
## Análise Exploratória: Primeiros passos - Artigo ALURA

### O que é?

A **análise exploratória** de dados é um tipo de análise de dados, com ela os cientistas de dados procuram *tirar algum conhecimento* sobre o dado que está sendo analisado.

### Elementos

Com a análise exploratória dos dados é possível se ter um panorama inicial sobre os dados que estão sendo analisados, podendo *identificar relações e padrões.*

#### Dataset

Um **dataset** é um *conjunto de dados* geralmente formado por colunas e linhas, onde cada valor é chamado de *dado*, consequentemente um dataset indica que as informações estão estruturadas na forma de uma *tabela* e geralmente são organizadas por *temas*.

Essa tabela possui um cabeçalho com os nomes das colunas bem definidos.

Este é um exemplo de um dataset:
![[Pasted image 20240328201202.png]]

#### Dicionário de dados

Um **dicionário de dados** é um documento que *centraliza as informações* sobre um conjunto de dados, com o objetivo de facilitar a interação e comunicação entre as pessoas envolvidas na análise.

Um dicionário serve como um mapa, guiando e mostrando os objetivos nas informações.

Porém mesmo que os dicionários sejam de grande ajuda para a análise de dados, é muito difícil encontrar Datasets com dicionário.

[Link para o artigo: Análise exploratória - Primeiros passos](https://www.alura.com.br/artigos/analise-exploratoria?_gl=1*xgnd2d*_ga*MTE5MTY2MTIxOC4xNzA4ODAxNDkz*_ga_1EPWSW3PCS*MTcxMTQ5NjU2Ni4xNC4xLjE3MTE0OTY1NjguMC4wLjA.*_fplc*WDQ0SXowOXRCRVFwbU83JTJCdFhtSDZHeW80bFh1cEdtR0pXVnElMkJ3RyUyRkd3UlZrNCUyQnRmWktPTFclMkJrYkNDRzR0WDRJa2k1bmVHOXB1Qzg4SEVkR28lMkYlMkZEb0Q5WHRhV3NUdTZVWU9oeUxGOGR6OVhuVHdyNEg0YmlkMHBVRUZkZGclM0QlM0Q)

---
## O que é IA Generativa? - Artigo ALURA

### O que é inteligência artificial

As IA's são sistemas capazes de realizar tarefas, que até o momento só poderiam ser realizadas por humanos. Juntamente com as IA's existem o aprendizado de máquina (machine learning) que são algoritmos que aprendem com dados que são fornecidos para eles.

>[!Important]- Redes Neurais
>Conjunto de algoritmos que após serem treinados podem responder com base naquele treinamento. A questão em si é passada por várias camadas, que ao final obtém uma resposta com base no que foi aprendido

>[!info]- O jogo da imitação
>Filme que conta como Alan Turing quebrou o enigma, um código que os alemães usam para enviar mensagens aos submarinos, durante a 2ª guerra mundial

### O que é IA generativa?

Uma IA generativa são IA's capazes de *criar novas informações* com base em dados pré-existentes. Essas IA's aprendem apartir de grandes bases de dados e apartir disso consehuem gerar novos dados semelhantes aos que foram usados na sua aprendizagem.

### Como funciona a tecnologia de um IA generativa?

A tecnologia que tem essa capacidade de aprendizado e geração de novos dados são as *GANs* (Redes Neurais Generativas Adversas). Essa tecnologia funciona da seguinte forma:

- Criando dados com uma *rede geradora*
- Avaliando os dados criados com uma *rede discriminadora*

Tudo isso funciona como um *ciclo*, com a rede geradora melhorando os dados com base na nota da rede discriminadora, isso acontece até que os dados alcancem uma boa qualidade.

>[!Importante]- O que Deep Learning?
>Várias camadas de IA's que a cada camada observam alguns pontos dos dados, e essas observaçoes passam para a próxima cada para outras IA's também poderem fazer a sua observação. 
>O deep learning está muito ligado com as redes neurais

As *IA's generativas podem aprender por conta própria*, identificando padrões dentro de um conjunto de dados. Muito diferente das IA's não generativas que precisam de vários exemplos que são dados por humanos para poderem ter esse aprendizado.

### Vantagens e desvantagens do uso de IA's generativas

#### Vantagens

As IA's generativas podem ser de grande ajuda quanto precisamos:

- Executar tarefas que necessitem de criatividade
- Criar textos com mais velocidade e facilidade
- Reduzir os custos em diversas áreas

Nas empresas elas podem ser usadas como ferramentas podendo:

- Automatizar tarefas repetitivas
- Fazer o onboarding de pessoas iniciantes
- Fazer análise de dados

#### Desvantagens

Porém as IA's generativas tambpem possuem algumas desvantagens, dentre elas as principais são:

- Geração de conteúdo nocivo
- Reprodução de vieses
- Limitação na capacidade de criação de conteúdo totalmente original

[Link para o artigo: O que é IA generativa?](https://www.alura.com.br/artigos/inteligencia-artificial-ia-generativa-chatgpt-gpt-midjourney?_gl=1*pd20gn*_ga*MTE5MTY2MTIxOC4xNzA4ODAxNDkz*_ga_1EPWSW3PCS*MTcxMTY2ODA5My4yMi4xLjE3MTE2NjgxMjguMC4wLjA.*_fplc*bVhCRlZtWGFzdDQ0bmY5R1ZtcWprVmFveEkwM25LTHdURHN0RGpJQkZIZnozbU14M3g4b1kwYW9jJTJCS0huRlptN0JzUlMzNHFmSjd2YSUyRnZxYXhJaFVCTTNNSCUyRnpFbUkzcHdFQjJYYjNiOFNkTVFqUHJRUFo4b1dxTktvWnh3JTNEJTNE)

---
## Podcast Hipsters - Tendencia e inovações no mercado finaceiro

[Podcast Hipsters - Tendencia e inovações no mercado financeiro](https://www.alura.com.br/podcast/hipsterstech-tendencias-e-inovacoes-no-mercado-financeiro-deep-dive-bradesco-1-hipsters-ponto-tech-361-a2326?_gl=1*xgnd2d*_ga*MTE5MTY2MTIxOC4xNzA4ODAxNDkz*_ga_1EPWSW3PCS*MTcxMTQ5NjU2Ni4xNC4xLjE3MTE0OTY1NjguMC4wLjA.*_fplc*WDQ0SXowOXRCRVFwbU83JTJCdFhtSDZHeW80bFh1cEdtR0pXVnElMkJ3RyUyRkd3UlZrNCUyQnRmWktPTFclMkJrYkNDRzR0WDRJa2k1bmVHOXB1Qzg4SEVkR28lMkYlMkZEb0Q5WHRhV3NUdTZVWU9oeUxGOGR6OVhuVHdyNEg0YmlkMHBVRUZkZGclM0QlM0Q)

---
## ChatGPT: o que é, como usar e dicas de comandos para o dia a dia - Artigo ALURA

### O que é?

O **ChatGPT** é um modelo de linguagem avançado desenvolvido pela OpenAI. Esta IA é baseasd na *arquitetura GPT* (Generative Pre-trained Transformer).

Ele foi treinado com uma grande quantidade de dados em forma de texto para gerar respostas de diferentes tópicos. Ele é feito para conversar e interagir com o usuário, podendo fornecer informações, esclarecer duvidas, e auxiliar em diversas tarefas.

[Link para o artigo: ChatGPT - Dicas e como usar](https://www.alura.com.br/artigos/chatgpt?_gl=1*xgnd2d*_ga*MTE5MTY2MTIxOC4xNzA4ODAxNDkz*_ga_1EPWSW3PCS*MTcxMTQ5NjU2Ni4xNC4xLjE3MTE0OTY1NjguMC4wLjA.*_fplc*WDQ0SXowOXRCRVFwbU83JTJCdFhtSDZHeW80bFh1cEdtR0pXVnElMkJ3RyUyRkd3UlZrNCUyQnRmWktPTFclMkJrYkNDRzR0WDRJa2k1bmVHOXB1Qzg4SEVkR28lMkYlMkZEb0Q5WHRhV3NUdTZVWU9oeUxGOGR6OVhuVHdyNEg0YmlkMHBVRUZkZGclM0QlM0Q)

