# Python App Deployment Using Azure App Service and Azure CLI

This project covers deploying a Python app to Azure App Service using CLI.

Steps Followed:
- Used `az webapp up --runtime PYTHON:3.9 --sku B1 --logs` to create and deploy the app
- App Service Plan, Resource Group, and Web App created automatically
- App accessed via `http://<app-name>.azurewebsites.net`
- Static or Flask-based app support
- Optional Docker container setup with:
  ```bash
  az webapp config container set --name <app-name> --resource-group <group-name> --docker-custom-image-name <dockerhub-username>/<image-name>
