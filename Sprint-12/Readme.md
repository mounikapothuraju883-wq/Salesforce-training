# 🚀 Sprint 12 – Source Control, Salesforce CLI & Deployment

## 📌 Overview

Sprint 12 focused on learning how to manage a Salesforce project using a **professional source-driven development and deployment workflow**.

In this sprint, I worked with **Git, GitHub, Salesforce CLI, Salesforce Metadata, branches, commits, Pull Requests, code reviews, deployment environments, and metadata deployment**.

The main objective was to understand how a Salesforce application can be maintained outside the Salesforce Org using a local project, tracked through source control, tested, reviewed, and deployed in a controlled manner.

---

## 🎯 Sprint Objectives

The major objectives of this sprint were:

* Understand the role of Git in Salesforce development.
* Create and manage a GitHub repository.
* Work with feature branches.
* Commit and push Salesforce project changes.
* Pull changes from a remote repository.
* Understand Pull Requests and code reviews.
* Understand Salesforce Metadata.
* Use Salesforce CLI for development tasks.
* Authenticate Salesforce Orgs using the CLI.
* Retrieve Salesforce Metadata into a local project.
* Deploy Metadata to a Salesforce Org.
* Understand Sandboxes and Scratch Orgs.
* Understand Changesets and Metadata API.
* Handle basic Git merge conflicts.
* Identify deployment dependencies.
* Perform testing before deployment.
* Understand a controlled Salesforce deployment process.

---

# 🧩 Engineering Sprint 35 – GitHub Repository & Source Control

## 📌 Objective

The first part of the sprint focused on creating a professional source-control workflow for the **Placement Management System**.

The Salesforce project was connected to a Git repository so that changes could be tracked and managed systematically.

### 🔄 Git Workflow

```text
Local Development
       ↓
Git Repository
       ↓
Feature Branch
       ↓
Make Changes
       ↓
Commit
       ↓
Push to GitHub
       ↓
Pull Request
       ↓
Code Review
       ↓
Merge
```

### 💻 Important Git Commands

```bash
git clone <repository-url>

git checkout -b feature/placement-update

git status

git add .

git commit -m "Add placement feature"

git push origin feature/placement-update

git pull
```

### 📚 Key Concepts

**Clone** – Downloads an existing Git repository to the local machine.

**Branch** – Creates an isolated workspace for developing a feature or change.

**Commit** – Records changes in the local Git history.

**Push** – Uploads committed changes to the remote GitHub repository.

**Pull** – Retrieves the latest changes from the remote repository.

---

# 🧩 Engineering Sprint 36 – Salesforce Metadata Management

## 📌 Objective

This part of the sprint focused on understanding **Salesforce Metadata** and how Salesforce configuration can be represented as source files.

Metadata includes components such as:

* Custom Objects
* Custom Fields
* Apex Classes
* Apex Triggers
* Lightning Web Components
* Flows
* Configuration Metadata

### 🔄 Metadata Workflow

```text
Salesforce Org
      ↓
Salesforce CLI
      ↓
Retrieve Metadata
      ↓
Local Salesforce Project
      ↓
Git Repository
```

### 💻 Salesforce CLI Commands

```bash
sf org list
```

Used to view authenticated Salesforce organizations.

```bash
sf project retrieve start
```

Used to retrieve Salesforce metadata into the local project.

This helped me understand how Salesforce components such as **Apex, LWC, Objects, Fields, and Flows** are represented and managed as source files.

---

# 🧩 Engineering Sprint 37 – Branching & Code Review

## 📌 Objective

This sprint focused on using a feature branch and understanding how changes can be reviewed before being merged into the main codebase.

### 🔄 Code Review Workflow

```text
Feature Branch
      ↓
Develop Feature
      ↓
Commit Changes
      ↓
Push to GitHub
      ↓
Create Pull Request
      ↓
Code Review
      ↓
Make Improvements
      ↓
Merge
```

### 🔍 Review Areas

#### Apex

* Bulkification
* Clear responsibilities
* SOQL usage
* DML outside loops
* Error handling
* Test coverage

#### LWC

* Clear component responsibility
* Meaningful naming
* Loading handling
* Error handling
* Avoiding unnecessary duplicated logic

#### Security

* Protect sensitive information.
* Review sharing and security considerations.
* Avoid exposing credentials.

#### Integration

