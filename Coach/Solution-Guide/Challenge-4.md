# Challenge 04: Implementing Monitoring Solutions for Contoso Traders

## Introduction

In this challenge, user/attendee will integrate Azure's monitoring tools—Azure Monitor and Application Insights—into their Azure-based application. Monitoring is vital for maintaining efficiency and resilience in cloud applications, enabling proactive issue identification and seamless user experiences.

This is the solution guide that contains all of the comprehensive, step-by-step directions needed to finish the challenge.

## Solution Guide

### Task 1: Deploy Monitoring Infrastructure

1. You will deploy the complete monitoring infrastructure using the bicep template. The monitoring infrastructure includes a Log Analytics workspace, Application Insights, a secret created for Application Insights, and a monitoring dashboard.

1. Open VS Code, update the variable `$userName` and `$password` in the code mentioned below, and execute the code. The below-mentioned code uses a bicep template named `monitorinfra.bicep` which contains code to deploy the complete monitoring infrastructure.
   
   - **Email/Username:** <inject key="GitHubUsername"></inject>
   - **Password:** <inject key="GitHubPassword"></inject>
```
$userName = shivashant@onmicrosoft.com
$password = qweqweqwew

$securePassword = $password | ConvertTo-SecureString -AsPlainText -Force
$cred = new-object -typename System.Management.Automation.PSCredential -argumentlist $userName, $SecurePassword

Connect-AzAccount -Credential $cred | Out-Null

$RGname = "contosotraders-$deploymentid"

cd C:\Workspaces\lab\devsecops\iac

New-AzResourceGroupDeployment -Name "createresources" -TemplateFile "monitorinfra.bicep" -TemplateParameterFile "monitorinfra.parameters.json" -ResourceGroup $RGname
```

### Task 2: Monitoring using Application Insights

1. In the Azure Portal, navigate to **contoso-traders-<inject key="Deploymentid" enableCopy="false" />** **(1)** resource group and select the **Application Insights** resource with the name  **contoso-traders-ai<inject key="Deploymentid" />** **(2)**.

   ![](media/upd-ex6-t1-openai.png)
   
1. From the Overview of **contoso-traders-ai<inject key="Deploymentid"  enableCopy="false" />** Application Insights resource, you can set the **Show data for last** as per your requirement of monitoring insights.

   ![](media/upd-ex6-t1-set-showdata.png)
   
1. In the first graph, you can see the number of failed requests for the Application access.

   ![](media/upd-ex6-t1-failedrequests.png)
   
1. In the next graph, you can see the average server response time.

   ![](media/upd-ex6-t1-server-response-time.png)
   
1. In the next graph, you can see the number of server requests.

   ![](media/upd-ex6-t1-server-requests.png)
   
1. In the last graph, you can see the average availability.

   ![](media/upd-ex6-t1-availability.png)  

## Success criteria:
To complete this challenge successfully:

- Successful integration of Azure Monitor and Application Insights within the application environment, ensuring seamless data collection and monitoring capabilities.
- Selection and configuration of key performance metrics relevant to the application's functionality and performance goals.
- Establishment of effective alerting mechanisms with well-defined thresholds, ensuring timely notifications for potential issues or deviations in monitored metrics.

## Additional Resources:

- Refer to [Application Insights Overview](https://learn.microsoft.com/en-us/azure/azure-monitor/app/app-insights-overview) for reference.
- [Application Insights for ASP.NET Core applications](https://learn.microsoft.com/en-us/azure/azure-monitor/app/asp-net-core?tabs=netcorenew%2Cnetcore6).
- Refer to [Azure Monitor vs Application Insights](https://azurelib.com/azure-monitor-vs-application-insights/) for reference.
