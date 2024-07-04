# Challenge 09: Securing DevOps with Microsoft Defender for Cloud

### Estimated Time: 30 minutes

### Introduction:
Contoso Traders, an e-commerce platform, is committed to delivering secure and efficient software solutions. In this challenge, as a DevSecOps engineer, you are responsible for ensuring the security of your applications throughout the development lifecycle. Your organization has recently adopted Microsoft Defender for Cloud to enhance the security posture of your DevOps pipelines.

Your task is to implement Microsoft Defender for Cloud DevOps security measures by configuring the necessary GitHub actions within your created GitHub repository, viewing the scanned results, and connecting your GitHub environment to Microsoft Defender for Cloud.

## Challenge Objectives:

>**Note:** The GitHub account provided whose credentials would be available in the environment details tab, has GitHub Enterprise with GitHub Advanced Security enabled for the ease of execution of this challenge.

1. **Connect GitHub Environment to Microsoft Defender for Cloud:**

   - Connect your GitHub environment to Microsoft Defender for Cloud.
   - Extend the security capabilities of Defender for Cloud to your GitHub resources by enabling the **Cloud Security Posture Management (CSPM) features**.
   - Ensure that the Microsoft Defender for cloud is configured such that it auto-discovers all repositories in GitHub organizations and any future organizations where the DevOps security GitHub application is installed.

2. **Configure Microsoft Security DevOps GitHub Action:**
   
   - Integrate the Microsoft Defender for Cloud GitHub Action into the workflow of your GitHub repository.
   - Create a `.github/workflows/msdevopssec.yml` file in your repository to perform static code analysis, vulnerability scanning, and compliance checks.

3. **Investigate and Remediate:**

   - Trigger the GitHub Action workflow created in the previous challenge objective to run Microsoft Defender for Cloud scans.
   - Review, identify, and understand the security findings and recommendations provided by Microsoft Defender for Cloud.
   - Implement fixes or enhancements to address the security findings identified during the scan.
   - Ensure that the GitHub Action workflow passes successfully after addressing the security issues.

## Success criteria:
To complete this challenge successfully:

- Appropriate integration and configuration of Microsoft Security DevOps GitHub Action.
- Successful connection of GitHub environment to Microsoft Defender for Cloud.

## Additional Resources:

- Refer to [Overview of Microsoft Defender for Cloud DevOps Security](https://learn.microsoft.com/en-us/azure/defender-for-cloud/defender-for-devops-introduction) for reference.
- Refer to [Configure the Microsoft Security DevOps GitHub action](https://learn.microsoft.com/en-us/azure/defender-for-cloud/github-action) for reference.
- Refer to [Connect your GitHub Environment to Microsoft Defender for Cloud](https://learn.microsoft.com/en-us/azure/defender-for-cloud/quickstart-onboard-github) for reference.

## Challenge Validations:

1. After completing the challenge, you need to visit the **Lab Validation (1)** tab and click on the **VALIDATE (2)** button under Actions to perform the validation steps. Verify that you have met the success criteria of the challenge. 
 
    ![](../media/validate01.png "Validation")
 
1. If the validation status displays **Success** for all the validation steps, **congratulations!**. This means that you have successfully completed the challenge.
 
     ![](../media/validate02.png "Validation")

1. If the validation status displays **Fail**, **don't worry!** This could mean that you did not perform the challenge correctly.
 
     ![](../media/validate03.png "Validation")
 
1. Hover your mouse over the `i` **(1)** icon to see the error message and determine the root cause of the failure. Based on the error message, revisit the challenge as necessary, and redo the validation by clicking on the **VALIDATE (3)** button again.

     ![](../media/validate04.png "Validation")
 
1. If you are still having trouble, you can reach out to the support team via `labs-support@spektrasystems.com` for further assistance. The support team is available to help you troubleshoot and resolve any technical issues or validation issues that may arise while the lab environment is live.

## Conclusion
Congratulations on completing the **Securing DevOps with Microsoft Defender for Cloud** challenge! Through this challenge you have seamlessly integrated and configured Microsoft Defender for Cloud within a DevOps context, ensuring a secure and resilient software development lifecycle.

Congratulations! You have successfully completed all the challenges.

