<sub> Data Science | By Sarah Faria Rezende </sub>

# ⚡ Functions - Commands - Libraries

Este espaço foi concebido com o propósito de fortalecer e aprofundar meus estudos.
Neste repositório, você descobrirá uma compilação dos comandos, funções e bibliotecas que faço uso em minhas análises. 

<details>
<summary>content</summary>

## 🔹 _Pandas_

O pandas é uma ferramenta essencial em Python para análise e manipulação de dados. 
Com estruturas flexíveis como DataFrame e Series, permite importar, limpar, transformar e analisar dados de várias fontes. 
Ele organiza dados em linhas e colunas, suporta diversos formatos de importação/exportação, facilita limpeza, manipulação e visualização. 
Ideal para cientistas de dados e analistas, o pandas é crucial na exploração de dados, identificação de padrões e análises. 
Amplamente usado, é uma ferramenta indispensável para projetos pessoais e empresariais, devido a sua eficiência e natureza intuitiva.

```python
import pandas as pd
```
### 🔸 Importanto arquivos CSV

O código _df = pd.read_csv("")_ é usado para ler um arquivo CSV e criar um DataFrame utilizando a biblioteca pandas em Python.

```python
    df = pd.read_csv("/content/listings.csv")
```
  * **df:** É uma variável que armazenará o DataFrame criado a partir do arquivo CSV. "df" é uma convenção comum para denotar um DataFrame.
  * **pd**: É um alias para a biblioteca pandas. Isso permite que você use funções da biblioteca pandas utilizando o prefixo "pd.".
  * **read_csv**: É uma função do pandas utilizada para ler arquivos CSV e criar DataFrames a partir deles.
  * **("/content/listings.csv")**: É o caminho do arquivo CSV que você deseja ler. Nesse exemplo, o arquivo "listings.csv" está localizado na pasta "/content".

Portanto, quando você executa esse código, ele carrega o arquivo CSV especificado e cria um DataFrame chamado "df" que contém os dados do arquivo CSV. Esse DataFrame pode ser usado para realizar várias operações de análise e manipulação de dados.

### 🔸 Qtd de atributos, entradas e tipos de variáveis

```python
print("Entradas: ", df[df.columns[0]].count())
print("Variáveis: ", df.shape[1])
```
Essas linhas de código estão realizando duas ações em relação a um DataFrame chamado "df":

* **print("Entradas: ", df[df.columns[0]].count())**: Esta linha imprime o número de entradas (ou linhas) presentes na primeira coluna do DataFrame "df". Isso é feito usando a função _count()_ que conta a quantidade de valores não nulos nessa coluna específica. O resultado é impresso na saída, junto com a mensagem "Entradas: ".

* **print("Variáveis: ", df.shape[1])**: Aqui, a linha imprime o número de variáveis (ou colunas) no DataFrame "df". Isso é feito usando o atributo _.shape_, que retorna uma tupla representando as dimensões do DataFrame (linhas, colunas). O índice 1 da tupla é utilizado para obter o número de colunas, e o resultado é impresso junto com a mensagem "Variáveis: ".

Em resumo, essas linhas de código estão fornecendo informações sobre o tamanho do DataFrame, contando o número de entradas (linhas) em uma coluna específica e o número total de variáveis (colunas) no DataFrame. Isso pode ser útil para entender a estrutura e a quantidade de dados no DataFrame.

### 🔸 Como verificar as 5 primeiras entradas do dataset

O código df.head() é utilizado para exibir as primeiras linhas de um DataFrame chamado "df". A função head() é uma função da biblioteca pandas em Python e é frequentemente usada para visualizar uma amostra inicial dos dados em um DataFrame. 
* o pandas irá mostrar por padrão as primeiras 5 linhas do DataFrame. Mas se você quiser ver mais ou menos linhas, pode passar um número como argumento para a função, por exemplo, df.head(10) irá mostrar as primeiras 10 linhas.

```python
df.head()
```
### 🔸 Verificar os tipos de variáveis

O _código display(df.dtypes)_ é usado para exibir os tipos de dados das colunas de um DataFrame "df". 
* A função _dtypes_ é uma função do pandas que retorna uma série contendo os tipos de dados de cada coluna do DataFrame.
* A função _display()_ é uma maneira de apresentar informações de forma mais formatada e amigável em ambientes como o Jupyter Notebook.

```python
display(df.dtypes)
```

### 🔸 Classificando Variáveis por Valores Ausentes em Ordem Decrescente

O código calcula a porcentagem de valores ausentes em cada coluna de um DataFrame "df" e, em seguida, 
classifica essas porcentagens em ordem decrescente.

```python
(round((df.isnull().sum()/df.shape[0]),2)*100).sort_values(ascending = False)
```
Aqui está o que cada parte do código faz:
* **df.isnull().sum()**: Calcula a quantidade de valores ausentes em cada coluna do DataFrame "df".
* **df.shape[0]**: Retorna o número total de linhas no DataFrame "df", ou seja, o total de entradas.
* **(df.isnull().sum()/df.shape[0])**: Calcula a proporção de valores ausentes em relação ao total de entradas para cada coluna.
* **round((df.isnull().sum()/df.shape[0]), 2)**: Arredonda as proporções calculadas para duas casas decimais.
* ***100**: Multiplica as proporções arredondadas por 100 para obter a porcentagem.
* **.sort_values(ascending=False)**: Classifica as porcentagens de valores ausentes em ordem decrescente, ou seja, da maior para a menor.

