# 📉 Análise de Evasão de Clientes em Telecomunicações

Este projeto tem como objetivo identificar os fatores que mais influenciam a evasão de clientes (churn) em uma empresa de telecomunicações, por meio da aplicação de técnicas de aprendizado de máquina. Com base nos resultados obtidos, são propostas estratégias de retenção para mitigar a saída de clientes e aumentar a fidelização.

---

## 📊 Objetivos

* Analisar o perfil dos clientes e os fatores relacionados à evasão.
* Aplicar e comparar modelos de machine learning para prever o churn.
* Avaliar o desempenho dos modelos com dados desbalanceados.
* Propor estratégias baseadas em dados para melhorar a retenção.

---

## 🔍 Etapas do Projeto

### 1. Pré-processamento

* Conversão de variáveis categóricas e binárias.
* Normalização das variáveis numéricas com `MinMaxScaler`.
* Divisão dos dados em treino e teste (70/30).

### 2. Análise Exploratória

* Visualizações com gráficos de correlação e boxplots.
* Análise de variáveis como tempo de contrato, tipo de internet, total gasto e serviços contratados, cruzando com evasão.

### 3. Modelagem

Modelos aplicados:

* **Regressão Logística**
* **Random Forest**

Os modelos foram treinados com **dados originais e desbalanceados**, para refletir a realidade do negócio.

---

## ✅ Conclusão

Com base na análise das variáveis e no desempenho dos modelos treinados, foi possível identificar os **principais fatores associados à evasão de clientes**:

### 🔍 Fatores com maior influência na evasão:

* **Contrato de curto prazo**: clientes com contratos mensais apresentaram maior probabilidade de evasão. Já contratos anuais ou bienais mostraram maior retenção.
* **Internet via fibra óptica**: usuários desse tipo de serviço tiveram maior índice de evasão.
* **Ausência de serviços adicionais**: clientes que **não utilizam** recursos como **suporte técnico, segurança online, backup e proteção de dispositivo** tendem a evadir com mais frequência.
* **Método de pagamento**: métodos como **cheque eletrônico** estiveram associados a maior evasão, enquanto **débito automático** e **boleto** apresentaram menor risco.
* **Cobrança mensal elevada**: faturas mais altas estiveram relacionadas a maiores taxas de saída.
* **Faturamento total menor**: clientes com **baixo valor total gasto** tendem a evadir, sugerindo menor engajamento ou tempo de permanência.

---

## 🤖 Avaliação dos Modelos

| Modelo              | Acurácia  | Recall (Classe 1 - Evadiu) |
| ------------------- | --------- | -------------------------- |
| Regressão Logística | 77,0%     | **81%**                    |
| Random Forest       | **77,9%** | 60%                        |

* A **Regressão Logística** destacou-se na detecção de clientes que evadiram, sendo eficaz para **identificar perfis em risco**.
* O **Random Forest** obteve **maior acurácia geral** e melhor equilíbrio entre as classes, mas com menor sensibilidade para prever a evasão.

---

## 📌 Estratégias de Retenção Recomendadas

Com base nos resultados obtidos, as seguintes ações são recomendadas:

1. **Incentivar contratos mais longos**, com fidelização e recompensas por permanência.
2. **Oferecer pacotes personalizados** com serviços adicionais (suporte técnico, segurança, backup), destacando seu valor agregado.
3. **Ajustar a precificação** para clientes com faturas elevadas, oferecendo descontos, bônus ou pacotes mais econômicos.
4. **Atuar com foco em novos clientes** com baixo gasto total, oferecendo onboarding eficiente, suporte inicial e campanhas de engajamento nos primeiros meses.
5. **Estimular métodos de pagamento mais estáveis**, como débito automático ou cartão de crédito recorrente.

---

## 🛠️ Tecnologias Utilizadas

* **Python**
* **Pandas, NumPy** – Manipulação de dados
* **Scikit-learn** – Modelagem e avaliação
* **Matplotlib, Seaborn** – Visualizações

---

## 📁 Estrutura do Projeto

```
├── data/                 # Dados originais e tratados
├── notebooks/            # Jupyter Notebooks com análises
├── models/               # Modelos treinados (opcional)
├── results/              # Gráficos e relatórios finais
└── README.md             # Este arquivo
```

---

## 👩‍💻 Autoria

Projeto desenvolvido por **Ana Raquel Silva de Oliveira Avendanha** como parte de seus estudos em **Ciência de Dados**.
