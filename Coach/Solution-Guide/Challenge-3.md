# Challenge 03: GitHub Advanced Security - Dependency Management and Secret Scanning

## Introduction

In this challenge, attendee/user will continue to focus on implementing crucial GitHub Advanced security features like GitHub Dependabots and Secret Scanning.

This is the solution guide, which provides all the specific, step-by-step directions needed to do the task.

## Solution Guide

### Task 1: Configure Dependabot Alerts:

In this task, you will use Dependabot to track the versions of the packages we use in our GitHub repository and create pull requests to update packages for us.

1. In your lab files GitHub repository, navigate to the **Settings** ***(1)*** tab and select the **Code security and analysis** ***(2)*** under Security from side blade. Make sure **Dependabot alerts** is **Enabled** ***(3)***, if not click on **Enable** to Enable Dependabot alerts. Click on **Enable** ***(4)*** to Enable Dependabot security updates.

   > **Note**: Enabling the `Dependabot security updates` will also automatically enable `Dependency graph` and `Dependabot alerts`.

   ![The GitHub Repository Security Overview tab.](media/cl3-t1-s1.png "GitHub Repository Security Overview")

   > **Note**: The alerts for the repository may take some time to appear. The rest of the steps for this task rely on the alerts to be present. You can continue with the next exercise as this is an independent task and doesn't affect the lab. Please visit this task later and complete the task.

1. To observe Dependabot issues, navigate to the **Security** ***(1)*** tab and select the **View Dependabot alerts** ***(2)*** link.

   ![GitHub Dependabot alerts in the Security tab.](media/cl3-t1-s2.png "GitHub Dependabot alerts")

1. You should arrive at the `Dependabot alerts` blade in the `Security` tab.

   ![GitHub Dependabot alerts in the Security tab.](mediacl3-t1-s3.png "GitHub Dependabot alerts")

1. Sort the Dependabot alerts by `Package name`. Under the **Package** ***(1)*** dropdown menu, search for **node-forge** ***(2)*** by typing in the search box and select **node-forge** ***(3)*** vulnerability.

   ![Summary of the `handlebars` Dependabot alert in the list of Dependabot alerts.](media/ex5-t3-node-forge.png "`handlebars` Dependabot alert")

1. Select any of the `node-forge` Dependabot alert entries to see the alert detail. After reviewing the alert, select **Review security update**.

   ![The `handlebars` Dependabot alert detail.](media/ex5-t3-reviewsu.png "Dependabot alert detail")
   
   **Note:** If you see Create Security Update option, click on it. After it is created then select Review security update. 

1. Navigate to **Pull Requests** ***(1)*** tab, find the Dependabot security patch pull request ***(2)*** and merge it to your main branch.

   ![List of Pull Requests.](media/cl3-t1-s6.png "Pull Requests")
   
1. Click on **Merge pull request** and followed by click on **Confirm merge**. 

   ![The Pull Request Merge Button in the Pull Request detail.](media/ex5-t3-merge-pr.png "Pull Request Merge Button")
    
   >**Note**: In case you see any errors with the merge request. Retry steps 4 to 6 by selecting any other Dependabot alert.

1. Pull the latest changes from your GitHub repository to your local GitHub folder.

   ```pwsh
   cd C:\Workspaces\lab\devsecops  # This path may vary depending on how
                                                            # you set up your lab files repository
   git pull
   ```
   
## Task 2: Implement Secret Scanning:

In this task, you'll explore how secret scanning works and see how it generates alerts. GitHub scans repositories for known types of secrets, to prevent fraudulent use of secrets that were committed accidentally.

1. From your GitHub repository, click on the **Settings** tab.

   ![](media/2dg110.png)
    
1. Select **Code security (1)** from the sidebar and make sure **Secret scanning is enabled (2)**.

   ![](media/2dg111.png)   
    
1. Navigate back to **Code (1)** and click on **src (2)** folder.

   ![](media/2dg112.png)    
   
1. Click on **Add file** and select **create new file** option.

   ![](media/2dg113.png)    
   
1. Add new file with name **build.docker-compose.yml (1)** name, add the code mentioned below **commit** the file. Here, you'll expose the **application ID** of a service principal.

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
   
   ![](media/2dg115.png)   
   
1. Select **Security (1)** tab and click on **Secret scanning (2)** from the sidebar. Here, you'll notice that an alert is generated referring to the same **Application ID** which was exposed in `build.docker-compose.yml` file. This is how the Secret scanning feature works and generates alerts to notify you.

   ![](media/2dg116.png) 

## Success criteria:
To complete this challenge successfully:

- Successful implementation of GitHub Dependabots for identifying and addressing security vulnerabilities.
- Setup secreting scanning and updated the code base to resolve the alerts.

## Additional Resources:

- Refer to [Secret Scanning](https://docs.github.com/en/code-security/secret-scanning/about-secret-scanning) for reference.
- Refer to [GitHub Dependabot](https://docs.github.com/en/code-security/dependabot/dependabot-alerts/about-dependabot-alerts) for reference.
