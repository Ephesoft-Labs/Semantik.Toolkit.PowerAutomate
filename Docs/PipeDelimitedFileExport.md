# Pipeline Delimited File Export
**Available for:** Semantik Invoice

## Overview
This flow converts a completed invoice to a pipe delimited file and then saves the file to a OneDrive for Business account.

PowerAutomate expects the following columns to be exported from Semantik in the order listed below:

- Item #
- Description
- Shipped
- Unit Price
- Ext Price

## Prerequisites
* Ephesoft Semantik account
* OneDrive for Business account

## How It Works
Each time the flow is triggered, invoice data is converted to a pipe delimited CSV file and saved to a OneDrive for Business folder.

**NOTE**: The folder path must exist in the OneDrive for Business account associated with the connection used for this flow. If the folder doesn't exist the flow will fail.