# Challenge 01: Continuous Integration and Deployment for .NET Apps using GitHub Actions

### Estimated Time: 90 minutes

## Introduction:
This challenge is designed to evaluate your skills in creating a robust CI/CD pipeline leveraging GitHub Actions specifically tailored for a .NET application. It aims to assess your capability to not only establish a seamless pipeline but also to guarantee the successful deployment of the application. Additionally, you will demonstrate their expertise by efficiently modifying and integrating new features into the existing codebase, showcasing their proficiency in adapting and evolving the application's functionality.

Through this challenge, you will set up a GitHub repository, implement a CI/CD workflow using GitHub Actions, deploy a .NET application to Azure, and make modifications to the application codebase.

## Accessing GitHub

1. To access the and login to GitHub, open the edge browser from inside the environment and navigate to **[GitHub](https://github.com/)**.

2. Sign in to GitHub by clicking on the **Sign in** button from the top right corner of the GitHub home page.

3. On the **Sign into GitHUb tab** you will see a login screen, enter the following email/username and then click on **Next**.

   - **Email/Username:** <inject key="AzureAdUserEmail"></inject>

1. Now enter the following password and click on **Sign in**.

   - **Password:** <inject key="AzureAdUserPassword"></inject>

## Accessing Azure portal

1. To access the Azure portal, open the edge browser from inside the environment and navigate to **[Azure Portal](https://portal.azure.com)**.

1. On the **Sign in to Microsoft Azure** tab, you will see a login screen. Enter the following email/username and then click on **Next**. 
   * Email/Username: <inject key="AzureAdUserEmail"></inject>
        
1. Now enter the following password and click on **Sign in**.
   * Password: <inject key="AzureAdUserPassword"></inject>
     
1. If you see the pop-up **Stay Signed in?**, click No.

1. If you see the pop-up **You have free Azure Advisor recommendations!**, close the window to continue the lab.

1. If a **Welcome to Microsoft Azure** pop-up window appears, click **Maybe Later** to skip the tour.
   
1. Now you will see the Azure Portal Dashboard. Click on **Resource groups** from the Navigate panel to see the resource groups.
  
1. Confirm you have a resource group **Activate-GenAI** present, as shown in the below screenshot. You need to use the **<inject key="Resource Group Name"/>** resource group throughout this challenge.

## Challenge Objectives:

>**Note:** Solely use GitHub and GitHub Actions for CI/CD; no usage of Azure DevOps or any external CI/CD services.

1. **Repository Setup:**
   - Create a new public repository on GitHub for the .NET application.
   - Initialize the repository with a basic .NET application structure or use an existing codebase.

2. **Setup CI/CD Workflow with GitHub Actions:**

   -  Create a GitHub Actions workflow file (e.g., **.github/workflows/main.yml**) to automate the CI/CD process.
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

- The application must be deployed using VS Code which supports GitHub Actions.
- A new repository must have been created.
- **CI/CD Implementation**: The CI/CD pipeline should be established using GitHub Actions, encompassing build, test, and deployment stages effectively.
- **Deployment Accuracy**: The application must be successfully deployed using GitHub Actions, and the chosen deployment strategy should align with the project's requirements.
- **Code Modification**: Clear adherence to best practices are expected for any modifications made to the codebase, ensuring seamless integration of new features.

## Additional Resources:

- Refer to [GitHub Actions and .NET](https://learn.microsoft.com/en-us/dotnet/devops/github-actions-overview) for reference.
- [Building and testing .NET](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-net).
- [Why CI/CD](https://resources.github.com/ci-cd/).
- [Continuous Deployment with Github Actions: An Example](https://www.dolthub.com/blog/2020-11-23-continous-deployment-with-github-actions/).
- [How to build a CI/CD pipeline with GitHub Actions in four simple steps](https://github.blog/2022-02-02-build-ci-cd-pipeline-github-actions-four-steps/).

## Challenge Validations: [WIP]

1. After completing the challenge, you need to visit the **Lab Validation (1)** tab and click on the **VALIDATE (2)** button under Actions to perform the validation steps. Verify that you have met the success criteria of the challenge. 
 
    ![](../media/validate01.png "Validation")
 
1. If the validation status displays **Success** for all the validation steps, **congratulations!**. This means that you have successfully completed the challenge.
 
     ![](../media/validate02.png "Validation")
1. If the validation status displays **Fail**, **don't worry!** This could mean that you did not perform the challenge correctly.
 
     ![](../media/validate03.png "Validation")
 
1. Hover your mouse over the `i` **(1)** icon to see the error message and determine the root cause of the failure. Based on the error message, revisit the challenge as necessary, and redo the validation by clicking on the **VALIDATE (3)** button again.
     ![](../media/validate04.png "Validation")
 
1. If you are still having trouble, you can reach out to the support team via `labs-support@spektrasystems.com` for further assistance. The support team is available to help you to troubleshoot and resolve any technical issues or validation issues that may arise while the lab environment is live.

## Conclusion:
Congratulations on successfully completing the **Continuous Integration and Deployment challenge for a .NET application using GitHub Actions** challenge. Thorough this challenge, you've not only showcased your technical skills but also demonstrated your ability to implement industry-standard CI/CD practices tailored for .NET applications. This experience will undoubtedly contribute to your expertise in modern software development methodologies and tools.
