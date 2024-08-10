# Projeto de Data Analytics para Retail

## Objetivo
Desenvolver um projeto de Data Analytics para uma empresa de retail, envolvendo a criação de uma arquitetura de dados na Azure e a construção de um Lakehouse. Este projeto será semelhante ao de grandes empresas de comércio e retail e visa a análise de dados para Business Intelligence (BI) e Machine Learning (ML).

## O que Vamos Fazer
- **Construir uma arquitetura de dados na Azure**
- **Construir um Lakehouse**
- Projeto típico de Analytics para BI e Machine Learning, similar aos de grandes empresas de comércio/retail.

## Ferramentas
- **Databricks**
- **Azure Data Lake Storage (ADLS)**
- **Azure Data Factory (ADF)**
- **Microsoft PowerBI**

## CI/CD e Processos
- Implementação de CI/CD
- Processos e Cultura de Engenharia de Dados

## Fases do Projeto

### V1 - Ingestão Simples
- Implementação de ingestão full load
- Projeto de ponta a ponta

### V2 - Ingestão Incremental e Workflows
- Ingestão incremental
- Implementação de workflows

### V3 - Unity Catalog e Delta Live Tables
- Implementação do Unity Catalog
- Uso de Delta Live Tables

### V4 - CI/CD
- Implementação de CI/CD

## Setup

### Configuração Inicial
- **Criar Subscription**
- **Integrar Recursos da Azure**
  - Grupo de Recursos
  - Databricks
  - ADLS
  - Azure Data Factory

### Azure Data Factory (ADF) + ADLS
- Configuração de **Linked Services**
- Criação de **Datasets**
- Desenvolvimento de **Pipelines**
- Implementação de ingestão com metadados
  - Tabela de controle
  - Loop nos metadados

### App Registration e Permissões
- Criação do recurso na Azure
- Definição de permissões de usuário e políticas de acesso
- Criação de segredos / senhas no **Key Vault**

### Databricks Secrets
- Criação de escopo de segredos do Databricks
- Integração com Azure Key Vault
- Armazenamento e teste dos segredos

## Camadas de Dados

### Camada Bronze
- Criação de Databases no Databricks (formato Delta)
  - **Managed**: Controle pelo Databricks
  - **External Tables**: Leitura do Data Lake
- Ingestão e transformação de arquivos
  - Funções e frameworks para orquestração

### Camada Prata
- Criação de Database no Hive_metastore (managed)
- Contextualização dos projetos
- Exemplos em SQL e PySpark
- Implementação de regras de qualidade de dados
- Criação de cadernos de configuração e transformação
  - Aplicação de lógicas com PySpark
  - Processamento de dados: Deduplication, Window Functions, Apply Schema, Upsert

### Camada Ouro
- ETL para Analytics e ML
- Criação da camada Ouro
- Governança de Dados

## Automação e Monitoramento
- **ADF Pipelines** e **ADB Workflows**
- **SQL Serverless** para consulta e análise de dados
- Monitoramento da qualidade dos dados em Databricks

## Governança e Avançado
- Implementação do **Unity Catalog**
- Planejamento e gerenciamento de custos
- **Azure DevOps** para CI/CD
- Utilização de **Delta Live Tables**
