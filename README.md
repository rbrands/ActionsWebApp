![ASP.NET web app core](https://github.com/rbrands/ActionsWebApp/workflows/ASP.NET%20web%20app%20core/badge.svg)

# ActionsWebApp
Demo App to play around with GitHub Actions

ActionsWebApp was created in Visual Studio 2010 as Razor App with .NET Core 3.1, then added to Version Control und published to GitHub

The Git workflow follows the "Release Flow" as used by Microsoft and described in https://docs.microsoft.com/en-us/azure/devops/learn/devops-at-microsoft/release-flow

GitHub actions are used for CI - every commit and pull request to branch "master" will be compiled and deployed to slot "dev" in Azure Web App https://actionswebapp-dev.azurewebsites.net/
Every branch name like 'releases/...' will trigger a compilation and deployment to slot "release" in Azure Web App https://actionswebapp-release.azurewebsites.net/
