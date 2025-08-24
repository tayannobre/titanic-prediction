# Titanic Survival Prediction

Projeto de classificação da sobrevivência dos passageiros do Titanic usando **Weka** e o algoritmo **J48 (árvore de decisão)**.

---

## 📝 Descrição do Projeto

O objetivo deste projeto é **prever a sobrevivência dos passageiros do Titanic** com base em características como idade, sexo, classe, tarifa e familiares a bordo.  
O modelo foi construído utilizando **Weka**, aplicando o classificador **J48** para gerar uma árvore de decisão interpretável.

---
## 📊 Dados
- **train.csv** → usado para treinar o modelo.
- **test.csv** → usado para gerar as predições.
- Fonte: [Kaggle - Titanic Dataset](https://www.kaggle.com/c/titanic).

## ⚙️ Metodologia
- Software: **Weka 3.8**
- Algoritmo: **J48 (Árvore de Decisão)**
- Classe alvo: **Survived (0 = não sobreviveu, 1 = sobreviveu)**
- Atributos utilizados:
  - **Pclass (classe do passageiro)**
  - **Sex**
  - **Age**
  - **SibSp (nº de irmãos/cônjuges a bordo)**
  - **Parch (nº de pais/filhos a bordo)**
  - **Fare (tarifa/preço da viagem)**
  - **Embarked (porto de embarque)**