### 🔸 Verificando a quantidade de itens por culuna

O código é usado para verificar a quantidade de itens não nulos (não ausentes) em cada coluna de um DataFrame "df" e, em seguida, classificar essas quantidades em ordem decrescente.

```python
df.count().sort_values(ascending=False)
```
Aqui está o que cada parte do código faz:
* **df.count()**: Calcula a quantidade de itens não nulos em cada coluna do DataFrame "df".
* **.sort_values(ascending=False)**: Classifica as quantidades de itens não nulos em ordem decrescente, ou seja, da maior para a menor.

---
## 🔹 _Numpy_
* O NumPy é essencial para **computação científica** em Python, com suporte a **arrays** multidimensionais e operações **matemáticas** rápidas. 
Introduz o objeto **ndarray** para criar **matrizes eficientes**, operações elementares sem **loops**, broadcasting automático e 
funções matemáticas embutidas. Permite indexação eficiente, manipulação de arrays e integração com outras bibliotecas. 
Sua eficiência, capacidade de lidar com grandes dados numéricos e código aberto o tornam vital para ciência de dados, análises e 
simulações. NumPy é central na computação científica em Python.

```python
import numpy as np
```
---
## 🔹 _Matplotlib_
* O Matplotlib é uma biblioteca Python para **visualização de dados**. Ele oferece ferramentas versáteis para criar diversos tipos de gráficos, 
desde simples até complexos, permitindo personalização de cores, estilos e marcadores. Compatível com diferentes formatos de saída, 
é usado para criação de gráficos em publicações científicas e relatórios. Pode ser integrado com o ambiente Jupyter para exibir gráficos 
diretamente no notebook, facilitando a análise interativa de dados. 
É uma escolha essencial para comunicar informações visuais de maneira eficaz.

```python

import matplotlib.pyplot as plt

```
### 🔸 Gráficos
* O **%matplotlib inline** é "magic command" específica da interface do IPython (um interpretador interativo do Python) que está 
frequentemente usado em notebooks Jupyter para controlar o comportamento dos gráficos gerados pela biblioteca Matplotlib. Ao utilizar _%matplotlib inline_ em um notebook, você faz com que os gráficos gerados pelo Matplotlib sejam exibidos automaticamente abaixo do 
código correspondente. Isso é útil para análise de dados e visualizações. Sem isso, seria necessário usar _plt.show()_ para mostrar gráficos. A partir do 
Matplotlib 2.0, _%matplotlib inline_ foi substituído por _%matplotlib_ com opções de renderização. O inline ainda mostra gráficos no notebook, mas agora 
o comando é mais flexível para ambientes gráficos diversos.

```python

%matplotlib inline

```
### 🔸 Tamanho dos gráficos
* Define o tamanho padrão das figuras (gráficos) criadas pelo Matplotlib. 
O valor [10,5] representa a largura e a altura da figura em polegadas. Isso afeta as dimensões das visualizações quando elas 
são mostradas ou salvas.

```python
plt.rcParams["figure.figsize"] = [10,5]
```
### 🔸 Tamanho da fonte
* Define o tamanho padrão da fonte nos textos dos gráficos, como rótulos de eixos, títulos e legendas.
O valor 12 especifica o tamanho da fonte em pontos.

```python
plt.rcParams["font.size"] = 12
```

---
## 🔹 _Seaborn_

* O Seaborn, extensão do **Matplotlib**, enfoca criar **visualizações estatísticas** atraentes em Python. 
Com funções de alto nível e estilos pré-configurados, simplifica gráficos complexos. Destacam-se estilos de plotagem melhorados, 
integração com DataFrames, gráficos estatísticos como dispersão com ajustes, agrupamento e paletas de cores intuitivas. 
Recurso Facet Grid facilita criar grades de gráficos com variáveis diferentes. Também suporta visualizações matriciais como mapas 
de calor. Popular entre cientistas de dados, o Seaborn melhora a comunicação de dados complexos e se integra a pandas e Matplotlib.

```python
import seaborn as sns
```
---
## 🔹 _Missingno_

* A biblioteca "missingno" em Python **visualiza dados ausentes** em conjuntos de dados, fornecendo gráficos para identificar claramente as 
áreas sem valores e padrões de ausência. Características incluem matriz de valores ausentes, gráfico de barras e mapa de calor, 
exibindo proporções de valores faltantes e correlações entre colunas. Útil na análise exploratória, auxilia cientistas de dados a 
entender a extensão e a natureza dos valores ausentes, orientando decisões sobre tratamentos para garantir qualidade dos dados.

```python
import missingno
```
---
## 🔹 _Folium_
* O Folium, biblioteca Python, gera mapas interativos no código usando HTML e recursos JavaScript do Leaflet. 
Usado para visualizar dados geoespaciais, permite criar mapas com marcadores, pop-ups, camadas personalizadas e mais. 
Integra dados geoespaciais, suporta personalização, marcadores, pop-ups, e alavanca recursos avançados JavaScript. 
Útil para análise de dados espaciais, relatórios e apresentações. Amplamente aplicado em áreas como geolocalização, 
ciência ambiental e visualização geográfica, tornando análise e comunicação de informações geoespaciais mais acessíveis e eficazes.

```python
import folium
```
---
