<p align="center">
 <img width="1050" height="320" alt="Capa_README_Tiamat" src="https://github.com/user-attachments/assets/989916a5-d8bf-4c71-8779-4d9f3f027b05" />
</p>

<h1 align="center">Criatura Lendária: Tiamat (Entrega Final)</h1>
Projeto final da disciplina de Aprendizado de Máquina- 2º Semestre de 2026 | Ilum Escola de Ciência (CNPEM)

---

### **Descrição**
Este trabalho propôs realizar uma classificação binária da citotoxicidade (`Toxicity`) de experimentos com nanopartículas de óxidos metálicos, a partir de propriedades físico-químicas e das condições do ensaio, utilizando estratégias de *Machine Learning*. Comparamos um baseline (Dummy e Regressão Logística) com Random Forest, XGBoost e SVM, cada um com 100 tentativas de hiperparâmetros no Optuna, usando divisão treino/teste e validação cruzada agrupadas **por material** para evitar vazamento de dados.

**Objetivo:** Comparar um baseline e três algoritmos (Random Forest, XGBoost e SVM), cada um com 100 conjuntos de hiperparâmetros testados pelo Optuna, em um problema de **classificação binária** (`Toxicity`).
**Dados:** Conjunto de dados *HaHa-Manual*, com dados de toxicidade extraídos manualmente da literatura (Ha e Ha, 2025), sendo estes dados experimentais reais, não sintéticos.

#### **Estrutura**
- `Entrega_2_Criatura_Tiamat.ipynb`: notebook do projeto com relatório e código completos (EDA, modelagem, comparação, explicação).
- `HaHa-Manual.csv`: dataset (ver "Como baixar os arquivos"). Deve ficar na mesma pasta do notebook.
`requirements.txt`: requisitos para execução do notebook.

#### **Como baixar os arquivos**
1. **Notebook:** baixe `Entrega_2_Criatura_Tiamat.ipynb` deste repositório;
2. **Dados:** baixe `HaHa-Manual.csv` no Zenodo: https://zenodo.org/records/15385143/files/HaHa-Manual.csv?download=1
3. Coloque os dois arquivos **na mesma pasta**, abra e rode o notebook a partir dela.

*Obs:* Se o CSV não estiver na pasta, o notebook tenta baixá-lo automaticamente do Zenodo na primeira execução.

### **Módulos Utilizados**
- **numpy e pandas**: manipulação numérica e de tabelas.
- **matplotlib e seaborn**: gráficos.
- **scikit-learn**: pré-processamento (ColumnTransformer, Pipeline, StandardScaler, OneHotEncoder, SimpleImputer), divisão e validação cruzada agrupadas (GroupShuffleSplit, StratifiedGroupKFold), modelos (DummyClassifier, LogisticRegression, RandomForestClassifier, SVC), métricas e importância por permutação.
- **xgboost**: classificador XGBoost.
- **optuna**: otimização de hiperparâmetros.
- **jupyter**: ambiente de execução do notebook.
- **os e warnings** (biblioteca padrão do Python): caminhos de arquivo e controle de avisos.

---

## Professor
### Daniel Roberto Cassar
Doutorado: Ciência e Engenharia de Materiais (UFSCar) – Pós-doutorado: UFSCar. Área de atuação: Informática de materiais.

---

## Autoria
### Angelica Aracava Lopes
Técnica em Biotecnologia e estudante de Ciência e Tecnologia na Ilum Escola de Ciência.

---

## Referências

- Ha, E.; Ha, S. *Structured Nanotoxicity Datasets with Physicochemical and Toxicological Attributes of Metal Oxide Nanoparticles* (HaHa-Manual). Zenodo, 2025. https://zenodo.org/records/15385143 (licença CC-BY-4.0).
- Akiba, T. et al. Optuna: A Next-generation Hyperparameter Optimization Framework. *KDD*, 2019.
- Chen, T.; Guestrin, C. XGBoost: A Scalable Tree Boosting System. *KDD*, 2016.
- Pedregosa, F. et al. Scikit-learn: Machine Learning in Python. *JMLR* 12, 2825–2830, 2011.
  
---

*Este projeto foi desenvolvido com o auxílio de IA generativa (Claude) para esclarecimento de dúvidas, ajustes no projeto e organização de fontes.*
