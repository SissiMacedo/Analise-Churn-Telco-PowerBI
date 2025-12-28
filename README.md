# Análise de Churn - Setor de Telecomunicações

Este projeto analisa o comportamento de cancelamento de clientes (Churn) para identificar padrões e prejuízos financeiros.

## 🛠️ Tecnologias e Ferramentas
* **Power BI**: Dashboards interativos.
* **Power Query**: Limpeza e transformação de dados (ETL).
* **DAX**: Cálculos de métricas de negócio.

## 📊 Principais Métricas Criadas
* **Taxa de Churn %**: `DIVIDE([Qtd Churn], [Total Clientes], 0)`
* **Receita Perdida**: `CALCULATE(SUM(Table[MonthlyCharges]), Table[Churn] = "Yes")`

## 📈 Conclusões
* Clientes com contrato mês a mês representam a grande maioria do churn, sugerindo a necessidade de incentivos para migração para planos anuais.
* Clientes de fibra óptica possuem maior taxa de evasão comparado ao DSL.
* O risco de cancelamento é drasticamente maior nos primeiros 6 meses, indicando que o processo de onboarding do cliente precisa de melhorias.
* A retenção aumenta significativamente após o 12º mês de contrato.

## Fonte de Dados
* Kaggle
