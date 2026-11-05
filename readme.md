# 🖥️ Banco de Dados - Central de Suporte de TI

Este repositório contém um script SQL estruturado para um sistema simples de gerenciamento de chamados de suporte de TI. O objetivo do projeto é demonstrar a modelagem de um banco de dados relacional e a aplicação de consultas utilizando `INNER JOIN`.

## 🗄️ Estrutura do Banco de Dados

O banco de dados, chamado `suporte_join`, é composto por duas tabelas principais:

* **`tecnico`**: Armazena as informações da equipe de suporte (nome, e-mail e nível de especialidade: N1, N2, N3).
* **`chamado`**: Armazena os tickets/chamados abertos pelos usuários (título, prioridade, status, data de abertura e o ID do técnico responsável).

Há um relacionamento de **1:N** (Um para Muitos) entre as tabelas, onde um técnico pode ter vários chamados atribuídos a ele.

## 🚀 Arquivos do Projeto

* `banco_suporteTiJoin.sql`: Script completo contendo:
  * Criação do banco de dados e tabelas.
  * Inserção de dados (técnicos e chamados de exemplo).
  * Consultas SQL de exemplo utilizando cláusulas importantes como `INNER JOIN`, `WHERE`, `ORDER BY`, `LIMIT`, `COUNT` e `DISTINCT`.

## 🛠️ Como usar

1. Faça o clone deste repositório na sua máquina.
2. Abra o seu gerenciador de banco de dados MySQL preferido (como MySQL Workbench, DBeaver, HeidiSQL, ou phpMyAdmin).
3. Importe ou abra o arquivo `banco_suporteTiJoin.sql`.
4. Execute o script para criar o ambiente, inserir os dados e testar as consultas de relacionamento.

## 💡 Exemplos de Consultas (Queries)

O script inclui exemplos práticos de como buscar dados cruzados, como:
* Listar todos os chamados com o nome dos respectivos técnicos.
* Filtrar chamados específicos de um técnico (ex: Aline Torres).
* Buscar chamados em aberto associados a técnicos de nível "N2".
* Contar a quantidade total de chamados já resolvidos.

---
*Projeto criado para fins de estudo e demonstração de consultas relacionais em SQL.*