# Challenge 05: Resilience Testing using Azure Chaos Studio

### Estimated Time: 1 Hour

## Introduction:
This challenge centers around Azure Load Testing and Azure Chaos Studio, empowering you to perform performance tests and enhance application resilience. In the modern digital landscape, guaranteeing optimal performance during heavy loads and fortifying against disruptions is essential. Through Azure's tools, you'll gain insights into proactive issue detection and methods to reinforce your applications.

## Challenge Objectives:

1. **Setting Up Azure Load Testing:**
   - Create an Azure Load Testing instance and execute a test using a JMeter file to simulate high-scale traffic on a web application.
     - Set up an Azure Load Testing instance within the Azure portal and then use a JMeter file—a script defining load testing scenarios—to simulate high-scale traffic on a web application hosted on Azure. The goal is to evaluate the application's performance, scalability, and capacity under heavy loads.

2. **Configuring Targets and Running Experiments in Azure Chaos Studio:**

   -  Utilize Azure Chaos Studio to assess the resilience of the web application by introducing real faults and disruptions.
     -  Participants will explore Azure Chaos Studio, a tool designed to measure and enhance cloud application resilience. Configure specific targets within their web application and create controlled experiments by introducing real-world disruptions, such as latency injection, fault injection, or other fault scenarios. The objective is to observe how the application responds to these disruptions and identify areas for improvement in its resilience and fault tolerance.
  
## Success criteria:
To complete this challenge successfully:

- Successful setup and execution of Azure Load Testing using a JMeter file to simulate high-scale traffic on the web application.
- Well-designed experiments within Azure Chaos Studio introducing real-world disruptions to the web application, showcasing a clear understanding of resilience testing principles.

## Additional Resources:

- Refer to [Continuous validation with Azure Load Testing and Azure Chaos Studio](https://learn.microsoft.com/en-us/azure/architecture/guide/testing/mission-critical-deployment-testing) for reference.
- [What is Azure Chaos Studio?](https://learn.microsoft.com/en-us/azure/chaos-studio/chaos-studio-overview).
- [Load test a website by using a JMeter script in Azure Load Testing](https://learn.microsoft.com/en-us/azure/load-testing/how-to-create-and-run-load-test-with-jmeter-script?tabs=portal).
- [Intro to Chaos Engineering and Azure Chaos Studio](https://pdtit.medium.com/intro-to-chaos-engineering-and-azure-chaos-studio-preview-5e85fff10642).

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
