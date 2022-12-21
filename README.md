# Detecção de anomalias
Códigos e experimentos para o desenvolvimento dos modelos de detecção de anomalias para o projeto de avaliação da qualidade de água, financiado pela CEMIG.

Especificamente para essa parte de detecção de anomalias, foi desenvolvido um artigo científico que assim que publicado, seu link será disponibilizado aqui. O repositório aqui presente faz referência ao artigo citado.

## Diretório 'codigos-datasets-experimentos-resultados'

Nesse diretório é possível encontrar todos os códigos implementados, datasets e experimentos realizados, além dos resultados obtidos, no que diz respeito ao desenvolvimento de um modelo de aprendizado de máquina usando a abordagem de detecção de anomalias.

A justificativa para o uso da abordagem de detecção de anomalias é pelo fato de que para o problema proposto de avaliação da qualidade da água, encontra-se um desbalanceamento claro entre os rótulos de água "boa" e água "ruim".

Cada subdiretório é nomeado por uma data de origem. No decorrer do projeto novos datasets foram obtidos e diferentes filtros de pré-processamento nos dados foram aplicados. Dessa forma, em cada um dos subdiretórios encontram-se diferentes arquivos com os dados e consequentemente os arquivos com extensão '.pynb' que armanezam as implementações em Python realizadas. Dentro dos arquivos '.pynb' situa-se os códigos, a metodologia dos experimentos bem como os resultados alcançados.

## Arquivo 'Demo_deteccao_anomalias.ipynb'

O arquivo 'Demo_deteccao_anomalias.ipynb' é um Jupyter Notebook que permite que qualquer pessoa possa fazer o treinamento e a inferência de dois modelos de aprendizado de máquina (SVM One Class e Florestas Isoladas) a partir de um dataset contendo amostras com 12 parâmetros (bandas) de entrada e sua respectiva classe binária.

O passo a passo para a execução do Jupyter Notebook é:

1) Carregamento das bibliotecas.
2) Carregamento do dataset.
3) Limpeza, pré-processamento e análise do dataset.
4) Divisão do dataset em subconjuntos de treino e teste.
5) Aplicação da técnica SMOTE para aumento de dados.
6) Padronização dos dados.
7) Definição dos parâmetros para o método SVM One Class.
8) Treinamento de diferentes modelos para variadas combinações de parâmetros empregando o método SVM One Class.
9) Avaliação e seleção do melhor modelo obtido para o método SVM One Class.
10) Definição dos parâmetros para o método Florestas Isoladas.
11) Treinamento de diferentes modelos para variadas combinações de parâmetros empregando o método Florestas Isoladas.
12) Avaliação e seleção do melhor modelo obtido para o método Florestas Isoladas.
13) Seleção do melhor modelo treinado dentre todas combinações de parâmetros e métodos de aprendizado de máquina avaliados.
14) Aplicação do teste estatístico de McNemar para verificação sobre a existência de diferença significativa entre os modelos de aprendizado treinados.
15) Carregamento do dataset (para esse caso contendo toda a represa de Três Marias, representado pelos pixels extraídos da imagem de satélite).
16) Inferência dos dados no melhor modelo obtido.
17) Geração do mapa.
18) Exportação do mapa em formato 'shapefile'.
