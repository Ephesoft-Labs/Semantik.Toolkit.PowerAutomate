# Pipeline Delimited File Export
**Available for:** Semantik Invoice

## Overview
This exports Semantik data into a pipe delimited file for columns with table headers that match (case-sensitive) the expected column names. Other columns are not placed in the file.

The expected column names are:

- Item #
- Description
- Shipped
- Unit Price
- Ext Price

**Note:** A column name with a period cannot be set as expected as it is an invalid character in Microsoft Flow expression language.

## Prerequisites
* Ephesoft Semantik account
* OneDrive for Business account

## How It Works
Each time the flow is triggered, invoice data is converted to a pipe delimited CSV file and saved to a OneDrive for Business folder.

**NOTE**: The folder path must exist in the OneDrive for Business account associated with the connection used for this flow. If the folder doesn't exist the flow will fail.