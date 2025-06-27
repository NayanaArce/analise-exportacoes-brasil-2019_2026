# 📄 Documentação Resumida

## 1. Coleta de Dados

Os dados utilizados foram obtidos da base oficial do **ComexStat**, plataforma do Governo Federal do Brasil que reúne dados sobre exportações e importações.

- Período: Janeiro de 2019 a Dezembro de 2024
- Origem: [https://comexstat.mdic.gov.br](https://comexstat.mdic.gov.br)
- Formato: CSV
- Campos principais: País, Produto (Descrição SH2), Valor FOB (US$), Peso (kg), Ano

O dataset original foi tratado e padronizado na etapa de pré-processamento.



## 2. Modelagem

Foram aplicadas técnicas de **análise exploratória de dados (EDA)** e **regressão supervisionada** para prever o valor das exportações brasileiras em 2026.

### Etapas de modelagem:
- Limpeza e normalização dos dados
- Engenharia de variáveis:
  - Valor por quilograma
  - Lags temporais (valor lag1 e lag2)
  - Crescimento percentual
- Codificação de variáveis categóricas (país e produto)
- Modelos testados:
  - Random Forest Regressor
  - Gradient Boosting
  - Regressão Linear
  - Decision Tree

### Melhor modelo:
- **Decision Tree**
- Métrica: R² ≈ 0.9763

---

## 3. Conclusões

- O valor total exportado entre 2019 e 2024 foi superior a US$ 1 trilhão.
- Os principais países exportadores foram China, EUA e Argentina.
- Os produtos mais exportados incluem commodities agropecuárias e minerais.
- A previsão para 2026 indica um crescimento total de **+17,10%** em relação a 2024.
- A análise permitiu identificar oportunidades estratégicas em produtos com maior valor agregado por quilograma e mercados com crescimento constante.

O resultado final pode ser consultado no dashboard interativo:

🔗 [Dashboard Looker Studio](https://lookerstudio.google.com/reporting/66f8cc76-a4c8-464d-adee-08688095e3fe)
