# ARM-Templates

Create Template Guidelines.

https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-authoring-templates

I have created below ARM Templates 

1. Create Azure Sql Database with import bacpac file, and firewall rules to access database

Input Parameters ( I have set default value for which I think best to keep, for some of need to update as per value)

1. databaseServerName - Azure Sql Database server name 
2. databaseLogin - Login  Username
3. databasePassword - Login Password
4. authAVLibraryCollation - Database collation
5. authAVLibraryDatabaseName
6. authAVLibraryTier - Database Tier
7. authAVLibrarySkuName - datbase SKU name
8. authAVLibraryMaxSizeBytes - Datbase max size bytes
9. authAVLibraryZoneRedundant - Zone Redundant
10. authAVLibraryStorageKeyType - Storage Key type
11. authAVLibraryStorageUri - Storage URL of bacpac file
12. authAVLibraryStorageKey  - storage key of bacpac file
13. authAVLibraryAuthenticationType - authentication type of import bacpac file

Resources

1. Database Server
2. Database (depends on #1 database server)
3. Firewall rules (depends on #1 database server, and #2 database)

