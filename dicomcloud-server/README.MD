# DICOMcloud Server (basic deployment)

**Development Branch:** <a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FDICOMcloud%2FDICOMcloud%2Fdevelopment%2Fazuredeploy.json">
<img src="https://camo.githubusercontent.com/9285dd3998997a0835869065bb15e5d500475034/687474703a2f2f617a7572656465706c6f792e6e65742f6465706c6f79627574746f6e2e706e67" data-canonical-src="http://azuredeploy.net/deploybutton.png" style="max-width:100%;">
</a> 

<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FDICOMcloud%2FDICOMcloud%2Fdevelopment%2Fazuredeploy.json" target="_blank">
<img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.png"/>
</a>

This template deploys a [**DICOMcloud server**](https://github.com/DICOMcloud/DICOMcloud). The **DICOMcloud server** implements the standard **[DICOMweb](https://www.dicomstandard.org/dicomweb/) protocol with qido-rs, wado-rs, stow-rs, wado-uri RESTful services**

## DICOMcloud server overview and deployed resources

This is an overview of the Simple DICOMcloud server deployment

The following resources are deployed as part of the solution

### Web Application

The DICOMcloud web application is where the server runs and can be accessed. The following resources will be created:

+ **HostingPlan**: The hosting plan where the website will be hosted. By default, the Free (F1) plan will be selected.
+ **Website**: The website running the DICOMcloud server
+ **DICOMcloud package**: The DICOMcloud package is built from the [repository here](https://github.com/DICOMcloud/DICOMcloud)

### SQL Database 

DICOMcloud utilizes Azure SQL Database to index the DICOM files. The following resources will be deployed:

+ **Azure SQL Database**: The SQL Server database. By default, te Basic Edition will be deployed (cost $5)

### Storage

DICOMcloud uses Azure Blob storage for storing the DICOM files. The following resource will be deployed:

+ **Azure Blob Storage**: 

## Deployment steps

You can click the "deploy to Azure" button at the beginning of this document or deploy from Visual Studio.

## Notes

Contact <support@zeuscloudimaging.com> For professional services deploying, managing or customizing the solution.

`Tags: DICOMcloud, DICOMweb, PACS`
