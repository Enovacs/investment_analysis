# Análise de Carteira de Investimentos — B3

## Objetivo
Analisar o desempenho histórico de uma carteira simulada com ações brasileiras (Itaú, Petrobras, Vale e WEG), comparando com o Ibovespa como benchmark, no período de janeiro/2022 a dezembro/2024.

## KPIs Analisados
- Preço médio, mínimo e máximo por ativo
- Retorno acumulado real no período
- Volatilidade anualizada
- Correlação entre ativos

## Principais Achados
- **Petrobras** liderou com +215% de retorno, mas foi o ativo mais volátil (33% a.a.)
- **Itaú** apresentou o melhor equilíbrio risco/retorno (+67%, volatilidade de 23%)
- **Vale** foi o único ativo com retorno negativo (-8%) no período
- Todos os ativos da carteira superaram o Ibovespa (+14%), exceto a Vale

## Ferramentas Utilizadas
- Python (yfinance, pandas, matplotlib, seaborn)
- PostgreSQL (armazenamento e consultas SQL)
- SQLAlchemy + psycopg2 (integração Python ↔ PostgreSQL)
- Jupyter Notebook

## Estrutura do Projeto
portfolio-investimentos/
├── notebooks/
│   └── portfolio_analysis.ipynb
├── images/
└── README.md

## Como Reproduzir
Os dados são coletados automaticamente via `yfinance` ao executar o notebook. É necessário ter o PostgreSQL instalado e criar o banco `portfolio_investimento` antes de rodar.

## Próximos Passos
- Calcular o Índice de Sharpe por ativo
- Implementar otimização de carteira via Fronteira Eficiente de Markowitz
- Expandir a análise para todos os ativos da B3 por setor