CI/CD Pipeline for Serverless .NET Applications on AWS

   Deploy an automated pipeline to build and deploy serverless .NET applications- 
   
 This Quick Start builds a continuous integration and delivery (CI/CD) pipeline for serverless .NET applications on the Amazon Web Services (AWS) Cloud. This scalable deployment helps you deliver features and updates rapidly and reliably. You have no build servers to manage, and you pay only for what you use. It deploys an AWS CodeCommit repository with a sample AWS Lambda application defined in an AWS Serverless Application Model (AWS SAM) template. Pushing changes to modify the application invokes AWS CodePipeline. The pipeline builds and deploys the application using AWS CloudFormation and exposes it to the internet with Amazon API Gateway.
 
How To Deploy?

1)Sign in to your AWS account. If you don't have an account, sign up at https://aws.amazon.com.
2)click on the link. Before you create the stack, choose the Region from the top toolbar.
3)Test the deployment. 

Amazon may share user-deployment information with the AWS Partner that collaborated with AWS on this solution

## .NET CI/CD for Serverless Applications — Quick Start

For architectural details, step-by-step instructions, and customization options, see the [deployment guide](https://fwd.aws/EvrJV?).

To post feedback, submit feature ideas, or report bugs, use the **Issues** section of this GitHub repo. 

To submit code for this Quick Start, see the [AWS Quick Start Contributor's Kit](https://aws-quickstart.github.io/).


## . https://aws-quickstart.s3.us-east-1.amazonaws.com/quickstart-dotnet-lambda-cicd/templates/serverless-cicd.template.yaml

The AWS CloudFormation template at the provided link sets up a Continuous Integration and Continuous Deployment (CI/CD) pipeline for a serverless .NET application using AWS Lambda and AWS CodePipeline. Here are the steps that the template performs:

1)It creates an Amazon S3 bucket to store the source code of the application and the pipeline artifacts.

2)It creates an AWS CodeCommit repository to store the source code of the application.

3)It creates an AWS CodeBuild project to build the application and package it as a zip file.

4)It creates an AWS Lambda function to deploy the application package to AWS Lambda.

5)It creates an AWS CodePipeline pipeline to automate the CI/CD process using the previously created AWS resources.

6)It sets up the permissions required for the CI/CD pipeline to access the AWS resources.


More specifically, the following resources are created by the template:

1)AWS::S3::Bucket: creates an S3 bucket to store the source code of the application and the pipeline artifacts.

2)AWS::CodeCommit::Repository: creates a CodeCommit repository to store the source code of the application.

3)AWS::CodeBuild::Project: creates a CodeBuild project to build the application and package it as a zip file.

4)AWS::Lambda::Function: creates a Lambda function to deploy the application package to AWS Lambda.

5)AWS::CodePipeline::Pipeline: creates a CodePipeline pipeline to automate the CI/CD process using the previously created AWS resources.

6)AWS::IAM::Role: creates an IAM role with the necessary permissions required by the CI/CD pipeline to access the AWS resources.


Overall, this CloudFormation template creates a complete CI/CD pipeline that automates the process of building, testing, and deploying a serverless .NET application using AWS services.
