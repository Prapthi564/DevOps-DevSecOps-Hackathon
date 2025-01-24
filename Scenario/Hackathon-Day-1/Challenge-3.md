# Challenge 03: GitHub Advanced Security - Dependency Management and Secret Scanning

### Estimated Time: 40 minutes

### Introduction:

In the previous challenge, you configured a few of the GitHub Advanced security features. In this challenge, as a DevSecOps engineer, your focus is on automating security processes and preventing security vulnerabilities. The Contoso Traders application, hosted on GitHub, will benefit from crucial GitHub Advanced security features like GitHub Dependabots and Secret Scanning.

**Dependabots**: Dependabot security updates are automated pull requests that help you update dependencies with known vulnerabilities. Dependabot version updates are automated pull requests that keep your dependencies updated, even when they don't have any vulnerabilities.

**Secret Scanning**: GitHub secret scanning is a security feature provided by GitHub to help identify and manage sensitive information, such as API keys, tokens, and other credentials, that may have been accidentally committed to a code repository.

## Challenge Objectives:

> **Note**: Use the same GitHub repository that you created in the last challenge.

1. **Configure Dependabot Alerts:**

   -  Use Dependabot and configure it to track the versions of the packages used in your GitHub repository and create pull requests to update packages for us.
   - Track and resolve any of the dependabots alert.
  
3. **Implement Secret Scanning:**
   - Enable the Secret Scanning security feature to the existing GitHub repository.
   - Check the working of the feature by exposing the application ID of a service principal and resolving the alerts.
  
## Success criteria:
To complete this challenge successfully:

- Successful implementation of GitHub Dependabots for identifying and addressing security vulnerabilities.
- Set up secreting scanning and update the code base to resolve the alerts.

## Additional Resources:


- Refer to [Secret Scanning](https://docs.github.com/en/code-security/secret-scanning/about-secret-scanning) for reference.
- Refer to [GitHub Dependabot](https://docs.github.com/en/code-security/dependabot/dependabot-alerts/about-dependabot-alerts) for reference.

## Challenge Validations:

1. After completing the challenge, you need to visit the **Lab Validation (1)** tab and click on the **VALIDATE (2)** button under Actions to perform the validation steps. Verify that you have met the success criteria of the challenge. 
 
    ![](../media/validate01.png "Validation")
 
1. If the validation status displays **Success** for all the validation steps, **congratulations!** This means that you have successfully completed the challenge.
 
     ![](../media/validate02.png "Validation")
1. If the validation status displays **Fail**, **don't worry!** This could mean that you did not perform the challenge correctly.
 
     ![](../media/validate03.png "Validation")
 
1. Hover your mouse over the `i` **(1)** icon to see the error message and determine the root cause of the failure. Based on the error message, revisit the challenge as necessary, and redo the validation by clicking on the **VALIDATE (3)** button again.
     ![](../media/validate04.png "Validation")
 
1. If you are still having trouble, you can reach out to the support team via `cloudlabs-support@spektrasystems.com` for further assistance. The support team is available to help you troubleshoot and resolve any technical issues or validation issues that may arise while the lab environment is live.

## Conclusion
Congratulations on completing the **GitHub Advanced Security - Dependency Management and Secret Scanning** challenge! By addressing critical aspects of sensitive data security, and organization-level security settings, you've significantly strengthened the security posture of your GitHub repository. In the next challenge, you will focus on implementing monitoring over the application.
