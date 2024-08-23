# DIO - Trilha .NET - API e Entity Framework: Gerenciador de Tarefas💻

Este repositório contém a solução para o desafio de projeto da trilha .NET - API e Entity Framework da DIO, que consiste em desenvolver um sistema gerenciador de tarefas com CRUD completo.

## 📜Descrição do Projeto

O sistema gerenciador de tarefas permite aos usuários cadastrar, visualizar, editar e excluir suas tarefas, auxiliando na organização da rotina. As funcionalidades implementadas incluem:

### CRUD completo: 
Criação, leitura, atualização e exclusão de tarefas.

### Entity Framework: 
Utilizado para a persistência dos dados em um banco de dados.

### Swagger: 
Documentação interativa da API para facilitar o uso e teste dos endpoints.

![Métodos Swagger](swagger.png)

### Endpoints específicos: 
Métodos para buscar tarefas por ID, título, data, status e obter todas as tarefas.

**Endpoints**

| Verbo  | Endpoint                | Parâmetro | Body          |
|--------|-------------------------|-----------|---------------|
| GET    | /Tarefa/{id}            | id        | N/A           |
| PUT    | /Tarefa/{id}            | id        | Schema Tarefa |
| DELETE | /Tarefa/{id}            | id        | N/A           |
| GET    | /Tarefa/ObterTodos      | N/A       | N/A           |
| GET    | /Tarefa/ObterPorTitulo  | titulo    | N/A           |
| GET    | /Tarefa/ObterPorData    | data      | N/A           |
| GET    | /Tarefa/ObterPorStatus  | status    | N/A           |
| POST   | /Tarefa                 | N/A       | Schema Tarefa |



## 📔Estrutura do Projeto
O projeto está organizado da seguinte forma:

### Data: 
Contém a classe TarefaContext para interagir com o banco de dados.

### Controllers: 
Contém os controladores da API para gerenciar as tarefas.

### Models:
Contém a definição da classe Tarefa.

```json
{
  "id": 0,
  "titulo": "string",
  "descricao": "string",
  "data": "2022-06-08T01:31:07.056Z",
  "status": "Pendente"
}
```

## 🔍Observações
O código foi desenvolvido de acordo com as especificações do desafio.
