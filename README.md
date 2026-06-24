# Sistema de Inteligência Artificial para Predição de Risco de Evasão Acadêmica 

Este projeto foi desenvolvido como **Trabalho Final Prático** da disciplina de **Inteligência Artificial** do curso de Engenharia de Software da Universidade Católica de Brasília (UCB). 

O objetivo principal é analisar o comportamento de estudantes a partir de múltiplos fatores acadêmicos e institucionais para mapear padrões e predizer o risco de evasão escolar (Baixo, Médio ou Alto), utilizando duas abordagens distintas da IA: **Machine Learning (Árvore de Decisão)** e **Lógica Fuzzy**.

## 👥 Autores
* Joelma Giovanna B. F. Rocha
* Késia Silva Viana
* Luciana Liebl de Freitas
* Larissa Kailane Lima Vieira da Veiga
* **Professor:** William Roberto Malvezzi

---

## 📊 Estrutura dos Dados (`evasao_300_alunos.csv`)
O modelo consome uma base de dados em formato CSV contendo o registro de 300 alunos. As colunas avaliadas são:
* `Frequencia`: Percentual de presença nas aulas (0 a 100).
* `Nota`: Nota final obtida no semestre (0.0 a 10.0).
* `Participacao_AVA`: Índice de acessos e interações no Ambiente Virtual de Aprendizagem (0 a 100).
* `Atividades_Entregues`: Percentual de tarefas enviadas (0 a 100).
* `Reprovacoes`: Quantidade de reprovações acumuladas (0 a 4).
* `Atrasos`: Quantidade de atrasos ou mensalidades pendentes (0 a 10).
* `Risco_Evasao`: Classificação real do aluno (*Baixo*, *Médio* ou *Alto*).

---

## 🛠️ Pré-requisitos e Dependências

Para executar o notebook, você precisará do Python 3 instalado e das seguintes bibliotecas:

* `numpy`
* `pandas`
* `matplotlib`
* `scikit-learn`
* `scikit-fuzzy`

---

## 🚀 Como Executar o Projeto

Você pode rodar este projeto de duas formas: localmente (via Jupyter Notebook) ou de forma totalmente online no Google Colab.

### Opção 1: Executando no Google Colab (Recomendado)
1. Acesse o [Google Colab](https://colab.research.google.com/).
2. Faça o upload do arquivo `Lógica_Fuzzy_e_Machine_Learning_.ipynb`.
3. Execute a **Célula 1** para instalar automaticamente a biblioteca `scikit-fuzzy`.
4. Execute as células subsequentes. 
5. Na **Célula 3**, o código solicitará o arquivo de dados. Clique no botão de upload que aparecerá na tela e selecione o arquivo `evasao_300_alunos.csv`.

### Opção 2: Executando Localmente (PC)
1. Certifique-se de ter o Python instalado. Clone este repositório ou baixe os arquivos em uma pasta.
2. Abra o terminal na pasta do projeto e instale as dependências executando:
   ```bash
   pip install numpy pandas matplotlib scikit-learn scikit-fuzzy jupyter
3. Inicie o Jupyter Notebook com o comando:
      ```bash
      jupyter notebook
4. Abra o arquivo Lógica_Fuzzy_e_Machine_Learning_.ipynb
5. Como a célula de carregamento de dados (Célula 3) foi desenhada para a interface do Google Colab (from google.colab import files), se você estiver rodando localmente, altere a Célula 3 para ler o arquivo diretamente:
   # Substitua a Célula 3 por isso se rodar localmente:
import pandas as pd
df = pd.read_csv("evasao_300_alunos.csv")
df.columns = df.columns.str.strip()

6. Execute todas as células do menu Cell > Run All.
