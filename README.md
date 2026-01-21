# Banco de Dados Lógico - Sistema de Oficina Mecânica
Banco de Dados Lógico para o cenário de uma oficina mecânica.

📌 Este projeto apresenta a modelagem, implementação e consulta de um banco de dados relacional para o cenário de uma oficina mecânica, desenvolvido como parte de um desafio prático de modelagem de banco de dados.

O foco principal é aplicar, de forma integrada, os conceitos de:

Modelagem Conceitual (DER)

Modelagem Lógica (Modelo Relacional)

Implementação Física em SQL

Persistência de dados

Consultas SQL avançadas orientadas a regras de negócio

O banco foi implementado em MySQL, com compatibilidade total com o MySQL Workbench.

---

🎯 Objetivos do Projeto

Mapear um DER conceitual refinado para o modelo relacional

Criar o script SQL completo do banco de dados

Definir corretamente chaves primárias e estrangeiras

Garantir integridade referencial

Persistir dados para testes (INSERT INTO)

Criar queries SQL avançadas, utilizando:

SELECT

WHERE

JOIN

ORDER BY

GROUP BY

HAVING

Funções de agregação (SUM, COUNT, AVG)

Elaborar perguntas de negócio respondidas pelas consultas

🧱 Modelagem Conceitual (DER)

O modelo conceitual foi desenvolvido para representar fielmente o funcionamento de uma oficina mecânica real, considerando clientes, veículos, ordens de serviço, serviços executados, peças utilizadas e funcionários envolvidos.

🔹 Principais Entidades

Cliente

Veículo

Funcionário

Ordem de Serviço

Serviço

Peça

🔹 Relacionamentos

Cliente → Veículo (1:N)

Veículo → Ordem de Serviço (1:N)

Funcionário → Ordem de Serviço (1:N)

Ordem de Serviço ↔ Serviço (N:M)

Ordem de Serviço ↔ Peça (N:M)

Os relacionamentos N:M foram corretamente resolvidos por meio de tabelas associativas, seguindo boas práticas de modelagem relacional.

📌 O DER refinado serviu como base direta para a construção do esquema lógico.

🗄️ Estrutura do Banco de Dados

O banco de dados é composto pelas seguintes tabelas:

✔️ cliente

✔️ veiculo

✔️ funcionario

✔️ ordem_servico

✔️ servico

✔️ peca

✔️ ordem_servico_servico (associativa)

✔️ ordem_servico_peca (associativa)

📌 Características do esquema:

🔹 Todas as tabelas possuem chave primária

🔹 Uso consistente de chaves estrangeiras

🔹 Tipos de dados adequados ao domínio

🔹 Estrutura normalizada

🧪 Persistência de Dados

Foram criados comandos INSERT INTO para todas as tabelas, permitindo:

✔️ Testes funcionais das queries

✔️ Simulação de cenários reais da oficina

✔️ Validação das regras de negócio

Os dados incluem:

✔️ Clientes com múltiplos veículos

✔️ Ordens de serviço em diferentes estados

✔️ Serviços e peças associados às ordens

🔍 Consultas SQL Desenvolvidas

As consultas SQL foram elaboradas para responder perguntas reais de negócio, como:

📊 Qual o valor total faturado por cada ordem de serviço?

👥 Quais clientes gastaram acima de um determinado valor?

🧑‍🔧 Quais funcionários executaram mais ordens de serviço?

🔧 Qual serviço foi mais realizado?

⏳ Quais ordens em andamento possuem valor estimado acima da média?

🔹 Recursos utilizados nas queries

✔️ Junções múltiplas (JOIN)

✔️ Funções de agregação (SUM, COUNT)

✔️ Atributos derivados

✔️ Filtros com WHERE

✔️ Agrupamentos com GROUP BY

✔️ Filtros avançados com HAVING

✔️ Subqueries

🧠 Boas Práticas Aplicadas

✔️ Normalização do esquema

✔️ Separação clara de responsabilidades entre tabelas

✔️ Resolução correta de relacionamentos N:M

✔️ Script organizado e legível

✔️ Queries compatíveis com ONLY_FULL_GROUP_BY

✔️ Estrutura adequada para avaliação acadêmica e portfólio profissional

🛠️ Tecnologias Utilizadas

✔️ MySQL

✔️ MySQL Workbench

✔️ SQL ANSI

✅ Status do Projeto

- ✔️ Modelagem conceitual validada 
- ✔️ Esquema lógico implementado
- ✔️ Dados persistidos
- ✔️ Queries avançadas desenvolvidas
- ✔️ Projeto pronto para avaliação e portfólio

📌 Considerações Finais

Este projeto foi desenvolvido atendendo integralmente ao cenário real de um sistema de oficina mecanica.

<img width="1307" height="1373" alt="Projeto Conceitual - Oficina_Refinado" src="https://github.com/user-attachments/assets/ebe9f833-a974-4e87-8840-6bbb18d9baea" />

