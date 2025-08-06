Introduction to AWS CI/CD Project
Introduction to AWS CI/CD Project
In this project, we will use AWS services to fetch your code, build it, and deploy it on AWS Elastic Beanstalk. Previously, we have seen Jenkins CI/CD projects or Jenkins CI/CD pipelines. Similarly, we are going to create a CodePipeline, but this time using AWS services.

To complete this project, first, we will create an AWS Elastic Beanstalk environment. We will build the code and deploy it on the Beanstalk environment. Then, we will create AWS RDS because our Vprofile application needs database connectivity. For that, we will use AWS RDS.

For the source code, we will use Bitbucket repositories. Previously, we used a GitHub repository, but in this project, we will use Bitbucket repository. I will talk about this shortly.

The Vprofile source code currently lives on a GitHub repository. We are going to migrate it from GitHub to Bitbucket. Then, we will use the AWS CodeBuild service, which will fetch the source code from Bitbucket and deploy it on Beanstalk after building the artifact.

We will use the AWS CodePipeline service to connect all these services together. Finally, we will test our CI/CD pipeline by doing a git commit and pushing the changes to our Bitbucket repository, which will trigger our pipeline.

This is the first time we are using Bitbucket repository, so let me quickly talk about it. Bitbucket is from Atlassian and is a very popular name among developers and DevOps engineers.

You can think of Bitbucket as GitHub. It provides all kinds of Git solutions. Many organizations use Atlassian services, and along with that, they use Bitbucket repositories. Therefore, there is a high chance that when you work in real time, you will be using Bitbucket repositories or Git repositories on Bitbucket.

Along with Git repositories, Bitbucket provides a complete CI/CD pipeline with various services in that pipeline.

Architectural Diagram Overview
Let's take a look at the architectural diagram. Our pipeline will be as follows:

We will have Git repositories on Bitbucket, migrated from GitHub.
AWS CodeBuild service will act like Jenkins build, fetching our source code from Bitbucket Git repositories.
CodeBuild will build our source code into an artifact and then deploy it on Beanstalk.
Since there is no default option to deploy on Beanstalk, we will use AWS CodePipeline service to connect all these pieces together.
CodePipeline will detect any new commit on our Bitbucket repository, fetch the source code, trigger the CodeBuild project, which will build the source code into an artifact, and then deploy it on AWS Elastic Beanstalk.

As you already know, our Vprofile application needs database connectivity, so we will have Amazon RDS, which will have schemas and tables for our Vprofile application.

Take a moment, pause the lecture, watch this architectural diagram once again, and then join me in the next lecture, where we will create the Beanstalk application first.

Key Takeaways
AWS services can be integrated to create a CI/CD pipeline for building and deploying applications.
AWS Elastic Beanstalk is used for deploying applications in this project.
Bitbucket repositories serve as the source code repository, replacing GitHub in this workflow.
AWS CodeBuild and CodePipeline services automate building and deployment triggered by code commits.
