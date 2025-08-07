# event-management

Este projeto é uma aplicação de gerenciamento de eventos.

---

## Como usar as massas de teste (Exemplos de cURL)

Para interagir com a API de gerenciamento de eventos, você pode usar os comandos `curl` abaixo. Certifique-se de que a aplicação esteja rodando em `http://localhost:8080`.

### 1. Listar Eventos
curl http://localhost:8080/api/events

### 2. Buscar por IDs
curl http://localhost:8080/api/events/1

### 3. Criar Evento
curl -X POST http://localhost:8080/api/events \
-H "Content-Type: application/json" \
-d '{
  "titulo": "Meu Evento",
  "descricao": "Descrição do evento",
  "dataEvento": "2025-12-25T10:00:00",
  "local": "Local do Evento"
}'

### 4. Atualizar Evento
curl -X PUT http://localhost:8080/api/events/1 \
-H "Content-Type: application/json" \
-d '{
  "titulo": "Evento Atualizado",
  "descricao": "Nova descrição",
  "dataEvento": "2025-12-26T14:00:00",
  "local": "Novo Local"
}'

### 5. Deletar Evento
curl -X DELETE http://localhost:8080/api/events/1


