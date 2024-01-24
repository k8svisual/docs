
OwnerRef Links provides a view of the owner reference chain for resources in the selected namespace.  

From the namespace drop-down select a single namespace.  Once a namespace has been selected press the "__View selected namespace__" button. 

If there is no selected namespace a warning message is displayed. 

The results are a graph of the relationships with the Owner at the highest level in the graph.  Click on any of the displayed color rectangles and the associated resource definition will be displayed.

Views can be a simple two-level ownership to a complex five or six level ownership across multiple resources.

#### OwnerRef - Simple view

This is a simple view with only three two-level resources.
<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_ownerref.png">
</p>

#### OwnerRef - Complex view

This is a complex view with multiple level resources. Also shown is a single resource owning multiple resources.
<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_ownerref2.png">
</p>

### Filter 

After selecting a Namespace and displaying the entire result the Filter screen will be populated with the resource Kinds found when the initial view is shown.  

Open the filter screen and select the desired kind(s) from the drop down.  Once selected press the button labeled __Populate resource names information__.  The detail for the selected kind(s) will be shown in a table in the filter screen.

Select one or more rows to be shown and then press the button labeled __Apply filter__.  

In the following filter screen the kind __ConfigMap__ was selected and populated the selection table.  From the selection table four items were selected. 

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_ownerref_filter.png">
</p>

#### Example results after applying filter

Selected items to be viewed when the filter was applied.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_ownerref_filter_results.png">
</p>

---
### Clear the filters

Return to the filter screen and press the button labeled __Clear all filters__ to reset and clear all filters.

<hr style="border:1px solid #aaaaaa">

