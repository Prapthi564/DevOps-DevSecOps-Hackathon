# Challenge 1: Code Security Enhancements

## Introduction:
This challenge equips participants with practical skills in fortifying code using GitHub's Advanced Security Features. The goal is to identify vulnerabilities, proactively address security issues, and establish robust security practices within repositories. In today's software landscape, security is crucial, and this challenge matters as it enables participants to leverage GitHub's tools effectively, fostering a proactive security culture through code scanning, CodeQL integration, and handling security advisories.
## Challenge Objectives:

1. **Repository Setup:**
   - Participants must create a new repository on GitHub for the .NET application.
   - Initialize the repository with a basic .NET application structure or use an existing codebase.

2. **Setup CI/CD Workflow with GitHub Actions:**

   -  Participants need to create a GitHub Actions workflow file (e.g., **.github/workflows/main.yml**) to automate the CI/CD process.
   -  Implement a workflow that includes steps for building the .NET application.
   -  Add necessary steps for running tests to ensure the application's stability.
  
3. **Deployment Setup:**
   - Configure the workflow to deploy the .NET application using GitHub Actions.
   - Use appropriate deployment strategies such that the application is deployed over Azure.

4. **Integration Testing and Feature Modification:**
   - Modify an existing feature or add a new feature to the .NET application codebase.
   - The modified/added feature must be integrated seamlessly with the existing application functionalities.
  
## Success criteria:
To complete this challenge successfully:

- The application can be deployed using VS Code which supports GitHub Actions.
- **CI/CD Implementation**: The CI/CD pipeline should be established using GitHub Actions, encompassing build, test, and deployment stages effectively.
- **Deployment Accuracy**: The application must be successfully deployed using GitHub Actions, and the chosen deployment strategy should align with the project's requirements.
- **Code Modification**: Clear adherence to best practices are expected for any modifications made to the codebase, ensuring seamless integration of new features.

## Additional Resources:

- Refer to [GitHub Actions and .NET](https://learn.microsoft.com/en-us/dotnet/devops/github-actions-overview) for reference.
- [Building and testing .NET](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-net).
- [Why CI/CD](https://resources.github.com/ci-cd/).
- [Continuous Deployment with Github Actions: An Example](https://www.dolthub.com/blog/2020-11-23-continous-deployment-with-github-actions/).
- [How to build a CI/CD pipeline with GitHub Actions in four simple steps](https://github.blog/2022-02-02-build-ci-cd-pipeline-github-actions-four-steps/).
