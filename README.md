# 🎓 Sistema Evento — Prática de Modelagem de Domínio com Spring Boot e JPA

Projeto desenvolvido em **Java com Spring Boot** com o objetivo de praticar modelagem de domínio, mapeamento objeto-relacional (ORM) e persistência de dados utilizando **Spring Data JPA e Hibernate**.

O sistema simula o gerenciamento de atividades de um evento acadêmico, servindo como um exercício prático para aplicar conceitos de arquitetura, modelagem orientada a objetos e relacionamento entre entidades.

---

## 👨‍💻 Sobre o Projeto

O sistema simula um cenário onde é possível gerenciar:

- Participantes
- Atividades (cursos, oficinas, palestras, etc.)
- Categorias de atividades
- Blocos de horários

Regras modeladas:

- Um participante pode se inscrever em várias atividades
- Uma atividade pode possuir vários participantes
- Cada atividade pertence a uma categoria
- Uma atividade pode possuir múltiplos blocos de horário (datas e intervalos)

O foco principal foi a correta representação dessas relações no modelo de domínio.

---

## 🧩 Modelagem de Domínio

A implementação foi guiada por modelagem UML, utilizada como base para estruturação das entidades e seus relacionamentos.

### 📊 Diagrama de Classes

![Diagrama de Classes](docs/Diagrama-classes.png)

O diagrama apresenta as entidades principais e suas associações, refletidas diretamente no mapeamento JPA.

---

## 🧪 Seeding de Dados

Para validação do modelo e facilitar testes, o projeto inclui seeding automático da base de dados.

### 📊 Diagrama de Objetos

![Diagrama de Objetos](docs/Diagrama-objetos.png)

Os dados simulam um cenário coerente de participantes e atividades em um evento acadêmico.

---

## 🏗️ Arquitetura do Projeto

Organização simples em camadas para separação de responsabilidades:

- **Domain**
    - Entidades e modelagem do negócio
- **Repository**
    - Interfaces de acesso a dados com Spring Data JPA
- **Config**
    - Configuração e carga inicial (seeding) da base

O objetivo foi exercitar organização básica de um projeto Spring Boot.

---

## 🚀 Tecnologias Utilizadas

- Java
- Spring Boot
- Spring Data JPA
- Hibernate
- Banco H2 (em memória)
- Maven

---

## 🧠 Conceitos Praticados

- Modelagem de domínio orientada a objetos
- Relacionamentos JPA:
    - Many-to-Many
    - One-to-Many
    - Many-to-One
- ORM com Hibernate
- Geração automática de schema
- Seeding de dados
- Organização básica em camadas

---
