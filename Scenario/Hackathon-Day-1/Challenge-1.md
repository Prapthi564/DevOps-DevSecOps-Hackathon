# Challenge 1:  Continuous Integration and Deployment for .NET Apps using GitHub Actions

## Introduction:
This challenge is designed to evaluate participants' skills in creating a robust CI/CD pipeline leveraging GitHub Actions specifically tailored for a .NET application. It aims to assess their capability to not only establish a seamless pipeline but also to guarantee the successful deployment of the application. Additionally, participants will demonstrate their expertise by efficiently modifying and integrating new features into the existing codebase, showcasing their proficiency in adapting and evolving the application's functionality.

## Challenge Objectives:

>**Note:** Solely the use GitHub and GitHub Actions for CI/CD; no usage of Azure DevOps or any external CI/CD services.

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

- Successfully deployed the Azure Search Service and the Azure Storage Account
- Successfully added the data into the storage account.
- Successfully indexed the documents in Azure AI Search using the Azure portal.
- Suuccessfully customized the index and configured the indexer in Azure AI Search.
- Successfully modified and explored search components using JSON definitions.
- Successfully utilized the Azure AI Search SDK to create a client application for search.
- Successfully ran the web application locally, performed searches, and refined search results successfully.

## Additional Resources:

- Refer to [What is Azure AI Search](https://learn.microsoft.com/en-us/azure/search/search-what-is-azure-search) for reference.
- [Create an Azure AI Search Solution](https://github.com/MicrosoftLearning/AI-102-AIEngineer/blob/master/Instructions/22-azure-search.md)
- [Searching document text at scale using Azure Cognitive Search](https://benalexkeen.com/searching-document-text-at-scale-using-azure-cognitive-search/)
