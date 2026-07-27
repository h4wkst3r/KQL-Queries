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

## Compute SSH Key Modification

`AzureMLComputeSSHKeyModification.kql`

This query will show when a caller modifies an Azure ML compute SSH public key or performs related compute stop/start activity.

## Training Job Creation

`AzureMLTrainingJobCreation.kql`

This query will show when a caller creates an Azure ML training job, including command, environment, and compute details when available in activity properties.

## Training Job Recon and Secret Hunting

`AzureMLTrainingJobReconAndSecretHunting.kql`

This query will show high-volume Azure ML job reads and related log blob downloads, which can indicate training job variable or log searching activity.

## Environment Config Access

`AzureMLEnvironmentConfigAccess.kql`

This query will show Azure ML environment reads and related Dockerfile or environment blob downloads.

## Notebook and Compute Recon

`AzureMLNotebookAndComputeRecon.kql`

This query will show Azure ML notebook and compute enumeration that can precede direct notebook code execution.

## MLOKit Use

`MLOKitUsage.kql`

This query will detect when MLOKit is used to interact with Azure storage blobs, which happens when attempting to perform dataset or model theft attacks.