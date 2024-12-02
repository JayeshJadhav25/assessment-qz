# Quiz App API

## Setup and Running the Service

### Prerequisites

- **Node.js Version**:Ensure you are using Node.js version 18 or greater. You can manage your Node.js version using [nvm (Node Version Manager)](https://github.com/nvm-sh/nvm).

- **Docker** : Install Docker to simplify the deployment and management of the application.

# Using Docker

1. ## Clone the repository :
   ```bash
   git clone https://github.com/JayeshJadhav25/assessment-qz.git
   cd assement-qz
    ```

2. ## Build and run with Docker :

    Make sure Docker is installed and running. Then, execute the following command:

    ### To build and run the app:
      ```bash
      docker-compose up --build 
      ```
    ### Or to run in detached mode 
      ```bash
    docker-compose up --build -d
      ```

3. # Access the App :

     The API will be accessible at: http://localhost:3000
    
     Swagger documentation will be accessible at: http://localhost:3000/api-docs



# Running Without Docker

## If you prefer not to use Docker, you can run the app locally:

1. ## Clone the repository :
   ```bash
   git clone https://github.com/JayeshJadhav25/assessment-qz.git
   cd assement-qz
    ```


2. ## Install Node.js : 

    Ensure you are using Node.js version 18 or greater. You can check your Node.js version with:
   ```bash
    node -v
    ```

3. ## Install dependencies :
   ```bash
    npm install
    ```

4. ## Run the app :
   ```bash
    npm start
    ```

5. ## Access the App :

    The API will be accessible at: http://localhost:3000
    Swagger documentation will be accessible at: http://localhost:3000/api-docs


# Running Unit Tests
The unit tests for the API and core logic are written using Jest. To run the tests, follow these steps:

## Install Jest (if not already installed):

  ```bash
  npm install --save-dev jest
  ```
## Run Tests:

To run all tests, execute the following command:

  ```bash
  npm test
  ```

# API Documentation

The API documentation is available via Swagger at:
http://localhost:3000/api-docs


# Design Overview

## Architecture

The application follows a RESTful API architecture where each endpoint represents a resource (such as quizzes, answers, etc.). This design was chosen for simplicity and scalability.

## Technologies Used

 **` Node.js `** : We chose Node.js for its asynchronous, event-driven architecture, which is well-suited for building scalable APIs. 

 **` Docker `** : Docker was chosen to containerize the application, ensuring that it runs consistently across different environments. This also simplifies the deployment process.
 
 **` In-memory Map `**: The application stores data in memory using a JavaScript Map object


## API Design

We followed RESTful principles for designing the API. Each resource is mapped to an endpoint (e.g., /quiz/submit/answer).

## Testing

The backend API has been tested using Postman for manual testing of each endpoint. Unit testing was implemented for core logic using Jest.









