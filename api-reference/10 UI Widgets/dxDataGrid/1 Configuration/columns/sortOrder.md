---
default: undefined
acceptValues: undefined | 'asc' | 'desc'
type: string
---
---
##### shortDescription
Specifies the initial sort order of column values.

---
By default, records in a grid are ordered according to the data source. You can, however, set a different initial sort order for the records in one or several columns. To sort grid records by one column, specify the required order using the **sortOrder** option. To sort grid records by several columns, use the [sortIndex](/api-reference/10%20UI%20Widgets/dxDataGrid/1%20Configuration/columns/sortIndex.md '/Documentation/ApiReference/UI_Widgets/dxDataGrid/Configuration/columns/#sortIndex') option in addition to the **sortOrder** option.

[note] If you specify the **sortOrder** option for several columns omitting the **sortIndex** option, a sort index will be assigned to each sort column according to its position in the **columns** array.

<a href="http://js.devexpress.com/Demos/WidgetsGallery/#demo/datagridgridfilteringandsortingsorting/" class="button orange small fix-width-155" style="margin-right: 20px;" target="_blank">View Demo</a>