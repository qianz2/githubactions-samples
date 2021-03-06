A repo for testing GitHub actions created by the [Oryx](https://github.com/microsoft/oryx) team.

| Action Version | App type | Links |
| - | - | - |
| v1 | Python - Django | [`Source Code`](sampleApps/python/django-app), [`Workflow File`](.github/workflows/v1.deployPythonAppToAzureWebApp.yml), [Runs](https://github.com/MicrosoftOryx/githubactions-samples/actions?query=workflow%3A.github%2Fworkflows%2Fv1.deployPythonAppToAzureWebApp.yml), [Live Site](http://v1-python-sampleapp.azurewebsites.net/uservoice/) |
| v1 | Node - Hello World | [`Source Code`](sampleApps/node/webfrontend), [`Workflow File`](.github/workflows/v1.deployNodeAppToAzureWebApp.yml), [Runs](https://github.com/MicrosoftOryx/githubactions-samples/actions?query=workflow%3A.github%2Fworkflows%2Fv1.deployNodeAppToAzureWebApp.yml), [Live Site](http://v1-node-sampleapp.azurewebsites.net/) |
| v1 | ASP.NET Core MVC | [`Source Code`](sampleApps/dotNetCore/NetCoreApp31.MvcApp), [`Workflow File`](.github/workflows/v1.deployDotNetCoreAppToAzureWebApp.yml), [Runs](https://github.com/MicrosoftOryx/githubactions-samples/actions?query=workflow%3A.github%2Fworkflows%2Fv1.deployDotNetCoreAppToAzureWebApp.yml), [Live Site](http://v1-dotnetcore-sampleapp.azurewebsites.net/) |
| v1 | PHP - Hello World | [`Source Code`](sampleApps/php/twig-example), [`Workflow File`](.github/workflows/v1.deployPhpAppToAzureWebApp.yml), [Runs](https://github.com/MicrosoftOryx/githubactions-samples/actions?query=workflow%3A.github%2Fworkflows%2Fv1.deployPhpAppToAzureWebApp.yml), [Live Site](http://v1-php-sampleapp.azurewebsites.net/) |
| v2 | Python - Django | [`Source Code`](sampleApps/python/django-app), [`Workflow File`](.github/workflows/v2.deployPythonAppToAzureWebApp.yml), [Runs](https://github.com/MicrosoftOryx/githubactions-samples/actions?query=workflow%3A.github%2Fworkflows%2Fv2.deployPythonAppToAzureWebApp.yml), [Live Site](http://v2beta-python-sampleapp.azurewebsites.net/uservoice/) |
| v2 | Node - Hello World | [`Source Code`](sampleApps/node/webfrontend), [`Workflow File`](.github/workflows/v2.deployNodeAppToAzureWebApp.yml), [Runs](https://github.com/MicrosoftOryx/githubactions-samples/actions?query=workflow%3A.github%2Fworkflows%2Fv2.deployNodeAppToAzureWebApp.yml), [Live Site](http://v2beta-node-sampleapp.azurewebsites.net/) |
| v2 | ASP.NET Core MVC | [`Source Code`](sampleApps/dotNetCore/NetCoreApp31.MvcApp), [`Workflow File`](.github/workflows/v2.deployDotNetCoreAppToAzureWebApp.yml), [Runs](https://github.com/MicrosoftOryx/githubactions-samples/actions?query=workflow%3A.github%2Fworkflows%2Fv2.deployDotNetCoreAppToAzureWebApp.yml), [Live Site](http://v2beta-dotnetcore-sampleapp.azurewebsites.net/) |
| v2 | ASP.NET Core MVC + React | [`Source Code`](sampleApps/multiPlatform/dotnetreact), [`Workflow File`](.github/workflows/v2.deployDotNetCoreReactAppToAzureWebApp.yml), [Runs](https://github.com/MicrosoftOryx/githubactions-samples/actions?query=workflow%3A.github%2Fworkflows%2Fv2.deployDotNetCoreReactAppToAzureWebApp.yml), [Live Site](http://v2-dotnetcore-sampleapp.azurewebsites.net/) |


#### To build and deploy sample apps on-demand
The command that used for kicking off a build:

```
curl -X POST https://api.github.com/repos/MicrosoftOryx/githubactions-samples/dispatches \
-H 'Accept: application/vnd.github.everest-preview+json' \
-H 'Authorization: token ${{secrets.YOUR_PERSONAL_ACCESS_TOKEN}}' \
--data '{"event_type": "build_application"}'
```
