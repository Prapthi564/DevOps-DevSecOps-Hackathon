# DevOps/DevSecOps Challenge - 1-Day Hackathon

Welcome to the DevOps/DevSecOps Challenge hackathon! 

- In this hackathon, you'll elevate your .NET applications to new heights! Dive into the world of Continuous Integration and Deployment (CI/CD) using GitHub Actions, fortify repository security with GitHub Advanced Security, enforce advanced security measures and policies, and implement monitoring solutions with resilience testing using Azure Chaos Studio.

## Table of Contents

- [Introduction](#introduction)
- [Learning Objectives](#learning-objectives)
- [Challenges](#challenges)
- [Prerequisites](#prerequisites)

## Introduction

In this hackathon, you will automate your development lifecycle with CI/CD using GitHub Actions, ensuring efficient builds, tests, and deployments. Strengthen repository security with GitHub Advanced Security, covering vulnerability detection, dependency scanning, and code analysis.

Explore and navigte through the advanced security challenges and enforce policies, aligning with industry standards. Transition to the cloud with Azure Chaos Studio, implementing monitoring solutions and resilience testing to enhance application reliability.

This hack consists of five challenges and is designed to be self-administered, so anyone can complete the material independently. Whether you have limited to no experience with DevSecOps or have not experimented using CI/CD and GitHub before, but want a deeper understanding of its implementation, this hack is for you.

## Learning Objectives

By participating in this hackathon, you will:

- Leveraging GitHub's Potential: Manage code efficiently with repositories, utilize GitHub Codespace for a personalized cloud dev environment, and automate your pipeline using workflows and actions.
- Explore GitHub's advanced security for proactive vulnerability detection. Safeguard your codebase with robust protective measures.

## Challenges

1. **Challenge 01: Continuous Integration and Deployment for .NET Apps using GitHub Actions**
   - Create a new repository on GitHub for the .NET application.
   - Initialize the repository with a basic .NET application structure or use an existing codebase.
   - Setup CI/CD Workflow with GitHub Actions by creating a YAML workflow file.
   - Deployment Setup:
      - Configure the workflow to deploy the .NET application using GitHub Actions and use appropriate deployment strategies such that the application is deployed over Azure.
   - Integration Testing and Feature Modification:
      - Modify an existing feature or add a new feature to the .NET application codebase which must be integrated seamlessly with the existing application functionalities.

2. **Challenge 02: Code Security Enhancements**
   - Activate code scanning for the repository.
      - Code scanning is set up in a repository (which could be a sample or personal project) to identify security vulnerabilities within the codebase. At least three of these vulnerabilities are addressed, and detailed documentation, including their impact and the steps taken to fix them, is provided along with before-and-after code snippets.
   - Enable CodeQL alerts to proactively identify and resolve security issues.
   - Enable repository security advisories to receive alerts about vulnerable dependencies.
   - Implement strategies to mitigate identified security risks in dependencies.
       
3. **Challenge 03: Dependency Management and Security**:
    - Dependency Security:
       - Analyze dependencies in a repository to identify and mitigate security risks.
    - Implement Dependabot in a repository for automated package version tracking, generating two pull requests to update outdated packages. Document the review process and decisions on merging or rejecting these pull requests.
    - Use GitHub's secret scanning capabilities to detect and secure sensitive information within a repository and identify instances where sensitive information (e.g., API keys, credentials) was successfully detected and secured.

4. **Challenge 04: Implementing Monitoring Solutions**
   - Integrate Azure Monitor and Application Insights seamlessly within the Azure-based application infrastructure.
   - Define and configure key performance metrics for monitoring purposes.
   - Create effective alerting mechanisms based on predefined thresholds.
   - Design comprehensive dashboards for real-time visualization of application health and performance metrics.
   - Optimize the monitoring setup for actionable insights and usability.

5. **Challenge 05: Resilience Testing using Azure Chaos Studio**
   - Create an Azure Load Testing instance and execute a test using a JMeter file to simulate high-scale traffic on a web application.
   - Configuring Targets and Running Experiments in Azure Chaos Studio

Each challenge comes with its own set of tasks and objectives.

Feel free to explore the challenges, learn, and have fun during this hackathon! If you have any questions, don't hesitate to reach out to your coach.

Happy hacking!
