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

---

## ⚙️ Metodologia
- Software: **Weka 3.8**
- Algoritmo: **J48 (Árvore de Decisão)**
- Classe alvo: **Survived (0 = não sobreviveu, 1 = sobreviveu)**
- Atributos utilizados:
  - **Passengerld (Classificação do passageiro)**
  - **Pclass (classe do passageiro)**
  - **Sex (Sexo)**
  - **Age (Idade)**
  - **SibSp (nº de irmãos/cônjuges a bordo)**
  - **Parch (nº de pais/filhos a bordo)**
  - **Fare (tarifa/preço da viagem)**
  - **Embarked (porto de embarque)**

---

## 🌳 Árvore gerada (J48)

![Image](https://github.com/user-attachments/assets/ced5231b-37e3-44f4-820b-cfb0c9ba7dd6)

📌 **Interpretação**:
- Passageiros **homens** → maioria não sobreviveu.
- Passageiras **mulheres** → maioria sobreviveu, especialmente nas classes **1ª e 2ª**.
- Na **3ª classe**, o porto de embarque fez diferença:
  - Southampton → maioria não sobreviveu.
  - Cherbourg/Queenstown → maior chance de sobrevivência.

**Avaliação do Modelo J48**

![Image](https://github.com/user-attachments/assets/6df8a4bb-7fa6-445b-91fe-058c555ffaf8)

📌 **Interpretação**:
- O modelo tem **79% de acurácia geral (desempenho estimado no train.csv)**, com desempenho melhor em prever quem **não sobreviveu** (classe 0).
- A matriz de confusão mostra que **132 sobreviventes foram classificados como não sobreviventes**.

---

## Envio para o Kaggle

Após gerar o arquivo final_submission.csv, a previsão foi enviada para o Kaggle. A plataforma compara o arquivo com os resultados reais do conjunto de teste e retorna uma **acurácia**, que indica a porcentagem de previsões corretas.

O modelo obteve cerca de **77% de acurácia**. Esse envio permite avaliar a performance do modelo em dados que ele nunca viu durante o treinamento.

### Observação sobre o arquivo final_submission.csv

O arquivo final_submission.csv está incluído dentro da **pasta zipada** disponível no repositório. Para acessá-lo, basta **baixar e descompactar a pasta**.

---
## 📈 Resultados finais

- **Acurácia no WEKA:** 79%
- **Pontuação no Kaggle**: 77%

| Avaliação                   | Acurácia |
|------------------------------|----------|
| WEKA (Cross-validation)      | ~79%     |
| Kaggle (test.csv - submissão)| 77%      |


Isso mostra que o modelo usado conseguiu generalizar bem, já que o desempenho no Kaggle ficou bem próximo ao observado durante o treinamento.

📌 Observações
- O atributo **Sex** foi o mais decisivo no modelo.
