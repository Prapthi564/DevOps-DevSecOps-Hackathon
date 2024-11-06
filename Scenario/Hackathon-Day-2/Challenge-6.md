# Challenge 06: DevSecOps with AI-Powered GitHub Actions

### Estimated Time: 40 minutes

### Introduction:
Contoso Traders, an e-commerce platform, is committed to delivering secure and efficient software solutions. In this challenge, as a Lead DevSecOps engineer, your focus is to enhance the DevSecOps workflow by leveraging AI-driven GitHub Actions that focus on code review and security checks for pull requests thus leading to improved code quality and enhanced security practices in the development lifecycle.

You need to focus on completing the implementation of the below-mentioned GitHub Actions:

**AI Code Review Action**: AI Code Reviewer is a GitHub Action that leverages OpenAI's GPT-4 API to provide intelligent feedback and suggestions on your pull requests. This powerful tool helps improve code quality and saves developers time by automating the code review process.

**AI Security Check for Pull Request**: This GitHub Action uses OpenAI's GPT to analyse code in pull requests and identify potential security and privacy vulnerabilities and comment to the pull request with the findings.

## Challenge Objectives:

>**Note:** This challenge requires you to sign in/sign up to a free tier OpenAI account. This free-tier provides you with a $5 credit limit that expires within a period of 3 months from the day of account activation.

1. **Configure and implement AI Code Review GitHub Action:**
   - Sign In/ Sign up to an OpenAI account and create a new secret key (API key).
     
      >**Note:** This API key will be used as you move forward in the challenge. Keep it handy!
   
   - Use this OpenAI API key to create a GitHub Secret in your repository with the name `OPENAI_API_KEY`.
   - Create a `.github/workflows/ai-code-review.yml` file in your repository to successfully implement `AI Code Reviewer` GitHub Action which provides intelligent feedback and suggestions on your pull requests.
  
     > **Congratulations** on completing the task! Now, it's time to validate it. Here are the steps:
     > - Hit the Validate button for the corresponding task. If you receive a success message, you can proceed to the next task. 
     > - If not, carefully read the error message and retry the step, following the instructions in the lab guide.
     > - If you need any assistance, please contact us at cloudlabs-support@spektrasystems.com We are available 24/7 to help
     
      <validation step="685d64ce-179b-4c15-8cc2-82d854a586c7" />

2. **Configure and implement AI Security Check for Pull Requests:**
   - Use the previously created OpenAI API key to create a GitHub Secret in your repository with the name `OPENAI_TOKEN`.
   - Create a new GitHub secret named `GH_TOKEN` with a GitHub Personal Access Token with the `repo` and `write:discussion` scopes enabled.
   - Create a new `./github/workflows/ai-security-check-for-pr.yml` workflow file in your repository to successfully implement `AI Security Check for Pull Requests` GitHub Action which analyzes the code in each pull request targeting the specified branch.
  
     > **Congratulations** on completing the task! Now, it's time to validate it. Here are the steps:
     > - Hit the Validate button for the corresponding task. If you receive a success message, you can proceed to the next task. 
     > - If not, carefully read the error message and retry the step, following the instructions in the lab guide.
     > - If you need any assistance, please contact us at cloudlabs-support@spektrasystems.com We are available 24/7 to help

     <validation step="b9e89676-4cb0-4324-b705-4afe80f5af32" />
  
## Success criteria:
To complete this challenge successfully:

- Successful implementation of the `AI Code Review Action` and generation of review comments based on the AI's response and added to the pull request.
- Successful implementation of the `AI Security Check for Pull Requests` and generation of comments to the pull requests based on AI's analysis of the code.

## Additional Resources:

- Refer to [AI Code Review Action](https://github.com/marketplace/actions/ai-code-review-action) for reference.
- Refer to [AI Security Check for Pull Request](https://github.com/marketplace/actions/ai-security-check-for-pull-request) for reference.


## Conclusion
Congratulations on completing the **DevSecOps with AI-Powered GitHub Actions** challenge! Through this challenge you have seamlessly integrated AI-driven GitHub Actions, elevated code quality, security, and developer productivity. In the next challenge, you will focus on using GitHub Copilot Chat to implement/add new features to the existing Contoso Traders Application and deploy the changes to Azure through CI/CD.
