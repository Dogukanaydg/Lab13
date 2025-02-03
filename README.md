# Lab 13

This repository contains the implementation for Lab 13 of the course. The project demonstrates a basic web application developed using Spring Boot, designed to showcase user management functionality with a connection to a SQLite database.

## Features

- **Environment Variables**: The application uses `.env` files to store database configurations.
- **Model-Repository-Service Architecture**: Implements a clean structure separating concerns.
- **SQLite Integration**: Simple database setup to persist user data.
- **REST API**: Basic endpoints for managing users.

## Requirements

- **Java**: Version 11 or higher
- **Gradle**: To build and run the project

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/Dogukanaydg/Lab13.git
   cd Lab13
   ```

2. Configure the `.env` file:
   ```plaintext
   DATABASE_URL=jdbc:sqlite:database.db
   ```

3. Build the project:
   ```bash
   ./gradlew build
   ```

4. Run the application:
   ```bash
   ./gradlew bootRun
   ```

5. Access the application:
   Open your browser and navigate to [http://localhost:8080](http://localhost:8080).

## Folder Structure

- `src/main/java/com/example/lab13`:
  - `model`: Contains the `User` entity class.
  - `repository`: Contains the `UserRepository` interface.
  - `service`: Contains the `UserService` class for business logic.
  - `controller`: Contains the controller to handle HTTP requests.

- `.env` and `.env.example`:
  Used for environment variable configurations.

- `build.gradle`:
  Gradle build configuration.

## Notes

- Ensure that you have SQLite installed and properly configured if testing outside the embedded setup.
- Use `gradlew` for consistent Gradle wrapper support.

---

