# ☕ Análise de Dados de Vendas de Café - Estudo de Caso

Este projeto consiste em uma análise exploratória de dados (EDA) de transações de uma cafeteria fictícia. O objetivo é entender o comportamento do consumidor, identificar padrões de vendas e extrair insights para otimização do negócio.

O notebook abrange desde a extração dos dados (via API do Kaggle), limpeza, tradução de colunas/valores e visualização de dados.

## 📋 Sobre o Projeto

* **Autor:** Thiago Pereira Magalhães
* **Contexto:** Trabalho desenvolvido para a disciplina de Engenharia e Análise de DADOS (Turma 2025.2).
* **Status:** Concluído (Outubro/2025).

## 🛠 Tecnologias Utilizadas

O projeto foi desenvolvido em **Python** utilizando as seguintes bibliotecas:

* **[Pandas](https://pandas.pydata.org/):** Manipulação, limpeza e agregação de dados.
* **[Matplotlib](https://matplotlib.org/):** Criação de gráficos para visualização de dados.
* **[KaggleHub](https://github.com/Kaggle/kagglehub):** Download automático do dataset diretamente do Kaggle.

## 🗂 Estrutura dos Dados

O dataset original possui cerca de 3.500 registros. Durante o pré-processamento, as colunas foram renomeadas e os dados categóricos traduzidos do inglês para o português para facilitar a interpretação local.

**Dicionário de Dados (Pós-processamento):**

| Coluna | Descrição |
| :--- | :--- |
| `data` | Data da transação |
| `hora_do_dia` | Hora em que a compra ocorreu |
| `metodo_de_pagamento` | Forma de pagamento (Dinheiro, Cartão, etc.) |
| `valor_gasto` | Valor total da transação |
| `nome_do_cafe` | Tipo de bebida adquirida |
| `turno_do_dia` | Manhã, Tarde ou Noite |
| `dia_da_semana` | Dia da semana (Segunda a Domingo) |
| `nome_do_mes` | Mês da transação |

## 📊 Etapas da Análise

1.  **Ingestão de Dados:** Download programático via `kagglehub`.
2.  **Limpeza e Transformação (ETL):**
    * Renomeação de colunas para o padrão snake_case em português.
    * Tradução de valores categóricos (Dias da semana, Meses, Turnos).
    * Verificação de tipos de dados e valores nulos.
3.  **Análise Exploratória (EDA):**
    * Análise de distribuição de vendas por produto.
    * Análise temporal (Hora, Dia da Semana, Mês).
    * Cálculo de Ticket Médio.

## 💡 Principais Insights

Com base na análise dos dados, chegamos às seguintes conclusões de negócio:

* **Produtos Estrela:** Os cafés **Latte** e **Americano com Leite** são os carros-chefe, gerando o maior volume de receita.
* **Horários de Pico:** O maior fluxo de vendas concentra-se entre **10h e 16h**.
* **Sazonalidade Semanal:** Curiosamente, **Terça-feira** e **Segunda-feira** apresentaram os maiores volumes de receita, contrariando a expectativa de fins de semana mais movimentados.
* **Ticket Médio:** O valor médio gasto por transação é de aproximadamente **R$ 31,65**, com baixa variabilidade (desvio padrão baixo), indicando consistência nos preços e no comportamento de compra.

## 🚀 Como Executar

Para rodar este notebook localmente:

1.  Clone este repositório.
2.  Certifique-se de ter o Python instalado.
3.  Instale as dependências necessárias:
    ```bash
    pip install pandas matplotlib kagglehub
    ```
4.  Execute o arquivo `.ipynb` usando Jupyter Notebook, Jupyter Lab ou VS Code.

---
*Este projeto é para fins educacionais e de portfólio.*
