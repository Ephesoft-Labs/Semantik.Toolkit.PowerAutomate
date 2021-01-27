# Invoice To CSV
**Available for:** Semantik Invoice

## Overview
This flow converts a completed invoice to CSV and then saves the file to a OneDrive for Business account.

## Prerequisites
* Ephesoft Semantik account
* OneDrive for Business account

## How It Works
This flow uses the [Ephesoft Semantik for Invoices connector](https://us.flow.microsoft.com/en-us/connectors/shared_ephesoftsemantikforinvoices/ephesoft-semantik-for-invoices/) to automatically start a flow each time a new invoice has completed review.  Each time the flow is triggered, invoice data is saved to a OneDrive for Business folder.

## Files Generated
Each time the flow runs, a set of files are generated:
* **< DocumentId >.pdf** - The exported invoice PDF
* **< DocumentId >-headerfooter.csv** - All available data from the invoice's header/footer data set
* **< DocumentId >-lineitems.csv** - All extracted line items from the invoice (only available if line items are extracted)

## Selecting the destination folder
Edit the flow generated from this template and update the step **Set OneDrive Invoice Folder Path**.  Simply change the default value '/InvoiceData' to the folder path required.

**NOTE**: The folder path must exist in the OneDrive for Business account associated with the connection used for this flow. If the folder doesn't exist the flow will fail.