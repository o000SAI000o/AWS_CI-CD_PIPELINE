# 🚀 AWS CI/CD Pipeline Project – Vprofile Application

This project demonstrates a complete CI/CD pipeline using **native AWS services** to automate building and deploying the `vprofile` application using **Bitbucket**, **AWS CodePipeline**, **CodeBuild**, and **Elastic Beanstalk**.

---

## 📌 Overview

- Source code is hosted on **Bitbucket** (migrated from GitHub).
- Application is deployed on **AWS Elastic Beanstalk**.
- **AWS CodeBuild** compiles and packages the application.
- **AWS CodePipeline** integrates all services to automate the workflow.
- **Amazon RDS** provides database connectivity for the application.

---

## 🏗️ Architecture

<br>

![DocScanner Aug 6, 2025 7-50 PM_1](https://github.com/user-attachments/assets/6e8c3553-13eb-4896-b9d1-ef9b3b1bddcd)

<br>

![DocScanner Aug 6, 2025 7-50 PM_2](https://github.com/user-attachments/assets/d1d5af75-b12d-4e47-b375-c07eb5f3fcde)

<br>

Bitbucket (Git Repo)
│
▼
AWS CodePipeline
│
▼
AWS CodeBuild ───▶ Builds Artifact
│
▼
AWS Elastic Beanstalk ───▶ Deploys App
│
▼
Amazon RDS ───▶ Database Backend


---

## 🛠️ Technologies Used

- ✅ **Bitbucket** – Git repository hosting.
- ✅ **AWS CodePipeline** – Automates CI/CD stages.
- ✅ **AWS CodeBuild** – Builds the project into deployable artifacts.
- ✅ **AWS Elastic Beanstalk** – Hosts and deploys the application.
- ✅ **Amazon RDS** – Manages relational databases.

---

## 🔄 Workflow

1. Developer pushes code to **Bitbucket**.
2. **CodePipeline** detects the new commit.
3. It triggers **CodeBuild** to:
   - Fetch the code
   - Install dependencies
   - Build the WAR/JAR artifact
4. Artifact is deployed on **Elastic Beanstalk**.
5. Application connects to **Amazon RDS** for data storage.

---

## 💡 Why Bitbucket?

Bitbucket by Atlassian is widely used in enterprise DevOps pipelines and offers similar Git functionality as GitHub. It's often integrated with other Atlassian tools like Jira, making it a popular real-world choice.

---

## 📈 Key Takeaways

- 🔧 Build and deployment fully handled by AWS.
- 💡 No Jenkins required – native AWS services manage the pipeline.
- ☁️ Easy and scalable application deployment with Beanstalk.
- 🔐 Database-backed applications using Amazon RDS.
- 🔄 Real-time automated deployments with every push to Bitbucket.

---

## ✅ Prerequisites

- AWS Account with admin-level access
- Bitbucket account
- IAM roles and policies for CodeBuild, CodePipeline, and Elastic Beanstalk
- Application source code (vprofile)
