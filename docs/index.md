# Trusted Application Pipeline Software Template
test this template
This application, **test-go-template**, was created from a Trusted Application Pipeline Software Template.

The software templates create a new source and gitops deployment repositories with a sample source application. 

## Repositories

The source code for your application can be found in [https://github.com/testrhtaporg/test-go-temp ](https://github.com/testrhtaporg/test-go-temp ).
 
The gitops repository, which contains the kubernetes manifests for the application can be found in 
[https://github.com/testrhtaporg/test-go-temp-gitops ](https://github.com/testrhtaporg/test-go-temp-gitops ) 

## Application namespaces 

The default application will be found in the following namespaces. Applications can be deployed into unique namespaces or multiple software templates can also bet generated into the same group namespaces.  

|  Namespace   |  Description   |  
| -------- | -------- |   
| **rhtap-app-development** | The default application during development. Every build will be deployed to this namespace for testing. | 
| **rhtap-app-stage** | The staging namespace for this application. Promotion from development to stage is manual via an update to the [gitops repository](https://github.com/testrhtaporg/test-go-temp-gitops ) in the components/test-go-template/overlays/prod directory |  
| **rhtap-app-prod** | The production namespace for this application. Promotion from stage to production is manual via an update to the [gitops repository](https://github.com/testrhtaporg/test-go-temp-gitops ) in the components/test-go-template/overlays/prod directory | 
