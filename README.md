# 📂 Projeto Telecom X – Predição de Churn

Este repositório contém a segunda parte do desafio **Telecom X**, com foco em **modelagem preditiva e análises de churn (evasão de clientes)**.  
O projeto foi estruturado em **três notebooks principais**, cada um correspondendo a uma etapa do fluxo de Data Science.

---

## 🗂 Estrutura do Projeto

### 1. [01_Preparacao_Dados.ipynb](01_Preparacao_Dados.ipynb)
🔹 Objetivo: preparar o dataset final para uso em modelos de Machine Learning.  
🔹 Principais etapas:
- Carregamento do dataset tratado (proveniente da Parte 1 do desafio).  
- Diagnósticos finais de integridade e consistência.  
- Encoding e normalização das variáveis.  
- Remoção de colunas irrelevantes.  
- Separação em treino e teste.  
- Exportação do dataset pronto para a modelagem.  

---

### 2. [02_Modelagem_TelecomX.ipynb](02_Modelagem_TelecomX.ipynb)
🔹 Objetivo: treinamento, avaliação e seleção do modelo preditivo.  
🔹 Principais etapas:
- Carregamento do dataset preparado.  
- Definição do target (`Evasao`) e variáveis preditoras.  
- Construção de **pipelines de Machine Learning** com:
  - pré-processamento,
  - balanceamento com **SMOTE** (aplicado somente no treino),
  - múltiplos algoritmos de classificação (Logistic Regression, Random Forest, KNN etc.).  
- Avaliação dos modelos com métricas (F1, Precisão, Recall, ROC-AUC).  
- Exportação do **melhor pipeline** para uso no Notebook 3.  

---

### 3. [03_Analises_TelecomX.ipynb](03_Analises_TelecomX.ipynb)
🔹 Objetivo: análise final dos resultados e geração de recomendações estratégicas.  
🔹 Principais etapas:
- Carregamento do modelo final exportado no Notebook 2.  
- Avaliação do desempenho no conjunto de teste (matriz de confusão, métricas executivas).  
- Análise de **Permutation Importance** e coeficientes para identificar os fatores mais relevantes para churn.  
- Construção da **Tabela Executiva de Drivers**, com interpretação de negócio para cada variável.  
- Geração de **recomendações de retenção** alinhadas aos fatores identificados.  
- Conclusão estratégica sobre o problema de churn e próximos passos sugeridos.  

---

## 📊 Principais Insights

- **Drivers de risco**: cobrança mensal/diária, fatura digital e pacotes de streaming (TV/Filmes) aumentam a probabilidade de evasão.  
- **Drivers de retenção**: ter telefone fixo, serviços adicionais como backup online, suporte técnico e dependentes/parceiro(a) reduzem o risco de churn.  
- **Estratégias recomendadas**:
  - Incentivar migração para contratos de maior prazo.  
  - Oferecer benefícios segmentados para clientes com alto risco.  
  - Melhorar a experiência de suporte.  
  - Promover planos familiares e pacotes de valor agregado.  

---

## 🚀 Como Executar
1. Clone este repositório.  
2. Abra os notebooks na ordem:
   - `01_Preparacao_Dados.ipynb`
   - `02_Modelagem_TelecomX.ipynb`
   - `03_Analises_TelecomX.ipynb`
3. Execute célula a célula para reproduzir o fluxo completo de preparação → modelagem → análises.  

---

## 📌 Conclusão
O projeto demonstra o uso de **Machine Learning aplicado a churn**, unindo:
- **Pipeline completo** (pré-processamento, balanceamento e modelagem).  
- **Explicabilidade** (Permutation Importance, coeficientes).  
- **Tradução em ações de negócio** (estratégias de retenção).

Este material pode ser usado como referência para **projetos reais de Data Science** voltados à redução de churn e aumento da fidelização de clientes.
