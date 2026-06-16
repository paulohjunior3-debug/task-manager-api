# Task Manager API

API REST para gerenciamento de tarefas, desenvolvida com Java e Spring Boot. Permite criar, listar, atualizar e deletar tarefas com controle de status.

## Tecnologias

- Java 21
- Spring Boot 3.5
- Spring Data JPA
- Banco de dados H2 (em memória)
- Lombok
- Maven

## Como rodar localmente

**Pré-requisitos:** Java 21+ e Maven instalados.

```bash
git clone https://github.com/paulohjunior3-debug/task-manager-api.git
cd task-manager-api
./mvnw spring-boot:run
```

A API estará disponível em `http://localhost:8080`.

## Endpoints

| Método | Rota | Descrição |
|--------|------|-----------|
| GET | /tasks | Listar todas as tarefas |
| GET | /tasks?status=PENDING | Filtrar por status |
| GET | /tasks/{id} | Buscar por ID |
| POST | /tasks | Criar tarefa |
| PUT | /tasks/{id} | Atualizar tarefa |
| DELETE | /tasks/{id} | Deletar tarefa |

## Status disponíveis

| Status | Descrição |
|--------|-----------|
| `PENDING` | Tarefa pendente (padrão) |
| `IN_PROGRESS` | Tarefa em andamento |
| `DONE` | Tarefa concluída |

## Estrutura do projeto

```
src/main/java/com/paulofaria/taskmanager/
├── controller/    
├── service/       
├── repository/    
└── model/         
```

## Autor

**Paulo Henrique** — [LinkedIn](https://www.linkedin.com/in/paulo-faria-dev) · [GitHub](https://github.com/paulohjunior3-debug)
