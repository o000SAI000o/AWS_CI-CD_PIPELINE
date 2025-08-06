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

![DocScanner Aug 6, 2025 7-50 PM_2](https://github.com/user-attachments/assets/fc11ab08-5e59-4afe-acce-12e78f3b721f)


![DocScanner Aug 6, 2025 7-50 PM_1](https://github.com/user-attachments/assets/edf04ca6-02db-4ec7-8c72-bbdcf145380e)


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

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).

---

## 🤝 Contributing

Contributions are welcome! Please read our [CONTRIBUTING.md](CONTRIBUTING.md) guide to get started.

---

**Happy DevOps-ing! 🚀**