* Use Named Credentials where required.
* Consider integration failures.
* Consider duplicate processing.

---

# 🧩 Engineering Sprint 38 – Salesforce Development Approaches

## 📌 Objective

I studied different approaches used to develop and move Salesforce metadata between environments.

| Approach                 | Purpose                                          |
| ------------------------ | ------------------------------------------------ |
| **Git + Salesforce CLI** | Source-driven Salesforce development             |
| **Changesets**           | Move metadata between related Salesforce Orgs    |
| **Metadata API**         | Programmatic metadata retrieval and deployment   |
| **Scratch Orgs**         | Temporary source-driven development environments |
| **Sandboxes**            | Development, testing, and UAT environments       |

### 🔹 Git + Salesforce CLI

Useful for a modern, source-driven development workflow.

### 🔹 Changesets

Useful for traditional Salesforce metadata movement between related Orgs.

### 🔹 Scratch Orgs

Useful for temporary and isolated development and testing.

### 🔹 Sandboxes

Useful for longer-lived development, testing, and UAT activities.

---

# 🧩 Engineering Sprint 39 – Controlled Deployment

## 📌 Objective

The final part of the sprint focused on understanding how Salesforce changes can move through a **controlled development and deployment process**.

### 🚀 Deployment Pipeline

```text
Development
     ↓
Feature Branch
     ↓
Commit
     ↓
Push
     ↓
Pull Request
     ↓
Code Review
     ↓
Merge
     ↓
Development / Test Org
     ↓
Run Tests
     ↓
Manual Verification
     ↓
Deployment
     ↓
Documentation
```

### 💻 Deployment Commands

#### Authenticate Salesforce

```bash
sf org login web
```

#### View Salesforce Orgs

```bash
sf org list
```

#### Retrieve Metadata

```bash
sf project retrieve start
```

#### Deploy Metadata

```bash
sf project deploy start
```

The exact authentication and deployment commands can vary depending on the Salesforce project and target environment.

---

# 🧪 Testing Before Deployment

Before deploying changes, I learned that the application should be properly tested.

Testing can include:

* Apex Tests
* Functional Testing
* Integration Testing
* LWC Testing where applicable
* Permission Checks
* Deployment Validation
* Regression Testing

A successful deployment is not determined only by whether the code worked in the development environment. The target environment and its dependencies must also be verified.

---

# ⚠️ Deployment Dependencies

Salesforce applications consist of multiple connected components.

For example:

```text
LWC
 ↓
Apex Controller
 ↓
Custom Object
 ↓
Custom Fields
```

If a required dependency is missing from the target Org, the deployment or application can fail.

Therefore, I learned to consider the **complete application and its dependencies**, rather than deploying individual files without checking their relationships.

---

# 🌿 Git Merge Conflicts

I also learned the basic process of handling Git merge conflicts.

A conflict can occur when different developers modify overlapping parts of the same file.

### 🔧 Conflict Resolution Process

1. Identify the conflicting file.
2. Understand both changes.
3. Check the business requirement.
4. Decide the correct implementation.
5. Resolve the conflict.
6. Test the code.
7. Commit the resolved changes.

The conflict should be resolved based on the intended application behavior rather than simply choosing one side.

---

# ☁️ Salesforce Environments

## Sandbox

A **Sandbox** is a separate Salesforce environment used for activities such as development, testing, and UAT.

It allows development work to be performed without directly modifying Production.

## Scratch Org

A **Scratch Org** is a temporary, source-driven Salesforce environment used for development and testing.

It supports reproducibility because the environment can be created from project configuration.

---

# 🔄 Metadata vs Business Data

An important concept covered in this sprint was the difference between **Salesforce Metadata** and **Business Data**.

### Metadata

Examples:

* Objects
* Fields
* Apex Classes
* Triggers
* LWC
* Flows
* Configuration

Metadata describes the structure and configuration of the Salesforce application.

### Business Data

Examples:

* Student Records
* Job Records
* Applications
* Employee Records
* Leave Requests

Metadata can be version-controlled and deployed, while business data should not automatically be treated as source code.

---

# 🔐 Security Considerations

I learned that sensitive information must not be committed to GitHub.

The following should never be stored directly in source control:

* Passwords
* Access Tokens
* Client Secrets
* API Keys
* Authentication Secrets
* Hard-coded Credentials

Environment-specific configuration and credentials should be handled securely.

---

