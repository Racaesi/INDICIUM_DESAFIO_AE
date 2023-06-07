# Lighthouse | Jornada Técnica - Analytics Engineering 2023-04

Certificação em Analytics Engineer by Indicium

## 🚀 A Certificação INDICIUM

O objetivo desta certificação é avaliar suas competências em um projeto prático de Engenharia de Analytics conforme a metodologia do Modern Analytics Stack, desenvolvida pela Indicium mas que guarda muitas semelhanças com o Modern Data Stack utilizado por milhares de times de dados modernos.

A certificação indica que o profissional:

* Entende o processo de construção de uma plataforma de analytics moderna;
* Entende os objetivos da modelagem dimensional em data warehouses modernos;
* Sabe aplicar a linguagem SQL e a ferramenta dbt para modelar dados em data warehouses modernos;
* Conhece as boas práticas de visualização de dados e sua aplicação em uma ferramenta de Self-Service BI.


## 📋 Contexto

A empresa contratou Adventure Works (AW) é uma indústria de bicicletas em franco crescimento que se orgulha de possuir mais de 500 produtos distintos, 20.000 clientes e 31.000 pedidos. Para manter seu ritmo de crescimento e se diferenciar da concorrência, a Adventure Works quer utilizar seus dados de forma estratégica, norteando suas decisões para se tornar uma empresa data driven. A diretoria da Adventure Works já listou uma série de perguntas que ela quer responder através de cruzamentos dos dados, e que devem guiar o desenvolvimento das tabelas de fatos e dimensões do data warehouse. Para iniciar o projeto e obter resultados rápidos, a opção foi iniciar pela área de vendas (sales), mas algumas tabelas de outras áreas podem ser necessárias para conseguir as informações desejadas. Em seu diagnóstico inicial, você identificou alguns sistemas que a Adventure Works utiliza e que geram dados relevantes para o negócio e que, em algum momento, devem fazer parte da infraestrutura de dados:

<div align="center">
<img src="![image](https://github.com/Racaesi/INDICIUM_DESAFIO_AE/assets/114450210/e86fd61d-eb2f-47df-b7d6-9d043c669728)" width="150px" />
</div>


### 🔧 Perguntas para serem respondidas:

- a) Qual o número de pedidos, quantidade comprada, valor total negociado por produto, tipo de cartão, motivo de venda, data de venda, cliente, status, cidade, estado e país?
- b) Quais os produtos com maior ticket médio por mês, ano, cidade, estado e país? (ticket médio = Faturamento bruto - descontos do produto / número de pedidos no período de análise)
- c) Quais os 10 melhores clientes por valor total negociado filtrado por produto, tipo de cartão, motivo de venda, data de venda, status, cidade, estado e país?
- d) Quais as 5 melhores cidades em valor total negociado por produto, tipo de cartão, motivo de venda, data de venda, cliente, status, cidade, estado e país?
- e) Qual o número de pedidos, quantidade comprada, valor total negociado por mês e ano (dica: gráfico de série de tempo)?
- f) Qual produto tem a maior quantidade de unidades compradas para o motivo de venda “Promotion”?

### ⚙️ Descrição dos dados
A Adventure Works possui um banco de dados transacional (PostgreSQL) que armazena os dados de suas diferentes áreas. Esses dados estão distribuídos em 68 tabelas divididas em 5 schemas: HR (recursos humanos), sales (vendas), production (produção) e purchasing (compras).

![AdventureWorksERD](https://github.com/Racaesi/INDICIUM_DESAFIO_AE/assets/114450210/36398730-f9e0-4795-ab38-250e21d2de03)


### ⚙️ Dicionário de dados

Para facilitar o entendimento dos dados, a Adventure Works disponibilizou um dicionário de dados necessários para seu projeto com algumas definições que eles utilizam internamente. Como o cliente utiliza atualmente relatórios exportados pelo sistema, podem ser necessárias outras tabelas para obter as informações, e cabe a você encontrar esses relacionamentos.

![image (1)](https://github.com/Racaesi/INDICIUM_DESAFIO_AE/assets/114450210/0beeff34-f3da-48d7-bcb5-343bfa5fd13e)


![image (2)](https://github.com/Racaesi/INDICIUM_DESAFIO_AE/assets/114450210/0145e0b5-37c2-41ff-a7e0-0b8c8b0ff225)



## ⌨️ Entregas 

* Diagrama conceitual do data warehouse: Modelo conceitual com as tabelas de fatos e dimensões necessárias para responder às perguntas de negócio. 

* Data warehouse na nuvem: Google BigQuery 

* Configuração e transformações de dados: DBT.
    - 1) **Documentação das tabelas e colunas nos marts**
    - 2) **Testes de sources**
    - 3) **Testes nas primary keys das tabelas de dimensão e fatos**
    - 4) **Teste de dados**
    - 5) **O código precisa estar em um repositório (github).**

* Painéis de BI: Responder as perguntas feitas anteriormente.

## 🛠️ Construído com:

* [DBT](https://docs.getdbt.com/) - Ferramenta de transformação de Dados
* [GoogleBigQuery](https://cloud.google.com/bigquery?hl=pt-br) - Data Warehouse em Nuvem
* [PowerBI](https://learn.microsoft.com/pt-br/power-bi/) - Ferramenta de BI.
* [Draw.IO](https://www.drawio.com/doc/) - Ferramenta de Desenho e Criação de Diagramas.


## ✒️ Autor

* **Raphael Caetano da Silva** - *Analytics Engineering*