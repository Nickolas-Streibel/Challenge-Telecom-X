# 📡 Telecom X – Análise de Evasão de Clientes (Churn)

![Status](https://img.shields.io/badge/status-concluído-brightgreen)  
![Python](https://img.shields.io/badge/python-3.11-blue)  
![Jupyter Notebook](https://img.shields.io/badge/jupyter-notebook-orange)

---

## 📌 Sobre

Este repositório reúne a análise exploratória de dados (EDA) da **Telecom X**, focada em entender e reduzir a **evasão de clientes** (churn). Nossa meta foi identificar quando, quem e por quê os clientes cancelam, gerando insights e recomendações estratégicas para melhorar retenção.

---

## 🎯 Objetivos

- Importar, limpar e tratar dados de mais de 7 000 clientes  
- Explorar padrões de churn em relação a tempo de contrato, gastos, serviços contratados e perfil demográfico  
- Apresentar visualizações claras para facilitar a tomada de decisão  
- Sugerir ações práticas para reduzir a evasão

---

## 🔗 Fonte dos Dados

- **TelecomX_Data.json** – arquivo hospedado no GitHub (raw).  
  ```text
  https://raw.githubusercontent.com/ingridcristh/challenge2-data-science/main/TelecomX_Data.json
  
---

## ⚙️ Tecnologias e Bibliotecas

- **Python 3.11**  
- **Jupyter Notebook**  
- `pandas` – manipulação de dados  
- `matplotlib` – visualização de dados  
- `seaborn` – visualização estatística  
- `plotly` – gráficos interativos (opcional)

---

## 📊 Etapas da Análise

### 🔧 1. Limpeza e Tratamento de Dados
- Leitura e transformação do JSON aninhado com `pd.json_normalize`
- Padronização dos nomes das colunas 
- Conversão de variáveis categóricas ('Yes'/'No') para binárias (`1` e `0`)
- Conversão de colunas numéricas que estavam como texto
- Criação de métricas auxiliares:
- **contas_diarias** = `gastos_totais` / `tempo_contrato_meses`
- **num_services** = total de serviços adicionais contratados

### 📊 2. Análise Exploratória de Dados (EDA)
- Distribuição geral da evasão (churn)
- Relação entre:
  - Tempo de contrato × Evasão
  - Gastos mensais, totais e diários × Evasão
  - Tipo de contrato × Evasão
  - Método de pagamento × Evasão
  - Tipo de internet × Evasão
  - Quantidade de serviços contratados × Evasão
  - Avaliação de perfil demográfico (idade, parceiro, dependentes)
  - Análise de correlação entre variáveis numéricas

### 🔍 3. Principais Descobertas
- **Taxa de evasão geral:** 26,6%
- **Tempo de contrato:** 47,7% da evasão ocorre nos primeiros 12 meses
- **Contratos:** Clientes com contratos mensais têm churn de 42,7%; contratos de 1 ano caem para 11,3% e de 2 anos, para 2,9%
- **Serviços de internet:** Fibra óptica apresenta maior churn (41,9%) do que DSL
- **Método de pagamento:** Cheque eletrônico é o método com maior churn (45,3%)
- **Serviços adicionais:** Clientes sem suporte técnico, segurança online, backup ou proteção no dispositivo têm taxas de evasão superiores
- **Perfil demográfico:** Clientes idosos e sem dependentes ou parceiros possuem maior probabilidade de churn

### 🚀 4. Recomendações
- Implantar **programas de retenção** focados nos primeiros 12 meses
- Incentivar migração de contratos mensais para anuais/bianuais
- Rever qualidade e atendimento da fibra óptica
- Melhorar comunicação e adesão dos serviços extras (backup, segurança, suporte)
- Avaliar processos do método de pagamento por cheque eletrônico
- Criar campanhas específicas para perfis de maior risco (idosos, sem parceiros, sem dependentes)

---

## 📈 Visualizações Destacadas

- 📊 Gráficos de barras para churn por contrato, método de pagamento e serviços
- 📈 Gráficos de dispersão para churn versus gastos e tempo
- 📦 Boxplots para distribuição do tempo de contrato por churn
- 🔥 Heatmap de correlação entre variáveis numéricas

---


## 🧠 Aprendizados

- Estruturação de dados JSON aninhados

- Análise exploratória profunda para problemas de churn

- Criação de variáveis derivadas relevantes para negócio

- Visualização de dados para tomada de decisão

- Geração de insights claros e acionáveis

---

## 📬 Contato

Se quiser tirar dúvidas ou conversar sobre este projeto, me envie um e-mail:
✉️ nickolasstreibel@gmail.com

---

## 👨‍💻 Autor
<img src="https://avatars.githubusercontent.com/u/195215720?s=400" width=100><br><sub>Nickolas Streibel</sub>
