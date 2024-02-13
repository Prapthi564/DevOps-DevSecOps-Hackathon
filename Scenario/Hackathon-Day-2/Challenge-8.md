# Challenge 08: Security Compliance as Code

### Estimated Time: 60 minutes

### Introduction:
In this challenge, you are a DevOps engineer responsible for ensuring the security compliance of your organization's Azure resources. Your task is to implement and enforce security policies using Azure Policy over the Azure resources and integrate compliance scanning into the GitHub CI/CD pipelines for your Azure projects. 

## Challenge Objectives:

1. **Implement Security Policies using Azure Policy:**
   - Enforce compliance by assigning *built-in* policy definition called **Inherit a tag from the resource group if missing** to add the specified tag with its value from the parent resource group to new or updated resources missing the tag.
   - Implement an Azure custom policy to restrict resource deployments to the **East US** region within a designated resource group.
   - Ensure that your policies are effective in preventing non-compliant resources from being deployed.
   
2. **Integrate Compliance Scanning in CI/CD pipeline:**
   - Integrate a compliance scanning step into your GitHub pipeline that checks for policy compliance before allowing deployment.
      - Implement **Azure Policy Compliance Scan** GitHub action within `.github/workflows/workflow.yml` which triggers a policy compliance scan on the provided subscription and continue/fail the workflow based on the compliance state of the resources.
   - Ensure that compliance scans are triggered automatically during the CI/CD process.

## Success criteria:
To complete this challenge successfully:

- Successful effectiveness of policies in enforcing security compliance.
- Successful integration of compliance scanning into the pipeline.
- Successful setup and execution of the GitHub Action.

## Additional Resources:

- Refer to [Overview of Azure Policy](https://learn.microsoft.com/en-us/azure/governance/policy/overview) for reference.
- Refer to [Azure Policy Compliance Scan](https://github.com/marketplace/actions/azure-policy-compliance-scan) for reference.

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
Congratulations on completing the **Security Compliance as Code** challenge! Through this challenge not only implemented security policies using Azure Policy but also emphasized the importance of automating the entire process through CI/CD pipelines thus ensuring continuous compliance in a dynamic cloud environment. The next challenge focuses on seamlessly integrating and configuring Microsoft Defender for Cloud within a DevOps context, ensuring a secure and resilient software development lifecycle.
