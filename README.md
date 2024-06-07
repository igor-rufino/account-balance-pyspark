# account-balance-pyspark

## Introduction

```account-balance-pyspark``` é um Notebook Python que utiliza o Apache Spark para calcular o saldo final de clientes com base em saldos iniciais e movimentações diárias de uma série de arquivos. O objetivo é consolidar todas as operações financeiras de cada cliente ao longo de um período especificado e aplicar eventuais estornos. A seguir, é descrita a estrutura e funcionamento do código.

## Estrutura do Projeto

O diretório do projeto contém os seguintes arquivos:

```
.
├── data
|   └── tabela_saldo_inicial.txt
|   └── movimentacao_dia_02_04_2022.txt
|   └── movimentacao_dia_03_04_2022.txt
|   └── ...
├── account_balance_pyspark.ipynb
└── README.md

```

**Descrição dos arquivos**:

- **tabela_saldo_inicial.txt**: Arquivo CSV que contém o saldo inicial dos clientes.
- **movimentacao_dia_DD_MM_YYYY.txt**: Arquivos CSV que contêm as movimentações diárias dos clientes, que serão processados donamicamente.
- **account_balance_pyspark.ipynb**: Notebook python para o processamento com Pyspark.
- **README.md**: Fornece uma visão geral e instruções de configuração para o projeto.


## Pré-requisitos

- Python 3.6 ou superior
- Apache Spark 3.0 ou superior
- Biblioteca pyspark


## Configuração

1. Instale o Apache Spark:

    Siga as instruções oficiais para instalar o [Apache Spark](https://spark.apache.org/).

2. Instale o PySpark:

    Você pode instalar o PySpark usando pip:
    ```
    pip install pyspark
    ```
3. Organize os Arquivos de Dados:

    - Certifique-se de que tenha um diretório chamado `data` na mesma pasta onde o script Python está localizado.
    - Certifique-se de que os arquivos `tabela_saldo_inicial.txt` e todos os arquivos `movimentacao_dia_DD_MM_YYYY.txt` estão no diretório `data`.

## Como Executar

O Notebook Python cuidará da execução dos códigos quando acionado. Podendo executar por blocos individuais de código, ou execução completa do notebook.


## Conclusão

Este script oferece uma maneira eficiente de calcular e atualizar saldos de clientes com base em dados de movimentações diárias usando o Apache Spark. A capacidade de aplicar estornos e processar grandes volumes de dados o torna adequado para aplicações em sistemas financeiros e de contabilidade.