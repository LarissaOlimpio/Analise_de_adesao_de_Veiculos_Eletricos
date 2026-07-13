# Análise de Adoção de Veículos Elétricos (EV Population Data)

## Sobre o projeto
Análise exploratória e modelagem de dados sobre a adoção de veículos elétricos, 
usando dataset público [nome/fonte do dataset]. Projeto de portfólio aplicando 
Python/Pandas (limpeza), SQL (modelagem e queries analíticas) e Power BI (dashboard).

## Ferramentas utilizadas
- Python (Pandas) — exploração e limpeza de dados
- SQL — modelagem relacional (Star Schema) e queries analíticas
- Power BI — dashboard e visualização

## Etapas do projeto
1. Exploração inicial dos dados
2. Limpeza e tratamento de dados
3. Modelagem em Star Schema (SQL)
4. Análises e queries de negócio
5. Dashboard Power BI

## Decisões de tratamento de dados
- **Coluna `Base MSRP`**: ~98% dos valores são 0, indicando dado não coletado 
  em vez de preço real. Excluída do escopo de análise.
- **Coluna `Electric Range`**: valores 0 concentrados exclusivamente em 
  veículos 100% elétricos (BEV), o que é logicamente inconsistente — tratado 
  como dado ausente, não autonomia real. Excluída do escopo de análise / 
  ocultada no dashboard.
- **Linhas removidas (5 registros)**: correspondiam a endereços fora da 
  cobertura geográfica dos EUA (Colúmbia Britânica - Canadá; endereços 
  militares no exterior), sem preenchimento possível nas colunas de 
  localização americana (condado, CEP, tract censitário).

## Notebook
- [Exploração e Limpeza](notebook/data_exploration_and _cleaning/data_analysis.ipynb)

## Principais insights (em andamento)
- (a preencher conforme as queries SQL forem feitas)

## Dashboard
- (prints/gif do Power BI aqui, quando pronto)
