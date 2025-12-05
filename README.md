# Análise Preditiva De Homicídios no Ceará (CVLI)

**Projeto de Portfólio | Análise de Séries Temporais e Modelagem Preditiva**

---

## 🎯 Objetivo Principal

Este projeto consiste na implementação de um **pipeline de Análise Exploratória (EDA)** e **Modelagem Preditiva** sobre dados de Crimes Violentos Letais Intencionais (CVLI) para uma região específica, com foco em Homicídios Dolosos.

O objetivo é transformar dados históricos em **inteligência de Segurança Pública**, realizando:
1.  Consolidação de séries temporais históricas (2009-2024) e demográficas.
2.  Cálculo da **Taxa de Criminalidade por 100 mil habitantes** (KPI).
3.  Implementação do modelo **SARIMA** (Sazonal ARIMA) para gerar **projeções de ocorrências** para os próximos meses (Forecasting).

---

## 🛠️ Stack Tecnológico e Metodologia

| Ferramenta | Finalidade no Projeto |
| :--- | :--- |
| **Python** | Ambiente de desenvolvimento. |
| **Pandas, NumPy** | ETL e manipulação de grandes volumes de dados. |
| **Statsmodels** | Modelagem preditiva (SARIMA). |
| **Matplotlib, Seaborn** | Visualização de tendências e sazonalidade. |

## 🔑 Resultados Chave e Insights Gerados

Esta análise gerou conclusões estratégicas baseadas em dados históricos:

* **Identificação de Foco (KPI):** O município com o maior volume de Homicídios por 100 mil habitantes (2009-2025) foi **São João do Jaguaribe**, seguido por **Ibicuitinga, Quixeré e Guaiuba**.
* **Projeção Preditiva (SARIMA):** O modelo foi treinado em dados históricos e utilizado para gerar previsões de ocorrências por método (ex: Arma de Fogo).
    * *Exemplo de Forecast:* Para Outubro de 2025, o modelo prevê **251.0 ocorrências de crimes com arma de fogo** e **242.0 para Novembro de 2025**.
...
* **Validação de Tendência e Impacto:** O modelo SARIMA previu uma queda consistente no número de ocorrências nas 4 cidades historicamente mais afetadas (Censo 2022). Esta queda é **validada pela realidade atual**, onde o foco da criminalidade se deslocou para novos municípios, como **Maranguape**.

**🔗 Link de Contexto (Notícia):** Este deslocamento de foco é corroborado por reportagens recentes sobre o aumento de violência em Maranguape. [Link da Notícia: https://g1.globo.com/ce/ceara/noticia/2025/11/29/com-maior-taxa-de-homicidios-do-pais-e-violencia-em-alta-maranguape-recebe-operacao-policial.ghtml]

...
* **Validação de Tendência:** A previsão do modelo indicou uma queda consistente no número de ocorrências nas 4 cidades historicamente mais afetadas (Censo 2022), validando a mudança do foco da criminalidade para outros municípios (ex: Maranguape).

### 📈 Desempenho do Modelo Preditivo

O modelo SARIMA foi validado em um conjunto de testes e demonstrou alta acurácia para a previsão de CVLI, comprovando a eficácia da modelagem para *forecasting*:

* **MAPE (Erro Médio Absoluto Percentual): 13.69%**
* **MAE (Erro Médio Absoluto): 35.54**
* **RMSE (Raiz do Erro Quadrático Médio): 42.39**

---

## 📦 Estrutura de Dados e Execução

O projeto utiliza três bases de dados principais (`.xlsx`) que devem estar no mesmo diretório do notebook principal para execução.

### Dados
* `CVLI_2009-2024.xlsx`: Dados históricos utilizados para treino e análise exploratória.
* `CVLI_2025.xlsx`: Arquivo de referência para validação das projeções de séries temporais.
* `DADOS_IBGE.xlsx`: Utilizado para enriquecimento dos dados e cálculo da Taxa por 100 mil habitantes.

### Dependências
```bash
pip install pandas matplotlib seaborn openpyxl numpy statsmodels



