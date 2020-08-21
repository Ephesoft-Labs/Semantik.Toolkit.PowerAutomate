# Semantik.Toolkit.PowerAutomate
This repisotory contains Semantik helper tools that can be used for Semantik related projects

## Table of Contents
- [Pipe delimited file Export](#Pipe-delimited-file-Export)
- [Pipe delimited file export with column filter](#Pipe-delimited-file-export-with-column-filter)


## Pipe delimited file Export
Exports Semantik data into a pipe delimited file.  The PowerAutomate application expects the following columns to be exported from Semantik in the order listed below:

- Item #
- Description
- Shipped
- Unit Price
- Ext Price


## Pipe delimited file export with column filter
Exports Semantik data into a pipe delimited file but only for columns whose table header exactly matches (case-sensitive) the expected column names. Other columns are disregarded and not placed in the file.
Currently, the expected column names are:

- Item #
- Description
- Shipped
- Unit Price
- Ext Price
**Note** that a column name with a period cannot be set as expected because it is an illegal character in flow expression language.
