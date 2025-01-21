# Challenge 06: Resilience Testing using Azure Load Testing & Azure Chaos Studio

### Estimated Time: 60 minutes

## Introduction:
As a DevOps Engineer specializing in performance and resilience testing, you are tasked with enhancing the Contoso Traders application's resilience using Azure Load Testing and Azure Chaos Studio. This challenge focuses on ensuring optimal performance during heavy loads and fortifying the application against disruptions.

The Contoso Traders application is hosted on Azure Kubernetes Service (AKS), and your goal is to assess and improve its resilience through performance testing and controlled chaos experiments.

## Challenge Objectives:

1. **Setting Up Azure Load Testing:**

   - Create an Azure Load Testing instance, and create and execute a quick test to check the load of 50 users for 2 minutes.
   - Resolve the errors if the test fails and take action to improve the application's resiliency.

2. **Create an experiment and target using Azure Chaos Studio:**

   -  Utilize Azure Chaos Studio to assess the resilience of the Azure Kubernetes service where the Contoso Traders' application is hosted.
   - Using Chaos Studio, target the AKS cluster resource.
   - Create an experiment and set up faults on AKS Chaos Mesh Pods for 5 minutes, and execute the experiment. 

## Success criteria:
To complete this challenge successfully:

- Successful setup and execution of Azure Load Testing using a quick test to simulate high-scale traffic on the web application.
- Create and verify experiment execution using Azure Chaos Studio showcasing a clear understanding of resilience testing principles.

## Additional Resources:

Here are a few documentation and guides to assist you in completing the challenge.
- [Continuous validation with Azure Load Testing and Azure Chaos Studio](https://learn.microsoft.com/en-us/azure/architecture/guide/testing/mission-critical-deployment-testing)
- [What is Azure Chaos Studio?](https://learn.microsoft.com/en-us/azure/chaos-studio/chaos-studio-overview).
- [Intro to Chaos Engineering and Azure Chaos Studio](https://pdtit.medium.com/intro-to-chaos-engineering-and-azure-chaos-studio-preview-5e85fff10642).

## Challenge Validations:

1. After completing the challenge, you need to visit the **Lab Validation (1)** tab and click on the **VALIDATE (2)** button under Actions to perform the validation steps. Verify that you have met the success criteria of the challenge. 
 
    ![](../media/validate01.png "Validation")
 
1. If the validation status displays **Success** for all the validation steps, **congratulations!** This means that you have successfully completed the challenge.
 
     ![](../media/validate02.png "Validation")
1. If the validation status displays **Fail**, **don't worry!** This could mean that you did not perform the challenge correctly.
 
     ![](../media/validate03.png "Validation")
 
1. Hover your mouse over the `i` **(1)** icon to see the error message and determine the root cause of the failure. Based on the error message, revisit the challenge as necessary, and redo the validation by clicking on the **VALIDATE (3)** button again.
     ![](../media/validate04.png "Validation")
 
1. If you are still having trouble, you can reach out to the support team via `labs-support@spektrasystems.com` for further assistance. The support team is available to help you troubleshoot and resolve any technical issues or validation issues that may arise while the lab environment is live.

## Conclusion
Congratulations on completing the **Resilience Testing using Azure Load Testing and Azure Chaos Studio** challenge! You learned about the implementation of Azure Load testing and experimented in Azure Chaos Studio. 

Congratulations! You have successfully completed all the challenges. 