# 🐛 Troubleshooting

## Salesforce CLI Not Recognized

If the `sf` command is not recognized, Salesforce CLI installation and system PATH configuration should be checked.

## Wrong Salesforce Org

Before performing deployment operations, verify the authenticated Orgs:

```bash
sf org list
```

The correct target Org must always be confirmed before deployment.

## Deployment Failure

Possible causes include:

* Missing Metadata
* Missing Dependencies
* Apex Test Failures
* Object or Field Dependencies
* Permission Issues
* Configuration Differences
* Integration Configuration
* Environment-Specific Settings

---

# 💡 Key Engineering Principles

### 1. Source Control

The Salesforce Org should not be treated as the only copy of the application.

### 2. Reproducibility

Another developer should be able to clone the repository and understand the project structure.

### 3. Controlled Deployment

Changes should move through appropriate development, review, testing, and deployment stages.

### 4. Dependency Awareness

The complete Salesforce system and its connected components should be considered during deployment.

### 5. Environment Awareness

The target Salesforce Org should always be verified before performing deployment operations.

---

# 🎓 Interview Questions Covered

### What is Git?

Git is a version-control system used to track changes and support collaboration during software development.

### Why is Git important in Salesforce?

Git provides source control, change history, collaboration, code review, and reproducibility for Salesforce projects.

### What is a Branch?

A branch provides an isolated environment for developing changes without directly modifying the main codebase.

### What is the difference between Commit and Push?

A **commit** records changes in the local Git repository, while a **push** sends those committed changes to the remote repository.

### What is a Pull Request?

A Pull Request is used to propose changes for review before merging them into another branch.

### What is Salesforce CLI?

Salesforce CLI is a command-line interface used to interact with Salesforce Orgs and perform development tasks such as authentication, metadata retrieval, and deployment.

### What is Salesforce Metadata?

Metadata describes the structure and configuration of a Salesforce application, including objects, fields, Apex, LWC, and Flows.

### What is a Sandbox?

A Sandbox is a separate Salesforce environment used for development, testing, or other controlled activities.

### What is a Scratch Org?

A Scratch Org is a temporary, source-driven Salesforce development environment.

### What is a Changeset?

A Changeset is a Salesforce-native mechanism for moving metadata between related Salesforce Orgs.

### What is Metadata API?

Metadata API provides programmatic mechanisms for retrieving and deploying Salesforce metadata.

### Why should the target Org be verified before deployment?

To prevent accidentally deploying changes to the wrong Salesforce environment, especially Production.

### Why can deployment fail even when the Apex code is correct?

Because Salesforce components have dependencies. Missing objects, fields, permissions, configuration, or other required metadata can cause deployment or runtime problems.

---

# 📋 Definition of Done

Sprint 12 is considered complete when:

* Git repository is created.
* Project structure is organized.
* Feature branches are understood.
* Meaningful commits are created.
* Pull Request workflow is understood.
* Salesforce metadata is stored in source control.
* Salesforce CLI authentication is configured.
* Metadata can be retrieved.
* Metadata can be deployed.
* Apex tests can be executed.
* Target Salesforce Org is verified.
* Deployment dependencies are understood.
* Deployment process is documented.

---

# 🎯 Sprint Outcome

Sprint 12 helped me understand how to move from simply **building Salesforce features** to managing a Salesforce application using a professional software development workflow.

I gained practical knowledge of:

* Git and GitHub
* Branching
* Commits
* Pull Requests
* Code Reviews
* Merge Conflicts
* Salesforce CLI
* Salesforce Metadata
* Source-Driven Development
* Sandboxes
* Scratch Orgs
* Changesets
* Metadata API
* Deployment Dependencies
* Testing
* Controlled Deployment
* Repository Documentation

---

# 🚀 Conclusion

Sprint 12 demonstrated how Salesforce development can be managed as a **source-controlled and reproducible software engineering process**.

The overall workflow can be summarized as:

```text
Git
 ↓
Branch
 ↓
Development
 ↓
Commit
 ↓
Push
 ↓
Pull Request
 ↓
Code Review
 ↓
Testing
 ↓
Salesforce CLI
 ↓
Metadata Deployment
 ↓
Verification
 ↓
Documentation
```

This sprint strengthened my understanding of the **professional Salesforce development lifecycle**, especially source control, metadata management, collaboration, testing, and controlled deployment.
