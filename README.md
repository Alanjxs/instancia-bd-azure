# 🗄️ Desafio Prático: Configuração de uma Instância de Banco de Dados no Microsoft Azure

Este repositório documenta minha experiência prática no desafio da DIO voltado à **configuração de uma instância de banco de dados** no Azure. O objetivo é consolidar os conhecimentos adquiridos durante o laboratório e disponibilizar um material de apoio útil para estudos futuros.

---

## 🎯 Objetivos do Desafio

- Criar e configurar uma instância de banco de dados na plataforma Azure
- Compreender os principais recursos de gerenciamento de bancos de dados na nuvem
- Registrar o processo técnico de forma clara e acessível
- Utilizar o GitHub como repositório de documentação técnica

---

## 🧪 Etapas Realizadas

### 1. Acesso ao Portal do Azure
- Acesse: [https://portal.azure.com](https://portal.azure.com)
- Utilize uma conta existente ou crie uma conta gratuita com créditos

### 2. Criação da Instância de Banco de Dados
- No menu, acesse **"Banco de Dados SQL"** ou **"Azure Database for..."** (ex: PostgreSQL, MySQL)
- Clique em **"Criar"**
- Preencha os dados:
  - **Assinatura e grupo de recursos**
  - **Nome do servidor** (único globalmente)
  - **Região** (ex: Brazil South)
  - **Tipo de banco de dados**: SQL, PostgreSQL, MySQL etc.
  - **Autenticação**: nome de usuário e senha
- Configure a performance (tamanho e DTUs) de acordo com os créditos
- Clique em **"Revisar + Criar"** e depois em **"Criar"**

### 3. Configuração do Firewall
- Após a criação, vá para o recurso do banco
- Configure a **regra de firewall** para permitir conexões do seu IP local
- Copie a **string de conexão** para usar no seu cliente local (ex: SSMS, DBeaver, Azure Data Studio)

### 4. Conexão e Teste
- Conecte-se com um cliente SQL usando a string de conexão
- Execute comandos básicos para testar a instância:
  ```sql
  CREATE DATABASE TesteAzure;
  SELECT name FROM sys.databases;
