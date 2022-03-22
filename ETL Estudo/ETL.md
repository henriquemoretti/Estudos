# ETL Estudo próprio

## O Que é ETL

ETL é uma técnica que visa a integração de dados, em que possuem fontes diversas, no caso da Totvs Zendesk e Jira.

## Significado da Expressão

E: Extraction - Extração
T: Transformation - Transformação
L: Load - Carregamento

## Ordem de funcionamento

O funcionamento à baixo segue a sequencia das letras em ETL

Source -> Staging Área -> Data Warehouse

Extraction vai em Source

Transformation em Stagin Área (acredito ser a base atual no postgree do VeD, mesmo não sendo uma fonte de dados em RAW, talvez exista um stagin anterior, acredito que não).

Load é o BigQuery, que é o Data Warehouse.

Seguindo o modelo à cima ficaria:

Zen/Jira -> Postgree -> BigQuery

## Como realizar os procedimentos

Extração -> Não possuo ainda a informação, visto que terie que me adequar ao Carlos

Transformação ->

* Filtragem, limpeza, remoção de duplicatas,

* Validações;

* Auditorias;

* Criptografia dos dados;

* Formatação dos dados em tabelas/unificação de tabelas para que estas correspondam ao schema do data warehouse alvo;

Load -> Os dados já transformados são movidos para o Data Warehouse e nicia uma carga total dos dados em um local específico e segue com cargas periódicas.

## Problemas atuais

1. Em Load, precisamos de duas fontes, uma com dados estáticos, que segue com cargas periódicas sem a atualização dos dados diretamente.
E precisamos dos dados vivos para desenvolvermos dashs dinâmicas.

## Serviços GCP

### Google Cloud Storage

Serviço de armazenamento de dados GCP, ainda não sei estimar se gerará custos.

### BigQuery

Data Warehouse gerenciável e serveless 'pay as you go'.

### Cloud Composer

Versão do Apache Airflow da GCP.

Serviço de orquestração de fluxo de trabalhos de dados, gerenciável, que permite a criação, agendamento e monitoramento de pipelines.

## Cloud Composer - Estudo

O Cloud Composer trabalha com o que chamam de Grafos Acíclicos Dirigidos, ou DAG's (Directed Acyclic Graph). São arquivos escritos em python que definem a sequência de execução de funções responsáveis por algum pipeline.

* Utiliza Buckets
* Gera Custos
* Pode ser uma alternativa para o automatização atual do VeD
* Possui uma tab 'Graph View', que mostra a sucesso das tasks

[Referência](https://ilegra.com/blog/construindo-um-etl-na-gcp-com-gcs-bigquery-e-cloud-composer/)
