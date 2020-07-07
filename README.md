# Zip pay challenge
API to manage Zip Pay users.

Hi Zip team. This project has been created to provide a solution for the Coding Challenge test - API to manage Zip Pay users - and as part of my application for a Software Engineer role at Zip. In the sections below you will find comments, assumptions and requirements to run this project. Thank you for the chance to solve this test.
Luis Del Valle
0452523942
luis@luis-delvalle.com

### Application components

This VS Solution includes
* APIs: .NET Core 3.1 Azure Functions Project to implement all the endpoints needed (CreateUser, GetUser, ListUsers, CreateAccount, ListAccounts)
* Database: Azure Storage Table is used to persist data in this project. The uniqueness of the records is guaranteed by using email as the Rowkey value 
* UnitTests: .NET Core 3.1 XUnit Test Project
* Testing: A collection of POSTMAN requests are provided in order to assist with testing 
* No GUI interface is provided, except for the Console Interface generated by running the API project.


### Prerequisites

To run this project on your local machine, you will need:

```
Visual Studio 2019 Version 16.4 or higher
```
```
.NET Core 3.1 SDK (or lower if you choose to point the project to another version of .NET Core, like 2.1 for example
```
```
Microsoft Azure Storage Emulator (link to install: https://docs.microsoft.com/en-us/azure/storage/common/storage-use-emulator#get-the-storage-emulator)
```

optionally, you can also install (to help visualise the data in the Storage Tables),

```
Microsoft Azure Storage Explorer (link to install: https://azure.microsoft.com/en-us/features/storage-explorer/)
```

alternatively, docker support has been added to this project.

### Database connections

I have provisioned an Azure Storage Table resource in my personal account in Azure. When running the project, the application will store all data into that provisioned resource, however if needed, the development storage emulator can be used instead by changing the following setting in local.settings.json:

```
"AzureWebJobsStorage": "UseDevelopmentStorage=true"
```


### To run this project

* After installing Microsoft Azure Storage Emulator in your machine, open the project in VS and run it.

### Assumptions

* No particular assumption were taken in the implementation of this solution.
