# An-lise-e-Previs-o-de-Homic-dios-no-Cear-
Projeto acadêmico, suposto  a melhorias 

________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

Descrição do Projeto
Este projeto consiste na análise exploratória e modelagem de séries temporais de Crimes Violentos Letais Intencionais (CVLI), com foco em Homicídios Dolosos. O objetivo principal é consolidar dados históricos e recentes, calcular taxas de criminalidade por 100 mil habitantes e realizar a previsão do número de ocorrências por meio utilizado, utilizando o modelo SARIMA.

________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

O projeto utiliza três bases de dados principais, que devem estar disponíveis no mesmo diretório do notebook para execução:


CVLI_2009-2024.xlsx: Dados históricos de CVLI.


CVLI_2025.xlsx: Dados de CVLI referentes ao ano de 2025 (provisórios/projeções).


DADOS_IBGE.xlsx: Dados populacionais e socioeconômicos do IBGE, utilizados para o cálculo da taxa por 100 mil habitantes (incluindo a População Estimada para 2025).
_______________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

Para executar este projeto, você precisará ter o Python instalado, juntamente com as seguintes bibliotecas:

pandas
matplotlib
seaborn
numpy
openpyxl
statsmodels (para a modelagem SARIMA)

Você pode instalar as dependências via pip:
pip install pandas matplotlib seaborn openpyxl numpy statsmodels
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

Como Executar
Certifique-se de que os três arquivos de dados (CVLI_2009-2024.xlsx, CVLI_2025.xlsx, DADOS_IBGE.xlsx) estão no mesmo diretório do notebook Projeto.pynb.

Abra o notebook em um ambiente como Jupyter ou Google Colab.

Execute as células do notebook sequencialmente.
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

Resultados Chave (Exemplos)
Alguns insights gerados pela análise:

Município com maior volume de Homicídios por 100mil habitantes foi São João do Jaguaribe (2009-2025)

Outros Municípios de Destaque: Ibicuitinga, Quixeré e Guaiuba.

Previsão SARIMA (Exemplo - Arma de Fogo): O modelo prevê 251.0 ocorrências de crimes com arma de fogo para Outubro de 2025 e 242.0 para Novembro de 2025, indicando uma projeção para os próximos meses
