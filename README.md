# Java Web App Deployment with AWS CI/CD
This README provides an overview of the project "Java Web App Deployment with AWS CI/CD," detailing the steps taken to set up a continuous integration and continuous deployment pipeline for a Java web application using AWS services and Git/GitHub.

<br>

## Table of contents
- [Introduction](#introduction) 
- [Technologies](#technologies) 
- [Setup](#setup) 
- [Contact](#contact) 
- [Conclusion](#conclusion) 

<br>

## Introduction
This project focuses on establishing a robust workflow for deploying a Java web application. It covers the essential steps from version control with Git and GitHub to preparing the local development environment and pushing code to a remote repository. The goal is to demonstrate a foundational setup that can be extended into a full CI/CD pipeline on AWS.

## Technologies

- Git: A distributed version control system used for tracking changes in source code, enabling collaboration among developers.

- GitHub: A web-based platform for version control and collaboration, hosting Git repositories and offering features like issue tracking and pull requests.

- AWS EC2: Amazon Elastic Compute Cloud, a web service that provides resizable compute capacity in the cloud. Used here as a remote server for development and deployment.
- Key pairs, SSH connections,
- Java Web App: The application being developed and deployed. Install Maven, Java and git on the EC2 instance running Amazon linus. Created a sample Java web app using Maven archetype

## Setup
The setup process involved several key stages:

1. Git Initialization:

- git init: Initialized a local Git repository in the project directory to begin tracking changes.

2. Connecting to GitHub Repository:

- git remote add origin [YOUR GITHUB REPO LINK]: Linked the local Git repository to a remote GitHub repository.

3. Staging and Committing Changes:

- git add .: Added all modified and new files to the Git staging area.

- git commit -m "Commit Message": Saved the staged changes as a new commit with a descriptive message.

4. Pushing to Remote Repository:

- git push -u origin master: Pushed the committed changes from the local master branch to the origin (GitHub) remote, setting it as the upstream.

5. GitHub Personal Access Token (PAT) for Authentication:

- A Personal Access Token was generated on GitHub and used as an alternative to password authentication for Git operations, providing enhanced security and granular control.

6. Git Configuration on EC2 Instance:

- git config --global user.name "Your Name" and git config --global user.email "your.email@example.com": Configured the Git user identity on the remote EC2 instance to ensure proper authorship of commits made from that environment. This configuration is isolated to the EC2 instance and does not affect your local machine's Git setup.

## Contact
For any questions or further collaboration on this project, please reach out via my GitHub profile or the project repository.<br>
- Ridwan - [ridwan.shittu@uni-bayreuth.de](mailto:ridwan.shittu@uni-bayreuth.de)
- [LinkedIn](https://www.linkedin.com/in/ridwan-shittu-aa350393/)

## Conclusion
This project successfully established the foundational version control and remote repository connection necessary for a Java web application. By leveraging Git, GitHub, and AWS EC2, we've laid the groundwork for future continuous integration and deployment efforts, ensuring code traceability and collaborative development.