# Desafio-Cientista-de-Dados
Conclusão do desafio indicium


Projeto de Previsão de Nota IMDB com Random Forest
Este projeto utiliza um notebook Jupyter (LH_CD_Felipe_Zambelli (1).ipynb) para analisar, processar e modelar dados de filmes. O objetivo principal é treinar um modelo de Machine Learning (Random Forest Regressor) capaz de prever a nota do IMDB de um filme com base em seus dados.

O notebook carrega um conjunto de dados brutos (df_final.csv), realiza o pré-processamento necessário, treina o modelo e avalia seu desempenho usando a métrica RMSE (Root Mean Squared Error). Ao final da execução, o modelo treinado é salvo no arquivo random_forest_imdb_model.pkl para uso futuro.

🚀 Como Executar o Projeto
Existem duas maneiras principais de executar este notebook:

Google Colab (Recomendado para facilidade de uso e ambiente pré-configurado).

Ambiente Local (Requer instalação manual das bibliotecas).

Opção 1: Execução no Google Colab (Recomendado)
O Google Colab é a maneira mais simples de executar este projeto, pois já inclui a maioria das bibliotecas de ciência de dados pré-instaladas.

Passos:

Acesse https://colab.research.google.com/.

Faça o upload do notebook: Vá em Arquivo > Fazer upload do notebook... e selecione o arquivo LH_CD_Felipe_Zambelli (1).ipynb.

Importante: Faça o upload dos dados de entrada. O notebook precisa do arquivo df_final.csv para funcionar.

No painel esquerdo do Colab, clique no ícone de pasta (📁).

Clique no ícone "Fazer upload" (uma página com uma seta para cima) e selecione o seu arquivo df_final.csv.

(Nota: O arquivo desaparecerá quando a sessão do Colab for encerrada. Você precisará carregá-lo novamente a cada nova sessão.)

Execute o notebook: Clique em Ambiente de execução > Executar tudo para rodar todas as células do notebook sequencialmente. O notebook irá ler o df_final.csv, processá-lo e treinar o modelo.

Opção 2: Instalação e Execução em Ambiente Local
Para executar o projeto em seu próprio computador, você precisará ter o Python 3 e o gerenciador de pacotes pip instalados.

1. Pré-requisitos (Arquivos)
Certifique-se de que os seguintes arquivos estejam no mesmo diretório (pasta) do projeto:

LH_CD_Felipe_Zambelli (1).ipynb (O notebook principal)

df_final.csv (O conjunto de dados brutos de entrada)

2. Configuração do Ambiente (Recomendado)
É uma boa prática criar um ambiente virtual (venv) para isolar as dependências do projeto:

Bash

# Crie um ambiente virtual chamado 'venv'
python -m venv venv

# Ative o ambiente
# No Windows (PowerShell/CMD):
.\venv\Scripts\activate

# No macOS/Linux:
source venv/bin/activate
3. Instalação das Dependências
O projeto depende de várias bibliotecas Python. Crie um arquivo chamado requirements.txt na pasta do projeto com o seguinte conteúdo:

requirements.txt:

Plaintext

pandas
numpy
scikit-learn
matplotlib
seaborn
wordcloud
scipy
jupyterlab
spacy
Em seguida, instale todas elas de uma vez usando o pip (com o seu ambiente virtual ativado):

Bash

pip install -r requirements.txt
4. Baixar o Modelo de Linguagem spaCy
O notebook utiliza a biblioteca spacy. Você precisa baixar o modelo de linguagem em inglês necessário para que ela funcione:

Bash

python -m spacy download en_core_web_sm
5. Executando o Jupyter
Após a instalação de todas as dependências, inicie o Jupyter Lab (ou Jupyter Notebook) no seu terminal:

Bash

jupyter lab
Seu navegador padrão será aberto. Na interface do Jupyter, clique no arquivo LH_CD_Felipe_Zambelli (1).ipynb para abri-lo e executar as células.
