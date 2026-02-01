# Jenkins_Assignment

# CI Lab Project – Jenkins

## Overview
This project demonstrates the implementation of Continuous Integration (CI) using Jenkins.  
It showcases source code management with GitHub, automated build and testing using Maven, execution of a Python script, and CI pipeline automation using both Freestyle and Multibranch Pipeline jobs.

---

## Project Structure
```plaintext
CILabProject/
├── src/
│ ├── main/
│ │ ├── java/com/muj/ci/Calculator.java
│ │ └── resources/
│ └── test/
│ └── java/com/muj/ci/CalculatorTest.java
├── pom.xml
├── Jenkinsfile
├── docker/
│ └── Dockerfile
├── scripts/
│ ├── build.bat
│ └── deploy.sh
│ └── hello.py
└── README.md
```


---

## Technologies Used
- Jenkins
- GitHub
- Java (JDK 17)
- Maven
- JUnit
- Python
- Docker

---

## Jenkins Jobs Implemented

### 1. Freestyle Job
- Connects to GitHub repository
- Polls SCM for changes
- Builds and tests Java code using Maven
- Executes a Python script
- Archives build artifacts
- Publishes JUnit test results
- Sends email notifications

### 2. Multibranch Pipeline
- Automatically discovers branches from GitHub
- Uses Jenkinsfile for pipeline definition
- Executes build and test stages for each branch
- Displays pipeline stage view and build status

---

## Jenkinsfile Overview
The Jenkinsfile defines a declarative pipeline with the following stages:
- Checkout
- Build
- Test

JUnit test results are published after execution, and the pipeline is configured to handle empty test results gracefully.

---

## How to Build and Test Locally
Make sure Java and Maven are installed, then run:
```bash
mvn clean test
```
```plaintext

Plugins Used in Jenkins

Pipeline

Blue Ocean

Git

GitHub

Subversion

Maven Integration

Gradle

Ant

JUnit

JaCoCo

Cobertura

Email Extension

Slack Notification

Docker

Kubernetes

SSH
```

Notes

Jenkins was run locally using jenkins.war

Email notifications may fail due to SMTP authentication restrictions, but configuration is completed as required

This project is intended for academic and learning purposes
