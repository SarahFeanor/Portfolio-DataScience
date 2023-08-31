[![capa](https://cdn.discordapp.com/attachments/1088554408469602305/1140659228382613654/Black_Technology_LinkedIn_Banner_5.jpg)](https://github.com/SarahFeanor?tab=repositories)

<sub> 🔗 [LinkedIn](https://www.linkedin.com/in/sarahfrezende/) | [Medium](https://medium.com/@sarahfrezende) |  [Portfólio de Data Science](https://github.com/sarahfeanor/Portfolio-DataScience)
 | [Portfólio Power BI](https://github.com/SarahFeanor/Portfolio_PowerBI)


# PYTHON FOR DATA SCIENCE 🐍

Este espaço foi concebido com o propósito de fortalecer e aprofundar meus estudos.
Neste repositório, você descobrirá uma compilação dos comandos, funções e bibliotecas que faço uso em minhas análises. 

---

<details>
<summary>PANDAS</summary>

## 🔹 PANDAS 

O pandas é uma biblioteca poderosa e amplamente utilizada em Python para análise de dados e manipulação de estruturas de dados tabulares. 
Aqui estão algumas das principais funções do pandas:

### **Criação de Estruturas de Dados:**

```python
pd.Series(): # Cria uma Series, que é uma estrutura de dados unidimensional semelhante a um array ou lista.
pd.DataFrame(): # Cria um DataFrame, uma estrutura de dados bidimensional que é semelhante a uma planilha ou tabela.
```

### **Leitura e Escrita de Dados:**

```python
# Funções para importar dados de diferentes fontes, como arquivos CSV, Excel e bancos de dados SQL.

pd.read_csv()
pd.read_excel()
pd.read_sql():

# Métodos para exportar os dados do DataFrame para diferentes formatos.

df.to_csv()
df.to_excel()
df.to_sql():
   
```

### **Indexação e Seleção de Dados:**

```python
# Formas de acessar e selecionar linhas e colunas específicas em um DataFrame.

df[]
df.loc[]
df.iloc[]

# Mostra as primeiras ou últimas linhas do DataFrame.

df.head()
df.tail()
```

### **Manipulação de Dados:**

```python
df.drop()`: # Remove linhas ou colunas do DataFrame.
df.rename(): # Renomeia colunas ou índices do DataFrame.
df.groupby(), df.pivot_table(): # Agrupa e realiza agregações em dados com base em determinados critérios.
```

### **Operações Estatísticas e Agregações:**

```python
# Calcula estatísticas sobre os dados em colunas específicas.
df.mean()
df.sum()
df.min()
df.max()

# Realiza várias operações de agregação em grupos específicos.
df.groupby()
agg()
```

### **Limpeza de Dados:**

```python
df.isnull(), `df.dropna()`, `df.fillna()`: # Lidam com valores ausentes (NaN) nos dados.
df.duplicated(), `df.drop_duplicates()`: # Lidam com valores duplicados.
```

### **Manipulação de Strings:**

```python

# Realiza operações de manipulação de strings em colunas.
df.str.upper()
df.str.lower()
df.str.replace()
```

### **Merging e Joining:**

```python
# Combinação de DataFrames.
pd.concat()
df.append()
                                          
# Realiza junções semelhantes a operações SQL.
pd.merge()

```

### **Visualização de Dados:**
```python
df.plot(): # Gera visualizações básicas diretamente do DataFrame.
```

### **Outras Funções:**
```python
df.info(): # Fornece informações sobre o DataFrame.
df.describe(): # Calcula estatísticas descritivas do DataFrame.
```

Essas são apenas algumas das muitas funções que o pandas oferece para facilitar a análise, manipulação e visualização de dados em Python. 
A biblioteca é amplamente usada por cientistas de dados e analistas para tarefas de pré-processamento, análise exploratória de dados e muito mais.
</details>

<details>
<summary>NUMPY</summary>
 
## 🔹 NUMPY
O NumPy é uma biblioteca fundamental para computação numérica em Python, e oferece uma ampla variedade de funções para manipulação de arrays, cálculos matemáticos e operações de álgebra linear. Abaixo estão algumas das principais funções do NumPy:

### Criação de Arrays:

- Uma biblioteca numérica do Python que oferece suporte a arrays multidimensionais e eficientes para operações matemáticas e científicas. 
Arrays são estruturas de dados fundamentais em programação e ciência da computação, usadas para armazenar coleções ordenadas de elementos do mesmo tipo. 

```python
np.array(): # Cria um array NumPy a partir de uma lista ou sequência.
np.zeros(): # Cria um array preenchido com zeros.
np.ones(): # Cria um array preenchido com uns.
np.arange(): # Cria um array com valores espaçados uniformemente dentro de um intervalo.
np.linspace(): # Cria um array com valores espaçados linearmente dentro de um intervalo.
```
### Operações Numéricas:
```python
np.add(), np.subtract(), np.multiply(), np.divide(): # Realizam operações aritméticas em arrays.
np.exp(): # Calcula a exponencial de cada elemento do array.
np.sqrt(): #Calcula a raiz quadrada de cada elemento do array.
np.sin(), np.cos(), np.tan(): # Calculam funções trigonométricas.
```
### Álgebra Linear:

```python
np.dot(): Realiza o produto escalar ou matricial entre arrays.
np.linalg.inv(): Calcula a matriz inversa.
np.linalg.det(): Calcula o determinante de uma matriz.
np.linalg.eig(): Calcula os autovalores e autovetores de uma matriz.
```
### Indexação e Fatias:

```python
Indexação: Acesso a elementos individuais do array.
Fatias: Criação de subconjuntos de arrays.
Indexação booleana: Seleção de elementos baseada em condições lógicas.
```

### Reduções e Estatísticas:

```python
np.sum(), np.mean(), np.median(), np.std(): Calculam estatísticas básicas.
np.min(), np.max(): Encontram os valores mínimo e máximo.
np.argmax(), np.argmin(): Encontram os índices do valor máximo e mínimo.
```

### Transformações:

```python
np.reshape(): Altera a forma (dimensões) do array.
np.transpose(): Transpõe a matriz (inverte linhas por colunas).
np.concatenate(): Concatena arrays ao longo de um eixo.
```

### Broadcasting:

Permite que arrays de diferentes formas sejam operados juntos.
Ordenação:

```python
np.sort(): Ordena os elementos de um array.
np.argsort(): Retorna os índices que ordenariam o array.
```
</details>

<details>
<summary>MATPLOTLIB</summary>
 
## 🔹 MATPLOTLIB

O Matplotlib é uma biblioteca popular para criação de visualizações gráficas em Python. Aqui estão alguns dos principais comandos e funções do Matplotlib:

### **Importação:**
   ```python
   import matplotlib.pyplot as plt
   ```

### **Criação de Gráficos:**
   - `plt.plot()`: Cria um gráfico de linhas ou pontos.
   - `plt.scatter()`: Cria um gráfico de dispersão.
   - `plt.bar()`, `plt.barh()`: Cria gráficos de barras verticais ou horizontais.
   - `plt.hist()`: Cria um histograma.
   - `plt.pie()`: Cria um gráfico de pizza.

### **Customização de Gráficos:**
   - `plt.xlabel()`, `plt.ylabel()`: Define rótulos para os eixos x e y.
   - `plt.title()`: Define o título do gráfico.
   - `plt.legend()`: Adiciona uma legenda.
   - `plt.grid()`: Adiciona grade ao gráfico.
   - `plt.xlim()`, `plt.ylim()`: Define os limites dos eixos x e y.

### **Anotações e Texto:**
   - `plt.text()`: Adiciona texto em uma posição específica no gráfico.
   - `plt.annotate()`: Adiciona uma anotação com seta.

### **Salvando e Mostrando Gráficos:**
   - `plt.show()`: Mostra o gráfico na tela.
   - `plt.savefig()`: Salva o gráfico em um arquivo.

### **Subplots e Layouts:**
   - `plt.subplots()`: Cria uma grade de subplots.
   - `plt.subplot()`: Cria um subplot individual.
   - `plt.tight_layout()`: Ajusta automaticamente o espaçamento entre subplots.

### **Estilos e Cores:**
   - `plt.style.use()`: Aplica um estilo de plotagem.
   - `plt.colors()`: Especifica cores nos gráficos.

### **Personalização Avançada:**
   - `plt.figure()`: Cria uma nova figura para gráficos.
   - `plt.subplots_adjust()`: Ajusta o espaçamento entre subplots manualmente.
   - `plt.plot()` com parâmetros adicionais: Permite personalização detalhada das linhas e pontos.

### **Manipulação de Eixos:**
   - `ax.set_xticks()`, `ax.set_yticks()`: Define as marcações dos eixos.
   - `ax.set_xticklabels()`, `ax.set_yticklabels()`: Define rótulos para as marcações dos eixos.
</details>

<details>
<summary>SEABORN</summary>

## 🔹 SEABORN

O Seaborn é uma biblioteca de visualização de dados baseada no Matplotlib, projetada para criar visualizações estatísticas atraentes e informativas.
Aqui estão alguns dos principais comandos e funções do Seaborn:

### Configuração e Estilo:

 ```python
sns.set_style(): # Define o estilo visual padrão dos gráficos.
sns.set_palette(): # Define a paleta de cores padrão.
 ```

### Visualizações Unidimensionais:

 ```python
sns.distplot(): # Histograma com uma curva de densidade.
sns.boxplot(): # Diagrama de caixa para visualizar a distribuição e outliers.
sns.violinplot(): # Gráfico de violino, combina um boxplot com um KDE.
 ```

### Visualizações Bidimensionais:

 ```python
sns.scatterplot(): # Gráfico de dispersão.
sns.lineplot(): # Gráfico de linhas.
sns.regplot(): # Gráfico de regressão linear com intervalo de confiança.
 ```

### Relações Estatísticas:

 ```python
sns.pairplot(): # Matriz de dispersão para visualizar relações entre pares de variáveis.
sns.heatmap(): # Mapa de calor para visualizar uma matriz de valores numéricos.
 ```

### Visualizações Categóricas:
 ```python
sns.countplot(): # Gráfico de contagem para variáveis categóricas.
sns.barplot(): # Gráfico de barras com médias e intervalos de confiança.
 ```

### Relações Lineares:
 ```python
sns.lmplot(): # Gráfico de dispersão com ajuste linear.
 ```
### Visualizações de Distribuição:
 ```python
sns.kdeplot(): # Estimativa de densidade do kernel.
sns.rugplot(): # Plotagem de "tapetes" ao longo do eixo.
 ```
### Visualizações de Matriz:
 ```python
sns.clustermap(): # Mapa de clusterização hierárquica de dados.
 ```
### Visualizações de Análise de Componentes Principais (PCA):
 ```python
sns.PairGrid(): # Grid de plots para análise de PCA.
 ```
### Personalização:
 ```python
sns.set(): # Configuração global de estilo.
sns.set_context(): # Define o contexto de exibição.
sns.set_palette(): # Define a paleta de cores.
sns.color_palette(): # Define uma paleta de cores personalizada.
 ```
Esses são apenas alguns exemplos dos principais comandos do Seaborn. 
A biblioteca oferece uma variedade de opções de personalização e visualização para ajudar a 
criar gráficos informativos e atraentes a partir de dados.

### **Tipos de Gráficos Avançados:**
 ```python
    - `plt.contour()`, `plt.contourf()`: # Cria gráficos de contorno.
    - `plt.imshow()`: # Exibe imagens.
    - `plt.quiver()`: # Cria gráficos de vetores.
 ```

Esses são apenas alguns dos principais comandos e funções que o Matplotlib oferece para criação e personalização de gráficos em Python. 
A biblioteca é altamente configurável e versátil, permitindo criar uma ampla variedade de visualizações para análise de dados.
</details>

<details>
<summary>PLOTLY</summary>

 ## 🔹 PLOTLY

O Plotly é uma biblioteca em Python que permite criar visualizações interativas e de alta qualidade. Aqui estão alguns dos principais comandos e funções do Plotly:

### **Criação de Gráficos Básicos:**
   - `import plotly.express as px`: Importa o módulo Express para gráficos simplificados.
   - `fig = px.bar()`, `fig = px.line()`, `fig = px.scatter()`: Cria gráficos de barras, linhas e dispersão, respectivamente.

### **Personalização e Configuração de Layout:**
   - `fig.update_layout()`: Permite configurar o layout geral do gráfico, como título, rótulos dos eixos e fontes.
   - `fig.update_xaxes()`, `fig.update_yaxes()`: Configurações específicas para os eixos x e y.

### **Adição de Traces (Camadas) aos Gráficos:**
   - `fig.add_trace()`: Adiciona camadas adicionais ao gráfico, como linhas, pontos ou barras.
   - `fig.update_traces()`: Configurações específicas para os traços individuais.

### **Gráficos 3D:**
   - `fig = px.scatter_3d()`, `fig = px.line_3d()`: Cria gráficos de dispersão e linhas em 3D.

### **Gráficos Geográficos:**
   - `fig = px.scatter_geo()`, `fig = px.choropleth()`: Cria gráficos geográficos com pontos ou mapas de calor.

### **Gráficos de Barras Empilhadas e Agrupadas:**
   - `fig = px.bar()`, `barmode='stack'` ou `barmode='group'`: Cria gráficos de barras empilhadas ou agrupadas.

### **Gráficos de Pizza e Rosca:**
   - `fig = px.pie()`, `fig = px.sunburst()`: Cria gráficos de pizza e rosca.

### **Gráficos de Superfície e Contorno:**
   - `fig = px.surface()`, `fig = px.contour()`: Cria gráficos de superfície e de contorno.

### **Gráficos Animados:**
   - `fig = px.scatter()`, `animation_frame='coluna'`: Cria gráficos animados baseados em colunas específicas.

### **Salvando e Exibindo Gráficos:**
    - `fig.show()`: Exibe o gráfico interativamente.
    - `fig.write_html()`, `fig.write_image()`: Salva o gráfico como HTML ou imagem.

### **Personalização de Cores e Temas:**
    - `fig.update_traces(marker_color='cor')`: Define cores personalizadas para traços.
    - `fig.update_layout(template='nome_template')`: Aplica temas pré-definidos ou personalizados.

### **Interação e Configuração de Eventos:**
    - `fig.update_layout(clickmode='eventos')`: Configura interações baseadas em eventos, como cliques.

### **Widgets e Controles de Exibição:**
    - `dcc.Dropdown()`, `dcc.RangeSlider()`: Cria widgets interativos para filtragem e controle.

### **Visualizações 3D Interativas:**
    - `import plotly.graph_objects as go`: Importa o módulo de gráficos do Plotly.
    - `fig = go.Figure()`: Cria figuras usando a biblioteca Graph Objects.
    - `fig.add_trace()`, `fig.update_layout()`, etc.: Funciona de maneira semelhante ao Express.

Esses são apenas alguns dos muitos recursos disponíveis no Plotly para criar visualizações interativas e personalizadas em Python. 
A biblioteca é amplamente usada para criar gráficos atraentes e interativos em notebooks Jupyter, aplicativos da web e muito mais.
</details>

<details>
<summary>SCIPY</summary>

## 🔹 SCIPY

O SciPy é uma biblioteca em Python que fornece funções para diversas operações matemáticas, científicas e de engenharia. 
Aqui estão algumas das principais funções e módulos do SciPy:

### **Álgebra Linear:**
   - `scipy.linalg`: Módulo para álgebra linear.
   - `scipy.linalg.solve()`: Resolve sistemas de equações lineares.
   - `scipy.linalg.eig()`: Calcula autovalores e autovetores.

### **Otimização:**
   - `scipy.optimize`: Módulo para otimização.
   - `scipy.optimize.minimize()`: Encontra o mínimo de uma função.
   - `scipy.optimize.curve_fit()`: Realiza ajuste de curvas.

### **Integração:**
   - `scipy.integrate`: Módulo para integração numérica.
   - `scipy.integrate.quad()`: Calcula integrais definidas.

### **Transformada de Fourier:**
   - `scipy.fft`: Módulo para transformada de Fourier.
   - `scipy.fft.fft()`: Calcula a transformada rápida de Fourier.

### **Equações Diferenciais:**
   - `scipy.integrate.odeint()`: Resolve equações diferenciais ordinárias.

### **Interpolação:**
   - `scipy.interpolate`: Módulo para interpolação.
   - `scipy.interpolate.interp1d()`: Realiza interpolação unidimensional.

### **Estatísticas:**
   - `scipy.stats`: Módulo para estatísticas.
   - `scipy.stats.norm()`: Distribuição normal.
   - `scipy.stats.ttest_ind()`: Teste t para duas amostras independentes.

### **Processamento de Sinais:**
   - `scipy.signal`: Módulo para processamento de sinais.
   - `scipy.signal.convolve()`: Convolução de sinais.

### **Transformada de Wavelet:**
   - `scipy.signal.cwt()`: Transformada contínua de Wavelet.

### **Processamento de Imagem:**
    - `scipy.ndimage`: Módulo para processamento de imagem.
    - `scipy.ndimage.imread()`: Lê imagens.

### **Álgebra Simbólica:**
    - `scipy.special`: Módulo para funções especiais.

Esses são apenas alguns exemplos das funcionalidades oferecidas pelo SciPy. 
A biblioteca é amplamente usada em áreas como matemática, ciência, engenharia, física, processamento de sinais e muito mais. Cada módulo fornece uma variedade de 
funções que podem ser exploradas para resolver problemas específicos nessas áreas.
</details>

<details>
<summary>SCIKIT-LEARN</summary>

## 🔹 SCIKIT-LEARN

O scikit-learn é uma das bibliotecas mais populares para aprendizado de máquina em Python. Aqui estão algumas das principais classes e funções que você encontrará no scikit-learn:

### **Pré-processamento de Dados:**
   - `preprocessing.StandardScaler`: Padroniza as características escalando-as para ter média zero e variância unitária.
   - `preprocessing.LabelEncoder`: Codifica rótulos de classes em valores numéricos.
   - `preprocessing.OneHotEncoder`: Converte variáveis categóricas em representações numéricas binárias.

### **Modelos de Aprendizado de Máquina:**
   - `linear_model.LinearRegression`: Modelo de regressão linear.
   - `svm.SVC`, `svm.SVR`: Máquinas de vetor de suporte para classificação e regressão.
   - `tree.DecisionTreeClassifier`, `tree.DecisionTreeRegressor`: Árvores de decisão para classificação e regressão.
   - `ensemble.RandomForestClassifier`, `ensemble.RandomForestRegressor`: Florestas aleatórias para classificação e regressão.

### **Avaliação de Modelos:**
   - `metrics.accuracy_score`: Calcula a acurácia de classificação.
   - `metrics.mean_squared_error`: Calcula o erro quadrático médio para regressão.
   - `metrics.confusion_matrix`: Calcula a matriz de confusão.
   - `metrics.classification_report`: Gera um relatório de métricas de classificação.

### **Divisão de Conjuntos de Dados:**
   - `model_selection.train_test_split`: Divide um conjunto de dados em treinamento e teste.

### **Validação Cruzada:**
   - `model_selection.cross_val_score`: Realiza validação cruzada para avaliar o desempenho do modelo.

### **Hiperparâmetros:**
   - `model_selection.GridSearchCV`: Realiza busca em grade para otimizar os hiperparâmetros do modelo.

### **Transformação de Dados:**
   - `decomposition.PCA`: Realiza a Análise de Componentes Principais para redução de dimensionalidade.
   - `feature_extraction.text.CountVectorizer`, `feature_extraction.text.TfidfVectorizer`: Vetorização de texto.

### **Aprendizado Não Supervisionado:**
   - `cluster.KMeans`: Algoritmo de clusterização K-Means.
   - `decomposition.PCA`: Análise de Componentes Principais para redução de dimensionalidade.

### **Salvando e Carregando Modelos:**
   - `joblib.dump`, `joblib.load`: Salva e carrega modelos treinados.

### **Pipeline:**
    - `pipeline.Pipeline`: Cria um pipeline que encapsula pré-processamento e modelagem.

### **Ensemble:**
    - `ensemble.VotingClassifier`, `ensemble.VotingRegressor`: Criação de modelos de ensemble.

Esses são apenas alguns dos muitos componentes e funcionalidades do scikit-learn. A biblioteca oferece uma variedade de ferramentas para tarefas de 
aprendizado de máquina, desde pré-processamento até modelagem e avaliação, tornando mais fácil para os cientistas de dados e analistas desenvolverem e 
avaliarem modelos de aprendizado de máquina.

</details>

<details>
<summary>STATSMODELS</summary>

## 🔹 STATSMODELS

O Statsmodels é uma biblioteca em Python focada em estatísticas e modelagem estatística. 
Ele fornece várias ferramentas para realizar análises estatísticas, ajustar modelos e explorar dados. 
Aqui estão alguns dos principais comandos e funções do Statsmodels:

### **Modelos de Regressão:**
   - `sm.OLS()`: Ajusta um modelo de regressão linear ordinária.
   - `sm.Logit()`: Ajusta um modelo de regressão logística.
   - `sm.GLM()`: Ajusta modelos de regressão generalizada linear.
   - `sm.WLS()`: Ajusta um modelo de regressão ponderada por mínimos quadrados.

### **Análise de Variância (ANOVA):**
   - `sm.OLS().anova()`: Realiza análise de variância para comparação de modelos.

### **Modelos de Séries Temporais:**
   - `sm.tsa.ARMA()`: Ajusta um modelo de média móvel autorregressiva.
   - `sm.tsa.SARIMAX()`: Ajusta um modelo SARIMA (Seasonal ARIMA).

### **Testes Estatísticos:**
   - `sm.tsa.adfuller()`: Teste ADF para estacionariedade de séries temporais.
   - `sm.stats.diagnostic.het_goldfeldquandt()`: Teste Goldfeld-Quandt para heteroscedasticidade.
   - `sm.stats.anova_lm()`: Realiza análise de variância (ANOVA).

### **Análise de Sobrevivência:**
   - `sm.SurvfuncRight()`: Estima a função de sobrevivência para dados censurados à direita.

### **Análise de Componentes Principais (PCA):**
   - `sm.PCA()`: Realiza análise de componentes principais.

### **Gráficos e Visualizações:**
   - `sm.graphics.plot_fit()`: Plota os ajustes dos modelos em relação aos dados.
   - `sm.graphics.qqplot()`: Plota gráficos Q-Q (quantil-quantil).

### **Testes de Hipóteses e Diagnósticos:**
   - `sm.stats.diagnostic.acorr_ljungbox()`: Teste de Ljung-Box para autocorrelação em resíduos.
   - `sm.stats.anova_lm()`: Realiza análise de variância (ANOVA).

### **Outras Funções:**
   - `sm.datasets.get_rdataset()`: Obtém conjuntos de dados incorporados no Statsmodels.
   - `sm.OLSResults()`: Classe para armazenar resultados de modelos de regressão linear.
   - `sm.LogitResults()`: Classe para armazenar resultados de modelos de regressão logística.

Lembre-se de que essa lista é apenas uma introdução às principais funções e comandos oferecidos pelo Statsmodels. 
A biblioteca oferece uma ampla gama de recursos estatísticos e de modelagem para atender às necessidades de análise de dados e modelagem estatística.

</details>

<details>
<summary>PYCARET</summary>

## 🔹 PYCARET

O PyCaret é uma biblioteca de automação de tarefas em aprendizado de máquina que simplifica o processo de treinamento, validação e comparação de modelos. Ele oferece uma interface fácil de usar para realizar várias tarefas relacionadas a machine learning. Aqui estão alguns dos principais comandos do PyCaret:

1. **setup():** Prepara o ambiente para a análise de dados e a construção de modelos. Realiza a pré-processamento dos dados, como tratamento de valores ausentes e codificação de variáveis categóricas.

2. **compare_models():** Treina e avalia vários modelos de machine learning usando validação cruzada. Retorna uma tabela com métricas de desempenho dos modelos.

3. **create_model():** Cria um modelo específico com base na seleção do usuário. Por exemplo, `create_model('rf')` criará um modelo Random Forest.

4. **tune_model():** Otimiza hiperparâmetros de um modelo criado usando busca em grid.

5. **plot_model():** Gera vários gráficos relacionados ao desempenho do modelo, como curvas ROC, matrizes de confusão, distribuição de resíduos etc.

6. **evaluate_model():** Fornecendo um modelo treinado, gera métricas de avaliação em um conjunto de validação separado.

7. **predict_model():** Faz previsões em um conjunto de dados usando um modelo treinado.

8. **finalize_model():** Finaliza o modelo selecionado para treinamento usando todo o conjunto de dados.

9. **save_model():** Salva o modelo treinado em disco para uso futuro.

10. **load_model():** Carrega um modelo previamente salvo do disco.

11. **interpret_model():** Fornece análises de interpretação para entender as decisões do modelo (requer a instalação da biblioteca SHAP).

12. **ensemble_model():** Combina modelos treinados usando a técnica de ensemble.

13. **blend_models():** Combina modelos treinados usando a técnica de blending.

14. **stack_models():** Combina modelos treinados usando a técnica de stacking.

15. **deploy_model():** Implanta um modelo treinado em um servidor em nuvem usando o PyCaret Deploy (parte do PyCaret 2.3.0 e posteriores).

16. **unstack_model():** Desfaz o empilhamento de modelos criado usando `stack_models()`.

17. **plot_model():** Gera visualizações interativas para análise de modelos.

Esses são apenas alguns dos principais comandos e funções oferecidos pelo PyCaret para simplificar o fluxo de trabalho de machine learning. 
A biblioteca é especialmente útil para quem deseja realizar experimentações rápidas e eficientes com diferentes modelos e técnicas de análise de dados.

</details>

<details>
<summary>TENSORFLOW</summary>

 ## 🔹 TENSORFLOW

O TensorFlow é uma biblioteca popular de código aberto para aprendizado de máquina e desenvolvimento de modelos de aprendizado profundo. 
Aqui estão algumas das principais funções e comandos do TensorFlow:

### **Criação de Tensores:**
   - `tf.constant()`: Cria um tensor constante com valores fixos.
   - `tf.Variable()`: Cria um tensor variável que pode ser otimizado durante o treinamento.
   - `tf.placeholder()`: Cria um espaço reservado para dados que serão alimentados durante a execução.

### **Operações Matemáticas:**
   - `tf.add()`, `tf.subtract()`, `tf.multiply()`, `tf.divide()`: Realiza operações matemáticas entre tensores.
   - `tf.matmul()`: Realiza multiplicação de matriz entre tensores.
   - `tf.reduce_sum()`, `tf.reduce_mean()`: Calcula a soma ou a média dos elementos de um tensor.

### **Construção de Modelos:**
   - `tf.keras.layers`: API de camadas para construir modelos sequenciais ou funcionais.
   - `tf.keras.Sequential()`: Cria um modelo sequencial empilhando camadas.
   - `tf.keras.Model()`: Cria um modelo mais complexo usando uma API funcional.

### **Otimização e Treinamento:**
   - `tf.keras.optimizers`: API para otimizadores de gradientes.
   - `tf.keras.losses`: API para funções de perda.
   - `tf.keras.metrics`: API para métricas de avaliação de modelos.
   - `tf.GradientTape()`: Grava operações para cálculo de gradientes durante o treinamento.

### **Treinamento de Modelos:**
   - `model.compile()`: Configura o modelo para treinamento, definindo otimizador, função de perda e métricas.
   - `model.fit()`: Treina o modelo nos dados de treinamento.
   - `model.evaluate()`: Avalia o modelo nos dados de teste.

### **Inferência e Predição:**
   - `model.predict()`: Realiza inferência e predição usando o modelo treinado.

### **Carregamento e Salvamento de Modelos:**
   - `tf.saved_model.save()`: Salva um modelo em formato TensorFlow SavedModel.
   - `tf.saved_model.load()`: Carrega um modelo TensorFlow SavedModel.

### **Trabalhando com Grafos:**
   - `tf.function()`: Anota uma função Python para compilação em um grafo TensorFlow.
   - `tf.Graph()`: Cria um novo grafo.

### **Distribuição e Paralelismo:**
   - `tf.distribute.Strategy`: API para treinamento distribuído em várias GPUs ou TPUs.
   - `tf.data.Dataset`: API para criar pipelines de entrada eficientes para treinamento distribuído.

### **Outras Funções:**
    - `tf.ones()`, `tf.zeros()`: Cria tensores preenchidos com uns ou zeros.
    - `tf.reshape()`, `tf.transpose()`: Realiza operações de reformatação e transposição.
    - `tf.argmax()`, `tf.argmin()`: Encontra o índice do valor máximo ou mínimo em um tensor.

Esses são apenas alguns dos muitos comandos e funções disponíveis no TensorFlow para criar, treinar e avaliar modelos de aprendizado de máquina e redes neurais profundas. 
A biblioteca é amplamente usada na comunidade de aprendizado de máquina e inteligência artificial.
</details>

<details>
<summary>PYTORCH</summary>

 ## 🔹 PYTORCH

O PyTorch é uma biblioteca de aprendizado profundo (deep learning) popular em Python que oferece uma variedade de recursos para criar, treinar e implantar modelos de redes neurais. Aqui estão alguns dos principais comandos e funções do PyTorch:

### **Criação de Tensores:**
   - `torch.tensor()`: Cria um tensor a partir de uma lista, array NumPy ou outro tensor existente.
   - `torch.zeros()`, `torch.ones()`: Cria tensores preenchidos com zeros ou uns.
   - `torch.rand()`, `torch.randn()`: Cria tensores com valores aleatórios.

### **Operações Matemáticas Básicas:**
   - `torch.add()`, `torch.sub()`, `torch.mul()`, `torch.div()`: Realiza operações aritméticas entre tensores.
   - `torch.dot()`: Calcula o produto escalar entre dois tensores.
   - `torch.matmul()`: Realiza multiplicação de matrizes.

### **Indexação e Seleção de Dados:**
   - `tensor[índice]`: Acessa elementos em um tensor.
   - `tensor[start:end]`: Fatiamento (slicing) de tensores.
   - `tensor[mask]`: Seleção baseada em máscaras booleanas.

### **Operações de Redução:**
   - `tensor.sum()`, `tensor.mean()`, `tensor.max()`, `tensor.min()`: Calcula estatísticas sobre um tensor.
   - `tensor.argmax()`, `tensor.argmin()`: Retorna os índices do maior e menor elemento.
   - `tensor.prod()`: Calcula o produto de todos os elementos.

### **Operações de Álgebra Linear:**
   - `torch.mm()`: Multiplicação de matrizes.
   - `torch.transpose()`, `tensor.t()`: Transposição de matrizes.
   - `torch.svd()`: Decomposição de valor singular.

### **Backpropagation e Otimização:**
   - `torch.autograd.Variable()`: Cria variáveis para rastrear operações para cálculo de gradientes.
   - `tensor.backward()`: Calcula gradientes usando o mecanismo de autograd do PyTorch.
   - Otimizadores como `torch.optim.SGD()`, `torch.optim.Adam()`: Utilizados para otimizar os pesos dos modelos durante o treinamento.

### **Criação de Modelos de Rede Neural:**
   - `torch.nn.Module()`: Classe base para criação de modelos de rede neural.
   - Módulos como `torch.nn.Linear()`, `torch.nn.Conv2d()`, `torch.nn.LSTM()`: Camadas típicas em redes neurais.

### **Funções de Ativação:**
   - `torch.nn.ReLU()`, `torch.nn.Sigmoid()`, `torch.nn.Tanh()`: Funções de ativação.
   - `torch.nn.Softmax()`: Função de ativação Softmax.

### **Treinamento de Modelos:**
   - Loop de treinamento com iterações, atualizações de pesos e cálculo de perdas.

### **Carregamento e Salvamento de Modelos:**
    - `torch.save()`: Salva um modelo treinado.
    - `torch.load()`: Carrega um modelo treinado.

Esses são apenas alguns dos principais comandos e funções oferecidos pelo PyTorch. 
A biblioteca é amplamente usada em projetos de aprendizado profundo devido à sua flexibilidade, eficiência e suporte para aceleração de hardware, como GPUs.

</details>

<details>
<summary>NLTK</summary>
 
## 🔹 NATURAL LANGUAGE TOOLKIT

O Natural Language Toolkit (NLTK) é uma biblioteca em Python amplamente usada para processamento de linguagem natural. Ela oferece uma variedade de recursos e funcionalidades para lidar com texto e análise de linguagem natural. Aqui estão alguns dos principais comandos e funcionalidades do NLTK:

### **Tokenização:**
   - `nltk.word_tokenize(text)`: Divide um texto em palavras individuais (tokens).
   - `nltk.sent_tokenize(text)`: Divide um texto em sentenças.

### **Stop Words:**
   - `nltk.corpus.stopwords.words(language)`: Retorna uma lista de palavras consideradas stopwords em um determinado idioma.

### **Stemming e Lemmatização:**
   - `nltk.stem.PorterStemmer()`: Implementa o algoritmo de stemming de Porter.
   - `nltk.stem.WordNetLemmatizer()`: Realiza a lematização das palavras.

### **Pos Tagging (Marcação de Partes do Discurso):**
   - `nltk.pos_tag(tokens)`: Marca as partes do discurso em uma lista de tokens.

### **Análise de Sentimento:**
   - `nltk.sentiment.SentimentIntensityAnalyzer()`: Calcula a polaridade do sentimento em um texto.

### **Processamento de Texto:**
   - `nltk.Text(tokens)`: Cria um objeto Text para análise de concordância e outras análises textuais.

### **FreqDist (Distribuição de Frequência):**
   - `nltk.FreqDist(tokens)`: Calcula a frequência de ocorrência de palavras em um texto.

### **Collocations (Colocações):**
   - `nltk.collocations.BigramCollocationFinder.from_words(tokens)`: Encontra colocações (pares de palavras frequentemente ocorrentes) em um texto.

### **N-gramas:**
   - `nltk.ngrams(tokens, n)`: Gera n-gramas (sequências de n palavras) a partir de uma lista de tokens.

### **Construção de Concordâncias:**
    - `nltk.Text(tokens).concordance(word)`: Mostra trechos de texto que contêm uma palavra específica.

### **WordNet:**
    - `nltk.corpus.wordnet.synsets(word)`: Retorna os synsets (conjuntos de sinônimos) de uma palavra.

### **Extração de Entidades:**
    - `nltk.ne_chunk(tokens)`: Identifica e classifica entidades nomeadas em um texto.

### **Word Clouds:**
    - `WordCloud()`: Cria nuvens de palavras com base na frequência das palavras em um texto.

### **Processamento de Linguagem:**
    - `nltk.RegexpTokenizer(pattern)`: Tokenizador baseado em expressões regulares.

Esses são apenas alguns dos principais comandos e funcionalidades do NLTK. 
A biblioteca oferece uma ampla gama de ferramentas para processamento de texto e análise de linguagem natural, tornando-a uma 
escolha popular entre os cientistas de dados e pesquisadores que trabalham com dados textuais.

</details>

<details>
<summary>SPACY</summary>

## 🔹 SPACY

O spaCy é uma biblioteca de processamento de linguagem natural (NLP) em Python que oferece várias funcionalidades poderosas para tarefas como tokenização, 
análise sintática, reconhecimento de entidades nomeadas, lematização e muito mais. Aqui estão algumas das principais funções e comandos do spaCy:

### **Carregamento do Modelo:**
   - `import spacy`
   - `nlp = spacy.load('modelo')`: Carrega um modelo específico do spaCy para processamento de linguagem.

### **Tokenização:**
   - `doc = nlp(texto)`: Processa um texto e cria um objeto Doc, que contém tokens e informações sobre eles.

### **Análise Sintática:**
   - `token.text`: Retorna o texto do token.
   - `token.lemma_`: Retorna o lema (forma base) do token.
   - `token.pos_`: Retorna a classe gramatical do token.
   - `token.dep_`: Retorna a dependência sintática do token.
   - `token.head`: Retorna o token pai do token.

### **Reconhecimento de Entidades Nomeadas:**
   - `doc.ents`: Retorna entidades nomeadas no texto.
   - `ent.text`: Retorna o texto da entidade.
   - `ent.label_`: Retorna o tipo de entidade (por exemplo, ORGANIZATION, PERSON, etc.).

### **Visualização de Análise:**
   - `displacy.render(doc, style='dep')`: Visualiza a árvore de dependências.
   - `displacy.render(doc, style='ent')`: Visualiza as entidades nomeadas no texto.

### **Filtros e Seleções:**
   - `span = doc[start:end]`: Seleciona um subconjunto contínuo de tokens (span) do Doc.

### **Ferramentas de Análise:**
   - `nlp.add_pipe(component)`: Adiciona um componente personalizado à pipeline do spaCy.

### **Processamento em Lote:**
   - `docs = list(nlp.pipe(textos))`: Processa uma lista de textos em lote.

### **Lematização e Stop Words:**
   - `token.is_stop`: Verifica se o token é uma stop word.
   - `token.is_alpha`: Verifica se o token é alfabético.
   - `token.is_punct`: Verifica se o token é um caractere de pontuação.
   - `token.lemma_`: Retorna o lema do token.

### **Personalização:**
    - `Doc.set_extension(name, default=None)`: Cria uma extensão personalizada no objeto Doc.

Estes são apenas alguns dos comandos e funções essenciais do spaCy. 
A biblioteca oferece muitos outros recursos para processamento de linguagem natural, incluindo análise de dependências, detecção de frases, identificação de padrões, 
treinamento personalizado de modelos e muito mais. É uma ferramenta poderosa para tarefas de processamento de texto e análise linguística.

</details>

<details>
<summary>BEAUTIFUL SOUP</summary>

## 🔹 BEAUTIFUL SOUP 

O Beautiful Soup é uma biblioteca em Python usada para extrair informações de páginas web e analisar documentos HTML ou XML. Aqui estão alguns dos principais comandos e métodos que você pode usar no Beautiful Soup:

### **Importação:**
   ```python
   from bs4 import BeautifulSoup
   ```

### **Criação de um objeto BeautifulSoup:**
   ```python
   soup = BeautifulSoup(html_content, 'html.parser')  # Cria um objeto BeautifulSoup a partir do conteúdo HTML
   ```

### **Navegação e Busca:**
   - `soup.find()`: Encontra a primeira ocorrência de uma tag.
   - `soup.find_all()`: Encontra todas as ocorrências de uma tag.
   - `soup.select()`: Seleciona elementos usando seletores CSS.

### **Acesso a Tags e Atributos:**
   - `tag.name`: Retorna o nome da tag.
   - `tag.text`: Retorna o conteúdo textual dentro da tag.
   - `tag['atributo']`: Retorna o valor de um atributo da tag.

### **Navegação Hierárquica:**
   - `tag.parent`: Retorna o elemento pai da tag.
   - `tag.children`: Retorna os elementos filhos diretos da tag.
   - `tag.next_sibling`, `tag.previous_sibling`: Retorna os irmãos próximos da tag.

### **Filtros:**
   - `soup.find_all('tag', class_='classe')`: Filtra tags por nome e classe.
   - `soup.find_all('tag', attrs={'atributo': 'valor'})`: Filtra tags por atributo.

### **Manipulação:**
   - `tag.string = 'Novo Texto'`: Altera o conteúdo textual de uma tag.
   - `tag['novo_atributo'] = 'valor'`: Adiciona um novo atributo a uma tag.

### **Remoção:**
   - `tag.extract()`: Remove uma tag específica do documento.
   - `tag.decompose()`: Remove uma tag e seu conteúdo completamente.

### **Prettify:**
   - `soup.prettify()`: Formata o documento para exibição mais legível.

Esses são apenas alguns dos principais comandos e métodos que você pode usar com o Beautiful Soup. 
A biblioteca oferece muitas outras funcionalidades para trabalhar com documentos HTML e XML de maneira eficiente, permitindo extrair 
informações relevantes de páginas web para análise e processamento.

</details>

<details>
<summary>NETWORKX</summary>

## 🔹 NETWORKX

O NetworkX é uma biblioteca em Python usada para análise e visualização de redes complexas, como redes sociais, redes de transporte, 
redes biológicas, entre outras. Aqui estão algumas das principais funções e comandos do NetworkX:

### **Criação de Gráficos:**
   - `nx.Graph()`, `nx.DiGraph()`: Criação de um grafo não direcionado ou direcionado.
   - `G.add_node()`: Adiciona um nó ao grafo.
   - `G.add_edge()`: Adiciona uma aresta ao grafo.

### **Acessando Informações do Grafo:**
   - `G.nodes()`, `G.edges()`: Retorna a lista de nós e arestas no grafo.
   - `G.number_of_nodes()`, `G.number_of_edges()`: Retorna o número de nós e arestas no grafo.
   - `G.neighbors()`: Retorna os vizinhos de um nó específico.

### **Análise de Grafos:**
   - `nx.degree()`: Calcula o grau de um nó (o número de arestas conectadas a ele).
   - `nx.shortest_path()`: Encontra o caminho mais curto entre dois nós.
   - `nx.connected_components()`: Identifica componentes conectados no grafo.

### **Medidas Centrais:**
   - `nx.betweenness_centrality()`: Calcula a centralidade de intermediação dos nós.
   - `nx.closeness_centrality()`: Calcula a centralidade de proximidade dos nós.
   - `nx.eigenvector_centrality()`: Calcula a centralidade do vetor próprio.

### **Visualização de Grafos:**
   - `nx.draw()`, `nx.draw_networkx()`: Funções para visualizar o grafo.
   - `nx.spring_layout()`, `nx.circular_layout()`: Algoritmos de posicionamento para layouts gráficos.

### **Operações em Grafos:**
   - `nx.subgraph()`: Cria um subgrafo a partir de um grafo maior.
   - `nx.compose()`, `nx.union()`: Combinam dois ou mais grafos.
   - `nx.isomorphism()`: Verifica se dois grafos são isomórficos.

### **Algoritmos de Caminho e Fluxo:**
   - `nx.shortest_path()`, `nx.shortest_path_length()`: Encontram o caminho mais curto e seu comprimento.
   - `nx.maximum_flow()`: Calcula o fluxo máximo em um grafo.

### **Análise de Componentes:**
   - `nx.connected_components()`, `nx.strongly_connected_components()`: Identificam componentes conectados.

### **Geradores de Grafos:**
   - `nx.erdos_renyi_graph()`, `nx.barabasi_albert_graph()`: Criação de grafos aleatórios ou livres de escala.

### **Algoritmos de Árvore e Floresta:**
    - `nx.minimum_spanning_tree()`: Encontra a árvore geradora mínima.
    - `nx.depth_first_search()`, `nx.breadth_first_search()`: Realizam busca em profundidade e largura.

Esses são apenas alguns dos principais comandos e funções oferecidos pela biblioteca NetworkX para a análise de redes complexas. 
Ela é amplamente usada para entender as estruturas e propriedades de redes em diversos campos, incluindo ciência de dados, ciências sociais, biologia, entre outros.

</details>

<details>
<summary>SCRAPY</summary>

## 🔹 SCRAPY

O Scrapy é um framework de web scraping em Python que permite extrair dados de websites de forma estruturada e automatizada. Aqui estão alguns dos principais comandos e conceitos do Scrapy:

### **Criar um Novo Projeto:**
   - `scrapy startproject nome_do_projeto`: Cria um novo projeto Scrapy com a estrutura de diretórios necessária.

### **Criar um Spider:**
   - `scrapy genspider nome_do_spider url_do_site`: Cria um spider, que é um programa que define como o Scrapy deve navegar e extrair dados de um site específico.

### **Executar um Spider:**
   - `scrapy crawl nome_do_spider`: Executa o spider criado para iniciar a extração de dados.

### **Seletores XPath e CSS:**
   - Utilize seletores XPath ou CSS para navegar pelo HTML da página e extrair os elementos desejados.
   - Exemplos: `response.xpath('//h1/text()').extract()` ou `response.css('p::text').extract()`

### **Armazenar Dados:**
   - Dentro do spider, você pode usar `yield` para enviar os dados extraídos para os pipelines.
   - Os pipelines são responsáveis por processar e armazenar os dados, como salvar em arquivos CSV ou banco de dados.

### **Configurações e Configuração do User-Agent:**
   - O arquivo `settings.py` contém configurações globais do projeto, incluindo as configurações do User-Agent para simular diferentes navegadores.

### **Limitar a Profundidade de Busca:**
   - Use a opção `-s DEPTH_LIMIT=n` ao executar um spider para limitar a profundidade da busca em níveis específicos.

### **Definir Delay e Random User-Agent:**
   - `DOWNLOAD_DELAY`: Configura um atraso entre as solicitações para evitar sobrecarregar o servidor.
   - `RANDOM_UA_PER_PROXY`: Rotaciona o User-Agent para simular diferentes navegadores.

### **Salvar Saída em um Arquivo JSON ou CSV:**
   - `scrapy crawl nome_do_spider -o arquivo_saida.json`: Salva a saída do spider em um arquivo JSON.
   - `scrapy crawl nome_do_spider -o arquivo_saida.csv`: Salva a saída em um arquivo CSV.

### **Debug e Testes:**
    - `scrapy shell url_do_site`: Inicia o shell interativo do Scrapy para testar seletores e comandos.
    - `scrapy check nome_do_spider`: Verifica se o spider está funcionando corretamente.

### **Concorrência e Paralelismo:**
    - O Scrapy possui suporte para realizar várias solicitações de forma concorrente para acelerar o processo de scraping.

### **Controle de Redirecionamento e Cookies:**
    - O Scrapy lida automaticamente com redirecionamentos e suporta cookies para sessões persistentes.

Esses são apenas alguns dos principais comandos e recursos do Scrapy. 
Ele é uma ferramenta muito poderosa para coleta de dados na web e oferece muitos recursos avançados para lidar com várias situações que podem surgir durante o processo de scraping.

</details>

<details>
<summary>OPENCV</summary>

## 🔹 OPENCV

O OpenCV (Open Source Computer Vision Library) é uma biblioteca popular em Python para processamento de imagens e visão computacional. Aqui estão algumas das principais funções e comandos do OpenCV:

### **Leitura e Escrita de Imagens e Vídeos:**
   - `cv2.imread()`: Lê uma imagem de um arquivo.
   - `cv2.imwrite()`: Salva uma imagem em um arquivo.
   - `cv2.VideoCapture()`: Inicia a captura de vídeo da câmera ou arquivo de vídeo.
   - `cv2.VideoWriter()`: Grava um vídeo a partir de imagens.

### **Manipulação de Cores e Canais:**
   - `cv2.cvtColor()`: Converte uma imagem de um espaço de cores para outro.
   - `cv2.split()`, `cv2.merge()`: Divide e combina canais de cores.
   - `cv2.inRange()`: Cria uma máscara para detectar intervalos de cor.

### **Operações Básicas de Processamento de Imagens:**
   - `cv2.resize()`: Redimensiona uma imagem.
   - `cv2.flip()`: Espelha uma imagem horizontal ou verticalmente.
   - `cv2.rotate()`: Rotaciona uma imagem.

### **Filtros e Convolução:**
   - `cv2.filter2D()`: Aplica uma máscara de convolução a uma imagem.
   - `cv2.GaussianBlur()`, `cv2.medianBlur()`, `cv2.bilateralFilter()`: Aplica filtros de suavização.
   - `cv2.Sobel()`, `cv2.Laplacian()`: Detecta bordas em uma imagem.

### **Detecção de Características:**
   - `cv2.Canny()`: Detecta bordas em uma imagem usando o algoritmo Canny.
   - `cv2.goodFeaturesToTrack()`, `cv2.cornerHarris()`: Detecta cantos e pontos de interesse.

### **Segmentação e Detecção de Objetos:**
   - `cv2.threshold()`: Realiza uma binarização de imagem.
   - `cv2.findContours()`, `cv2.drawContours()`: Encontra e desenha contornos em uma imagem.

### **Transformações Geométricas:**
   - `cv2.warpAffine()`, `cv2.warpPerspective()`: Realiza transformações de afinamento e perspectiva.

### **Detecção de Rostos e Objetos:**
   - `cv2.CascadeClassifier()`: Detecta objetos usando classificadores em cascata (como detecção de rostos).

### **Operações em Vídeo:**
   - `cv2.VideoCapture()`: Captura frames de vídeo.
   - `cv2.VideoWriter()`: Gravação de vídeo.
   - `cv2.imshow()`, `cv2.waitKey()`, `cv2.destroyAllWindows()`: Exibição de vídeo em uma janela.

### **Aplicações em Visão Computacional:**
    - Reconhecimento de objetos, detecção de movimento, rastreamento de objetos, calibração de câmera e muito mais.

Estes são apenas alguns dos principais comandos e funções oferecidos pelo OpenCV. 
A biblioteca é amplamente usada em projetos de visão computacional e processamento de imagens, desde tarefas simples de processamento até aplicações mais complexas.

</details>

<details>
<summary>XGBOOST</summary>
 
## 🔹 XGBOOST

O XGBoost (Extreme Gradient Boosting) é uma biblioteca popular para aprendizado de máquina baseado em árvores. Aqui estão alguns dos principais comandos e funções do XGBoost em Python:

### **Importação da Biblioteca:**
```python
import xgboost as xgb
```

### **Criação de um Modelo XGBoost:**
```python
model = xgb.XGBClassifier()  # Para classificação
model = xgb.XGBRegressor()   # Para regressão
```

### **Treinamento do Modelo:**
```python
model.fit(X_train, y_train)
```

### **Previsões com o Modelo Treinado:**
```python
predictions = model.predict(X_test)
```

### **Ajuste de Parâmetros:**
```python
# Exemplo de ajuste de alguns parâmetros
model = xgb.XGBClassifier(
    n_estimators=100,
    max_depth=3,
    learning_rate=0.1
)
```

### **Importância das Características:**
```python
importance = model.feature_importances_
```

### **Validação Cruzada:**
```python
from sklearn.model_selection import cross_val_score
scores = cross_val_score(model, X, y, cv=5)
```

### **Ajuste de Hiperparâmetros:**
```python
from sklearn.model_selection import GridSearchCV
param_grid = {'max_depth': [3, 6, 9], 'n_estimators': [50, 100, 150]}
grid_search = GridSearchCV(model, param_grid, cv=3)
grid_search.fit(X, y)
```

### **Salvando e Carregando Modelos:**
```python
# Salvar o modelo
model.save_model('model_name.model')

# Carregar o modelo
loaded_model = xgb.Booster()
loaded_model.load_model('model_name.model')
```

### **Visualização da Árvore do Modelo (para modelos com árvores únicas):**
```python
from xgboost import plot_tree
import matplotlib.pyplot as plt
plot_tree(model, num_trees=0)
plt.show()
```

Lembrando que o XGBoost oferece uma ampla gama de parâmetros para ajustar e otimizar o desempenho do modelo, incluindo controle sobre a complexidade das árvores, 
taxas de aprendizado, regularização e mais. A seleção adequada de parâmetros é crucial para obter um modelo bem ajustado e de alta qualidade.

</details>

<details>
<summary>LIGHTGBM</summary>

## 🔹 LIGHTGBM

O LightGBM é um algoritmo de gradient boosting framework de código aberto que é projetado para ser eficiente em termos de uso de recursos e oferece 
desempenho superior em muitos cenários. Aqui estão alguns dos principais comandos e funções do LightGBM:

### **Importando a Biblioteca:**
   ```python
   import lightgbm as lgb
   ```

### **Criando um Conjunto de Dados LightGBM:**
   ```python
   lgb_train = lgb.Dataset(data=X_train, label=y_train)
   lgb_valid = lgb.Dataset(data=X_valid, label=y_valid, reference=lgb_train)
   ```

### **Definindo os Parâmetros do Modelo:**
   ```python
   params = {
       'boosting_type': 'gbdt',  # Tipo de boosting (Gradient Boosting Decision Tree)
       'objective': 'regression',  # Objetivo da tarefa (regressão)
       'metric': 'rmse',  # Métrica de avaliação (Root Mean Squared Error)
       'num_leaves': 31,  # Número máximo de folhas em uma árvore
       'learning_rate': 0.05,  # Taxa de aprendizado
       'feature_fraction': 0.9,  # Fração de recursos a serem usados em cada árvore
       'bagging_fraction': 0.8,  # Fração de amostras usadas para treinamento de árvores
       'bagging_freq': 5,  # Frequência para o bagging
       'verbose': 0  # Nível de verbosidade (0 para silencioso)
   }
   ```

### **Treinando o Modelo:**
   ```python
   model = lgb.train(params, 
                     train_set=lgb_train, 
                     num_boost_round=1000,  # Número de iterações (árvores)
                     valid_sets=[lgb_train, lgb_valid],
                     early_stopping_rounds=50)  # Parar se a métrica de validação não melhorar após 50 iterações
   ```

### **Fazendo Previsões:**
   ```python
   predictions = model.predict(X_test, num_iteration=model.best_iteration)
   ```

### **Importância das Features:**
   ```python
   feature_importance = model.feature_importance()
   ```

### **Salvando e Carregando Modelos:**
   ```python
   model.save_model('model.txt')  # Salvar modelo
   loaded_model = lgb.Booster(model_file='model.txt')  # Carregar modelo
   ```

### **Parâmetros Avançados:**
   O LightGBM oferece uma ampla variedade de parâmetros avançados para ajustar o desempenho e o comportamento do modelo. Alguns deles incluem
   `max_depth`, `min_child_samples`, `subsample`, `colsample_bytree`, `lambda`, `alpha`, entre outros.

### **Tuning de Hiperparâmetros:**
O ajuste de hiperparâmetros é uma parte importante do treinamento de modelos. O LightGBM oferece suporte a técnicas como busca em grade (Grid Search) e
busca aleatória (Random Search) para encontrar os melhores valores de hiperparâmetros.

Lembrando que essa é apenas uma introdução aos principais comandos do LightGBM. A documentação oficial do LightGBM é uma excelente fonte para entender todos os 
parâmetros e funcionalidades em detalhes: [Documentação do LightGBM](https://lightgbm.readthedocs.io/en/latest/).

</details>

<details>
<summary>CATBOOST</summary>
 
## 🔹 CATBOOST

O CatBoost é uma biblioteca de gradient boosting que é especialmente projetada para trabalhar com dados categóricos e tem um desempenho excepcional em 
muitos casos. Aqui estão alguns dos principais comandos e funções do CatBoost:

### **Importando a Biblioteca:**
   ```python
   from catboost import CatBoostClassifier, CatBoostRegressor
   ```

### **Criando um Modelo:**
   - Para classificação:
     ```python
     model = CatBoostClassifier(iterations=1000, depth=6, learning_rate=0.1, loss_function='Logloss')
     ```
   - Para regressão:
     ```python
     model = CatBoostRegressor(iterations=1000, depth=6, learning_rate=0.1, loss_function='RMSE')
     ```

 ### **Treinando o Modelo:**
   ```python
   model.fit(X_train, y_train, cat_features=categorical_features)
   ```

### **Fazendo Previsões:**
   ```python
   predictions = model.predict(X_test)
   ```

### **Avaliando o Modelo:**
   - Para classificação:
     ```python
     accuracy = model.score(X_test, y_test)
     ```
   - Para regressão:
     ```python
     rmse = mean_squared_error(y_test, predictions, squared=False)
     ```

### **Hiperparâmetros Principais:**
   - `iterations`: Número de iterações (árvores) no treinamento.
   - `depth`: Profundidade máxima das árvores.
   - `learning_rate`: Taxa de aprendizado.
   - `loss_function`: Função de perda, como 'Logloss' para classificação ou 'RMSE' para regressão.
   - `cat_features`: Índices das colunas categóricas.
   - `verbose`: Nível de detalhes da saída durante o treinamento.

### **Tratamento de Dados Categóricos:**
   O CatBoost trata automaticamente as variáveis categóricas, mas você pode especificar explicitamente as colunas categóricas usando o parâmetro `cat_features`.

### **Validação Cruzada:**
   ```python
   from catboost import cv
   params = {"iterations": 1000, "depth": 6, "learning_rate": 0.1, "loss_function": "Logloss"}
   cv_data = cv(Pool(X, label=y, cat_features=categorical_features), params, fold_count=5)
   ```

### **Importância das Features:**
   ```python
   feature_importances = model.get_feature_importance(prettified=True)
   ```

### **Salvando e Carregando Modelos:**
    ```python
    model.save_model("model.cbm")
    loaded_model = CatBoostClassifier().load_model("model.cbm")
    ```

Lembre-se de consultar a documentação oficial do CatBoost para obter informações detalhadas sobre os parâmetros, recursos e exemplos adicionais de uso.
</details>

