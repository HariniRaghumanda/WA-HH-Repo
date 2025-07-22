# Spring WhatsApp Backend API

This is a Spring Boot backend API built for WhatsApp-like chat features using Java, Spring Boot, Swagger, and H2.

# Features

- User Management (Create, View, Delete, Update)
-  Chatroom Creation
-  Message Sending with Attachments (Text, Image, Video)
-  Emoji Reactions to Messages
-  Pagination Support
-  File Validation (≤10MB)
-  API Documentation with Swagger UI

# Swagger UI
 Swagger UI is available locally at `http://localhost:8080/swagger-ui/index.html`.
| Endpoint                              | Method | Description                       |
| ------------------------------------- | ------ | --------------------------------- |
| `/api/users`                          | POST   | Create a new user                 |
| `/api/users`                          | GET    | List all users                    |
| `/api/users/{id}`                     | GET    | View a user profile               |
| `/api/users/{id}`                     | PUT    | Update user profile               |
| `/api/users/{id}`                     | DELETE | Delete a user                     |
| `/api/chatrooms`                      | POST   | Create chatroom                   |
| `/api/chatrooms`                      | GET    | List chatrooms                    |
| `/api/messages`                       | POST   | Send message with file attachment |
| `/api/messages/{id}`                  | GET    | View message                      |
| `/api/messages/chatroom/{chatroomId}` | GET    | List messages with pagination     |
| `/api/messages/{id}/attachment`       | GET    | Download attachment (image/video) |
| `/api/reactions`                      | POST   | Add emoji reaction                |


# Run Locally

```bash
git clone https://github.com/HariniRaghumanda/WA-HH-Repo.git
cd Spring-Whatsapp
mvn spring-boot:run
