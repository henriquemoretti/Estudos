# Gerenciamento Custos BigQuery

## Prática recomendada bigquery

![bigquery prática recomendada](bigquery1.png)

## Auditoria de uso de dados

Link que explica como gerenciar o consumo do BigQuery e o consumo das requisições, assim como controle de acesso e desenvolvimento de logs <https://cloud.google.com/bigquery/docs/reference/auditlogs?hl=pt-br>

## Estimativa de custos no presente

Minha estimativa de baixo custo pressupõe que não utlizaremos um bucket, ou seja, o armazenamento de dados brutos(raw) não será de nosso gerenciamento. Foi realizado uma conta com mais de 20gb de armazenamento em tabelas próprias do BigQuery, em que serão realizado as consultas, como descrito na imagem abaixo.

![bigquery pulando buckets](bigquery2.png)
