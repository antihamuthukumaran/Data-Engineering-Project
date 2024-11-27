# Data-Engineering-Project

  Welcome to the Data-Engineering-Project repository! This project is designed to showcase key concepts and skills in data engineering, including data extraction, transformation, loading (ETL), and pipeline creation.

#Project Overview

  This project aims to:

   * Extract raw data from various sources.
   * Transform the data to make it usable for analysis.
   * Load the processed data into a target destination (e.g., a database, data warehouse).
   *  Automate and monitor data pipelines.

  #Steps Involved:
   * Environment Setup
   * Data Ingestion
   * Data Transformation
   * Data Loading
   * Data Reporting
   * End to End Pipeline Testing

![Picture4](https://github.com/user-attachments/assets/1c955a06-7dbc-4dde-a6e4-6e6043612f9e)

#Here’s a step-by-step guide to create the necessary resources for your Data Engineering Project in Azure:

  1. Create a Resource Group
	   * Go to the Azure Portal: https://portal.azure.com.
     * In the search bar, type Resource Groups and select it.
  	 * Click + Create.
      *	Fill in the required details:
        *	Subscription: Choose your subscription.
        *	Resource Group Name: Anitha_Data_Engineering_Project.
        *	Region: Choose a location (e.g., East US, Central Canada).
 	   * Click Review + Create, then click Create.

  2. Create a Storage Account
      *	In the search bar, type Storage accounts and select it.
        *	Click + Create.
        *	Fill in the required details:
            *	Subscription: Use the same as the Resource Group.
            *	Resource Group: Select Anitha_Data_Engineering_Project.
            *	Storage Account Name: Choose a unique name (e.g., anithaengineeringdata).
            *	Region: Same as the Resource Group.
            *	Performance: Standard.
            *	Redundancy: Locally-redundant storage (LRS) is cost-effective.
      *	Click Review + Create, then click Create.
        
	 3.Create a Data Factory
       *	In the search bar, type Data Factory and select it.
         *	Click + Create.
         *	Fill in the required details:
              *	Subscription: Use the same as the Resource Group.
              *	Resource Group: Select Anitha_Data_Engineering_Project.
              *	Region: Choose the same region.
              *	Name: Give it a unique name (e.g., anithadatafactory).
         *	Click Git Configuration:
            *	Skip it for now or connect it to a Git repository if required.
         *	Click Review + Create, then click Create.

	   4.Create an Azure Databricks Workspace
        * In the search bar, type Azure Databricks and select it.
           * Click + Create.
           * Fill in the required details:
               * Subscription: Use the same as the Resource Group.
              *	Resource Group: Select Anitha_Data_Engineering_Project.
              *	Workspace Name: Give it a name (e.g., anithadatabricks).
              *	Region: Choose the same region.
              *	Pricing Tier: Standard or Premium based on requirements.
           *	Click Review + Create, then click Create.
 
     	  5.Create a Key Vault
         	 * In the search bar, type Key Vaults and select it.
            *	Click + Create.
            *	Fill in the required details:
                *	Subscription: Use the same as the Resource Group.
                *	Resource Group: Select Anitha_Data_Engineering_Project.
                *	Vault Name: Give it a unique name (e.g., anithakeyvault).
                *	Region: Choose the same region.
                *	Settings:
            *	Soft Delete: Enabled (recommended).
            *	Purge Protection: Enabled (recommended).
            *	Click Review + Create, then click Create.
 
    	  6.Create a Synapse Workspace
     				 *	In the search bar, type Azure Synapse Analytics and select it.
             *	Click + Create.
              *	Fill in the required details:
                *	Subscription: Use the same as the Resource Group.
                *	Resource Group: Select Anitha_Data_Engineering_Project.
                *	Workspace Name: Give it a unique name (e.g., anithasynapse).
                *	Region: Choose the same region.
                *	Data Lake Storage:
            *	Select the storage account you created earlier.
            *	Choose a new file system name (e.g., datalake).
            *	Click Security:
                *	Use an existing Key Vault or select the one you created earlier.
            *	Click Review + Create, then click Create.
