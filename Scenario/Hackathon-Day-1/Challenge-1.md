# Challenge 01: Continuous Integration and Deployment for Contoso Traders using GitHub Actions

### Estimated Time: 90 minutes

## Introduction:
This challenge is designed to evaluate your skills in creating a robust CI/CD pipeline leveraging GitHub Actions. It aims to assess your capability to not only establish a seamless pipeline but also to guarantee the successful deployment of the application.

You are a DevOps engineer tasked with setting up a robust Continuous Integration and Continuous Deployment (CI/CD) pipeline for an e-commerce application named Contoso Traders. The goal is to set up a GitHub repository, implement a CI/CD workflow using GitHub Actions, deploy the application to Azure, and make rolling updates to the repository.

## Accessing GitHub

1. To access and login to GitHub, open the edge browser from inside the environment and navigate to **[GitHub](https://github.com/)**.

2. Sign in to GitHub by clicking on the **Sign in** button from the top right corner of the GitHub home page.

3. On the **Sign into GitHub tab** you will see a login screen, enter the following email/username and then click on **Next**.

   - **Email/Username:** <inject key="GitHubUsername"></inject>

1. Now enter the following password and click on **Sign in**.

   - **Password:** <inject key="GitHubPassword"></inject>

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
  
1. Confirm you have a resource group **DevOps-DevSecOps** present, as shown in the below screenshot. You need to use the **<inject key="Resource Group Name"/>** resource group throughout this challenge.

## Challenge Objectives:

>**Note:** Solely use GitHub and GitHub Actions for CI/CD; no usage of Azure DevOps or any external CI/CD services.

1. **Setup a GitHub repository:**
   - Create a new GitHub repository with public access permission.
   - You are provided with an e-commerce application named Contoso Traders which needs to be deployed and hosted in Azure.
   - You can navigate to `C:\Workspaces\lab\aiw-devops-with-github-lab-files` directory and find the complete code base of the application.
   - Using Visual Studio code, connect to the GitHub repository which you created in earlier step and push the application code base to your GitHub repository.

2. **Deploy Infrastructure:**
   - Create an Azure resource group in your Azure subscription with name **Contoso-Traders<inject key="DeploymentID" enableCopy="false" />**.
   - Deploy the below-mentioned bicep template using GitHub Action name **deploy-infrastructure.yml** which is present in `.github/workflow` directory .
      
2. **Setup CI/CD Workflow:**

   - Create GitHub secrets with same name as mentioned below.
      - **SQL_PASSWORD** - You need to store ADO.NET connection string of your SQL database in this secret.
      - **SERVICEPRINCIPAL** - create a secret to store service principal details. You can find the details in Environment details tab of your environment.
      - **ENVIRONMENT**: create a secret to store the deployment ID. You can find the details in Environment details tab of your environment.
   - In GitHub repository, navigate to  **.github/workflow** where you will be able find the yaml workflow. This YAML file is partially updated, you need to update the YAML files with right steps and complete the workflow. This workflow should deploy the application into Azure. 
  
3. **Deploy the application using GitHub Actions:**
   - Use GitHub Actions and run the workflow file which you updated in previous task.

4. **Test the application and perform rolling updates:**
   - Navigate to Azure portal and check the application status using Azure Endpoint.
   - Update the workflow file to intitate Action run on changes to the GitHub repository.
  
## Success criteria:
To complete this challenge successfully:

- Verify the successful deployment of the Infrastructure of the application in the Azure portal.
- Verify the GitHub Action, all the jobs in GitHub Action should be completed without any error.
- Verify the deployment and hosting of the Contoso Traders application in Azure.

## Additional Resources:

Here are a few documentation and guides to assist you in completing the challenge.
- [GitHub Actions](https://docs.github.com/en/actions)
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
Congratulations on successfully completing the **Continuous Integration and Deployment using GitHub** challenge. You have successfully verified the configuration of a GitHub repository, established a functional CI/CD workflow, utilized GitHub Actions to deploy the .NET application. In the next challenge, you will look into implementing security features offered by GitHub.




