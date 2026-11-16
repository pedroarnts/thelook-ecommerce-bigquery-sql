# Análise Exploratória e Financeira — TheLook eCommerce (BigQuery)

Projeto de análise de dados em SQL utilizando o **Google BigQuery** (via Python SDK) sobre a base pública `bigquery-public-data.thelook_ecommerce`.

## Objetivos
* Configurar acesso seguro ao BigQuery com controle de custos (`dry_run` e `maximum_bytes_billed`).
* Explorar esquemas, volumetria e ciclo de vida dos pedidos (`orders`, `order_items`, `products` e `users`).
* Desenvolver consultas analíticas envolvendo filtros temporais, agregações mensais, cálculo de SLA de entrega e margem bruta por categoria.
* Validar qualidade dos dados (unicidade de chaves, integridade referencial e tratamento de nulos) e exportar os resultados em CSV.

## Estrutura do Repositório
* `projeto_bigquery_2.ipynb`: Notebook com todo o código Python/SQL, validações e interpretações de negócio.
* `q01_amostra_pedidos.csv`: Amostra inicial da tabela de pedidos.
* `q02_prazo_entrega_pedidos.csv`: Top 50 pedidos concluídos mais recentes com maior prazo de entrega.
* `q03_receita_mensal_status.csv`: Evolução mensal de receita, pedidos e ticket médio por status.
* `q04_margem_por_categoria.csv`: Receita e margem bruta percentual por categoria de produto.

## Tecnologias Utilizadas
* **SQL (Google BigQuery)**
* **Python** (`google-cloud-bigquery`, `pandas`)