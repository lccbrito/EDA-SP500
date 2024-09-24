# Análise Exploratória de Dados: Empresas do S&P 500 e Dados de Ações
### 📋 Contexto e Objetivo

Este projeto realiza uma **Análise Exploratória de Dados (EDA)** sobre as empresas que compõem o índice **S&P 500**, um dos principais indicadores do mercado financeiro dos Estados Unidos. O índice S&P 500 é composto pelas 500 maiores empresas, listadas principalmente nas bolsas **NYSE** e **NASDAQ**, abrangendo diversos setores e indústrias.

O objetivo desta análise é obter insights sobre as características dessas empresas, explorar padrões financeiros e de mercado, além de fornecer informações úteis para analistas, investidores e estudos econômicos. A análise busca responder perguntas como:

* Qual é a distribuição dos setores e indústrias dentro do S&P 500?
* Quais são as empresas com maior valor de mercado?
* Como é a distribuição geográfica dessas empresas?
* Como os preços das ações variam ao longo do tempo?

### 🗂️ Conjuntos de Dados

A análise é baseada em dois conjuntos de dados principais:
**1. Empresas do S&P 500**: Informações sobre a bolsa onde estão listadas, dados financeiros (valor de mercado, crescimento de receita), setor, indústria e localização geográfica.
**2. Dados Históricos das Ações do S&P 500:** Dados históricos das ações, como preços de abertura e fechamento diários, volume negociado e variação de preços.

Os conjuntos de dados foram retirados do Kaggle, disponível em [S&P 500 Stocks (daily updated)](https://www.kaggle.com/datasets/andrewmvd/sp-500-stocks). Eles contêm os seguintes campos:

##### **1. Empresas do S&P 500** 

* **exchange:** Bolsa de valores onde a ação da empresa está listada (Ex.: "NMS" para NASDAQ).
* **symbol:** Símbolo usado para identificar a ação.
* **shortname:** Nome abreviado da empresa.
* **longname:** Nome completo da empresa.
* **sector:** Setor onde a empresa atua (Ex.: "Technology", "Communication Services").
* **industry:** Indústria específica dentro de um setor onde a empresa atua (e.g., "Consumer Electronics", "Semiconductors").
* **currentprice:** Preço atual das ações.
* **marketcap:** Valor de mercado da empresa em dólares, representando o valor total de suas ações.
* **ebitda:** Lucros antes de juros, impostos, depreciação e amortização (EBITDA) em dólares.
* **revenuegrowth:** Taxa de crescimento da receita da empresa.
* **city:** Cidade onde a sede da empresa está localizada (cidade matriz).
* **state:** Estado onde a empresa está localizada.
* **country:** País onde a empresa está localizada.
* **fulltimeemployees:** Número de funcionários em tempo integral.
* **longbusinesssummary:** Resumo da empresa. 

##### **2. Dados Históricos das Ações do S&P 500** 
* **date:** Data da transação.
* **symbol:** Símbolo/ticker da ação para identificar a empresa.
* **adj_close:** Preço ajustado de fechamento da ação (considerando dividendos e splits).
* **close:** Preço de fechamento da ação no dia.
* **high:** Preço máximo da ação no período.
* **low:** Preço mínimo no período.
* **open:** Preço de abertura no mercado.
* **volume:** Volume total de ações negociadas no período.

### 🔑 Principais Insights
1. **NYSE e NASDAQ** dominam como as principais bolsas das maiores empresas.
2. **Empresas de tecnologia** lideram tanto em número quanto em valor de mercado, com gigantes como Alphabet, Apple, Microsoft e NVIDIA.
3. A maioria das empresas está sediada nos **Estados Unidos**, reforçando o papel do país como um centro financeiro global.
4. Embora a tecnologia tenha o maior peso no índice, setores como saúde, serviços financeiros e comunicações também têm um impacto significativo no mercado.
5. As indústrias mais representadas incluem Serviços Públicos Regulados e Máquinas Industriais Especializadas, além das gigantes tecnológicas.

### 🛠️ Estrutura do Projeto
* database/: Contém os arquivos dos conjuntos de dados utilizados na análise.
* Notebooks Jupyter contendo o passo a passo da EDA.
* README.md: Este arquivo.

### 🚀 Abordagem da Análise

1. **Limpeza e Preparação de Dados:**
   - Remoção de dados ausentes ou irrelevantes;
   - Padronização de nomes e formatos de colunas.
   
2. **Análise Descritiva:**
   - Análise de estatísticas, como distribuição de valor de mercado e número de empresas por setor.
   
3. **Visualizações:**
   - Gráficos para representar as distribuições setoriais, capitalizações de mercado das empresas e dados geográficos.

4. **Análise de Séries Temporais:**
   - Análise de tendências de preços das ações ao longo do tempo para empresas selecionadas.

### 📊 Principais Visualizações

- **Distribuição de Empresas por Bolsa de Valores:** Mostra o número de empresas por Exchange (Bolsa).
- **Distribuição de Setores e Indústrias:**  Mostra o número de empresas por setores e indústrias.
- **Distribuição do Peso no S&P 500 por Setor:** * Mostra o número de empresas e seu peso em diferentes setores.
- **Top 10 Empresas por Valor de Mercado:** Destaca as maiores empresas em termos de valor de mercado.
- **Distribuição Geográfica:** fornece informações sobre a localização das sedes das empresas por país.

### 🔧 Ferramentas e Bibliotecas

- **Python:** 3.12.4;
- **Pandas:** para manipulação de dados;
- **Matplotlib** e **Seaborn:** para visualização de dados;
- **Jupyter Notebook:** para a análise exploratória.