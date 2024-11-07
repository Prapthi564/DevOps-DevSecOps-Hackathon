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
      - Implement **Azure Policy Compliance Scan** GitHub action within `.github/workflows/complaince-scan.yml` which triggers a policy compliance scan on the provided subscription and continue/fail the workflow based on the compliance state of the resources.
   - Ensure that compliance scans are triggered automatically during the CI/CD process.

     > **Congratulations** on completing the task! Now, it's time to validate it. Here are the steps:
     > - Hit the Validate button for the corresponding task. If you receive a success message, you can proceed to the next task. 
     > - If not, carefully read the error message and retry the step, following the instructions in the lab guide.
     > - If you need any assistance, please contact us at cloudlabs-support@spektrasystems.com We are available 24/7 to help

     <validation step="c4116d8a-97eb-4c0f-9e24-2077e5ea6a49" />
     
## Success criteria:
To complete this challenge successfully:

- Successful effectiveness of policies in enforcing security compliance.
- Successful integration of compliance scanning into the pipeline.
- Successful setup and execution of the GitHub Action.

## Additional Resources:

- Refer to [Overview of Azure Policy](https://learn.microsoft.com/en-us/azure/governance/policy/overview) for reference.
- Refer to [Azure Policy Compliance Scan](https://github.com/marketplace/actions/azure-policy-compliance-scan) for reference.


## Conclusion
Congratulations on completing the **Security Compliance as Code** challenge! Through this challenge not only implemented security policies using Azure Policy but also emphasized the importance of automating the entire process through CI/CD pipelines thus ensuring continuous compliance in a dynamic cloud environment. The next challenge focuses on seamlessly integrating and configuring Microsoft Defender for Cloud within a DevOps context, ensuring a secure and resilient software development lifecycle.
