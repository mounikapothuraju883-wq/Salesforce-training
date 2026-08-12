# 🚀 Sprint 04 – Building Business Logic with Apex

## 📌 Overview

This sprint focused on understanding and designing **business logic using Apex** for the Placement Management System. Instead of directly writing code, I first learned how to analyze business requirements, identify business rules, and organize application responsibilities into a structured service layer.

The main goal was to understand how Salesforce applications can be designed in a **scalable, maintainable, and organized way** before implementing the complete functionality.

---

## 📚 Topics Covered

* Business Logic
* Business Requirements
* Business Rules
* Apex Service Classes
* Application Service Layer
* Software Architecture
* Methods & Parameters
* SOQL Concepts
* DML Concepts
* Separation of Responsibilities
* Scalable Application Design
* Code Maintainability

---

## 💻 What I Learned

### 1. Understanding Business Requirements

I learned how to convert customer or application requirements into technical business rules.

For the Placement Management System, I identified requirements such as:

* Students should be able to submit placement applications.
* Student eligibility should be validated.
* Duplicate applications should be prevented.
* Valid applications should be saved in Salesforce.
* The system should return meaningful results or messages.

### 2. Separating Business Logic

I learned why business logic should not be placed directly inside the user interface or tightly coupled with other components.

Instead, business operations can be organized into dedicated **Apex Service Classes**.

This makes the application:

* Easier to maintain
* Easier to test
* Reusable
* More organized
* Easier to extend in the future

### 3. ApplicationService Design

Designed an **`ApplicationService`** class to represent application-related business operations.

The service is responsible for handling activities such as:

* Receiving placement applications
* Validating eligibility
* Checking for duplicate applications
* Saving valid application records
* Returning meaningful results

### 4. Methods & Parameters

I learned how methods represent individual business activities.

For example:

* A method can represent submitting an application.
* A method can validate student eligibility.
* A method can check whether an application already exists.

Parameters represent the information required by the business operation, such as:

* Student information
* Job or company information
* Application details

This approach makes the code more organized and reusable.

### 5. SOQL & DML Concepts

I also reviewed how Salesforce data is accessed and modified using Apex.

**SOQL (Salesforce Object Query Language)** is used to retrieve records from Salesforce.

**DML (Data Manipulation Language)** operations are used to create, update, delete, or otherwise modify Salesforce records.

The service layer can use SOQL and DML to implement business requirements while keeping the logic organized.

---

## 🏗️ Application Service Approach

The basic approach followed in this sprint was:

**Business Requirement → Business Rule → Service Design → Methods → SOQL/DML → Result**

For example:

**Student submits application**

↓

Check student eligibility

↓

Check for duplicate application

↓

Create application record

↓

Save the record

↓

Return the result

This approach helped me understand how business requirements can be converted into structured Apex application logic.

---

## ❓ Sprint Reflection

### 1. Why does `ApplicationService` exist?

`ApplicationService` provides a dedicated place for managing **placement application-related business operations**.

This prevents business logic from being scattered across different parts of the application.

### 2. What business responsibility does it represent?

It represents the responsibility of managing placement applications, including:

* Receiving applications
* Validating eligibility
* Checking duplicates
* Saving valid applications
* Returning meaningful results

### 3. Why do we create methods?

Methods represent individual business activities. They help divide a large business process into smaller, reusable, and maintainable units of functionality.

### 4. Why separate business logic from the UI?

Separating business logic from the UI makes the application easier to maintain and allows the same business logic to potentially be reused by different interfaces such as **LWC, APIs, or other Apex code**.

### 5. What is the role of SOQL?

SOQL is used to **retrieve Salesforce records** required by the business logic.

### 6. What is the role of DML?

DML is used to **perform operations on Salesforce records**, such as inserting, updating, or deleting records.

### 7. What did I learn in this sprint?

I learned that good Salesforce development starts with understanding the **business requirement and designing the architecture** before writing the implementation code.

---

## 🛠️ Technologies & Tools Used

* Salesforce Playground
* Apex
* SOQL
* DML
* VS Code
* Salesforce CLI

---

## 📂 Project Files

* `ApplicationService.cls`
* `BusinessRules.md`
* `ArchitectureNotes.md`
* `SprintReflection.md`
* Screenshots
* README

---

## 🎯 Outcome

This sprint helped me understand how **enterprise Salesforce applications are designed using structured business logic**. I learned how to identify business requirements, convert them into business rules, and organize application responsibilities using an Apex Service Class.

I also gained a better understanding of how **methods, parameters, SOQL, and DML** work together within a service layer.

Most importantly, I learned that effective development is not just about writing code—it starts with **understanding the requirement, designing the responsibility clearly, and then implementing the solution in a scalable and maintainable way**.
