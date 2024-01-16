
Statistics for the cluster are shown in two primary views, a tree map graph and a tabular view. For each view 
it may be toggled to swithch between totals by k8s resource kind and k8s namespace.

<hr style="border:1px solid #aaaaaa">

###  Graph view

The treemap graph displays data by color rectangles. The size and color of the rectangle provides a graphic 
view of the amount associated with that rectangle.  

Since a treemap graph can become very dense and messy the ability to show or hide the labels associated with
each rectangle is provided.  Also data can be filtered by minimum amount, maximum amount, and either kind or 
namespace.

Mouse over any rectangle to view summary information.  Click any rectangle to view the associated data in the
Search tab.  If the Namespace view is toggled the Search will also filter for the associated namespace.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_stats_treeMap.png">
</p>

<hr style="border:1px solid #aaaaaa">

###  Report view

The report view is a tabular view of the data with collapsible sections.  Click the small black triangles to
toggle the collapsed sections.

Click any of the lines of the report to view the associated data in the Search tab.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_stats_reportView.png">
</p>


<hr style="border:1px solid #aaaaaa">