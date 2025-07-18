
# 🎓 Predição de Conclusão de Curso de Graduação

Este projeto visa prever a probabilidade de um aluno de graduação concluir o curso no semestre seguinte, utilizando dados acadêmicos históricos da UFRN. Através de modelos de aprendizado de máquina supervisionado, o objetivo é identificar precocemente alunos em risco de evasão ou trancamento, permitindo intervenções e suporte personalizados.

---

## 🎯 Objetivos do Projeto

- **Antecipar a Conclusão:** Prever quando os alunos estão aptos a concluir o curso, otimizando o planejamento acadêmico.
- **Detectar Alunos em Risco:** Identificar estudantes com alta probabilidade de evasão ou trancamento.
- **Apoiar a Gestão Acadêmica:** Subsidiar decisões sobre oferta de disciplinas e alocação de recursos.
- **Oferecer Suporte Personalizado:** Direcionar programas de apoio para alunos com maior necessidade.

---

## 📊 Dados e Pré-processamento

- Fonte: Dados Abertos da UFRN.
- Curso: Engenharia Civil (ID: 2000025).
- Período: 2018.1 a 2024.2.
- Datasets: Situações Discentes e Matrículas em Componentes Curriculares.

### Principais Etapas:

- **Importação:** Coleta automática via URLs públicas.
- **Filtragem:** Seleção de colunas relevantes por curso e nível.
- **Tratamento:** Conversão de tipos e imputação de valores ausentes.
- **Feature Engineering:** Criação de variáveis como média de notas, total de faltas, disciplinas cursadas e razão faltas/disciplina.
- **Variável Alvo:** `vai_concluir_no_proximo` (binária).

---

## 📈 Análise Exploratória (EDA)

- Distribuição das situações acadêmicas por semestre.
- Evolução dos alunos concluintes.
- Boxplots de disciplinas cursadas e médias por semestre.
- Distribuição de faltas em relação à conclusão.

---

## 🤖 Modelos Utilizados

- **K-Nearest Neighbors (KNN):** Baseado em proximidade entre instâncias.
- **Árvore de Decisão:** Algoritmo interpretável baseado em regras hierárquicas.

### Features utilizadas:

- `media_notas`, `faltas_totais`, `qtd_disciplinas`, `razao_faltas_disciplinas`

### Avaliação:

- **Acurácia:** KNN (0.8887), Árvore de Decisão (0.8898)
- **Precision (Concluintes):** KNN (0.7638), Árvore (0.7413)
- **Recall (Concluintes):** KNN (0.3477), Árvore (0.3799)
- **F1-Score:** KNN (0.4778), Árvore (0.5024)

> A Árvore de Decisão apresentou melhor equilíbrio entre precisão e cobertura, sendo mais eficaz para detectar alunos que efetivamente concluirão o curso.

---

## ⚙️ Tecnologias Utilizadas

- Python
- Pandas, NumPy
- Scikit-learn, Imbalanced-learn
- Matplotlib, Seaborn
- Google Colab

---

## 🛠️ Próximos Passos

- Aplicar padronização com `StandardScaler`.
- Balancear as classes com `SMOTE`.
- Otimizar hiperparâmetros com `GridSearchCV`.
- Adicionar novos modelos e comparar desempenho.

---

## 🚀 Como Executar

1. Clone o repositório:
```bash
git clone https://github.com/deboraeverlyab/etl-predicao-ia.git
```

2. Acesse o notebook no [Google Colab](https://colab.research.google.com/) ou ambiente Jupyter.

3. Execute as células sequencialmente.

---

## 🤝 Como Contribuir

Contribuições são bem-vindas! Abra issues ou envie pull requests com sugestões e melhorias.

---

> ⚠️ Para mais detalhes, veja o notebook [`projeto3_final.ipynb`](./projeto3_final.ipynb)


## 📧 Contato

Débora Everly  
Engenheira de Dados | QA | IA  
[LinkedIn](https://www.linkedin.com/in/debora-everly/)



---
