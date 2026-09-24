# Data Analysis with Databricks

Projeto de estudo de Engenharia de Dados no Databricks, construindo um pipeline Lakehouse com o dataset Indian E-commerce.

## Fluxo

```text
Landing -> Bronze -> Silver -> Gold -> Views
```

- **Bronze:** ingestão dos arquivos CSV com metadados de origem e horário da carga.
- **Silver:** tipagem, tratamento de nulos, deduplicação e padronização de datas.
- **Gold:** tabelas analíticas de vendas, clientes e produtos.
- **Views:** visões para facilitar o consumo das tabelas Gold.

## Notebooks

Execute nesta ordem:

1. `Training-Bronze.ipynb`
2. `Training-Silver.ipynb`
3. `Training-Gold.ipynb`
4. `Training-Creating-Views.ipynb`

## Tecnologias

- Databricks
- Apache Spark e Spark SQL
- Delta Lake
- Unity Catalog

Antes de executar, ajuste os nomes do catálogo, schemas e caminhos dos volumes para o seu ambiente.
