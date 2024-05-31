# Software Requirements Specification (SRS)

## 1. Introduction

### 1.1 Purpose
The purpose of this document is to provide a detailed description of the Personal Finance Management System (PFMS). This SRS will outline the system's functionality, performance, and interface requirements.

### 1.2 Scope
The PFMS is designed to help users manage their personal finances. It allows users to track their expenses, incomes, set financial goals, and manage their budgets. The system provides user registration, login, and various financial tracking features.

### 1.3 Definitions, Acronyms, and Abbreviations
- **PFMS**: Personal Finance Management System
- **SRS**: Software Requirements Specification
- **JWT**: JSON Web Token
- **API**: Application Programming Interface
- **UI**: User Interface

### 1.4 References
- [GitHub Repository](https://github.com/hardikSinghBehl/personal-finance-management-system)
- Swagger-UI for API documentation

## 2. Overall Description

### 2.1 Product Perspective
The PFMS is a standalone system that utilizes Java Spring Boot for the backend and PostgreSQL for the database. It employs Spring Security for authentication and authorization using JWT.

### 2.2 Product Functions
- User registration and authentication
- Expense and income tracking
- Budget management
- Financial goal setting
- Monthly spending thresholds
- Financial notes and tagging system

### 2.3 User Classes and Characteristics
- **Registered Users**: Can access all features after logging in.
- **Guests**: Can only register and login.

### 2.4 Operating Environment
- **Server**: Java 15, Spring Boot, PostgreSQL
- **Client**: Any web browser

### 2.5 Design and Implementation Constraints
- The application must use Java 15.
- The database must be PostgreSQL.
- Authentication must be handled via JWT.

### 2.6 User Documentation
- Setup and usage instructions are provided in the README file on the GitHub repository.

## 3. System Features

### 3.1 User Registration and Login
#### 3.1.1 Description
Users can register by providing their email, password, and other required details. They can log in using their credentials to access the system.

#### 3.1.2 Functional Requirements
- **FR1**: The system shall allow users to register.
- **FR2**: The system shall authenticate users via JWT upon login.

### 3.2 Expense and Income Tracking
#### 3.2.1 Description
Users can log their expenses and incomes, categorize them, and view a summary.

#### 3.2.2 Functional Requirements
- **FR3**: The system shall allow users to add, edit, and delete expenses.
- **FR4**: The system shall allow users to add, edit, and delete incomes.

### 3.3 Budget Management
#### 3.3.1 Description
Users can set budgets for different categories and track their spending against these budgets.

#### 3.3.2 Functional Requirements
- **FR5**: The system shall allow users to set and update budgets.
- **FR6**: The system shall provide a summary of budget vs. actual spending.

### 3.4 Financial Goal Setting
#### 3.4.1 Description
Users can set financial goals and track their progress.

#### 3.4.2 Functional Requirements
- **FR7**: The system shall allow users to set financial goals.
- **FR8**: The system shall track progress towards these goals.

### 3.5 Monthly Spending Thresholds
#### 3.5.1 Description
Users can set monthly spending limits and receive alerts if they exceed them.

#### 3.5.2 Functional Requirements
- **FR9**: The system shall allow users to set monthly spending thresholds.
- **FR10**: The system shall automatically calculate and report spending at the end of each month.

### 3.6 Financial Notes and Tagging
#### 3.6.1 Description
Users can create notes and assign tags for easier tracking and categorization.

#### 3.6.2 Functional Requirements
- **FR11**: The system shall allow users to create, edit, and delete financial notes.
- **FR12**: The system shall allow users to assign tags to expenses, incomes, and notes.

## 4. External Interface Requirements

### 4.1 User Interfaces
- **Login Page**
- **Dashboard**
- **Expense/Income Entry Forms**
- **Budget Management Page**
- **Goal Tracking Page**
- **Notes and Tagging Page**

### 4.2 Hardware Interfaces
No specific hardware interfaces are required.

### 4.3 Software Interfaces
- PostgreSQL for database management
- Java Spring Boot for backend services
- Swagger-UI for API documentation

### 4.4 Communication Interfaces
- HTTPS for secure communication between client and server

## 5. Other Nonfunctional Requirements

### 5.1 Performance Requirements
- The system should handle up to 100 concurrent users.
- Responses to user actions should be within 2 seconds.

### 5.2 Safety Requirements
- Data integrity must be ensured during all CRUD operations.

### 5.3 Security Requirements
- User data must be secured using JWT for authentication.
- Passwords must be stored using strong encryption techniques.

### 5.4 Software Quality Attributes
- **Reliability**: The system should be available 99.9% of the time.
- **Maintainability**: The codebase should be modular and well-documented.

## 6. Other Requirements
- Regular backups of the database should be taken to prevent data loss.
- The system should comply with relevant financial data regulations.
