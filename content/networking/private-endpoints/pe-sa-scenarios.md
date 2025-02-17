# Special Case - Storage Accounts

[home](./readme.md)

Storage accounts have a special consideration due to the fact that they do not have one single endpoint, but instead have an endpoint for each of their sub-resources.

When creating a Private Endpoint for a storage, you would be prompted to select which sub-resource that you wish to use.

![Selecting a sub-resource for a storage account in the create a private endpoint experience](img/sa-options.png)

Each one of these sub-resources will need their own DNS zone considerations, and their own private endpoints.

## Special Note on Data Lake Gen2

When you are using the Data Lake Gen2 function (by enabling hierarchical namespaces on the storage account) you will need both the DFS sub-resource endpoint/zone and the Blob sub-resource endpoint/zone.

[home](./readme.md)
