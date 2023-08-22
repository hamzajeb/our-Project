# STM-skeleton
STM offers a comprehensive range of services, including the creation of web projects. One of their specialized services involves the development of web projects that utilize the FastAPI framework for the backend and React for the frontend. This combination of cutting-edge technologies ensures a robust and modern web application.

## STM Web Project Skeleton Description
The STM's web project skeleton provides a solid foundation for building web applications. It includes:
* **Directory Structure:** A well-organized directory structure that separates backend and frontend code, making it easier to manage and maintain the project.
* **Backend Configuration:** Pre-configured settings for the FastAPI backend, including routing, authentication, and database connectivity.
* **Frontend Setup:** A base setup for the React frontend, including essential libraries and tools for state management, routing, and styling.
* **API Integration:** Integration between the backend API (built with FastAPI) and the frontend components (built with React), enabling seamless communication between the two parts of the application.
* **PostgreSQL Database:** The application employs PostgreSQL as the relational database management system. PostgreSQL's reliability, extensibility, and advanced features make it a preferred choice for storing and managing structured data. The backend communicates with the database to store, retrieve, and manipulate information.
* **Docker Containerization:** The skeleton includes Dockerfiles for both the frontend and backend components. Docker provides a consistent and isolated environment for development, testing, and deployment. This approach ensures that the application runs consistently across different environments, minimizing potential deployment issues.
* **docker-compose.yml:** The docker-compose.yml file orchestrates the deployment of the frontend, backend, and database containers. It simplifies the setup by defining the services, their configurations, and dependencies. With a single command, developers can start the entire application stack, facilitating collaboration and testing.

### Backend with FastAPI:
The backend of the web project is built using FastAPI, a high-performance web framework for Python. FastAPI offers an intuitive and efficient way to develop APIs with automatic validation, serialization, and documentation generation. This ensures that the backend code is both reliable and well-documented, making maintenance and expansion easier. Here's a breakdown of the folders and their contents:

1. **api:** The 'api' folder is where you'll define the routes and business logic of your application's API. You would have separate files for each route or set of related routes. These files define the HTTP endpoints, request handling, and API logic.
2. **core:** This folder is the heart of your backend application, containing essential configurations and settings, such as settings for environment variables, application parameters, and other crucial configurations needed to run your application.
3. **database:** The 'database' folder contains everything related to the database interactions of your application.
 * **connection.py**: Here, you'll find code related to establishing connections to your database. This might include database connection settings, database engine setup.
4. **models:** This folder would contain the data models or schema definitions for your application's database tables. These models define the structure of your data and how it's stored in the database.
5. **requirements.txt:** The 'requirements.txt' file is used to specify the dependencies your project relies on. These dependencies will be installed when setting up your application. This file is particularly useful when you're using Docker to containerize your application, ensuring that the necessary dependencies are included.
6. **Dockerfile:** This Dockerfile sets up an environment that's capable of running a FastAPI application. It installs necessary dependencies, copies your application code, and configures the execution command. When you build and run a container using this Dockerfile, it will host your FastAPI web application on port 8000 within the container. **the port mentioned in the Dockerfile is just an example port number. When you use this Dockerfile to build and run your container, you can replace the port number with the actual port that you intend to use for your FastAPI application.**.

### Frontend with React:

