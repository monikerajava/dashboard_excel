# dashboard_excel
Dashboard de Vendas utilizando Excel

🎮 Xbox Game Pass — Dashboard de Vendas 2024
Dashboard interativo construído em Excel para análise de desempenho de vendas de assinaturas do Xbox Game Pass, cobrindo o período de Janeiro a Dezembro de 2024.
---
📋 Sobre o Projeto
Este projeto transforma dados brutos de assinaturas em visualizações claras e acionáveis, permitindo análise rápida de:
Distribuição de assinantes por plano (Core, Standard, Ultimate)
Receita total e ticket médio por assinante
Tipos de assinatura (Mensal, Trimestral, Anual)
Adoção de Season Passes (EA Play e Minecraft)
Evolução mensal da receita ao longo do ano
Taxa de renovação automática
---
📊 Dados Utilizados
Campo	Descrição
Subscriber ID	Identificador único do assinante
Name	Nome do assinante
Plan	Plano contratado: Core, Standard ou Ultimate
Start Date	Data de início da assinatura
Auto Renewal	Renovação automática habilitada (Yes/No)
Subscription Price	Preço base da assinatura (R$)
Subscription Type	Tipo: Monthly, Quarterly ou Annual
EA Play Season Pass	Adesão ao pass EA Play (Yes/No)
EA Play Season Pass Price	Preço do EA Play Pass (R$)
Minecraft Season Pass	Adesão ao Minecraft Pass (Yes/No)
Minecraft Season Pass Price	Preço do Minecraft Pass (R$)
Coupon Value	Valor de desconto aplicado (R$)
Total Value	Valor total pago pelo assinante (R$)
Total de registros: 295 assinantes  
Período: Jan/2024 – Dez/2024
---
📈 KPIs Destacados
Indicador	Valor
Total de Assinantes	295
Receita Total	R$ 7.633
Ticket Médio	R$ 25,87
Taxa de Renovação Automática	50,2%
Total de Descontos Aplicados	R$ 2.122
Adeptos EA Play Season Pass	98 (33%)
Adeptos Minecraft Season Pass	194 (66%)
---
🗂️ Estrutura do Arquivo Excel
O arquivo `Xbox_GamePass_Dashboard_Vendas_2024.xlsx` contém 3 abas:
Aba	Conteúdo
Dashboard	Painel visual principal com KPIs e gráficos
Cálculos	Tabelas pivot intermediárias que alimentam os gráficos
Bases	Base de dados completa e formatada (295 linhas)
---
📊 Visualizações do Dashboard
5 Cards de KPI — Assinantes, Receita, Ticket Médio, Renovação, Descontos
Gráfico de Colunas — Receita por Plano (Core / Standard / Ultimate)
Gráfico de Pizza — Distribuição de Assinantes por Plano
Gráfico de Linhas — Evolução Mensal da Receita (Jan–Dez 2024)
Gráfico de Barras — Receita por Tipo de Assinatura
Gráfico de Pizza — Adoção de Season Passes (EA Play vs Minecraft)
---
🚀 Como Reproduzir
Requisitos
Microsoft Excel 2016+ ou LibreOffice Calc 7+
Python 3.10+ com as bibliotecas: `pandas`, `openpyxl`
Passos
```bash
# 1. Clone o repositório
git clone https://github.com/monikerajava/dashboard_excel.git
cd xbox-dashboard-vendas

# 2. Instale as dependências Python (para re-gerar o arquivo)
pip install pandas openpyxl

# 3. Abra o dashboard diretamente
# Abra Xbox_GamePass_Dashboard_Vendas_2024.xlsx no Excel ou LibreOffice
```
Para re-gerar o dashboard via Python
```bash
python build_dashboard.py
```
---
🎨 Design
O dashboard utiliza a identidade visual do Xbox:
Verde Xbox `#107C10` — cor primária de destaque
Verde claro `#9BC848` — títulos e acentos
Teal/Mint `#2AE6B1` — bordas e destaques secundários
Fundo escuro `#0D1117` — background do painel
Fonte: Arial (compatível com Excel e LibreOffice)
---
📁 Estrutura do Repositório
```
xbox-dashboard-vendas/
├── README.md
├── Xbox_GamePass_Dashboard_Vendas_2024.xlsx   ← Dashboard completo
└── build_dashboard.py                          ← Script de geração (opcional)
```
---
📝 Licença
Projeto desenvolvido para fins educacionais — Desafio de Dashboard de Vendas.
