# Go JWT Project

This is a simple Go project that demonstrates user authentication and authorization using JSON Web Tokens (JWT).

## Getting Started

Follow the instructions below to set up and run the project on your local machine.

### Prerequisites

Make sure you have the following tools installed:

- [Go](https://golang.org/dl/)
- [Gin](https://gin-gonic.com/docs/getting-started/installation/)

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/Mayejacob/go-jwt.git
    ```

2. Change to the project directory:

    ```bash
    cd go-jwt-project
    ```

3. Install dependencies:

    ```bash
    go mod tidy
    ```
4. Run the application:

    ```bash
    go run main.go
    ```

    Or alternatively:

    ```bash
    go run .
    ```

   The server will start on [http://localhost:9000](http://localhost:9000).

## API Endpoints

- **Sign Up:** `POST /users/signup`
- **Login:** `POST /user/login`
- **All Users:** `GET /users`
- **Get User by id:** `GET /users/:user_id`


# MongoDB connection string
mongo_uri: "mongodb://localhost:27017/your-database"

# Authentication Routes

## Signup

- **Endpoint:** `POST /users/signup`
- **Description:** Sign up a new user.
- **Request Body:**

  ```json
  {
    "First_name": "maye",
    "Last_name": "Jayboss",
    "Password": "12345678",
    "email": "test@gmail.com",
    "Phone": "081690000",
    "User_type": "ADMIN"
    }```
     ```json
  {
    "First_name": "maye",
    "Last_name": "Jayboss",
    "Password": "12345678",
    "email": "test@gmail.com",
    "Phone": "081690000",
    "User_type": "USER"
    }```
## login

- **Endpoint:** `POST /users/login`
- **Description:** login user.
- **Request Body:**

  ```json
{
  "email": "john.doe@example.com",
  "password": "your_password"
}```
