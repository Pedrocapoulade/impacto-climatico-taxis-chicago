Análise de Impacto Climático na Duração de Viagens de Táxi (Chicago)

Este projeto investiga a relação entre as condições meteorológicas e a performance do serviço de táxis na cidade de Chicago. O foco principal foi validar, através de métodos estatísticos, se fenómenos climáticos (como chuva) alteram de forma significativa a duração média das viagens entre pontos específicos da cidade.

Descrição do Projeto

Como analista de uma nova empresa de táxis que está a ser lançada em Chicago, foi necessário compreender os padrões de passageiros e o impacto de fatores externos na operação. A análise dividiu-se em duas frentes: identificação dos bairros com maior procura e a realização de testes de hipóteses sobre o impacto da chuva na duração das viagens.

Objetivos Principais

Identificação de Market Share: Analisar o volume de viagens por empresa de táxi.

Mapeamento de Destinos: Identificar os 10 principais bairros de destino em termos de volume de viagens.

Validação Estatística: Testar a hipótese de que a duração média das viagens do Loop para o Aeroporto Internacional O'Hare muda em sábados chuvosos.

Metodologia e Fluxo de Trabalho

O projeto foi executado através de uma abordagem híbrida entre extração de dados estruturados e análise estatística avançada:

Extração e Agregação (SQL): - Utilização de comandos SQL (Joins, Grupos e Filtros) para consolidar dados de viagens, bairros e condições climáticas a partir de um banco de dados relacional.

Cruzamento da tabela de logs de viagens com tabelas de eventos meteorológicos.

Análise Exploratória (Python): - Importação dos datasets extraídos para ambiente Jupyter Notebook.

Limpeza e formatação de tipos de dados.

Visualização gráfica da distribuição de destinos e volume por empresa.

Teste de Hipóteses:

Hipótese Nula (H0): A duração média das viagens do Loop para o Aeroporto Internacional O'Hare em sábados chuvosos é igual à duração em sábados ensolarados.

Hipótese Alternativa (H1): A duração média das viagens muda em sábados chuvosos.

Critério: Utilização do Teste T de Student para amostras independentes com nível de significância (alfa) de 5%.

Tecnologias e Ferramentas

SQL (PostgreSQL): Extração de dados complexos.

Python : Processamento e análise.

Pandas: Manipulação de estruturas de dados.

SciPy (stats): Aplicação de testes estatísticos de hipóteses.

Matplotlib & Seaborn: Geração de gráficos para análise de distribuição.

Conclusões e Resultados

Liderança de Mercado: Identificou-se que empresas específicas detêm a maioria do volume de viagens, correlacionando possivelmente com a frota disponível ou contratos corporativos.

Concentração Geográfica: Bairros como Loop e River North apresentam uma densidade de desembarque significativamente superior aos demais.

Resultado Estatístico: O teste de hipóteses revelou um valor-p (p-value) inferior ao nível de significância adotado. Portanto, a hipótese nula foi rejeitada, confirmando estatisticamente que o clima chuvoso impacta a duração média das viagens para o aeroporto.

Estrutura do Repositório

notebook_chicago_taxi.ipynb: Jupyter Notebook contendo a análise estatística completa.
