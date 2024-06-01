# Design Document
 

## Personal Finance Management System

 

### Table of Contents

1. Introduction
    1.1 Purpose
    1.2 Scope
    1.3 Definitions, Acronyms, and Abbreviations
    1.4 References

2. System Overview

3. Design Considerations

    3.1 Assumptions and Dependencies

    3.2 Constraints

    3.3 System Environment

4. System Architecture

    4.1 Architectural Design

    4.2 Component Design

5. Data Design

    5.1 Data Description

    5.2 Data Dictionary

6. Component Design

    6.1 Web Application

    6.2 API Gateway

    6.3 Services

        6.3.1 Authentication Service

        6.3.2 Expense Management Service

        6.3.3 Income Management Service

        6.3.4 Budget Management Service

        6.3.5 Goal Management Service

        6.3.6 Notes and Tagging Service

    6.4 Database

7. User Interface Design

8. Design Principles

9. Conclusion

 

## 1. Introduction

 

### 1.1 Purpose

The purpose of this document is to provide a comprehensive design overview of the Personal Finance Management System (PFMS), outlining the architecture, data design, component interactions, and user interface.

 

### 1.2 Scope

This document covers the design aspects of the PFMS including its web application, API gateway, microservices, and database interactions.

 

### 1.3 Definitions, Acronyms, and Abbreviations

- **PFMS**: Personal Finance Management System

- **JWT**: JSON Web Token

- **API**: Application Programming Interface

- **UI**: User Interface

 

### 1.4 References

- [SWEBOK](https://www.computer.org/education/bodies-of-knowledge/software-engineering)
 

## 2. System Overview

The PFMS is a web-based application designed to help users manage their personal finances. It includes features for tracking expenses, managing budgets, setting financial goals, and maintaining financial notes.

 

## 3. Design Considerations

 

### 3.1 Assumptions and Dependencies

- The system will be deployed in a cloud environment.

- Users will access the system via modern web browsers.

- The backend will use Java Spring Boot and the database will be PostgreSQL.

 

### 3.2 Constraints

- The application must be built using Java 15 and Spring Boot.

- Data must be stored in a PostgreSQL database.

- Security must be handled using JWT.

 

### 3.3 System Environment

The system will operate on a cloud-based environment, utilizing microservices architecture for scalability and maintainability.

 

## 4. System Architecture

 

### 4.1 Architectural Design

The PFMS follows a microservices architecture. The main components include:

- Web Application (Frontend)

- API Gateway

- Microservices (Authentication, Expense Management, Income Management, Budget Management, Goal Management, Notes and Tagging)

- PostgreSQL Database

 

### 4.2 Component Design

Each microservice is independently deployable and communicates with the others via RESTful APIs.

 

## 5. Data Design

 

### 5.1 Data Description

The primary data entities include users, expenses, incomes, budgets, goals, and notes.

 

### 5.2 Data Dictionary

- **User**: Contains user information such as email, password, and profile details.

- **Expense**: Contains details of expenses logged by the user.

- **Income**: Contains details of income entries logged by the user.

- **Budget**: Contains budget information set by the user.

- **Goal**: Contains financial goals set by the user.

- **Note**: Contains financial notes and tags created by the user.

 

## 6. Component Design

 

### 6.1 Web Application

The web application is developed using React, providing the user interface for interacting with the system.

 

### 6.2 API Gateway

The API Gateway, developed with Spring Boot, acts as a single entry point for all client requests and routes them to the appropriate microservices.

 

### 6.3 Services

 

#### 6.3.1 Authentication Service

Handles user registration, login, and JWT authentication.

 

#### 6.3.2 Expense Management Service

Manages expense entries including creation, updating, and deletion.

 

#### 6.3.3 Income Management Service

Manages income entries including creation, updating, and deletion.

 

#### 6.3.4 Budget Management Service

Allows users to set and track budgets.

 

#### 6.3.5 Goal Management Service

Enables users to set and monitor financial goals.

 

#### 6.3.6 Notes and Tagging Service

Provides functionality for creating and managing financial notes and tags.

 

### 6.4 Database

PostgreSQL is used to store all application data securely.

 

## 7. User Interface Design

The UI is designed to be intuitive and user-friendly, with components for managing expenses, incomes, budgets, goals, and notes.

 

## 8. Design Principles

The design of PFMS follows these principles:

- **Modularity**: Each service is a separate module that can be developed, deployed, and scaled independently.

- **Security**: Uses JWT for secure authentication.

- **Scalability**: Microservices architecture ensures the system can scale horizontally.

- **Maintainability**: Clear separation of concerns between different services.

## 9. Conclusion 

This document follows the guidelines from the SWEBOK, incorporating important design principles and activity diagrams to give a clear and detailed understanding of the system.
