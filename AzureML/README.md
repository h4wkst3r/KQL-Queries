# Azure ML KQL Queries

The KQL queries in this folder can be used as part of threat hunting rules or scheduled analytic rules within Microsoft Sentinel.

## Dataset Poisoning

`AzureMLDatasetPoisoning.kql`

This query will show when a dataset has been modified.

## Dataset Recon

`AzureMLDatasetRecon.kql`

This query will show when a user has listed all datasets within a workspace, which is indicative of dataset recon.

## Dataset Theft

`AzureMLDatasetTheft.kql`

This query will show when a user has read a dataset from a workspace and also a datastore.

## Model Recon

`AzureMLModelRecon.kql`

This query will shown when a user has listed all models within a workspace, which is indicative of model recon

## Model Theft

`AzureMLModelTheft.kql`

This query will show when a user has read a model from a workspace and also downloaded a file from an Azure storage blob.

## Model Poisoning

`AzureMLModelPoisoning.kql`

This query will show when a user has read a model from a workspace and also uploaded a file to an Azure storage blob.

## MLOKit Use

`MLOKitUsage.kql`

This query will detect when MLOKit is used to interact with Azure storage blobs, which happens when attempting to perform dataset or model theft attacks.


