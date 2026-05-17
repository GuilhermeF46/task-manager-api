# Task Manager API

API REST desenvolvida com Spring Boot para gerenciamento de tarefas, utilizando PostgreSQL e arquitetura em camadas.

---

## 🚀 Tecnologias

- Java 21
- Spring Boot
- Spring Data JPA
- PostgreSQL
- Maven
- Swagger / OpenAPI
- Render (Deploy)
- Neon (Database)

---

## 📌 Funcionalidades

- Criar tarefas
- Listar tarefas com paginação e ordenação
- Buscar tarefa por ID
- Atualizar tarefa
- Remover tarefa
- Marcar tarefa como concluída
- Marcar tarefa como prioridade
- Validação de dados
- Tratamento global de exceções

---

## 🧱 Arquitetura

O projeto segue arquitetura em camadas:

```text
Controller → Service → Repository → Database
```

Estrutura:

```text
src/main/java
├── controller
├── service
├── repository
├── entity
├── dto
└── exception
```

---

## 🌐 API Online

Base URL:

```text
https://task-manager-api-qxrn.onrender.com
```

---

## 📄 Documentação Swagger

Disponível em:

```text
https://SUA-API.onrender.com/swagger-ui.html
```

---

## ⚙️ Executando localmente

### 1. Clonar repositório

```bash
git clone https://github.com/GuilhermeF46/task-manager-api.git
```

### 2. Configurar variáveis

No `application.properties`:

```properties
spring.datasource.url=YOUR_DATABASE_URL
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD
```

### 3. Rodar aplicação

```bash
./mvnw spring-boot:run
```

---

## 📌 Endpoints

| Método | Endpoint | Descrição |
|---|---|---|
| GET | `/tasks` | Lista tarefas por paginação e ordenação |
| GET | `/tasks/{id}` | Busca por ID |
| POST | `/tasks` | Cria tarefa |
| PUT | `/tasks/{id}` | Atualiza tarefa |
| PATCH | `/tasks/{id}/complete` | Marca como concluída |
| PATCH | `/tasks/{id}/priority` | Marca prioridade da tarefa |
| DELETE | `/tasks/{id}` | Remove tarefa por ID |
| DELETE | `/tasks` | Remove todas tarefas |

---

## 📦 Exemplo de requisição

### POST `/tasks`

```json
{
  "description": "Limpar telhado"
}
```

---

## ☁️ Deploy

Aplicação hospedada no:

- Render (API)
- Neon (PostgreSQL)

---

## 👨‍💻 Autor

Guilherme Ferreira dos Santos
