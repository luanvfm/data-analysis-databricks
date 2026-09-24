# Data Analysis with Databricks

Projeto de estudo de Engenharia de Dados no Databricks com o dataset Indian E-commerce.

## Fluxo

```text
Landing -> Auto Loader/Bronze -> Silver -> Gold -> Views
```

- **Landing:** arquivos CSV armazenados em um Volume do Unity Catalog.
- **Bronze:** ingestão dos arquivos com rastreabilidade, incluindo uma prática com Auto Loader, schema location e checkpoint.
- **Silver:** tipagem, tratamento de nulos, deduplicação e padronização de datas.
- **Gold:** tabelas analíticas e modelo estrela com dimensões e fato de vendas.
- **Views:** visões para facilitar o consumo das tabelas Gold.

## Notebooks

Execute nesta ordem:

1. `Training-Bronze.ipynb`
2. `Training-Silver.ipynb`
3. `Training-Gold.ipynb`
4. `Training-Creating-Views.ipynb`

Extensões de estudo:

- `AutoLoader-Bronze.ipynb`: ingestão incremental de arquivos.
- `Star Schema Gold Modelling.ipynb`: dimensões, tabela fato, surrogate keys, validações e agregações com PySpark.

Os notebooks principais também foram organizados em um Databricks Job com dependências entre Bronze, Silver, Gold e Views.

## Tecnologias

- Databricks
- Apache Spark e Spark SQL
- Delta Lake
- Unity Catalog
- Auto Loader
- Lakeflow Jobs
- PySpark

Antes de executar, ajuste os nomes do catálogo, schemas e caminhos dos volumes para o seu ambiente.
