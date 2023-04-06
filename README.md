<!-- default badges list -->
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/T1157860)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->
# Grid for Blazor - Customize an Exported Document

This example demonstrates how to export the [DevExpress Blazor Grid](https://docs.devexpress.com/Blazor/403143/grid) data to an XLSX file and customize the export result.

![Export Grid Data](export-grid-data.gif)

## Overview

Set a column's [ExportEnabled](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGridDataColumn.ExportEnabled) property to `false` to prevent the Grid from exporting this column. To export grid data to an XLSX file, call the Grid's [ExportToXlsxAsync](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.ExportToXlsxAsync(System.String-DevExpress.Blazor.GridXlExportOptions)) method. The method accepts a [GridXlExportOptions](https://docs.devexpress.com/Blazor/DevExpress.Blazor.GridXlExportOptions) object as a parameter. Specify the parameter's properties to set up export settings.

The example code sets the following `GridXlExportOptions` properties:

**[CustomizeCell](https://docs.devexpress.com/Blazor/DevExpress.Blazor.GridExportOptions.CustomizeCell)**  
Allows you to customize a cell in the result document based on custom conditions.

**[CustomizeColumn](https://docs.devexpress.com/Blazor/DevExpress.Blazor.GridXlExportOptions.CustomizeColumn)**  
Allows you to customize a column in the result document.

**[CustomizeSheet](https://docs.devexpress.com/Blazor/DevExpress.Blazor.GridXlExportOptions.CustomizeSheet)**  
Allows you to customize sheet settings in the result document.

**[ExportDisplayText](https://docs.devexpress.com/Blazor/DevExpress.Blazor.GridExportOptions.ExportDisplayText)**  
Specifies whether the Grid exports cell values in the same format they are displayed in the grid.

**[ExportUnboundExpressionAsFunction](https://docs.devexpress.com/Blazor/DevExpress.Blazor.GridXlExportOptions.ExportUnboundExpressionAsFunction)**  
Specifies whether the grid exports an unbound column expression as a function or as a result value.

**[RowExporting](https://docs.devexpress.com/Blazor/DevExpress.Blazor.GridExportOptions.RowExporting)**  
Allows you to filter exported data.

**[SheetName](https://docs.devexpress.com/Blazor/DevExpress.Blazor.GridXlExportOptions.SheetName)**  
Specifies a name of the sheet in the result document.

## Files to Look At

* [Index.razor](./CS/Pages/Index.razor)

## Documentation

- [Export Data](https://docs.devexpress.com/Blazor/404338/grid/export)

## More Examples

- [Grid for Blazor - How to use DevExpress Reporting tools to implement export in a server application](https://github.com/DevExpress-Examples/blazor-server-dxgrid-export)
