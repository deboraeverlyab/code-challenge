# Projeto de ETL e Predição com Modelos de IA

Este projeto tem como objetivo realizar a extração, transformação e carga (ETL) de dados educacionais, seguido da aplicação de algoritmos de Inteligência Artificial para prever a conclusão de curso por parte dos alunos.

O notebook foi desenvolvido no Google Colab e contém todas as etapas, desde a limpeza de dados até a comparação entre diferentes modelos preditivos, com foco em problemas de classificação desbalanceada.

---

## 📌 Etapas do Projeto

### 1. **ETL (Extração, Transformação e Carga)**
- Leitura e inspeção inicial dos dados.
- Tratamento de valores ausentes e inconsistências.
- Transformação de variáveis categóricas.
- Análise exploratória com visualizações.
- Preparação do dataset para modelagem.

### 2. **Modelagem Preditiva**
- Separação entre treino e teste.
- Treinamento de dois modelos:
  - K-Nearest Neighbors (KNN)
  - Árvore de Decisão (Decision Tree)
- Otimização de hiperparâmetros.
- Avaliação com métricas clássicas de classificação.

---

## 📈 Resultados

### **Comparação: KNN vs. Árvore de Decisão**

Após o processo de avaliação no conjunto de teste, os modelos apresentaram a seguinte performance:

- **Acurácia Geral**
  - KNN: `0.8887`
  - Árvore de Decisão: `0.8898`
  - *Conclusão*: Ambos classificam corretamente a maioria dos alunos.

- **Precision para "Concluintes" (classe minoritária)**
  - KNN: `0.7638`
  - Árvore de Decisão: `0.7413`
  - *Conclusão*: KNN é levemente mais preciso ao prever quem irá concluir.

- **Recall para "Concluintes"**
  - KNN: `0.3477`
  - Árvore de Decisão: `0.3799`
  - *Conclusão*: A Árvore de Decisão detecta um pouco mais dos que realmente concluem.

- **F1-score para "Concluintes"**
  - KNN: `0.4778`
  - Árvore de Decisão: `0.5024`
  - *Conclusão*: A Árvore de Decisão apresenta melhor equilíbrio entre precisão e cobertura.

Apesar da boa performance geral, os modelos ainda têm margem de melhoria no Recall da classe positiva, sinalizando a importância de explorar técnicas adicionais como oversampling ou algoritmos focados em desbalanceamento de classes.

> ⚠️ Para mais detalhes, veja o notebook [`projeto3_final.ipynb`](./projeto3_final.ipynb)

---
