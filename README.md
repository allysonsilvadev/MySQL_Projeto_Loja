# 🛒 Projeto Banco de Dados – Loja (MySQL)

Este projeto contém a modelagem e criação de um banco de dados simples para uma loja, desenvolvido em **MySQL**.  
O repositório inclui:

- Estrutura das tabelas (DDL)  
- Inserção de dados fictícios (DML)  
- Consultas SQL solicitadas no exercício  
- Script completo do banco (`projeto_loja_mysql.sql`)

---

## 📁 Estrutura do Banco de Dados

O banco é composto por **4 tabelas principais**:

### 🧍 Tabela `CLIENTE`
Armazena informações dos clientes da loja.

| Campo     | Tipo         | Descrição |
|-----------|--------------|-----------|
| codigo    | INT          | Chave primária, auto incremento |
| nome      | VARCHAR(50)  | Nome do cliente |
| endereco  | VARCHAR(30)  | Endereço |
| cidade    | VARCHAR(25)  | Cidade |
| estado    | VARCHAR(2)   | UF |
| telefone  | VARCHAR(15)  | Telefone |

---

### 🏢 Tabela `FORNECEDOR`
Registra os fornecedores dos produtos.

| Campo     | Tipo         | Descrição |
|-----------|--------------|-----------|
| codigo    | INT          | Chave primária |
| nome      | VARCHAR(50)  | Nome da empresa |
| cnpj      | VARCHAR(15)  | CNPJ |
| endereco  | VARCHAR(20)  | Endereço |
| cidade    | VARCHAR(30)  | Cidade |
| estado    | VARCHAR(2)   | UF |
| telefone  | VARCHAR(15)  | Telefone |

---

### 📦 Tabela `PRODUTO`
Armazena dados dos produtos vendidos.

| Campo     | Tipo           | Descrição |
|-----------|----------------|-----------|
| codigo    | INT            | Chave primária |
| nome      | VARCHAR(50)    | Nome do produto |
| preco     | NUMERIC(6,2)   | Preço unitário |
| estoque   | INT            | Quantidade em estoque |

---

### 🧾 Tabela `VENDA`
Registra vendas realizadas pela loja.

| Campo             | Tipo           | Descrição |
|-------------------|----------------|-----------|
| numeroDaNotaFiscal | INT           | Chave primária |
| dataVenda          | DATE          | Data da venda |
| valorVenda         | NUMERIC(6,2)  | Valor total |

---

## 📝 Consultas SQL Incluídas

O script contém consultas como:

- Clientes que moram em MG  
- Clientes cujo telefone começa com DDD 37  
- Fornecedores de Bom Despacho  
- Produtos com estoque > 20 e preço > 50  
- Vendas a partir de 2016 com valor > 200  
- Produtos com preço >= 50 e estoque entre 20 e 50  

---

## 🚀 Como usar este banco de dados

1. Baixe o arquivo `.sql` deste repositório  
2. Importe no seu MySQL (DBeaver, Workbench, HeidiSQL etc.)  
3. Execute o script completo  
4. Comece a consultar os dados!

---

## 📌 Tecnologias utilizadas
- **MySQL 8+**
- **DBeaver** (para gerenciamento)

---

## 👩‍💻 Autor
**Allyson Silva**  
Repositório criado para estudos de SQL e modelagem de banco de dados.

---

## ⭐ Gostou do projeto?
Deixe uma **estrelinha no GitHub** ⭐ para apoiar!

