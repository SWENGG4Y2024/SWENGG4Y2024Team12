# User Requirements Document (URD) for Personal Finance Management System

## 1. Introduction

### 1.1 Purpose
The purpose of this document is to provide a comprehensive overview of the user requirements for the Personal Finance Management System. This system is intended to help users manage, track, and optimize their financial activities through a range of features including registration, balance management, expense tracking, financial goal setting, and more.

### 1.2 Scope
This document covers the functionalities, performance requirements, design constraints, and other specific requirements for the Personal Finance Management System. It is intended for the development team, project managers, and stakeholders involved in the development and deployment of the system.

### 1.3 Definitions, Acronyms, and Abbreviations
- **URD**: User Requirements Document
- **PFMS**: Personal Finance Management System
- **UI**: User Interface

### 1.5 Overview
This document is structured into several sections, including general description, specific requirements, and appendices. Each section elaborates on different aspects of the system requirements, ensuring a comprehensive understanding of user needs and system functionalities.

## 2. General Description

### 2.1 Product Perspective
The Personal Finance Management System is a standalone application designed to assist users in managing their personal finances. It integrates functionalities for tracking balances, expenses, and gains, setting financial goals, and managing financial notes and tags.

### 2.2 Product Functions
The system provides the following key functions:
- User Registration and Authentication
- Balance Management
- Expense and Gain Tracking
- Financial Goal Setting and Tracking
- Monthly Spending Threshold Tracking
- Financial Notes Management
- Tagging and Querying

### 2.3 User Characteristics
The primary users of this system are individuals seeking to manage their personal finances effectively. They are expected to have basic computer literacy and access to the internet.

### 2.4 Constraints
- The system must ensure data privacy and security.
- The system should be accessible via web browsers and mobile devices.
- The system must handle concurrent user sessions efficiently.

### 2.5 Assumptions and Dependencies
- Users will have access to a stable internet connection.
- The system will be integrated with third-party services for user authentication and financial data retrieval where necessary.

## 3. Specific Requirements

### 3.1 User Registration and Authentication

#### 3.1.1 Registration
- Users shall be able to register by providing necessary details such as username, email, and password.
- The system shall send a confirmation email upon successful registration.

#### 3.1.2 Login
- Users shall be able to log in using their registered email and password.
- The system shall implement CAPTCHA to prevent automated login attempts.

#### 3.1.3 Update Details
- Users shall be able to update their personal details such as name, email, and contact information.

#### 3.1.4 Change Password
- Users shall be able to change their password.
- The system shall enforce strong password policies.

### 3.2 Balance Management
- Users shall be able to add, edit, and delete balance entries for different financial accounts (e.g., bank accounts, wallets).
- The system shall display a summary of the total balance across all accounts.

### 3.3 Expense and Gain Tracking

#### 3.3.1 Current Expenses/Gains
- Users shall be able to log their current expenses and gains with details such as amount, date, and description.
- The system shall provide a summary of current expenses and gains.

#### 3.3.2 Future Expenses/Gains
- Users shall be able to schedule future expenses and gains.
- The system shall send reminders for upcoming expenses/gains.

### 3.4 Financial Goal Setting and Tracking
- Users shall be able to set financial goals with target amounts and deadlines.
- The system shall track the progress of each goal and provide updates.

### 3.5 Monthly Spending Threshold Tracking
- Users shall be able to set a monthly spending threshold.
- The system shall track spending and provide notifications when the threshold is approached or exceeded.
- The system shall automatically calculate monthly spending at month-end using Spring scheduler and cron expressions.

### 3.6 Financial Notes Management
- Users shall be able to create, edit, and delete financial notes for personal reference.

### 3.7 Tagging and Querying
- Users shall be able to assign tags to their expense/gain entries and notes.
- The system shall support querying and filtering based on tags.

## 4. Appendices

### 4.1 Glossary
- **Balance**: The amount of money available in a user's financial accounts.
- **Expense**: Money spent by the user.
- **Gain**: Money earned or received by the user.
- **Financial Goal**: A target amount of money that a user aims to save or spend within a specified time frame.
- **Threshold**: A limit set by the user for monthly spending.

### 4.2 Acronyms
- **URD**: User Requirements Document
- **PFMS**: Personal Finance Management System
- **UI**: User Interface
