# Family Cash Card REST API & Security

A comprehensive RESTful Web Service built with **Spring Boot 3**, **Spring Data JDBC**, and **Spring Security**, strictly developed using **Test-Driven Development (TDD)** methodologies based on the VMware / Broadcom Spring Academy curriculum.

## 🚀 Features & Key Implementation
- **Full RESTful CRUD Operations:** Implemented endpoints for resource creation (`POST`), retrieval (`GET` single & paginated list), update (`PUT`), and deletion (`DELETE`).
- **Persistence Layer:** Integrated **Spring Data JDBC** for database interactions and object relational mapping.
- **Security & Authorization:** Integrated **Spring Security** enforcing Role-Based Access Control (RBAC) to ensure resource isolation per authenticated user.
- **Test-Driven Development (TDD):** Authored integration test suites following the Red-Green-Refactor cycle using **JUnit 5**, **AssertJ**, and **TestRestTemplate**.

## 🛠️ Tech Stack
- **Framework:** Spring Boot 3, Spring Web, Spring Data JDBC, Spring Security
- **Language:** Java 17
- **Testing:** JUnit 5, TestRestTemplate, AssertJ
- **Build Tool:** Maven

## 🔗 API Endpoints Summary
| HTTP Method | Endpoint | Description | Auth Required | Status Code |
| :--- | :--- | :--- | :--- | :--- |
| `GET` | `/cashcards/{id}` | Fetch Cash Card by ID | Yes | `200 OK` / `404 NOT FOUND` |
| `GET` | `/cashcards` | Fetch Paginated List | Yes | `200 OK` |
| `POST` | `/cashcards` | Create New Card | Yes | `201 CREATED` |
| `PUT` | `/cashcards/{id}` | Update Existing Card | Yes | `204 NO CONTENT` |
| `DELETE` | `/cashcards/{id}` | Delete Cash Card | Yes | `204 NO CONTENT` |
