# databricks-sales-pipeline

## Overview
This project implements a Bronze → Silver → Gold data pipeline using Databricks.

## Data Layers
- Raw: original CSV ingested as Delta tables
- Silver: cleaned, normalized, deduplicated views
- Gold: BI-ready views: a wide ventas_gold (fact + dimensions) and aggregate views (sales by employee, product, store). Includes an employee validity flag to handle historical/offboarded IDs.


The raw data consists of sales data in CSV files. These are not included in this repository.
Schema examples:
- clientes.csv
- productos.csv
- empleados.csv
- locales.csv
- facturas.csv
