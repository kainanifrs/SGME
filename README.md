# 🎓 Sistema de Gerenciamento de Mensalidades Escolares(SGME)

Sistema desenvolvido para gerenciar **alunos, responsáveis financeiros, turmas e mensalidades** de uma escola particular.

A aplicação permite realizar cadastros, alterações, remoções, pesquisas, controle financeiro e geração de relatórios.

## 👥 Desenvolvedores

- **Gilmar Brum Carabajal**
- **Kainã Machado Griebeler Márquez**

---

## 📋 Funcionalidades

### 👨‍🎓 Cadastro de Alunos

O sistema permite cadastrar, editar e remover alunos, contendo:

- Nome
- Matrícula
- Data de nascimento
- Turma
- Responsável financeiro

### 🏫 Cadastro de Turmas

Gerenciamento das turmas da escola:

- Código da turma
- Série
- Turno
- Lista de alunos

### 👤 Cadastro de Responsáveis

Cadastro dos responsáveis financeiros dos alunos:

- Nome
- CPF
- Telefone
- E-mail

### 💰 Cadastro de Mensalidades

Cada mensalidade possui informações como:

- Aluno
- Mês/Ano
- Valor
- Data de vencimento
- Status da mensalidade
- Data de pagamento
- Forma de pagamento

### 📊 Controle Financeiro

O sistema possui recursos para:

- Verificar atrasos automaticamente
- Atualizar o status das mensalidades
- Aplicar multa simples de **2%** em mensalidades atrasadas
- Registrar pagamentos

### 🔎 Pesquisa de Alunos

É possível localizar alunos através de:

- Matrícula
- Turma
- Nome
- Responsável financeiro

### 📑 Relatórios

O sistema permite gerar informações sobre:

- Alunos inadimplentes
- Mensalidades vencidas
- Pagamentos do mês
- Quantidade de alunos por turma

---

## 🛡️ Tratamento de Erros e Exceções

A aplicação possui validações para evitar situações inválidas, como:

- Matrícula duplicada
- CPF inválido
- Pagamento com valor inválido
- Busca por informações inexistentes

---

## 💾 Persistência de Dados

Os dados do sistema são armazenados em memória utilizando **coleções de objetos da linguagem Java**, como `ArrayList`.

Também é usado a persistência em **banco de dados relacional**, utilizando os conceitos de **DAO** e **DTO**.

---

## 🏗️ Arquitetura

O projeto é organizado seguindo a separação de responsabilidades baseada no padrão **MVC (Model, View e Controller)**.

```text
Model
 ├── Entidades
 ├── Regras de negócio
 └── Dados

View
 └── Interface com o usuário

Controller
 └── Controle das operações do sistema
```

---

## 🔌 Interfaces

O sistema utiliza interfaces para padronizar comportamentos entre diferentes classes.

Entre os exemplos estão:

- Pagamento
- Relatório
- Pesquisa
- DAO

---

## 🔖 Enumerações

São utilizadas enumerações para representar informações com valores pré-definidos.

### Status da mensalidade

```java
PENDENTE
PAGA
ATRASADA
```

### Forma de pagamento

```java
PIX
CARTÃO
BOLETO
DINHEIRO
```

---

## ☕ Conceitos de Java

O projeto também contempla a aplicação de diversos recursos da linguagem Java:

- Wrapper Classes
- Generics
- Classes internas
- Funções
- Lambdas
- Streams
- Coleções

---

## 🧩 Padrões de Projeto

O sistema utiliza diferentes padrões de projeto, organizados em três categorias:

### Criacionais

- **Builder**
- **Factory**

### Estrutural

- **Facade**

### Comportamental

- **Command**

---

## 🛠️ Tecnologias e conceitos

- **Java**
- Programação Orientada a Objetos
- Collections
- `ArrayList`
- Generics
- Lambda Expressions
- Streams
- DAO
- Repository
- DTO
- MVC
- Banco de dados relacional
- Padrões de projeto

---

## 🎯 Objetivo

O objetivo do projeto é desenvolver uma aplicação capaz de centralizar o gerenciamento das informações escolares e financeiras de uma escola particular, facilitando o controle de alunos, turmas, responsáveis e mensalidades.

Além da implementação das funcionalidades, o projeto também busca aplicar conceitos de **Programação Orientada a Objetos, arquitetura de software, persistência de dados, tratamento de exceções e padrões de projeto**.
