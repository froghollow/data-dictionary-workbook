# Data Dictionary Workbook

A **Data Dictionary** is a database that stores information about data.   This information, called **Metadata**, includes the name of the data, type of data, the location of the data, and the meaning of the data.  

Metadata is not only useful as documentation for humans to understand data.   Metadata is also useful as input parameters queried by process automation scripts.  Metadata-driven automation enables common processes to be generally applied to various and sundry datasets described in the data dictionary.  Metadata is the key to implementing an Enterprise approach to process automation.

It is ideal, of course, is to have a common centralized Data Dictionary.  But various tools use different metadata stores.  So, we need to be able to transform metadata among formats in order to support these various tools as their adoption and utilization evolves throughout the Enterprise.

We are currently using, or planning to use, several Data Dictionary formats:
- **AWS Glue Catalog** stores structural metadata about data assets hosted on AWS Native Services
- **Data Asset Structure Metadata** (attached 'data/dataAssetMetadata.csv', ref Ch 3 of OCDO Playbook Fig. 3.2)
- **FiscalData** Data Dictionaries (csv) and Meta Objects (json) embedded in API result sets to publically-accessible Bureau information.
- **RAML** is a modeling language for REST APIs.  It is used to describe the functionality and data content of the API.   Mulesoft, at the core of the Fiscal Service Enterprise API Strategy, utilizes RAML to define APIs published on Exchange.
- **Tableau Catalog** describes data, processes, and lineage within the Tableau tool set.  DDMAP has implemented Tableau and Tableau Prep for self-service analytics, reporting, and data transformation.  DDMAP exports selected data sets from Tableau in Glue Catalog and S3 for downstream access by AWS native services.
- **Unity Catalog** (future) stores structural metadata about data assets hosted on the Databricks platform (USA Spending, FS Data Hub).

This notebook contains tools to transform metadata among some of these Data Dictionary formats.

## Contents

- [**/data**](./data) folder contains sample input and output files.
- [**/python**](./python) folder contains Python code modules
- [**data-dictionary-workbook.ipynb**](data-dictionary-workbook.ipynb) is a Jupyter notebook that demonstrates how to use the Python code.

You can copy these files and folders into your Jupyter environment and run the Notebook.   Or source the modules into your execution environment and write your own calls.


