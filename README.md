# Contact Database Application

This repository contains the source code for the Contact Database Application. It is a web application built using ASP.NET MVC framework.

## Prerequisites

Before deploying the Contact Database Application, make sure you have the following prerequisites:

- Azure subscription
- Azure Resource Group
- Azure SQL Database
- Visual Studio or Visual Studio Code

## Deployment Steps

Follow the steps below to deploy the Contact Database Application using an ARM template:

1. Clone this repository to your local machine.

2. Open the `ContactDatabaseApp` solution in Visual Studio.

3. Update the connection string in the `Web.config` file to point to your Azure SQL Database.

4. Build the solution to ensure all dependencies are resolved.

5. Right-click on the `ContactDatabaseApp` project and select **Publish**.

6. In the Publish dialog, select **Azure** as the target.

7. Sign in to your Azure account and select the Azure subscription and resource group where you want to deploy the application.

8. Click on **Publish** to start the deployment process.

9. Once the deployment is complete, you can access the Contact Database Application using the provided URL.

## GitHub Actions Pipeline Workflow

To automate the deployment process, this repository includes a GitHub Actions pipeline workflow file. The workflow file is located at `.github/workflows/deploy.yml`.

The workflow file contains the necessary steps to build and deploy the Contact Database Application to Azure using the ARM template.

To use the GitHub Actions pipeline workflow, follow these steps:

1. Fork this repository to your GitHub account.

2. Navigate to the **Actions** tab in your forked repository.

3. Click on **Set up a workflow yourself**.

4. Replace the contents of the editor with the following code:
5. Replace `<your-app-name>` with the name of your Azure Web App.

6. Replace `<your-slot-name>` with the name of your deployment slot (optional).

7. Commit the changes to the workflow file.

8. Push the changes to the `master` branch of your forked repository.

9. The GitHub Actions pipeline will automatically trigger and deploy the Contact Database Application to Azure.

## License

This project is licensed under the [MIT License](LICENSE).
