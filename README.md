# 📊 Análise e Previsão de Gastos da Cota Parlamentar

## 📄 Descrição do Projeto
Este projeto em **Python** tem como objetivo realizar uma análise completa dos gastos da **Cota para o Exercício da Atividade Parlamentar dos Senadores (CEAPS)**.  
O processo envolve:

- **Coleta de dados** de múltiplos arquivos.  
- **Limpeza e padronização** das informações com a biblioteca **Pandas**.  
- **Criação de visualizações interativas** para insights com **Plotly Express**.  
- **Previsão de tendências futuras** de gastos usando a biblioteca **Prophet**.  

O propósito é transformar dados brutos em um **relatório visual e dinâmico**, revelando padrões de despesa, comparando o uso da cota entre diferentes anos e senadores, e projetando o comportamento dos gastos para os próximos **90 dias**.

---

## 🚀 Tecnologias Utilizadas
- **Python** – Linguagem de programação principal.
- **Pandas** – Manipulação, limpeza e análise de dados.
- **NumPy** – Operações numéricas de alto desempenho.
- **Plotly Express** – Gráficos interativos e visualizações estatísticas.
- **Prophet** – Modelagem de séries temporais e previsão de gastos.

---

## ⚙️ Estrutura e Funcionalidades

### 1. Coleta e Limpeza de Dados
- **Consolidação de Dados**: Combina diversos arquivos CSV de gastos de diferentes anos em um único DataFrame.
- **Preenchimento de Nulos**: Trata valores ausentes em colunas como `DETALHAMENTO` e `DOCUMENTO`.
- **Padronização de Dados**: Converte colunas de data/mês para formatos adequados e transforma valores para tipo numérico.

### 2. Análise Exploratória e Visualizações
- **Gasto Anual Total**: Gráfico de barras por ano fiscal.
- **Top 10 Senadores por Gasto**: Gráfico de barras horizontais com os maiores gastos por senador.
- **Distribuição por Tipo de Despesa**: Treemap mostrando proporções por categoria.
- **Evolução Mensal (Top 3)**: Gráficos de linha para os três senadores com maiores despesas.

### 3. Previsão de Gastos com Prophet
- Modelo treinado com dados históricos diários.
- Projeção para os próximos 90 dias com `yhat`, `yhat_upper` e `yhat_lower`.
- Resultados salvos em `previsao_gastos_ceaps.csv`.
- Gráficos interativos detalhando tendência e sazonalidade.

---

## 📈 Conclusões e Insights
- **Variação Anual e Mensal**: Identificação de flutuações ao longo dos anos e meses.
- **Foco das Despesas**: Destaque das categorias mais significativas de gasto.
- **Disparidade de Gastos**: Diferença considerável entre senadores no uso da cota.
- **Tendências Futuras**: Possibilidade de antecipar o comportamento dos gastos para planejamento.

---

## ⚙️ Como Executar o Projeto

Estrutura de pastas esperada:
```
└── Dados/
├── despesa_ceaps_2018.csv
├── despesa_ceaps_2019.csv
├── despesa_ceaps_2020.csv
├── despesa_ceaps_2021.csv
└── dataset_ceaps_forecasting.csv
```
## Passos:
1. Coloque todos os arquivos de dados na pasta `Dados/`.
2. Execute o script Python principal.
3. O código irá:
   - Processar e limpar os dados.
   - Gerar as visualizações interativas.
   - Salvar o arquivo `previsao_gastos_ceaps.csv` com a projeção.
