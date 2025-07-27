# Projeto: Data-Driven Insights

**Autora:** Juliete da Silva  
**Base analisada:** `sales_data_sample.csv`  
**Tamanho da base:** 2823 linhas × 25 colunas

---

## Objetivo

Explorar dados de vendas utilizando ferramentas do Python como **listas**, **dicionários**, **tuplas**, **NumPy**, **agrupamentos com pandas** e **gráficos com Matplotlib**, extraindo insights de negócio ao final.

---

## Etapas Exploradas

### 1. Estrutura do DataFrame
- Leitura com `pandas` e exploração inicial com `.shape`, `.columns` e `.dtypes`
- Conversão da coluna `ORDERDATE` para o tipo `datetime`

### 2. Listas, Dicionários e Tuplas
- Criação de lista com as categorias de produto (`PRODUCTLINE`)
- Dicionário produto:cliente
- Tupla com múltiplos dados de uma linha
- *Observação:* Dicionários mantêm apenas chaves únicas, então dados repetidos são sobrescritos.

### 3. Condicionais e Laços
- Classificação de valores como "alto", "intermediário" ou "baixo"
- Soma dos 5 primeiros valores de `SALES` com `for`
- Localização de um valor com `while`
- Resultado: Média das 5 primeiras vendas foi de R$ 3.694,64

### 4. Operações NumPy
- Manipulação de arrays contendo `NaN`
- Uso de `.nansum()`, `.nanmean()` e fatiamento
- Substituição de valores e análise de padrões

### 5. Agrupamentos
- `value_counts()` para frequência de países e produtos
- `groupby()` para soma e média de vendas por país e por linha de produto
- Destaques:
  - Classic Cars lidera em vendas totais e média por pedido
  - EUA é o país com maior volume e faturamento

### 6. Gráficos
- Linha: Vendas ao longo do tempo (2003–2005), com variações e picos claros
- Barras: Média de vendas por `PRODUCTLINE`
- Dispersão: Relação entre `QUANTITYORDERED` e `SALES`, com outliers

---

## Principais Insights

- **Classic Cars** lidera em quantidade de vendas e ticket médio (acima de R$ 4.000)
- **EUA** é o principal mercado, com mais de 900 vendas e R$ 3,5 milhões em faturamento
- A maioria das vendas ocorre em pedidos de **25 a 40 unidades**
- Existem **outliers com vendas acima de R$ 12.000**, mesmo em pedidos pequenos
- **Sazonalidade aparente** com picos entre setembro/2004 e fevereiro/2005

---

## Bibliotecas Python

- `Pandas`
- `NumPy`
- `Matplotlib`

---
