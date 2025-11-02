# Backend Java 25 com Spring Boot — Projeto de Portfólio

Este projeto implementa uma API backend moderna utilizando **Java 25** + **Spring Boot**, seguindo padrões e boas práticas adotadas no mercado.
O objetivo é demonstrar um backend profissional com autenticação JWT, CRUD, testes, CI/CD, containerização e boas práticas.

---

## 🚀 Funcionalidades

* ✅ Registro e login de usuários com **JWT**
* ✅ Hash de senha com **BCrypt**
* ✅ CRUD de Clientes protegido por autenticação
* ✅ Controle de permissões (roles)
* ✅ Documentação da API com **OpenAPI/Swagger**
* ✅ Migrações de banco com **Flyway**
* ✅ Banco de dados **PostgreSQL**
* ✅ Execução com **Docker** + `docker-compose`
* ✅ Testes unitários e integrados com **JUnit + Testcontainers**
* ✅ Observabilidade com **Spring Actuator**
* ✅ Qualidade de código (Checkstyle/SpotBugs)
* ✅ Pipeline CI/CD com **GitHub Actions** (build, test e push Docker Hub)

---

## 🏗️ Arquitetura e Tecnologias

| Categoria       | Tecnologia                       |
| --------------- | -------------------------------- |
| Linguagem       | Java 25                          |
| Framework       | Spring Boot                      |
| Autenticação    | Spring Security + JWT            |
| Banco           | PostgreSQL                       |
| Migrations      | Flyway                           |
| Testes          | JUnit 5, Mockito, Testcontainers |
| Container       | Docker / Docker Compose          |
| CI/CD           | GitHub Actions                   |
| Documentação    | OpenAPI / Swagger                |
| Logging         | Logback estruturado              |
| Observabilidade | Spring Actuator + Micrometer     |

---

## 📂 Estrutura do Projeto (simplificada)

```
src/
 ├── main/java/com/app
 │    ├── config
 │    ├── controller
 │    ├── dto
 │    ├── entity
 │    ├── repository
 │    └── service
 ├── test/java/com/app
 │    └── integration
Dockerfile
docker-compose.yml
pom.xml
```

---

## 🐳 Executando via Docker

### **Subir o ambiente**

```bash
docker-compose up --build
```

A API ficará disponível em:

```
http://localhost:8080
```

### **Swagger UI**

```
http://localhost:8080/swagger-ui
```

---

## 🔐 Endpoints Principais

| Endpoint             | Método | Descrição                                   |
| -------------------- | ------ | ------------------------------------------- |
| `/api/auth/register` | POST   | Registrar usuário                           |
| `/api/auth/login`    | POST   | Autenticar e receber JWT                    |
| `/api/clients`       | CRUD   | Gerenciamento de clientes (JWT obrigatório) |

---

## 🧪 Testes

* **JUnit 5**
* **Mockito**
* **Testcontainers** (PostgreSQL real em container)

```bash
mvn test
```

---

## ⚙️ CI/CD

Pipeline automática com **GitHub Actions**:

* Build e testes
* Análise de código
* Build de imagem Docker
* Push para Docker Hub

---

## 🎯 Objetivo do Projeto

Demonstração profissional de:

* Arquitetura limpa com Spring
* Autenticação segura com JWT
* Testes e qualidade de código
* CI/CD moderno
* Infraestrutura com containers

Este repositório serve como base para aplicações corporativas e estudo de boas práticas em Java.

---

## ⭐ Como Contribuir

Fique à vontade para:

* Abrir PRs
* Sugerir melhorias
* Reportar issues
* Deixar uma ⭐ se gostar!

---

📩 Em breve: link para versão em produção!
