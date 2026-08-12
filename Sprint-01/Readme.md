# Sprint 01 – Salesforce Development Fundamentals

## 📌 Overview

This sprint focused on building a strong foundation in Salesforce development through hands-on practice. I worked on data modeling, Apex programming, SOQL queries, Apex Triggers, Trigger Handler patterns, Governor Limits, bulkification, asynchronous Apex, and Lightning Web Components (LWC).

The sprint also focused on writing efficient, scalable, and maintainable Salesforce solutions by applying best practices such as avoiding SOQL and DML operations inside loops and using Apex Collections for bulk processing.

---

## 📚 Topics Covered

### Salesforce Data & Development

* Data Modeling
* Custom Objects
* Object Relationships
* Apex Basics
* SOQL Queries
* Apex Triggers
* Trigger Handler Pattern

### Apex & Best Practices

* Apex Collections

  * List
  * Set
  * Map
* Governor Limits
* Bulkification
* SOQL Best Practices
* Asynchronous Apex
* `@future` Methods
* Queueable Apex – Introduction

### Lightning Web Components

* Building Basic LWCs
* Using `@wire`
* Displaying Salesforce Records
* Parent-to-Child Communication
* Child-to-Parent Communication
* `@api`
* Custom Events

---

## 💻 Key Activities

### 1. Data Modeling

* Created custom Salesforce objects.
* Created relationships between objects.
* Designed the data model according to the application requirements.
* Worked with Salesforce data using standard Salesforce development practices.

### 2. Apex Programming

* Practiced Apex programming using Execute Anonymous.
* Created and executed Apex classes and methods.
* Tested Apex code directly in the Salesforce environment.
* Worked with Apex Collections such as Lists, Sets, and Maps.

### 3. SOQL

* Wrote and tested SOQL queries.
* Retrieved records from Salesforce objects.
* Practiced filtering and processing queried records.
* Learned why SOQL should not be unnecessarily placed inside loops.

### 4. Apex Triggers

* Developed Apex Triggers for business validations and automation.
* Created an intentionally inefficient trigger to understand Governor Limit exceptions.
* Refactored the trigger to make it bulkified and efficient.
* Implemented the Trigger Handler pattern to separate trigger logic from the trigger itself.

### 5. Collections & Bulkification

* Used **Lists** to store ordered collections of records.
* Used **Sets** to store unique values and efficiently identify records.
* Used **Maps** to associate record IDs with records and perform efficient lookups.
* Used Collections to process multiple records efficiently.
* Learned to avoid SOQL and DML operations inside loops.
* Converted inefficient trigger logic into a bulkified solution.

### 6. Governor Limits

* Studied Salesforce Governor Limits and their importance.
* Understood why Salesforce limits the amount of resources an Apex transaction can consume.
* Observed Governor Limit exceptions using inefficient code.
* Optimized Apex code to work efficiently within platform limits.

### 7. Asynchronous Apex

* Implemented a simple `@future` method for asynchronous processing.
* Executed asynchronous Apex jobs.
* Verified asynchronous job execution through the **Apex Jobs** page.
* Learned the basic concept of Queueable Apex.

### 8. Lightning Web Components

* Built an LWC to display custom Salesforce object records.
* Used `@wire` to retrieve Salesforce data.
* Created Parent and Child Lightning Web Components.
* Implemented **Parent-to-Child communication** using `@api`.
* Implemented **Child-to-Parent communication** using Custom Events.
* Practiced connecting LWC components with Salesforce data and application logic.

---

## 🛠️ Technologies & Tools Used

* Salesforce Playground
* Apex
* SOQL
* Apex Triggers
* Trigger Handler Pattern
* Apex Collections
* Asynchronous Apex
* Lightning Web Components (LWC)
* Lightning App Builder
* Developer Console
* VS Code
* Salesforce CLI

---

## 📂 Project Files

* Apex Collection Examples
* Apex Classes
* SOQL Query Examples
* Bulkified Trigger
* Trigger Handler Class
* Future Method
* LWC Parent Component
* LWC Child Component
* LWC Record Display Component
* Screenshots
* README

---

## 🎯 Key Learnings

Through this sprint, I learned how to:

* Design Salesforce data models using custom objects and relationships.
* Write and execute Apex code.
* Query Salesforce data using SOQL.
* Develop Apex Triggers for business requirements.
* Separate trigger logic using the Trigger Handler pattern.
* Work with Lists, Sets, and Maps in Apex.
* Understand and work within Salesforce Governor Limits.
* Write bulkified and scalable Apex code.
* Follow SOQL and DML best practices.
* Implement asynchronous processing using `@future`.
* Understand the basics of Queueable Apex.
* Build Lightning Web Components.
* Retrieve Salesforce data using `@wire`.
* Implement communication between Parent and Child LWCs.
* Use `@api` for Parent-to-Child communication.
* Use Custom Events for Child-to-Parent communication.

---

## 🎯 Outcome

This sprint strengthened my understanding of Salesforce development fundamentals and best practices. I gained practical experience in **Apex, SOQL, Data Modeling, Apex Triggers, Trigger Handler patterns, Collections, Governor Limits, Bulkification, Asynchronous Apex, and Lightning Web Components**.

By the end of the sprint, I was able to build Salesforce solutions that are not only functional but also **efficient, scalable, and maintainable**, following Salesforce development best practices.

