# 🚀 Sprint 02 – Validation Rules, Flows & Declarative Automation

## 📌 Overview

This sprint focused on Salesforce **declarative automation** using Validation Rules and Record-Triggered Flows. I learned how to enforce data quality, automate repetitive business processes, and configure Salesforce automation without writing Apex code.

I also explored the differences between **Validation Rules, Record-Triggered Flows, and Apex Triggers** to understand which automation approach is most suitable for different business requirements.

---

## 📚 Topics Covered

* Validation Rules
* Validation Rule Formulas
* Record-Triggered Flows
* Flow Builder
* Flow Actions
* Before-Save Flows
* After-Save Flows
* Flow vs Apex Trigger
* Declarative Automation
* Data Validation
* Automated Email Notifications

---

## 💻 What I Implemented

### 1. Record-Triggered Flow

* Created a **Record-Triggered Flow** to automate the Application process.
* Configured the flow to automatically populate the **Application Date**.
* Used Flow Builder to define the automation logic.
* Configured the flow based on record creation/update requirements.

### 2. Email Notification

* Added an **Email Action** to the flow.
* Configured the automation to notify the **Placement Officer** when the required condition is met.
* Learned how Flow Actions can be used to automate communication.

### 3. Validation Rules

Created Validation Rules to maintain data accuracy and prevent invalid records.

Implemented validations for:

* **Student CGPA Validation** – Ensured CGPA values follow the required conditions.
* **Application Date Validation** – Prevented invalid application dates.
* **Mandatory Field Validation** – Ensured required information is entered before a record can be saved.

### 4. Before-Save & After-Save Flows

* Learned the difference between **Before-Save** and **After-Save** Record-Triggered Flows.
* Understood when each type should be used.
* Practiced using Before-Save Flows for updating fields on the same record.
* Learned how After-Save Flows can be used when additional actions or related-record processing is required.

### 5. Flow vs Apex Trigger

Compared Salesforce automation tools based on business requirements:

| Automation           | Main Purpose                                             |
| -------------------- | -------------------------------------------------------- |
| **Validation Rule**  | Prevents users from saving invalid data                  |
| **Before-Save Flow** | Efficiently updates fields on the triggering record      |
| **After-Save Flow**  | Performs actions after a record is saved                 |
| **Apex Trigger**     | Handles complex automation and logic requiring Apex code |

I learned to prefer **declarative automation** such as Flow when the requirement can be achieved efficiently without code, while using **Apex Triggers** when more complex or highly customized logic is required.

---

## 🛠️ Technologies & Tools Used

* Salesforce Playground
* Salesforce Flow Builder
* Record-Triggered Flow
* Validation Rules
* Flow Actions
* Lightning App Builder
* Salesforce Platform

---

## 📂 Project Files

* Record-Triggered Flow
* Validation Rule Formulas
* Flow Configuration
* Flow vs Trigger Notes
* Interview Questions & Answers
* Screenshots
* README

---

## 🎯 Key Learnings

Through this sprint, I learned how to:

* Create and configure Validation Rules.
* Improve Salesforce data quality using declarative validation.
* Build Record-Triggered Flows.
* Automate field updates using Flow.
* Configure automated email notifications.
* Understand Before-Save and After-Save Flows.
* Choose the appropriate Flow type for a business requirement.
* Compare Validation Rules, Flows, and Apex Triggers.
* Understand when declarative automation is preferred over programmatic automation.
* Build Salesforce automation while minimizing the need for Apex code.

---

## 🎯 Outcome

This sprint strengthened my understanding of **Salesforce declarative automation** and gave me hands-on experience with **Validation Rules, Record-Triggered Flows, Flow Actions, and automated notifications**.

I also developed a better understanding of choosing between **Validation Rules, Flows, and Apex Triggers** based on business requirements. This helped me understand how Salesforce developers can combine declarative and programmatic automation to build **efficient, reliable, and maintainable Salesforce applications**.

