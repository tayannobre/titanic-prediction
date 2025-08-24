# titanic-prediction
Classificação da sobrevivência do Titanic usando o software Weka.
# Titanic Survival Prediction

Projeto de classificação da sobrevivência dos passageiros do Titanic usando **Weka** e o algoritmo **J48 (árvore de decisão)**.

---

## 📝 Descrição do Projeto

O objetivo deste projeto é **prever a sobrevivência dos passageiros do Titanic** com base em características como idade, sexo, classe, tarifa e familiares a bordo.  
O modelo foi construído utilizando **Weka**, aplicando o classificador **J48** para gerar uma árvore de decisão interpretável.

O projeto permite analisar a importância de cada atributo e entender regras simples que impactam a sobrevivência.

---

## 📂 Estrutura do Projeto

Perfeito! Então podemos simplificar o README para focar apenas no J48, mantendo ele limpo e profissional. Aqui está a versão ajustada:

# Titanic Survival Prediction

Projeto de classificação da sobrevivência dos passageiros do Titanic usando **Weka** e o algoritmo **J48 (árvore de decisão)**.

---

## 📝 Descrição do Projeto

O objetivo deste projeto é **prever a sobrevivência dos passageiros do Titanic** com base em características como idade, sexo, classe, tarifa e familiares a bordo.  
O modelo foi construído utilizando **Weka**, aplicando o classificador **J48** para gerar uma árvore de decisão interpretável.

O projeto permite analisar a importância de cada atributo e entender regras simples que impactam a sobrevivência.

---

## 📂 Estrutura do Projeto

titanic-weka/ ├─ data/ │  ├─ train.csv       # Dados de treino │  └─ test.csv        # Dados de teste ├─ models/ │  └─ titanic.model   # Modelo treinado (opcional) ├─ README.md          # Este arquivo └─ .gitignore

---

## ⚙️ Como Rodar o Projeto

1. Abra o **Weka**.
2. Clique em **Explorer → Open file → data/train.csv** (ou .arff se convertido).
3. Configure o **class attribute** como `Survived`.
4. Selecione o classificador **J48** e clique em **Start**.
5. Analise:
   - Matriz de confusão
   - Precisão, recall e acurácia
   - Árvore de decisão gerada

> Para salvar o modelo treinado:
> 1. Clique em **More options → Save model**.
> 2. Salve em `models/titanic.model`.

---

## 📊 Resultados Esperados

- Acurácia aproximada: **74–78%**.
- Principais atributos influenciando a sobrevivência:
  - **Sex** (sexo)
  - **Pclass** (classe do passageiro)
  - **Fare** (tarifa)
  - **Age** (idade)
- Exemplo de regra da árvore de decisão:
  - Passageiros femininos da 1ª classe têm alta probabilidade de sobreviver.
  - Passageiros masculinos da 3ª classe têm alta probabilidade de não sobreviver.

---

## 🔗 Links Úteis

- [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic)
- [Documentação Weka](https://www.cs.waikato.ac.nz/ml/weka/)

---

## 🛠 Tecnologias Utilizadas

- [Weka](https://www.cs.waikato.ac.nz/ml/weka/)
- CSV / ARFF para armazenamento de dados
- GitHub para versionamento

---

## 📌 Conclusão

Este projeto demonstra **aprendizado de máquina supervisionado** utilizando árvores de decisão, mostrando como atributos simples podem gerar regras interpretáveis e fornecer insights sobre os fatores que influenciam a sobrevivência no Titanic.


---
