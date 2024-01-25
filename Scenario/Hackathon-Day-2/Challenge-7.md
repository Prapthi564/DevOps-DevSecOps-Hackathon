# Challenge 07: Enhancing Contoso Traders with GitHub Copilot

### Estimated Time: 60 minutes

### Introduction:
Contoso Traders is a web application for stock trading. In this challenge, as a DevOps engineer, your focus is to seamlessly implement and test new features with Copilot, ensuring accuracy and alignment. Conduct a thorough code review and enhance security using GitHub Advanced Security's CodeQL. Streamline development with a GitHub Actions CI/CD pipeline for Contoso Traders, ensuring efficient and secure deployment.

## Challenge Objectives:

1. **Feature Addition with GitHub Copilot:**
   
2. **Unit Test Generation with Copilot:**
   - After implementing the feature, you should use GitHub Copilot to generate unit tests for the new functionality which includes assessing the accuracy and completeness of the generated unit tests.
   - Ensure that the generated test cases are alligning with the code analogy with successful test passes.
   - Resolve any unit test failures with the help of GitHub Copilot chat.

3. **Code Review and Security Check:**
   - Perform a code review and on the new feature implemented using GitHub Copilot.
   >**Hint:** Focus areas include code readability, adherence to best practices, and ensuring that the new feature aligns with the existing codebase.
   - Run a security check on the newly implemented code using GitHub Advanced Security features thus resolving any alerts to vulnerabilities and catch any potential security issues using CodeQL over the repository.

4. **CI/CD Pipeline Setup and Deployment:**
   - Set up a GitHub Actions CI/CD pipeline for Contoso Traders hosted on GitHub.
   - The pipeline should include steps for building, testing, and deploying the new feature to the hosted application on Azure.

## Success criteria:
To complete this challenge successfully:

- Successful implementation of the new feature.
- Accuracy and completeness of the generated unit tests with all successful passes.
- Successful setup and execution of the CI/CD pipeline.

## Additional Resources:

- Refer to [About GitHub Copilot Chat](https://docs.github.com/en/copilot/github-copilot-chat/about-github-copilot-chat) for reference.
- Refer to [Copilot Chat writes Unit Tests](https://dev.to/this-is-learning/copilot-chat-writes-unit-tests-for-you-1c82) for reference.
- Refer to [Using GitHub Copilot Chat in your IDE](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat-in-your-ide) for reference.

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

## Conclusion
Congratulations on completing the **Enhancing Contoso Traders with GitHub Copilot** challenge! Through this challenge you have not only focused on finding and fixing vulnerabilities but also promoted a security-conscious development mindset. The next challenge focuses on implemeting security policies using Azure Policy and integrating compliance scanning within your GitHub CI/CD pipelines.
