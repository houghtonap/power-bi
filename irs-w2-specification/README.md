---
date:  "2022-04-21"
export_on_save:
  html: true
html:
  embed_local_images: true
  embed_svg:          true
  offline:            false
print_background: false
---

# IRS W-2 Specification Example

<!-- @import "[TOC]" {cmd="toc" depthFrom=2 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [Document Summary](#document-summary)
- [Build Environment](#build-environment)
  - [Data Sources Used](#data-sources-used)
  - [Documentation Tools](#documentation-tools)
  - [Platform OS and Tools](#platform-os-and-tools)
- [Power BI Parameters](#power-bi-parameters)
  - [ParamIRSW2SpecificationPDF](#paramirsw2specificationpdf)
  - [ParamIRSW2SpecificationXML](#paramirsw2specificationxml)
- [Power BI Queries](#power-bi-queries)
  - [QueryIRSW2AppendixF](#queryirsw2appendixf)
  - [QueryIRSW2AppendixG](#queryirsw2appendixg)
  - [QueryIRSW2RecordTypes](#queryirsw2recordtypes)

<!-- /code_chunk_output -->

## Document Summary

This example demonstrates two methods for extracting tables from a PDF document using Microsoft Excel Power Query or Microsoft Power BI Desktop.

1. The `PDF.Tables` method is demonstrated in the [QueryIRSW2AppendixF](#queryirsw2appendixf) and [QueryIRSW2AppendixG](#queryirsw2appendixg) queries.
1. The `XML.Document` method is demonstrated in the [QueryIRSW2RecordTypes](#queryirsw2recordtypes) query.

## Build Environment

### Data Sources Used

* [IRS EFW2 Publication 42-007](https://www.socialsecurity.gov/employer/efw/21efw2.pdf), tax year 2021 version 2

### Documentation Tools

* [Microsoft VS Code](https://code.visualstudio.com/), version 1.66.2
* [Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced) extension, version 0.6.2

### Platform OS and Tools

* [Adobe Acrobat DC](https://www.adobe.com/acrobat.html)
* [Microsoft Excel](https://www.microsoft.com/en-us/microsoft-365/excel), version 2203 build 16.0.15028.20218 64-bit
* [Microsoft Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/), version 2.103.661.0 64-bit (March 2022)
* [Microsoft Windows 10 Pro](https://www.microsoft.com/en-us/windowsforbusiness/windows-10-pro), version 10.0.19044 build 19044

## Power BI Parameters

### ParamIRSW2SpecificationPDF

The location of the IRS W-2 specification PDF document.

### ParamIRSW2SpecificationXML

The location of the IRS W-2 specification PDF-XML document.

## Power BI Queries

### QueryIRSW2AppendixF

A query that imports a PDF document and creates a table from Appendix F found in the IRS W-2 specification.

### QueryIRSW2AppendixG

A query that imports a PDF document and creates a table from Appendix G found in the IRS W-2 specification.

### QueryIRSW2RecordTypes

A query that imports a PDF-XML document and creates a table from the W-2 record types and their field specifications that are found in sections 4.5 through 4.13 of the IRS W-2 specification.
