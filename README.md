# Product Management System Nunes Sports V1 :soccer: (launched 01/10/2024)

## Overview :eyeglasses:

This is a simple Product Management System developed using Java Spring Boot for the backend, PostgreSQL as the database, and HTML/CSS/JS for the frontend. The system allows users to perform CRUD (Create, Read, Update, Delete) operations on a list of products.

## Prerequisites :exclamation:

Before you begin, ensure you have met the following requirements:

- Java Development Kit (JDK) installed
- Apache Maven or Gradle installed (if not using the Spring Boot CLI)
- PostgreSQL database installed and running
- Git installed
- Your preferred Integrated Development Environment (IDE)

## Getting Started :point_left:

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/product-management.git
    ```

2. Navigate to the project directory:

    ```bash
    cd product-management
    ```

3. **Configure the Database:**

    - Ensure that PostgreSQL is installed and running on your local machine or update the database configuration accordingly.
    
    - Create a new PostgreSQL database for the project with the following columns:

        - `id` (Product ID)
        - `code` (Product Code)
        - `name` (Product Name)
        - `description` (Product Description)
        - `price` (Product Price)

        You can do this using a PostgreSQL client or command line:

        ```sql
        CREATE DATABASE your_database;
        ```

    - Open `src/main/resources/application.properties` and update the database URL, username, and password:

        ```properties
        spring.datasource.url=jdbc:postgresql://localhost:5432/your_database
        spring.datasource.username=your_username
        spring.datasource.password=your_password
        spring.jpa.hibernate.ddl-auto=update
        ```

4. **Build and Run the Project:**

    ```bash
    # Using Maven
    ./mvnw spring-boot:run

    # Using Gradle
    ./gradlew bootRun
    ```

5. Open your web browser and go to [http://localhost:8080](http://localhost:8080) to access the application.

## Project Structure

- `src/main/java/com/example/controller`: Contains the backend controllers.
- `src/main/resources/static`: Contains static resources (CSS, JS).
- `src/main/resources/templates`: Contains HTML templates.

## Technologies Used

- Java Spring Boot
- PostgreSQL
- HTML/CSS/JS (Thymeleaf for templating)

## What's Included

- **Backend:**
    - Spring Boot application with RESTful endpoints for managing products.
    - Integration with a PostgreSQL database for persistent storage.

Future implementations in V2:
- **Frontend:**
    - Simple HTML templates for displaying and interacting with the product data.
    - Basic styling with CSS.
    - JavaScript for asynchronous communication with the backend.
    - Repository:  

## Contributing

Feel free to contribute to this project by opening issues or creating pull requests. Your feedback and contributions are highly appreciated.

## License

This project is licensed under the [MIT License](LICENSE).
