# Semantik.Toolkit.PowerAutomate
**Available for:** Semantik Invoice

## Overview
This repository contains helper tools that can be used for Semantik-related projects to export the necessary data from Semantik Invoice. 

## Prerequisites
You will need access to Semantik Invoice and Microsoft PowerAutomate to complete the integration.

## Pipe delimited file Export
This exports Semantik data into a pipe delimited file. PowerAutomate expects the following columns to be exported from Semantik in the order listed below:

- Item #
- Description
- Shipped
- Unit Price
- Ext Price


## Pipe delimited file export with column filter
This exports Semantik data into a pipe delimited file for columns with table headers that match (case-sensitive) the expected column names. Other columns are not placed in the file.

The expected column names are:

- Item #
- Description
- Shipped
- Unit Price
- Ext Price
**Note:** A column name with a period cannot be set as expected as it is an invalid character in Microsoft Flow expression language.

## License
Ephesoft Labs is licensed under the [Ephesoft Source Code License]. 
