# Análise Exploratória de Dados — Uber Ride Bookings 2024

## Descrição

Este projeto apresenta uma Análise Exploratória de Dados (AED) desenvolvida como atividade prática extra do curso **Introdução à Inteligência Artificial (IP 20h A)** do programa SCTEC/Carreira Tech do **SENAI SC LAB365**.

O dataset utilizado é o "Uber Ride Analytics Dashboard", disponibilizado publicamente no Kaggle, composto por 150.000 registros de corridas referentes ao ano de 2024. A análise busca compreender os padrões de utilização do serviço, variações temporais, comportamentos de cancelamento e métricas de avaliação, com vistas a identificar possíveis aplicações em modelos de Machine Learning.

---

## Estrutura do Projeto

```
desafio_extra_lab365_senai/
├── data/
│   └── ncr_ride_bookings.csv
├── docs/
│   └── enunciado_atividade.pdf
├── notebooks/
│   └── eda_ncr_ride_bookings.ipynb
├── visualizacoes/
│   └── *.png  (15 visualizações)
├── .gitignore
├── README.md
└── requirements.txt
```

---

## Etapas da Análise

1. **Setup e Imports** — configuração do ambiente, bibliotecas e caminhos
2. **Carregamento e Inspeção Inicial** — leitura do CSV, verificação de tipos, nulos e duplicatas
3. **Limpeza e Preparação dos Dados** — padronização snake_case, remoção de aspas em IDs
4. **Engenharia de Features** — criação de variáveis temporais, flags e métricas derivadas
5. **Análise Univariada — Variáveis Categóricas** — distribuição de status, veículos, pagamento e período
6. **Análise Univariada — Variáveis Numéricas** — estatísticas descritivas e distribuições
7. **Análise Temporal** — série semanal, padrões mensais, volume por hora e heatmap hora × dia
8. **Análise de Cancelamentos** — taxas por veículo, motivos e relação com VTAT
9. **Análise Bivariada** — scatter distância × valor, boxplots por veículo, heatmap de correlação
10. **Análise de Avaliações** — distribuições de ratings e comparativo por veículo
11. **Síntese dos Principais Insights** — consolidação dos 10 achados mais relevantes
12. **Possíveis Aplicações em Machine Learning** — classificação de booking_status e pré-processamento recomendado

---

## Tecnologias Utilizadas

- Python 3.x
- Pandas 2.3.1 · NumPy 2.3.2 · Matplotlib 3.10.5 · Seaborn 0.13.2
- Jupyter Lab 4.4.3

---

## Como Executar

1. Clone o repositório e instale as dependências:
```bash
git clone https://github.com/jhonatanalves/desafio_extra_lab365_senai.git
cd desafio_extra_lab365_senai
pip install -r requirements.txt
```

2. Execute o notebook:
```bash
jupyter notebook notebooks/eda_ncr_ride_bookings.ipynb
```

3. Rode todas as células em sequência: **Kernel → Restart & Run All**