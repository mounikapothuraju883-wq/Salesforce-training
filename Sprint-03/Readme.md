# 🚀 Sprint 03 – My First Lightning Web Component (LWC)

## 📌 Overview

This sprint focused on getting started with **Lightning Web Components (LWC)** in Salesforce. I built my first LWC for the Placement Management System and learned how to create an interactive user interface using **HTML, JavaScript, and CSS**.

I also practiced data binding, handling user interactions through JavaScript events, dynamically updating the UI, and deploying the component to a Salesforce Lightning Page.

---

## 📚 Topics Covered

* Lightning Web Components (LWC)
* LWC Component Structure
* HTML
* JavaScript
* CSS
* Data Binding
* Event Handling
* Dynamic UI Updates
* Button Events
* Lightning App Builder
* LWC Deployment

---

## 💻 What I Built

### 1. Placement Home Component

Created a Lightning Web Component named **`placementHome`** for the Placement Management System.

The component displays student information such as:

* Student Name
* Student ID
* Department

### 2. Welcome Message

Added a **Show Welcome Message** button.

When the user clicks the button, a welcome message is displayed dynamically using JavaScript event handling.

### 3. Application Status

Added an **Apply** button that changes the application status from:

**Not Applied → Applied**

This helped me understand how JavaScript can handle user actions and dynamically update values displayed on the page.

### 4. Placement Portal Dashboard

Created a simple **Placement Portal Dashboard** that displays:

* Today's Date
* Companies
* Available Jobs
* Applications Submitted
* Student Information
* Application Status

### 5. LWC Deployment

* Created the component using VS Code.
* Added the required LWC files.
* Configured the component metadata.
* Deployed the component to Salesforce.
* Added the component to a Lightning Page using **Lightning App Builder**.
* Tested the component after deployment.

---

## 🧩 LWC File Structure

The `placementHome` component contains the following files:

### `placementHome.html`

Contains the **HTML template** and defines the structure of the user interface.

### `placementHome.js`

Contains the **JavaScript logic**, data, and event-handling methods.

### `placementHome.css`

Contains the **CSS styling** used to customize the appearance of the component.

### `placementHome.js-meta.xml`

Contains the **metadata configuration** that defines how and where the LWC can be used in Salesforce.

---

## ❓ README Questions

### 1. What is LWC?

**Lightning Web Components (LWC)** is Salesforce's modern framework for building fast, reusable, and interactive user interfaces using standard web technologies such as **HTML, JavaScript, and CSS**.

### 2. What did you build?

I built a **Placement Portal** component that displays student information, placement statistics, a welcome message, and the student's application status.

### 3. Which file contains HTML?

The HTML template is written in:

`placementHome.html`

### 4. Which file contains JavaScript?

The JavaScript logic is written in:

`placementHome.js`

### 5. Which file contains CSS?

The styling is written in:

`placementHome.css`

### 6. What is the purpose of the `.js-meta.xml` file?

The `.js-meta.xml` file contains the component's metadata and configuration. It determines where the LWC can be exposed and used, such as in Lightning App Builder.

### 7. How did you handle button events?

I used **JavaScript event-handling methods**. When the user clicks a button, the corresponding JavaScript method executes and updates the component data or UI.

### 8. What is data binding?

Data binding connects the data defined in the JavaScript file with the HTML template, allowing values to be displayed dynamically in the component.

### 9. What did you learn in this sprint?

I learned how to:

* Create an LWC from scratch.
* Understand the basic LWC file structure.
* Use HTML, JavaScript, and CSS together.
* Display dynamic information.
* Handle button click events.
* Update the UI based on user actions.
* Create a simple Placement Portal dashboard.
* Deploy an LWC to Salesforce.
* Add an LWC to a Lightning Page using Lightning App Builder.

---

## 🛠️ Technologies & Tools Used

* Salesforce Playground
* Lightning Web Components (LWC)
* HTML
* JavaScript
* CSS
* Lightning App Builder
* VS Code
* Salesforce CLI

---

## 📂 Project Files

* `placementHome.html`
* `placementHome.js`
* `placementHome.css`
* `placementHome.js-meta.xml`
* Screenshots
* README

---

## 🎯 Outcome

This sprint provided my first hands-on experience with **Lightning Web Components**. I learned how to build an interactive Salesforce user interface, connect HTML with JavaScript, handle user events, update information dynamically, style a component using CSS, and deploy the component to a Lightning Page.

This sprint established a strong foundation for developing more advanced **LWC-based Salesforce applications** in future sprints.
