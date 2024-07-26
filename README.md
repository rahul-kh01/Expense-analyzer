

# Expense-Tracker-API

REST API for tracking expenses.

A RESTful API created using Spring Boot. We have used PostgreSQL as the relational database and JdbcTemplate to interact with it. Additionally, JSON Web Token (JWT) is used for authentication. JWT helps protect certain endpoints, ensuring that users must be logged in to access them.

## Used Tools and Technologies:

- Spring Boot 3.0.10

  >. spring-boot-devtools
  >. spring-boot-starter-jdbc
  >. spring-boot-starter-web
  >. JSON Web Token (JWT)

- DataBase

  >. postgresql

- Tools

  >. STS (Spring Tool Suite)
  >. PostMan

## Setup and Installation

1. **Clone the repo from GitHub**
   ```sh
   git clone https://github.com/rahul_kh01/Expense-analyzer.git
   cd expense-tracker-api
   ```

2. **Create database objects**

   In the root application directory (`expense-tracker-api`), there is an SQL script file (`expensetracker_db.sql`) for creating all database objects.

3. **Update database configurations in `application.properties`**

   If your database is hosted on a cloud platform or if you have modified the SQL script file with a different username and password, update the `src/main/resources/application.properties` file accordingly:
   ```properties
   spring.datasource.url=jdbc:postgresql://localhost:5432/expensetrackerdb
   spring.datasource.username=expensetracker
   spring.datasource.password=password
   ```

4. **Run the Spring Boot application**
   ```sh
   ./mvnw spring-boot:run
   ```
   This runs on port 8080, so all endpoints can be accessed starting from `http://localhost:8080`.

---
