
This is a high-level 3D view of the cluster.  The view is interactive and can be rotated, tilted, zoomed in or out, and filtered.  

The left-hand side of the screen has a slide out that enables filtering the 3D view, control sound, and save the current filter settings as the default.

The right-hand side of the screen has a slide out that provides __Properties__ for any item in the 3D view that is clicked/selected.  Once an item is selected the item will have a red circle plane shown to identify the selected item.


### Cluster tab

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_cluster.png">
</p>

---

### Properties drill down

As k8s resource items are selected in the 3D view the properties slide-out will change based on the selected k8s resource.
Several of the properties provide the ability to drill down and view detail in the associated tab with the context for the 
tab set to match the property.  Examples of the drill downs are shown below.

#### Pod drill down

This property supports viewing the associated Schecmatic and OwnerRef tabs

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_cluster_drill_down1.png">
</p>

#### StorageClass drill down

This property supports viewing the associated Storage tab

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_cluster_drill_down3.png">
</p>

#### API category drill down

This property supports viewing the associated Search tab

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_cluster_drill_down4.png">
</p>



### Cluster Timelapse

In the upper portion of this tab is a button labeled __Timelapse__.  When clicked this button will clear the 3D view and open the timelapse controls. This feature will display changes to the cluster in time sequence as they occur via intervals. The duration of each interval is dynamic.  The shortes duration is one second and the longest duration is based on the amount of time between the next change to the cluster.

The timelapse will automatically display all collected changes for the cluster or can be manually stepped forward or backward 
for each interval.  

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_cluster_timelapse.png">
</p>

The controls are as follows. 

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_cluster_timelapse_controls.png">
</p>

Once the auto play button is pressed the triangle button with switch to a 'pause' button.  
Press that at any time to stop the auto play.  Once paused the detail for the currently displayed time interval can be 
viewed by pressing the blue circle with an 'i'.  This will display all changes in the interval in a tabular form.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_cluster_timelapse_detail.png">
</p>


### Cluster Legend

The blue circle button with and 'i' provides information related to the displayed icons and planes.  


<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_cluster_legend.png">
</p>

<hr style="border:1px solid #aaaaaa">

