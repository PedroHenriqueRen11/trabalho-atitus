# 🚀 Microserviços - Trabalho Atitus

Repositório destinado ao desenvolvimento de microserviços utilizando **Spring Boot** e **Java 17**, como parte das atividades da disciplina de Paradigmas de Linguagem de Programação.

## 🏗️ Estrutura do Projeto

O projeto é composto por 4 microserviços principais que se comunicam para gerenciar informações de produtos e conversão de moedas:

* **config-service**: Centralizador de configurações para os demais serviços.
* **greeting-service**: Serviço básico de saudação para teste de conectividade.
* **currency-service**: Responsável pela lógica de conversão de moedas.
* **product-service**: Gerenciamento de produtos, integrado ao banco de dados PostgreSQL.

## 🛠️ Tecnologias Utilizadas

- **Java 17**
- **Spring Boot 3**
- **Spring Data JPA**
- **PostgreSQL** (Banco de dados)
- **Flyway** (Gerenciamento de Migrations)
- **Maven** (Gerenciador de dependências)

## 📦 Como rodar o projeto

1.  Certifique-se de ter o **PostgreSQL** rodando localmente.
2.  Crie o banco de dados chamado `bd_product`.
3.  Inicie o `config-service` (Porta padrão: 8888).
4.  Inicie os demais serviços conforme a necessidade.
5.  O `product-service` estará disponível em: `http://localhost:8001/products/{id}?targetCurrency=USD`

## 🔎 Endpoints Principais (Product Service)

| Método | Endpoint | Descrição |
| :--- | :--- | :--- |
| `GET` | `/products/{id}?targetCurrency=XXX` | Retorna os detalhes de um produto e prepara a conversão de moeda. |

---
Desenvolvido por **Pedro Henrique** 🎓
