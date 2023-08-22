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
***
### Backend with FastAPI:
The backend of the web project is built using FastAPI, a high-performance web framework for Python. FastAPI offers an intuitive and efficient way to develop APIs with automatic validation, serialization, and documentation generation. This ensures that the backend code is both reliable and well-documented, making maintenance and expansion easier. Here's a breakdown of the folders and their contents:

1. **api:** The 'api' folder is where you'll define the routes and business logic of your application's API. You would have separate files for each route or set of related routes. These files define the HTTP endpoints, request handling, and API logic.
2. **core:** This folder is the heart of your backend application, containing essential configurations and settings, such as settings for environment variables, application parameters, configuration of logs, and other crucial configurations needed to run your application.
3. **database:** The 'database' folder contains everything related to the database interactions of your application:
* **logs:** The 'logs' sub-folder is dedicated to the storage of log files that capture various events and activities related to your application's database interactions. This strategic inclusion of logs in the 'database' folder offers several advantages: Consolidated Tracking,Configurable Logging ...
* **connection.py:** Here, you'll find code related to establishing connections to your database. This might include database connection settings, database engine setup.
4. **models:** This folder would contain the data models or schema definitions for your application's database tables. These models define the structure of your data and how it's stored in the database.
5. **requirements.txt:** The 'requirements.txt' file is used to specify the dependencies your project relies on. These dependencies will be installed when setting up your application. This file is particularly useful when you're using Docker to containerize your application, ensuring that the necessary dependencies are included.
6. **Dockerfile:** This Dockerfile sets up an environment that's capable of running a FastAPI application. It installs necessary dependencies, copies your application code, and configures the execution command. When you build and run a container using this Dockerfile, it will host your FastAPI web application on port 8000 within the container. **the port mentioned in the Dockerfile is just an example port number. When you use this Dockerfile to build and run your container, you can replace the port number with the actual port that you intend to use for your FastAPI application.**.
***
### Frontend with React:
Our skeleton of frontend is organized into various folders, each serving a specific purpose and contributing to the overall structure and functionality of your application.

1. **Assets:** The 'assets' folder contains static assets such as images, icons, fonts, and other files that are used in your application's user interface.
2. **components:** The 'components' folder houses reusable UI components that are used throughout your application. Components are modular building blocks of your interface, designed to be easily integrated and reused across different parts of your application. Organizing them in this folder encourages consistency in design and functionality.
3. **helpers:** The 'helpers' folder likely contains utility functions or helper modules that assist in various tasks across your application. These functions might perform common calculations, formatting, data manipulation, or other tasks that are used in multiple places within your codebase.
4. **hooks:** The 'hooks' folder might hold custom React hooks that encapsulate certain logic or behaviors that can be shared across different components.
5. **layouts:** The 'layouts' folder contains layout components that define the overall structure of different pages or sections of your application. Layout components help maintain a consistent visual and structural theme across your app's various views.
6. **pages:** Within the 'pages' folder, you organize your application's views or screens, each corresponding to a distinct page or route in your app. Each page can consist of multiple components, and this separation allows you to manage and update each page's functionality independently.
7. **utils:** The 'utils' folder is a place for housing utility functions, modules, or classes that are not directly tied to UI components but serve various purposes throughout your application. These utilities can include functions related to data manipulation, API calls.
8. **.env:** The ".env" configuration file is utilized during app development to store environment variables that impact app behavior. It contains settings such as port numbers ("PORT") and API URLs ("REACT_APP_API") . These placeholders like "PORT" and "URL" need to be substituted with actual values pertinent to the app's requirements before building. 
***
### Docker Compose:

 you can make changes in the following places:

* **Image Names:** Replace **stm-skeleton-back** and **stm-skeleton-frontv with the actual image names for your backend and frontend.
* **Container Names:** Change the container_name values to something relevant for your application.
* **Port Mapping:** Modify the host ports to whatever ports you want to use for accessing the backend and frontend from your host machine.
* **Environment Variables:** Adjust the environment variables under the db service to match your desired database configuration.

