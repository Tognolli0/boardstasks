# 📋 Board Manager API

Este projeto é uma API robusta para gerenciamento de quadros de tarefas (boards), focada em organizar fluxos de trabalho através de colunas e cartões, utilizando as melhores práticas de desenvolvimento Java.

## 🛠️ Tecnologias e Ferramentas

* **Linguagem:** Java 17
* **Gerenciador de Dependências:** Gradle (Kotlin DSL)
* **Banco de Dados:** PostgreSQL (Suporte a H2 para testes)
* **Migrações:** Liquibase (Gerenciamento de versionamento do esquema do banco)
* **Arquitetura:** Baseada em camadas (Controller, Service, Repository, DTO)

## 🌟 Diferenciais Técnicos

* **Liquibase:** Controle rigoroso de versão do banco de dados, permitindo evolução segura do schema.
* **Gradle DSL:** Configuração de build moderna e performática utilizando Kotlin.
* **RESTful API:** Endpoints estruturados seguindo os padrões de verbos HTTP e códigos de status.

## 📂 Estrutura do Projeto

* `src/main/java`: Contém a lógica de negócio, entidades e controladores.
* `src/main/resources`: Configurações do Spring e arquivos de migração do Liquibase (`db/changelog`).
* `build.gradle.kts`: Configurações de dependências e build do projeto.

## 🚀 Como Iniciar

### Pré-requisitos
* Java 17+ instalado.
* Docker (opcional, para o banco de dados).

### Instalação
1. Clone o repositório:
   ```bash
   git clone [https://github.com/Tognolli0/boardstasks.git](https://github.com/seu-usuario/board.git)
   ./gradlew build
   ./gradlew bootRun


   Método,Endpoint,Descrição
POST,/boards,Cria um novo quadro
GET,/boards/{id},Detalha um quadro e suas colunas
POST,/boards/{id}/columns,Adiciona colunas ao quadro
POST,/cards,Cria uma nova tarefa dentro de uma coluna
PATCH,/cards/{id}/move,Move o card entre colunas
   
   
