# Challenge 08: Security Compliance as Code

## Introduction

In this challenge, you are a DevOps engineer responsible for ensuring the security compliance of your organization's Azure resources. Your task is to implement and enforce security policies using Azure Policy over the Azure resources and integrate compliance scanning into the GitHub CI/CD pipelines for your Azure projects.

This is the solution guide, which provides all the specific, step-by-step directions needed to do the task.

## Solution Guide

## Exercise 1: Azure Policy Implementation

### Task 1: Assign a Built-In policy

In this task, you will enforse compliance with Azure Policy by assigning a policy definition. A policy definition defines under what condition a policy is enforced and what effect to take. In this solution, you will assign the built-in policy definition called **Inherit a tag from the resource group if missing** to add the specified tag with its value from the parent resource group to new or updated resources missing the tag and then implement a new custom policy for the resources that have been deployed with the specific SKU's.

1. Go to the Azure portal to assign policies. Search for and select **Policy**.

   ![](../media/cl8-ex1-t1-s1.png)

2. Select **Assignments** on the left side of the Azure Policy page. An assignment is a policy that has been assigned to take place within a specific scope.

   ![](../media/cl8-ex1-t1-s2.png)

3. Select **Assign Policy** from the top of the **Policy - Assignments** page.

   ![](../media/cl8-ex1-t1-s3.png)

4. On the **Assign Policy** page and **Basics** tab, perform the following steps:
   - Select the **Scope** by selecting the ellipsis and selecting either a management group or subscription **(1)**. Optionally, select a resource group. A scope determines what resources or grouping of resources the policy assignment gets enforced on.
   - Click on **Select** at the bottom of the Scope pane **(2)**.

   ![](../media/cl8-ex1-t1-s4.png)

5. Resources can be excluded based on the **Scope**. **Exclusions** start at one level lower than the level of the **Scope**. **Exclusions** are optional, so leave it blank for now.

6. Select the **Policy definition** ellipsis to open the list of available definitions. You can filter the policy definition Type to Built-in to view all and read their descriptions.

7. Select **Inherit a tag from the resource group if missing**. If you can't find it right away, type **inherit a tag** into the search box and then press ENTER or select out of the search box. Click on **Select** at the bottom of the **Available Definitions** page once you have found and selected the policy definition.

   ![](../media/cl8-ex1-t1-s7.png)

8. The **Assignment name** is automatically populated with the policy name you selected, but you can change it. For this example, leave **Inherit a tag from the resource group if missing**. You can also add an optional **Description**. The description provides details about this policy assignment.

9. Leave **Policy enforcement** as **Enabled**. When Disabled, this setting allows testing the outcome of the policy without triggering the effect.

10. **Assigned by** is automatically filled based on who is logged in. This field is optional, so custom values can be entered.

11. Select the **Parameters** tab at the top of the wizard.

12. For **Tag Name**, enter **Environment**.

13. Select the **Remediation** tab at the top of the wizard.

14. Leave **Create a remediation task** unchecked. This box allows you to create a task to alter existing resources in addition to new or updated resources.

15. **Create a Managed Identity** is automatically checked since this policy definition uses the modify effect. **Permissions** is set to Contributor automatically based on the policy definition.

16. Select the **Non-compliance messages** tab at the top of the wizard.

17. Set the **Non-compliance message** to **This resource doesn't have the required tag**. This custom message is displayed when a resource is denied or for non-compliant resources during regular evaluation.

18. Select the **Review + create** tab at the top of the wizard.

19. Review your selections, then select **Create** at the bottom of the page.

### Task 2: Implement a new custom policy

Now that you've assigned a built-in policy definition, you can do more with Azure Policy. Next, create a new custom policy to save costs by validating that virtual machines created in your environment can't be in the G series. This way, every time a user in your organization tries to create a virtual machine in the G series, the request is denied.

1. Select **Definitions** under **Authoring** in the left side of the Azure Policy page.

   ![](../media/cl8-ex1-t2-s1.png)

2. Select **+ Policy definition** at the top of the page. This button opens to the **Policy definition** page and enter the following information:
   - Select the **Definition location** **(1)** by selecting the ellipsis and selecting a subscription. Optionally, select a resource group. A scope determines what resources or grouping of resources the policy assignment gets enforced on.
   - **Name:** Require VM SKUs not in the G series. **(2)**
   - **Description:** This policy definition enforces that all virtual machines created in this scope have SKUs other than the G series to reduce cost. **(3)**
   - **Category:** Create a new catrgory named **Compute**.  **(4)**

   ![](../media/cl8-ex1-t2-s2.png)

3. Copy the following JSON code and then update it for your needs with:

   - The policy parameters.
   - The policy rules/conditions, in this case - VM SKU size equal to G series
   - The policy effect, in this case - **Deny**.

   ```
   {
       "policyRule": {
           "if": {
               "allOf": [{
                       "field": "type",
                       "equals": "Microsoft.Compute/virtualMachines"
                   },
                   {
                       "field": "Microsoft.Compute/virtualMachines/sku.name",
                       "like": "Standard_G*"
                   }
               ]
           },
           "then": {
               "effect": "deny"
           }
       }
   }
   ```

   >**Note:** The **field** property in the policy rule must be a supported value. An example of an alias might be `Microsoft.Compute/VirtualMachines/Size`.
   
## Task 2: Implement Azure Policy Compliance Scan:

In this task, you'll explore how secret scanning works and how it generates alerts. GitHub scans repositories for known types of secrets to prevent fraudulent use of secrets that were accidentally committed.

1. From your GitHub repository, click on the **Settings** tab.

   ![](../media/2dg110.png)
    
1. Select **Code security (1)** from the sidebar and make sure **Secret scanning is enabled (2)**.

   ![](../media/2dg111.png)   
    
1. Navigate back to **Code (1)** and click on the **src (2)** folder.

   ![](../media/2dg112.png)    
   
1. Click on **Add file** and select the **create new file** option.

   ![](../media/2dg113.png)    
   
1. Add a new file with the name **build.docker-compose.yml (1)**, add the code mentioned below **commit** the file. Here, you'll expose the **application ID** of a service principal.

   ```
   version: "3.4"
   services:
   api:
      build: ./ContosoTraders.Ui.Website/
      app id: 36540dcd-7bc3-4e16-90ca-4decb9ff8c36
      app secret: i1R8Q~Hn8dHn86VlWE7xJtLR4FKTIcQBXcebqcv4
   web:
      build: ./ContosoTraders.Api.Products
   ```
   
   ![](../media/2dg115.png)   
   
1. Select the **Security (1)** tab and click on **Secret scanning (2)** from the sidebar. Here, you'll notice that an alert is generated referring to the same **Application ID** that was exposed in the `build.docker-compose.yml` file. This is how the Secret scanning feature works and generates alerts to notify you.

   ![](../media/2dg116.png) 

## Success criteria:
To complete this challenge successfully:

- Successful effectiveness of policies in enforcing security compliance.
- Successful integration of compliance scanning into the pipeline.
- Successful setup and execution of the CI/CD pipeline.

## Additional Resources:

- Refer to [Overview of Azure Policy](https://learn.microsoft.com/en-us/azure/governance/policy/overview) for reference.
- Refer to [Azure Policy Compliance Scan](https://github.com/marketplace/actions/azure-policy-compliance-scan) for reference.
