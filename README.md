# Desafio beAnalytic - Extração de Dados do SteamDB

##Descrição do Projeto

Este projeto tem como objetivo extrair dados de promoções do site SteamDB, processar essas informações e armazená-las no Google BigQuery. Posteriormente, os dados são conectados ao Google Sheets para facilitar a visualização e compartilhamento.

## Passos Realizados

### 1. Configuração do Ambiente

- Ferramentas Utilizadas:
  - Python
  - Selenium
  - Pandas
  - Google BigQuery
  - Google Sheets
 
- Bibliotecas Instaladas:
  - selenium
  - google-cloud-bigquery
  - pandas-gbq
  - webdriver-manager
    
### 2. Extração de Dados

Utilizamos a biblioteca Selenium para automatizar a navegação e extração de dados do site SteamDB. O script faz a navegação por todas as páginas de promoções e coleta as informações de cada item listado.

### 3. Processamento dos Dados
- Formatação dos Dados:
  - Ajustamos os dados extraídos para garantir consistência e integridade.
  - Colunas como Percentage, Price, Rating, Release, foram limpas e convertidas para formatos apropriados.
    
### 4. Armazenamento no Google BigQuery

- Configuração das Credenciais:
  - Configuramos as credenciais do Google Cloud para permitir o acesso ao BigQuery.
  - Definimos o schema do dataset e carregamos os dados processados para uma tabela no BigQuery.
 
### 5. Conexão com Google Sheets
- Exportação dos Dados:
  - Conectamos a tabela do BigQuery ao Google Sheets para facilitar a visualização e compartilhamento dos dados.
