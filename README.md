# Store API Bruno

## API Test Suite

This project is an API with architecture RestFul for an online store. The tests are designed to ensure that all API functionalities work correctly, including the creation, reading, updating, and deletion of products.

## Directory Structure

The test project is structured to ensure clear organization and ease of maintenance:

- `spec/`: This directory contains all the test files organized by functionality. Each subdirectory within `spec/` corresponds to a specific functionality of the application. 

    Example:
    - `auth/`: Contains tests related to authentication

### Successful Test Cases

The successful test cases verify that the API works correctly under normal conditions. These cases include:

- **Request Method Validation**: Verifies that the API accepts the correct HTTP method (e.g., GET, POST).
- **Response Status Validation**: Ensures the API responds with the correct HTTP status code (e.g., 200 OK).
- **Response Time Validation**: Checks that the API responds within an acceptable time frame.
- **Headers Validation**: Verifies that the request and response headers are correct.
- **Data Validation**: Ensures that the data returned by the API has the expected types and values.

## Environment File

To execute the tests, an environment file containing the necessary variables is required. This file is located in the `environments` directory and is named `TEST.bru` y `PRODUCTION.bru`. 

## Cloning the project

To clone the project, run the following command in your terminal:

```bash
git clone https://github.com/jonaleo87/store-api-bruno.git
```

Then, navigate to the project directory:

```bash
cd store-api-bruno
```

## Installing Dependencies

Install the necessary dependencies by running:

```bash
npm install
```

## Running test

### From the interface

To running the project from the interface, open your Api-Client `Bruno` y load the collection from the cloned directory 

### From the console

To execute all tests in the "TEST" environment, navigate to the `store-api-bruno` directory and use the following command:

```bash
bru run --env TEST
```

To run tests related to specific functionalities, for example, student categories:

```bash
bru run store-api-bruno/spec/categories.test.bru --env TEST
```

This command will run all test defined in the project and display the result in the console

## Adding New Tests

1. Create a new file in the `spec/` directory corresponding to the functionality.
2. Follow the structure of the existing test files.
3. Ensure each test is documented with clear comments.

## Contributing

Please adhere to the coding conventions and ensure all tests pass before submitting a pull request.

### Coding Conventions

- Use descriptive variable names.
- Follow JavaScript coding standards.
- Ensure all tests pass before submitting a pull request.

### Submitting Pull Requests

1. Create a new branch for your feature or bug fix.
2. Ensure all tests pass.
3. Submit a pull request to the `main` branch.