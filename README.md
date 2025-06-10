### Dataform demo

### Demo overview

Demo of how [Dataform](https://cloud.google.com/dataform/docs/quickstart-create-workflow) can be used to create a workflow 
of actions to compute several reports of a fictitious eCommerce company. 

The source data is from a BigQuery public datset

```shell
bigquery-public-data.thelook_ecommerce
```

TheLook is a fictitious eCommerce clothing site developed by the Google Looker team. 
The dataset contains information about customers, products, orders, logistics, web events and digital marketing campaigns. 
The contents of this dataset are synthetic, and are provided to industry practitioners for the purpose of product discovery, testing, and evaluation.
This public dataset is hosted in Google BigQuery. 

This Dataform worklfow computes: 

 * top customers according to their spend
 * top products acording to historical sales

This Dataform worklfow splits out the following to mimic best practice:

 * source definitions to identify the BigQuery public dataset & tables used 
 * staging to define the BigQuery views holding intermediate results
 * reporting to define BigQuery tables holding the top customers & top products reports


