# Kaiburr-Task-1 : Server Manager API
Welcome to the Server Manager API, a robust Java-based RESTful service that allows you to effortlessly manage and monitor your server infrastructure. This project showcases the power of Spring Boot and MongoDB in building a seamless API for your server management needs.

## **✨Quick Start**

### **Prerequisites**

Before you embark on this journey, make sure you have these tools installed:

- **Java Development Kit (JDK)**: We recommend Java 8 or higher for maximum awesomeness.
- **Maven**: The trusty companion for building your projects.
- **Spring Boot**: The magic wand for creating robust APIs.
- **MongoDB**: Your trusty data vault.
- **Postman**: Your superhero sidekick for testing API endpoints.
### **Installation**

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
2.**Build and Run the Project**

   mvn clean install
   mvn spring-boot:run

## 🛠️ Features

Discover the incredible features that make this API truly awesome:

1. **Create Servers**: Add new servers effortlessly to your infrastructure.

2. **Retrieve Servers**: Get a complete list of all servers or fetch a specific server by its unique ID.

3. **Update Servers**: Seamlessly update server information using their IDs.

4. **Delete Servers**: Bid farewell to servers that have served their purpose.

5. **Find Servers by Name**: Quickly search for servers by name, because we know naming things can be hard.
.

## 📁 Project Structure



- `src/`: Home to your source code and resources.
  - `main/`: The heart of your application.
    - `java/`: The source code, where the magic happens.
    - `resources/`: Essential resource files and configurations.
  - `test/`: Where we ensure your code behaves like a charm.
    - `java/`: Test source files to guarantee your API is rock-solid.
    - `resources/`: Test-related resources to keep your tests running smoothly.
## 🔍 Implementation Details

Let's dive deeper into the workings of this awesome API:

### Create a Server (POST Request)

Add a new server with a POST request to `/api/servers`. Simply send a JSON request body like this:

Example --JSON Format
{
  "id": "123",
  "name": "New Server",
  "language": "Java",
  "framework": "Spring Boot"
}
### Get Servers (GET Request)

Retrieve all servers or a specific server by its unique ID.

- **Get All Servers**:
  - **Request**: GET `/api/servers`
  - **Description**: Fetch a list of all servers.

- **Get a Server by ID**:
  - **Request**: GET `/api/servers/{id}`
  - **Description**: Retrieve a server with the specified ID.
### Update Server (PUT Request)

To update server details, make a PUT request to `/api/servers/{id}` with the updated JSON information. The server with the specified ID will be updated accordingly.

Example JSON request body for updating a server:

{
  "id": "123",
  "name": "Updated Server Name",
  "language": "Java",
  "framework": "Spring Boot"
}

### Delete Server (DELETE Request)

Bid farewell to a server by sending a DELETE request to `/api/servers/{id}`. The server will gracefully exit your inventory.

### Find Servers by Name (GET Request)

Need to find servers by name? Use `/api/servers/findByName?name=ServerName` to get all servers with matching names.










