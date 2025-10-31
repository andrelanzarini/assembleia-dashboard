# assembleia-dashboard
Dashboard interativo que apresenta despesas da Assembleia Legislativa do Paraná.

1. Objetivo do projeto
 - Construir um dashboard interativo e público que apresente, de forma clara e acessível:
 - Despesas parlamentares (por deputado, gabinete, natureza da despesa, etc.);
 - Despesas com pessoal (ativos, comissionados, aposentados);
 - Contratos e licitações (valores, fornecedores, prazos, modalidades);
 - Comparativos históricos e gráficos para análise orçamentária.

<code>
assembleia-dashboard/
├── data/
│ └── despesas_pessoal_sample.csv
├── src/
│ ├── main.py
│ └── utils/
│ ├── loaders.py
│ └── charts.py
├── requirements.txt
├── README.md
└── .streamlit/config.toml
</code>

<h2>Layout do Dashboard</h2>

O menu lateral (sidebar) permitirá navegar entre as seções:
 - Despesas Parlamentares
 - Pessoal
 - Contratos
 - Licitações
 - Painel Comparativo

Cada página exibirá:
 - Filtros (ano, tipo de despesa, deputado, fornecedor, etc.)
 - Tabelas dinâmicas (st.dataframe com filtros e paginação)
 - Gráficos interativos (plotly.express ou altair)
 - Indicadores resumidos (st.metric com variação %)

