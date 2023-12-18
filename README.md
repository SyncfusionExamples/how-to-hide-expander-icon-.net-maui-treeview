# how-to-hide-expander-icon-.net-maui-treeview
This example demonstrates about how to hide the expander icon in TreeViewNode in .NET MAUI TreeView (SfTreeView).

In [.NET MAUI TreeView](https://www.syncfusion.com/maui-controls/maui-treeview), the ability to expand and collapse nodes. However, there may be scenarios where you want to remove expander icon expand/collapse functionality. This can be achieved by hiding the expander of the TreeView nodes. Below is the article on how to hide the expander in .NET MAUI TreeView.

**XAML**
 
```xml
<syncfusion:SfTreeView x:Name="treeView"
                           ExpandActionTarget="Node"
                           ExpanderWidth="0"
                           ItemsSource="{Binding Folders}"
                           ChildPropertyName="Files">
        
        <syncfusion:SfTreeView.ItemTemplate>
            <DataTemplate>
                <Grid x:Name="grid"
                      RowSpacing="0"
                      ColumnDefinitions="40, *"
                      BackgroundColor="Transparent">
                    <Grid Padding="5,5,5,5">
                        <Image Source="{Binding ImageIcon}"
                               VerticalOptions="Center"
                               HorizontalOptions="Center"
                               HeightRequest="35"
                               WidthRequest="35" />
                    </Grid>
                    <Grid Grid.Column="1"
                          RowSpacing="1"
                          Padding="1,0,0,0"
                          VerticalOptions="Center">
                        <Label LineBreakMode="NoWrap"
                               Text="{Binding ItemName}"
                               VerticalTextAlignment="Center" />
                    </Grid>
                </Grid>
            </DataTemplate>
        </syncfusion:SfTreeView.ItemTemplate>
    </syncfusion:SfTreeView>

 ```

[View sample in GitHub](https://github.com/SyncfusionExamples/how-to-hide-expander-icon-.net-maui-treeview)

**Conclusion**
I hope you enjoyed learning about How to hide expander in .NET MAUI TreeView.
You can refer to our [.NET MAUI TreeView](https://www.syncfusion.com/maui-controls/maui-treeview) feature tour page to know about its other groundbreaking feature representations and documentation, and how to quickly get started for configuration specifications. You can also explore our .NET MAUI TreeView example to understand how to create and present data. For current customers, you can check out our components from the License and Downloads page. If you are new to Syncfusion, you can try our 30-day free trial to check out our other controls.

If you have any queries or require clarifications, please let us know in the comments section below. You can also contact us through our support forums, Direct-Trac, or feedback portal. We are always happy to assist you!
