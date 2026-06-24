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

### Opção Recomendada: Executando no Google Colab (Recomendado)
1. Acesse o [Google Colab](https://colab.research.google.com/).
2. Faça o upload do arquivo `Lógica_Fuzzy_e_Machine_Learning_.ipynb`.
3. Execute a **Célula 1** para instalar automaticamente a biblioteca `scikit-fuzzy`.
4. Execute as células subsequentes. 
5. Na **Célula 3**, o código solicitará o arquivo de dados. Clique no botão de upload que aparecerá na tela e selecione o arquivo `evasao_300_alunos.csv`.

