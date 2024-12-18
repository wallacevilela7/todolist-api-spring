# Spring Boot To-Do List

Este repositório é uma aplicação simples de lista de tarefas (To-Do List) desenvolvida como parte do curso de introdução ao Spring Boot oferecido pela Build & Run. O projeto foi desenvolvido com foco em compreender os conceitos fundamentais do Spring Boot, incluindo:

- Estrutura de projetos no Spring Boot.
- Desenvolvimento de APIs REST.
- Validações e boas práticas.

## Funcionalidades

- **Criar tarefas**: Adicionar uma nova tarefa à lista.
- **Listar tarefas**: Visualizar todas as tarefas cadastradas.
- **Atualizar tarefas**: Editar o título ou status de uma tarefa.
- **Excluir tarefas**: Remover uma tarefa da lista.
- **Excluir todas tarefas**: Limpa a lista de tarefas.

## Tecnologias Utilizadas

- **Java 21**
- **Spring Boot 3.4.0**

- **Maven** (gerenciador de dependências)

## Endpoints da API

### **Criar uma tarefa**
- **POST** `/tasks`
- **Body**:
  ```json
  {
    "id" : 1,
    "description": "Tarefa 1"
  }
  ```
- **Response**:
  ```json
  {
    "id" : 1,
    "description": "Tarefa 1"
  }
  ```

### **Listar tarefas**
- **GET** `/tasks`
- **Response**:
  ```json
  [
    {
      "id": 1,
      "description": "Desenvolver o projeto"
    },
  {
      "id": 2,
      "description": "Testar o projeto"
    }
  ]
  ```

### **Atualizar tarefa**
- **PUT** `/tasks/{id}`
- **Body**:
  ```json
  {
    "description": "Desenvolver o projeto - ok",
  }

### **Excluir tarefa**
- **DELETE** `/tasks/{id}`
- **Response**: `204 No Content`

## Como Executar o Projeto

1. Clone o repositório:
   ```bash
   git clone <url-do-repositorio>
   ```
2. Navegue até o diretório do projeto:
   ```bash
   cd todolistapp
   ```
3. Execute o projeto utilizando o Maven:
   ```bash
   ./mvnw spring-boot:run
   ```
4. Acesse a aplicação no navegador ou via Postman em: [http://localhost:8080](http://localhost:8080).


## Contribuição

Se desejar contribuir com melhorias ou novas funcionalidades, sinta-se à vontade para abrir uma issue ou enviar um pull request.

