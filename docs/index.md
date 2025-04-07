# Trusted Application Pipeline Software Template

This application, **z9mbbmvbw-dotnet-basic**, was created from a Trusted Application Pipeline Software Template.

The software templates create a new source and gitops deployment repositories with a sample source application. 

## Repositories

The source code for your application can be found in [https://github.com/rhtap-rhdh-qe/z9mbbmvbw-dotnet-basic ](https://github.com/rhtap-rhdh-qe/z9mbbmvbw-dotnet-basic ).
 
The gitops repository, which contains the kubernetes manifests for the application can be found in 
[https://github.com/rhtap-rhdh-qe/z9mbbmvbw-dotnet-basic-gitops ](https://github.com/rhtap-rhdh-qe/z9mbbmvbw-dotnet-basic-gitops ) 

## Application namespaces 

The default application will be found in the following namespaces. Applications can be deployed into unique namespaces or multiple software templates can also bet generated into the same group namespaces.  

|  Namespace   |  Description   |  
| -------- | -------- |
| **rhtap-app-ci** | The namespace used for CI workloads |
| **rhtap-app-development** | The default application during development. Every build will be deployed to this namespace for testing. |
| **rhtap-app-stage** | The staging namespace for this application. Promotion from development to stage is manual via an update to the [gitops repository](https://github.com/rhtap-rhdh-qe/z9mbbmvbw-dotnet-basic-gitops ) in the components/z9mbbmvbw-dotnet-basic/overlays/stage directory |
| **rhtap-app-prod** | The production namespace for this application. Promotion from stage to production is manual via an update to the [gitops repository](https://github.com/rhtap-rhdh-qe/z9mbbmvbw-dotnet-basic-gitops ) in the components/z9mbbmvbw-dotnet-basic/overlays/prod directory |