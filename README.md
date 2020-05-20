![Deploy "master" to slot "dev"](https://github.com/rbrands/ActionsWebApp/workflows/Deploy%20%22master%22%20to%20slot%20%22dev%22/badge.svg)

# ActionsWebApp
Demo App to play around with GitHub Actions

ActionsWebApp was created in Visual Studio 2019 as Razor App with .NET Core 3.1, then added to Version Control und published to GitHub

The Git workflow follows the "Release Flow" as used by Microsoft and described in https://docs.microsoft.com/en-us/azure/devops/learn/devops-at-microsoft/release-flow

GitHub actions are used for CI - every commit and pull request to branch "master" will be compiled and deployed to slot "dev" in Azure Web App https://actionswebapp-dev.azurewebsites.net/
Every branch name like 'releases/...' will trigger a compilation and deployment to slot "release" in Azure Web App https://actionswebapp-release.azurewebsites.net/

Further documentation:
Deployment: https://docs.microsoft.com/en-us/azure/app-service/deploy-continuous-deployment
Action do deploy App Service: https://docs.microsoft.com/en-us/azure/app-service/deploy-github-actions
List mit SDK Versionen: https://dotnet.microsoft.com/download/dotnet-core/3.1

The most easiest way to start with actions is to create the workflow from the Deployment Center in the Azure App Service
