#  React > Terraform & CircleCI > AWS S3

A template/workflow for the automated deployment (including infrastrusture provisioning) of an React app to AWS S3.


![Template - React App on AWS S3 with CircleCI and Terraform](https://i.imgur.com/h1OKYel.jpg)

Terraform > IaC setup of resources on AWS (S3 buckets and policies)

CircleCI > Automated checkout on commit, building and deploy to AWS

#  Notes

React App was created with "npx create-react-app my-app".

Circle CI requires a setup of the deployment pipeline via your CircleCI account (repo only contains config files).

Never include your AWS login credentials in your git repo (and/or terraform files)!!

AWS credentials where provided to terraform via local environment variables, please see documentation here:
[Link](https://www.terraform.io/docs/providers/aws/index.html)