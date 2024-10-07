# API Testing with REST Assured

## Project Overview
This project focuses on API testing using the REST Assured library in Java. The aim is to validate various endpoints of the DummyJSON API, covering authentication and product management functionalities.

## Objective
To understand how to perform different types of HTTP requests (GET, POST, PUT, DELETE) using REST Assured and validate the specified endpoints of the DummyJSON API.

## Tools Required
- **IDE**: Spring Tool Suite or Eclipse for Java development.
- **Dependencies**: REST Assured library for HTTP requests.

## Endpoints to Validate

### Auth API: `https://dummyjson.com/docs/auth`
- **Login and Get Token**
  - Request:
    ```json
    {
      "username": "emilys",
      "password": "emilyspass",
      "expiresInMins": 30
    }
    ```
- **Get Auth User**
- **Refresh Token**

### Products API: `https://dummyjson.com/docs/products`
- **Get all Products**
- **Get a Single Product**
- **Search Products**
- **Limit and Skip Products**
- **Sort Products**
- **Get all Product Categories**
- **Get Products Categories List**
- **Get Products of Category**
- **Add a Product**
- **Update a Product**
- **Delete a Product**

## Implementation Steps

### 1. Create a New Maven Project
Create a new Maven project in Spring Tool Suite or Eclipse.

### 2. Add Dependencies
Add the required dependencies in the `pom.xml` file:

```xml
<dependencies>
    <dependency>
        <groupId>io.rest-assured</groupId>
        <artifactId>rest-assured</artifactId>
        <version>5.4.0</version>
        <scope>test</scope>
    </dependency>
    <dependency>
        <groupId>org.hamcrest</groupId>
        <artifactId>hamcrest</artifactId>
        <version>2.2</version>
    </dependency>
</dependencies>
