# 🚀 Sprint 09 – Lightning Web Components (LWC)

## 📌 Overview

Sprint 09 focused on developing **Lightning Web Components (LWC)** and connecting the Salesforce user interface with the **Apex Service Layer** developed in the previous sprints.

The main objective was to understand how an LWC communicates with Apex, retrieves Salesforce data, handles user interactions, and supports real-world business workflows in the **Student Placement Management System**.

I also learned how to build responsive and user-friendly components by handling different UI states such as **loading, success, empty, and error states**.

---

## 🎯 Sprint Objectives

* Understand the structure of Lightning Web Components.
* Build reusable and interactive Salesforce UI components.
* Connect LWC with Salesforce data.
* Use Lightning Data Service and Wire Service.
* Integrate LWC with Apex methods.
* Implement user-driven business workflows.
* Handle asynchronous Apex responses.
* Implement Parent-to-Child and Child-to-Parent communication.
* Refresh component data after record changes.
* Debug LWC and Apex integration issues.

---

## 📚 Topics Covered

### LWC Fundamentals

* Lightning Web Components
* LWC Component Structure
* HTML Templates
* JavaScript
* Component Metadata
* Data Binding
* Event Handling
* Component Lifecycle

### Salesforce Data Integration

* Lightning Data Service
* Wire Service
* `@wire`
* Apex Integration
* Imperative Apex
* SOQL
* DML

### Component Communication

* Parent-to-Child Communication
* Child-to-Parent Communication
* `@api`
* Custom Events

### User Experience

* Loading State
* Success State
* Empty State
* Error State
* UI Refresh
* User Feedback
* LWC Debugging

---

## 💻 What I Implemented

### 1. Eligible Jobs Component

Built an **Eligible Jobs LWC** for the Student Placement Management System.

The component retrieves job opportunities that match the student's eligibility criteria and displays them in the Salesforce UI.

The component provides information such as:

* Company
* Job Role
* Eligibility Criteria
* Application Availability
* Other relevant job information

---

### 2. Apex Integration

Connected the LWC with the Apex Service Layer.

The flow allows the component to request data from Apex, while Apex handles the required business logic and Salesforce database operations.

The communication follows:

```text
LWC
 ↓
Apex Controller / Service
 ↓
Business Logic
 ↓
SOQL / DML
 ↓
Salesforce Database
```

This approach keeps the UI separate from the business logic.

---

### 3. Imperative Apex

Used **Imperative Apex** when data or an operation needs to be requested as a result of a specific user action.

For example:

```text
User clicks "Apply"
        ↓
LWC calls Apex
        ↓
Apex validates application
        ↓
ApplicationService processes request
        ↓
DML creates application
        ↓
LWC receives result
        ↓
UI is refreshed
```

This helped me understand how user actions can trigger Apex business operations.

---

### 4. Apply Job Workflow

Implemented the basic **Apply Job** workflow.

The process includes:

* Displaying eligible jobs.
* Allowing the student to select a job.
* Sending the application request to Apex.
* Validating the application through the Service Layer.
* Preventing invalid or duplicate applications.
* Creating the application record when validation succeeds.
* Displaying the result to the user.
* Refreshing the UI after the application is processed.

---

## 🔄 Application Flow

The complete application architecture follows:

```text
                    User
                      ↓
                     LWC
                      ↓
            Apex Controller / Method
                      ↓
                Service Layer
                      ↓
               Business Logic
                      ↓
                SOQL / DML
                      ↓
             Salesforce Database
                      ↓
                Apex Response
                      ↓
                     LWC
                      ↓
                Updated UI
```

This architecture provides a clear separation between the **presentation layer, business logic, and data layer**.

---

## 🔗 LWC Communication

### Parent-to-Child Communication

Used `@api` to allow a parent component to pass data or values to a child component.

```text
Parent LWC
    ↓
   @api
    ↓
Child LWC
```

### Child-to-Parent Communication

Used **Custom Events** to allow a child component to communicate user actions or information back to its parent.

```text
Child LWC
    ↓
Custom Event
    ↓
Parent LWC
```

This helped me understand how multiple LWCs can work together as a single application.

---

## 🔄 UI States

Implemented different UI states to improve the user experience.

### Loading State

Displayed while data or an Apex operation is being processed.

### Success State

Displayed when an operation such as applying for a job completes successfully.

### Empty State

Displayed when no eligible jobs or records are available.

### Error State

Displayed when an Apex operation or data retrieval process fails.

Handling these states makes the application more user-friendly and easier to understand.

---

## 🔄 UI Refresh

After an application is successfully submitted, the component refreshes the displayed data so that the user immediately sees the updated application state.

This ensures that the UI remains synchronized with Salesforce data.

---

## 🧪 Testing & Debugging

During this sprint, I practiced:

* Testing LWC functionality.
* Testing Apex integration.
* Verifying SOQL results.
* Testing successful job applications.
* Testing duplicate application scenarios.
* Testing empty job results.
* Testing error scenarios.
* Checking browser console errors.
* Debugging Apex and LWC communication.
* Verifying UI updates after database operations.

---

## 🛠️ Technologies Used

* Salesforce
* Lightning Web Components (LWC)
* HTML
* JavaScript
* CSS
* Apex
* SOQL
* DML
* Lightning Data Service
* Wire Service
* VS Code
* Salesforce CLI

---

## 📂 Project Components

* Eligible Jobs LWC
* Apply Job LWC
* Parent Component
* Child Component
* Apex Controller
* ApplicationService
* JavaScript Files
* HTML Templates
* CSS Files
* Metadata XML Files
* Test Classes
* Screenshots
* README

---

## 💡 Key Learnings

Through this sprint, I learned how to:

* Build reusable Lightning Web Components.
* Understand the complete LWC file structure.
* Display Salesforce data dynamically.
* Use the Wire Service and `@wire`.
* Understand when to use Imperative Apex.
* Connect LWC with Apex Service Classes.
* Implement real-world business workflows.
* Handle user events.
* Communicate between Parent and Child components.
* Use Custom Events.
* Handle loading, success, empty, and error states.
* Refresh the UI after data changes.
* Debug LWC and Apex integration.
* Maintain separation between UI and business logic.

---

## 🎯 Outcome

This sprint strengthened my understanding of **Lightning Web Components and Salesforce application architecture**.

I gained practical experience in connecting the frontend with the **Apex Service Layer**, retrieving and modifying Salesforce data, implementing the **Apply Job workflow**, handling different UI states, and communicating between multiple LWCs.

The sprint also helped me understand how a complete Salesforce application works across different layers:

**LWC → Apex → Service Layer → Business Logic → SOQL/DML → Salesforce Database**

This provided a strong foundation for developing **interactive, scalable, and maintainable Salesforce applications**.
