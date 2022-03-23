# Pipeline

## O Que é Pipeline

Em Software, um pipeline consistem em uma cadeia de elementos de processamento - processos, threads, funções - dispostos de modo que a saída de cada elemento seja a entrada do próximo, gerando uma entrega contínua.

Nesse Estudo limitarei os estudos ao Pipeline de Software / Pipeline ci/cd (continuous integration / continuous delivery)

## O que é pipeline CI/CD

[Link Pipeline CI/CD RedHat](https://www.redhat.com/pt-br/topics/devops/what-cicd-pipeline)

Consistem em uma série de etapas a serem realizadas para a disponibilização de uma nova versão de softaware. Os pipelines de integração e entregas contínuas são uma prática que tem como objetivo acelerar a disponibilização de softwares, adotando a abordagem de DevOps ou de Engenharia de confiabilidade de sites (SRE)

O Pipeli de CI/CD inclui monitoramento e automação para melhora o processo de desenvolvimento de aplicações principalmente nos estágios de integração e teste, mas também na entrega e e na implantação. É possível executar manualmente cada etapa do CI/CD, mas o real valor dele está na automação.

### Elementos de um pipeline CI/CD

As etapas que compõe  um pipeline CI/CD são subconjuntos distintos de tarefas agrupadas no que chamamos de estágio de pipeline. Os estágios típicos do pipline são:

* Compilação: Estágio em que a aplicação é compilada.
* Testes: Automação dos testes do código.
* Lançamento: Estágio em que a aplicação é enviada ao repositório.
* Validade e conformidade: Validar se a versão está de acordo com as necessidades.

![Imagem RedHat Estágio Pipeline](https://www.redhat.com/cms/managed-files/styles/wysiwyg_full_width/s3/ci-cd-flow-desktop_0.png?itok=QgBYmjA2)
