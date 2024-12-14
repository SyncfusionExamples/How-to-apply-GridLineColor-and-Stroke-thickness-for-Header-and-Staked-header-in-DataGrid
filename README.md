# How to apply GridLineColor and Stroke thickness for Header and StakedHeader in DataGrid?
In this article, we will show you how to apply GridLineColor and Stroke thickness for Header and StakedHeader in [.Net Maui DataGrid](https://www.syncfusion.com/maui-controls/maui-datagrid).

## xaml
### Default Style
The code below demonstrates how to customize the Header stroke thickness and Header line Color with default styling in DataGrid.
```
<ContentPage.BindingContext>
    <local:EmployeeViewModel x:Name="viewModel" />
</ContentPage.BindingContext>

<syncfusion:SfDataGrid x:Name="dataGrid" 
                       ColumnWidthMode="Auto"
                       GridLinesVisibility="Both"
                       HeaderGridLinesVisibility="Both"
                       AutoGenerateColumnsMode="None"
                       ItemsSource="{Binding Employees}">

    <syncfusion:SfDataGrid.DefaultStyle>
        <syncfusion:DataGridStyle HeaderGridLineColor="Red"
                                  HeaderGridLineStrokeThickness="5" />
    </syncfusion:SfDataGrid.DefaultStyle>

    <syncfusion:SfDataGrid.Columns>
        <syncfusion:DataGridNumericColumn MappingName="EmployeeID"
                                          Format="#"
                                          HeaderText="Employee ID" />
        <syncfusion:DataGridTextColumn MappingName="Name"
                                       HeaderText="Employee Name" />
        <syncfusion:DataGridTextColumn MappingName="Title"
                                       HeaderText="Designation" />
        <syncfusion:DataGridDateColumn MappingName="HireDate"
                                       HeaderText="Hire Date" />

    </syncfusion:SfDataGrid.Columns>

    <syncfusion:SfDataGrid.StackedHeaderRows>
        <syncfusion:DataGridStackedHeaderRow>
            <syncfusion:DataGridStackedHeaderRow.Columns>
                <syncfusion:DataGridStackedColumn ColumnMappingNames="EmployeeID,Name,Title,HireDate"
                                                  Text="Employee Details Section"
                                                  MappingName="SalesDetails" />
            </syncfusion:DataGridStackedHeaderRow.Columns>
        </syncfusion:DataGridStackedHeaderRow>
        <syncfusion:DataGridStackedHeaderRow>
            <syncfusion:DataGridStackedHeaderRow.Columns>
                <syncfusion:DataGridStackedColumn ColumnMappingNames="EmployeeID,Name"
                                                  Text="Employee Details"
                                                  MappingName="OrderDetails" />
                <syncfusion:DataGridStackedColumn ColumnMappingNames="Title,HireDate"
                                                  Text="Work Details"
                                                  MappingName="CustomerDetails" />
            </syncfusion:DataGridStackedHeaderRow.Columns>
        </syncfusion:DataGridStackedHeaderRow>
    </syncfusion:SfDataGrid.StackedHeaderRows>
</syncfusion:SfDataGrid>
``` 

 ![headerGirLineColor.png](https://support.syncfusion.com/kb/agent/attachment/inline?token=eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjMzOTgyIiwib3JnaWQiOiIzIiwiaXNzIjoic3VwcG9ydC5zeW5jZnVzaW9uLmNvbSJ9.gV0YUw1895OOXDeq0Bc2cYLCmNiw1Bvf-JjyTwlbOtA)

[View sample in GitHub](https://github.com/SyncfusionExamples/How-to-apply-GridLineColor-and-Stroke-thickness-for-Header-and-Staked-header-in-DataGrid)

Take a moment to explore this [documentation](https://help.syncfusion.com/maui/datagrid/overview), where you can find more information about Syncfusion .NET MAUI DataGrid (SfDataGrid) with code examples. Please refer to this [link](https://www.syncfusion.com/maui-controls/maui-datagrid) to learn about the essential features of Syncfusion .NET MAUI DataGrid (SfDataGrid).
 
##### Conclusion
 
I hope you enjoyed learning about how to customize the Header stroke thickness and Header line Color in .NET MAUI DataGrid (SfDataGrid).
 
You can refer to our [.NET MAUI DataGrid’s feature tour](https://www.syncfusion.com/maui-controls/maui-datagrid) page to learn about its other groundbreaking feature representations. You can also explore our [.NET MAUI DataGrid Documentation](https://help.syncfusion.com/maui/datagrid/getting-started) to understand how to present and manipulate data. 
For current customers, you can check out our .NET MAUI components on the [License and Downloads](https://www.syncfusion.com/sales/teamlicense) page. If you are new to Syncfusion, you can try our 30-day [free trial](https://www.syncfusion.com/downloads/maui) to explore our .NET MAUI DataGrid and other .NET MAUI components.
 
If you have any queries or require clarifications, please let us know in the comments below. You can also contact us through our [support forums](https://www.syncfusion.com/forums), [Direct-Trac](https://support.syncfusion.com/create) or [feedback portal](https://www.syncfusion.com/feedback/maui?control=sfdatagrid), or the feedback portal. We are always happy to assist you!