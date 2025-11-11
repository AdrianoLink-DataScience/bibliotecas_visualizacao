Análise Exploratória de Dados (EDA), desde a importação e tratamento até a visualização de dados de imigração para o Canadá usando Matplotlib, Seaborn e Plotly.
-----

# Análise e Visualização de Dados de Imigração para o Canadá (1980-2013)

Este repositório contém uma análise detalhada dos dados de imigração para o Canadá entre os anos de 1980 e 2013. O projeto utiliza Pandas para a manipulação e tratamento dos dados, e demonstra uma comparação prática entre as bibliotecas de visualização `Matplotlib`, `Seaborn` e `Plotly`.

O notebook `tratamento_e_visualização_de_dados.ipynb` é o arquivo principal onde toda a análise é conduzida.

## 📈 Sobre o Projeto

O objetivo principal deste projeto é demonstrar um fluxo de trabalho de análise de dados, focando em:

  * **Tratamento de Dados:** Limpeza, transformação e filtragem de dados usando `pandas`.
  * **Análise Exploratória (EDA):** Extração de insights, com foco especial na imigração de países da América do Sul, incluindo o Brasil.
  * **Visualização Comparativa:** Criação de visualizações estáticas e interativas para comparar as tendências de imigração, demonstrando os pontos fortes das bibliotecas `matplotlib`, `seaborn` e `plotly`.

## 📊 Dataset

O dataset utilizado (`imigrantes_canada.csv`) contém dados anuais de imigração para o Canadá, categorizados por país de origem, região e continente, de 1980 a 2013. Os dados são carregados diretamente de um repositório público no GitHub.

## 🛠️ Tecnologias Utilizadas

Este projeto utiliza as seguintes bibliotecas Python:

  * **Pandas:** Para importação, manipulação e análise dos dados.
  * **Matplotlib:** Para a criação de gráficos estáticos e subplots.
  * **Seaborn:** Para a criação de gráficos estatísticos, como barras.
  * **Plotly Express:** Para a criação de gráficos interativos.
  * **Jupyter Notebook:** Como ambiente de desenvolvimento e apresentação da análise.

## 🚀 Instalação e Uso

Para executar este projeto localmente, siga os passos abaixo:

1.  **Clone o repositório:**

    ```bash
    git clone https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
    cd SEU-REPOSITORIO
    ```

2.  **Crie e ative um ambiente virtual (Recomendado):**

    ```bash
    python -m venv venv
    source venv/bin/activate   # Em Windows: venv\Scripts\activate
    ```

3.  **Instale as dependências:**

    ```bash
    pip install pandas matplotlib seaborn plotly
    ```

4.  **Inicie o Jupyter Notebook:**

    ```bash
    jupyter notebook
    ```

5.  Abra o arquivo `tratamento_e_visualização_de_dados.ipynb` e execute as células.

## 🔬 Principais Análises e Visualizações

O notebook aborda diversas técnicas de análise e plotagem:

### 1\. Preparação dos Dados

  * Importação do CSV e definição do 'País' como índice.
  * Criação de uma coluna 'Total' para agregar os dados de imigração ao longo dos anos.
  * Filtragem de dados para focar em regiões específicas (América do Sul) e países (Brasil).
  * Identificação dos 10 países com maior imigração total (`top_10`).
  * Transposição dos dados (`america_sul_final`) para facilitar a plotagem de séries temporais.

### 2\. Visualização com Matplotlib

  * **Gráfico de Linha:** Tendência de imigração do Brasil para o Canadá (1980-2013).
  * **Subplots (2x2):** Comparação das tendências de Brasil, Argentina, Colômbia e Peru.
  * **Customização:** Demonstração de como ajustar títulos, rótulos (labels), ticks dos eixos e grades.
  * **Exportação:** Salvamento de um gráfico como arquivo PNG (`imigracao_brasil_canada.png`).

### 3\. Visualização com Seaborn

  * **Gráfico de Barras (Vertical):** Plotagem do `top_10` de países por imigração total.
  * **Gráfico de Barras (Horizontal):** Mesma análise com orientação horizontal para melhor legibilidade dos nomes dos países.

### 4\. Visualização com Plotly Express

  * **Gráfico de Linha Interativo:** Análise da imigração brasileira com *hover* para detalhes.
  * **Gráfico de Barras Interativo:** Imigração total dos países da América do Sul.
  * **Gráfico de Área Interativo:** Visualização da contribuição percentual de cada país sul-americano ao longo do tempo.
  * **Exportação:** Salvamento de um gráfico interativo como arquivo HTML (`imigracao_america_sul.html`).

## 📂 Estrutura do Projeto

```
.
├── imigracao_america_sul.html               # Saída de gráfico interativo (Plotly)
├── imigracao_brasil_canada.png                # Saída de gráfico estático (Matplotlib)
├── tratamento_e_visualização_de_dados.ipynb   # Notebook principal com a análise
└── README.md                                  # Este arquivo
```

## 📄 Licença

Este projeto é distribuído sob a licença MIT.
