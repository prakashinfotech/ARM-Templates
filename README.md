# ARM-Templates 

ARM Templates to create azure sql database with restore database (bacpac) file from blob url.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

ARM Templates

### Installing

The template consists of JSON and expressions that you can use to construct values for your deployment. For a step-by-step tutorial on creating a template, see [Create your first Azure Resource Manager template](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-authoring-templates)

ARM Template code includes code to create following resources

* Database Server
* Database (depends on #1 database server)
* Firewall rules (depends on #1 database server, and #2 database)


### Create Azure Sql Database with import bacpac file, and firewall rules to access database

Input Parameters ( I have set default value for which I think best to keep, for some of need to update as per value)

* databaseServerName - Azure Sql Database server name 
* databaseLogin - Login  Username
* databasePassword - Login Password
* authAVLibraryCollation - Database collation
* authAVLibraryDatabaseName
* authAVLibraryTier - Database Tier
* authAVLibrarySkuName - datbase SKU name
* authAVLibraryMaxSizeBytes - Datbase max size bytes
* authAVLibraryZoneRedundant - Zone Redundant
* authAVLibraryStorageKeyType - Storage Key type
* authAVLibraryStorageUri - Storage URL of bacpac file
* authAVLibraryStorageKey  - storage key of bacpac file
* authAVLibraryAuthenticationType - authentication type of import bacpac file


## Deployment

[Deploy resources with Resource Manager templates and Azure portal](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-template-deploy-portal)

## Authors

* **Hiral Patel** (https://github.com/mehiralpatel)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

