# 📊 Case Técnico de Data Analysis – iFood  
**Análise de Teste A/B de Cupons**  
Autor: **Caio Santos**

---

## 📌 Visão Geral

Este repositório contém a solução para o Case Técnico de Data Analysis do iFood.  
O objetivo é avaliar o impacto de uma estratégia de cupons por meio de um teste A/B, analisar sua viabilidade financeira, explorar heterogeneidades por cidade e segmento de usuários e propor recomendações estratégicas baseadas em dados.

A solução foi estruturada para simular um cenário real de tomada de decisão orientada a dados, seguindo boas práticas de ETL, experimentação e comunicação executiva, conforme solicitado no enunciado do case.

---

## 🎯 Objetivos do Case

- Avaliar o impacto do cupom em métricas-chave de negócio  
- Validar estatisticamente os resultados do teste A/B  
- Analisar a viabilidade financeira da iniciativa  
- Explorar variações de efeito por cidade e segmento de usuários  
- Propor oportunidades de melhoria e um novo desenho de teste A/B  
- Comunicar resultados para uma audiência não técnica  

---

## 🗂 Estrutura do Repositório

- README.md  
- .gitignore  
- notebooks/  
  - 01_(Pipeline_ETL).ipynb  
  - 02_Analise.ipynb  
- reports/  
  - Relatorio_Analise_Cupom_iFood_Caio_Santos.pdf  

---

## 📘 Descrição dos Notebooks

### 01_(Pipeline_ETL).ipynb

Notebook responsável pelo processo de ingestão e preparação dos dados, incluindo:

- Download programático dos datasets conforme especificado no case  
- Descompactação de arquivos .gz e .tar.gz  
- Limpeza, tipagem e padronização dos dados  
- Estruturação dos dados para análise  
- Execução idempotente, permitindo reprocessamento seguro  

---

### 02_Analise.ipynb

Notebook contendo a análise principal do case, incluindo:

- Análise do Teste A/B (grupo controle vs. experimento)  
- Definição e avaliação das métricas de sucesso  
- Validação estatística dos resultados  
- Análise de viabilidade financeira (break-even)  
- Heterogeneidade de efeito por cidade  
- Segmentação de usuários  
- Recomendações estratégicas e proposta de novo teste A/B  

---

## ⚙️ Configuração do Caminho dos Dados

O diretório onde os dados são armazenados é definido nas primeiras células do notebook 01_(Pipeline_ETL).ipynb por meio de uma variável de configuração.

Exemplo padrão:

BASE_PATH = "./data"

Caso esteja executando no Google Colab, o caminho pode ser ajustado, por exemplo, para:

BASE_PATH = "/content/drive/MyDrive/ifood_case"

Importante: apenas esta variável precisa ser alterada. Nenhuma outra modificação no código é necessária para executar o projeto em ambientes diferentes.

---

## 📄 Relatório Executivo

O relatório final está disponível em:

reports/Relatorio_Analise_Cupom_iFood_Caio_Santos.pdf

O documento foi elaborado para lideranças de negócio, priorizando linguagem clara, visualizações acessíveis e insights acionáveis para tomada de decisão.

---

## 📦 Sobre os Dados

Os datasets originais não são versionados no GitHub devido ao grande volume de dados.  
O pipeline realiza o download, descompactação e processamento de forma programática, garantindo replicabilidade da análise.

---

## ▶️ Como Executar o Projeto

Execução recomendada via Google Colab:

1. Abrir os notebooks no Google Colab  
2. Ajustar a variável BASE_PATH, se necessário  
3. Executar o notebook 01_(Pipeline_ETL).ipynb  
4. Em seguida, executar o notebook 02_Analise.ipynb  

Execução local:

1. Clonar o repositório  
2. Executar os notebooks na mesma ordem descrita acima  

---

## 🧠 Considerações Finais

Este projeto foi estruturado como um entregável completo de análise de dados, com foco não apenas na mensuração de resultados, mas também na tomada de decisão estratégica, eficiência de investimento e clareza na comunicação com áreas de negócio.
