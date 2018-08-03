# dotnet-core-store

A sample e-commerce demo using asp.net core 2.1 &amp; angular 6

## Required Dependencies

Install latest sdk and cli tools _(2.1 required for WebApiController annotations)_

- .net core sdk 2.1
- .net core cli 2.1

Update dotnet project templates

- `dotnet new --install Microsoft.DotNet.Web.Spa.ProjectTemplates::2.1.0`
- `dotnet new --install Microsoft.AspNetCore.SpaTemplates::2.1.0-preview1-final`

Install global Angular CLI tools

```
npm i -g // TODO
```

## Getting Started

Generate a new project using the angular spa template

`dotnet new angular -o dotnet-core-store`

If packages didn't restore automatically, do it manually

`dotnet restore`

Update npm dependencies for the client app

`cd clientapp && npm install`

Run the app. The client app will start automatically in the background with `ng serve` configured for HMR in dev mode

`cd .. && dotnet run`

## Deploying to Azure

We will deploy to an Azure App Service Free Tier instance. The client app will be built automatically using `ng build` when the `dotnet publish` command is invoked.

## Next Steps

- Add Swagger/Swashbuckle integration for auto-generated API docs (3rd party middleware example)
- Add tests and configure a CI/CD pipeline tool (basic DevOps configuration)
- Configure Docker containers to deploy to Linux and Windows hosts with one command (showcase cross-platform features)
