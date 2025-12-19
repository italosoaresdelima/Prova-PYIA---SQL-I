# 🗄️ Fundamentos de SQL: Gestão de Clientes

Este repositório armazena estudos e scripts práticos de SQL. O foco é a estruturação de bancos de dados relacionais e a aplicação de boas práticas em DDL (*Data Definition Language*).

---

## 📌 Sobre o Projeto
O objetivo desta atividade foi criar uma tabela de clientes robusta, utilizando identificadores únicos e tipos de dados otimizados para performance e integridade.

## 🏗️ Estrutura da Tabela `Clientes`

| Coluna | Tipo | Atributos | Função |
| :--- | :--- | :--- | :--- |
| **ID** | `INT` | `PK`, `AUTO_INCREMENT` | Chave primária automática |
| **Nome** | `VARCHAR(100)` | `NOT NULL` | Nome (obrigatório) |
| **Idade** | `INT` | - | Idade do cliente |
| **Cidade** | `VARCHAR(100)` | - | Localidade |

---

## 💻 Script de Criação

```sql
CREATE TABLE Clientes (
    ID INT AUTO_INCREMENT PRIMARY KEY,
    Nome VARCHAR(100) NOT NULL,
    Idade INT,
    Cidade VARCHAR(100)
);
