# 🚀 Placement Management System

A Salesforce Apex-based project that demonstrates how to design and implement a complete **placement application workflow** using **Apex, SOQL, DML, custom objects, and service classes**.

The project focuses on retrieving student and job information, validating business rules, preventing duplicate applications, creating application records, and updating application status.

---

## 📌 Project Overview

The **Placement Management System** simulates a real-world college placement process in Salesforce.

Students can apply for available job opportunities, while the system performs the required validations before creating an application.

The application follows a structured business flow:

* Retrieve student information.
* Retrieve job information and eligibility criteria.
* Check whether the student has already applied.
* Validate the student's eligibility.
* Create a new application record.
* Save the application using DML.
* Update the application status when required.

The project is designed using separate Apex service classes to keep the business logic **organized, reusable, and maintainable**.

---

## ✨ Key Features

* 🔍 **Retrieve Student Information** using SOQL
* 💼 **Retrieve Job Information & Eligibility Criteria**
* 🎓 **Validate Student Eligibility**
* 🚫 **Prevent Duplicate Applications**
* 📝 **Create New Application Records** using DML
* 🔄 **Update Application Status**
* ⚙️ **Separate Business Logic using Apex Service Classes**
* 🔗 **Complete End-to-End Placement Application Transaction**

---

## 🛠️ Technologies Used

* Salesforce Apex
* SOQL – Salesforce Object Query Language
* DML – Data Manipulation Language
* Salesforce Custom Objects
* Salesforce Developer Console
* VS Code
* Salesforce CLI

---

## 📂 Custom Objects

The project uses the following custom objects:

### 👨‍🎓 Student

Stores student-related information required for the placement process.

Example information:

* Student Name
* Student ID
* Department
* CGPA
* Other eligibility-related details

### 💼 Job

Stores information about available placement opportunities.

Example information:

* Company
* Job Role
* Required CGPA
* Eligibility Criteria
* Job Details

### 📝 Application

Stores the student's placement application.

Example information:

* Student
* Job
* Application Date
* Application Status

---

## 📁 Apex Classes

### `StudentService.cls`

Responsible for retrieving student information required during the placement process.

### `JobService.cls`

Responsible for retrieving job information and eligibility criteria.

### `ApplicationService.cls`

Handles application-related business logic such as:

* Validating applications
* Checking duplicate applications
* Creating application records

### `UpdateApplicationService.cls`

Handles updating existing application records and their status.

### `PlacementService.cls`

Coordinates the complete placement application workflow by bringing the required service operations together.

---

## 🔄 Business Flow

```text
                Receive Application Request
                           ↓
                  Retrieve Student
                           ↓
                    Retrieve Job
                           ↓
              Check Student Eligibility
                           ↓
             Check Duplicate Application
                           ↓
                  Create Application
                           ↓
                     Save Record
                        (DML)
                           ↓
                 Update Status if Required
                           ↓
                 Display Confirmation
```

---

## 🔍 Detailed Process

### Step 1 – Receive Request

The system receives the information required to process a placement application, such as the student and job details.

### Step 2 – Retrieve Student

SOQL is used to retrieve the student's Salesforce record.

The retrieved information is used for eligibility validation.

### Step 3 – Retrieve Job

The system retrieves the selected job and its eligibility requirements using SOQL.

### Step 4 – Validate Eligibility

The student's details are compared with the job's eligibility criteria.

For example, the student's CGPA can be checked against the minimum required CGPA.

### Step 5 – Check Duplicate Application

Before creating a new application, the system checks whether the student has already applied for the same job.

This prevents duplicate application records.

### Step 6 – Create Application

If the student is eligible and no duplicate application exists, a new Application record is created.

### Step 7 – Save Record

DML is used to insert the new Application record into Salesforce.

### Step 8 – Update Application Status

The application status can be updated as the application progresses through the placement process.

---

## 📚 Sprint Coverage

### Sprint 07 – Student Information

Focused on retrieving the student information required for the placement application and eligibility validation using SOQL.

### Sprint 08 – Job Eligibility

Implemented retrieval of job information and eligibility criteria required to determine whether a student can apply.

### Sprint 09 – Duplicate Prevention

Implemented logic to check for existing applications and prevent a student from submitting duplicate applications for the same job.

### Sprint 10 – Application Creation

Implemented the creation and saving of new Application records using Apex and DML.

### Sprint 11 – Application Status

Implemented functionality to update the status of an existing application based on the application process.

### Sprint 12 – Complete Transaction

Combined the individual services into a complete placement transaction using **Apex, SOQL, business validation, and DML**.

---

## 🎯 Learning Outcomes

Through this project, I learned how to:

* Retrieve Salesforce records using SOQL.
* Perform insert and update operations using DML.
* Validate business requirements before performing database operations.
* Prevent duplicate records through business logic.
* Organize Apex logic into reusable service classes.
* Separate responsibilities between different service classes.
* Design an end-to-end Salesforce business transaction.
* Understand how multiple Apex classes work together to complete a business process.
* Apply Salesforce development concepts to a real-world placement management scenario.

---

## 🏗️ Project Architecture

The project follows a service-based approach:

```text
PlacementService
       │
       ├── StudentService
       │       └── Retrieve Student
       │
       ├── JobService
       │       └── Retrieve Job & Eligibility
       │
       ├── ApplicationService
       │       ├── Validate Application
       │       ├── Check Duplicate
       │       └── Create Application
       │
       └── UpdateApplicationService
               └── Update Application Status
```

This structure keeps individual responsibilities separated and makes the application easier to understand, maintain, and extend.

---

## 📸 Project Screenshots

Add relevant screenshots from the Salesforce project here:

* Student Record
* Job Record
* Application Record
* `StudentService.cls`
* `JobService.cls`
* `ApplicationService.cls`
* `UpdateApplicationService.cls`
* `PlacementService.cls`
* Execute Anonymous Results
* Debug Logs
* Successful Application Creation
* Updated Application Status

---

## 🎯 Final Outcome

The **Placement Management System** gave me practical experience in building a Salesforce application using **Apex, SOQL, DML, custom objects, and service classes**.

I learned how to convert a real-world placement requirement into a structured business transaction, retrieve and validate data, prevent duplicate applications, create and update records, and organize business logic into reusable Apex services.

This project strengthened my understanding of **Salesforce backend development and enterprise application design** and provided a foundation for building more advanced Salesforce applications.
