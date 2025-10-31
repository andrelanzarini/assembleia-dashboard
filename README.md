# assembleia-dashboard
Dashboard interativo que apresenta despesas da Assembleia Legislativa do Paraná.

1. Objetivo do projeto
 - Construir um dashboard interativo e público que apresente, de forma clara e acessível:
 - Despesas parlamentares (por deputado, gabinete, natureza da despesa, etc.);
 - Despesas com pessoal (ativos, comissionados, aposentados);
 - Contratos e licitações (valores, fornecedores, prazos, modalidades);
 - Comparativos históricos e gráficos para análise orçamentária.

assembleia-dashboard/
│
├── data/                     # Dados brutos e tratados
│   ├── despesas.csv
│   ├── contratos.csv
│   ├── pessoal.csv
│   └── licitacoes.csv
│
├── src/
│   ├── main.py               # Ponto de entrada Streamlit
│   ├── pages/
│   │   ├── despesas.py
│   │   ├── contratos.py
│   │   ├── pessoal.py
│   │   └── licitacoes.py
│   ├── utils/
│   │   ├── loaders.py        # Funções de carga e atualização de dados
│   │   └── charts.py         # Geração de gráficos e análises
│
├── requirements.txt
├── README.md
└── .streamlit/
    └── config.toml           # Tema, layout e modo wide


Layout do Dashboard

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

