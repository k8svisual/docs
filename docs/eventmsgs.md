
This tab provides statistics regarding event messages and two views.  Once view is a timeline and the other view is 
tabular view. 

There are three buttons, a drop down for Namespace, along with a input field for the first minute to display.  Use the
buttons to select the desired view and the drop down and input field to filter what is shown.

### Statistics view

This view is a bar chart graph with the volume of messages shown by each minute.  The left axis is the count of messages. 
If more than 800 message occured in the associated minute the bar will be shown in the color red.  Otherwise the bar will
be shown in green.  The bottom axis is the minute when the messages occur. Mouse over the bar to view the total message and
the associated minute.

Mouse over the small green rectangles to view summary information.  Click the title or the small green rectangle to view 
the resource detail. 

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_event_msgs_graph.png">
</p>


### Timeline view

This view is scrollable view with collapsed sections.  Toggle the small black triangle to open the collapsed view.a bar chart graph with the volume of messages shown by each minute.  There are also buttons at the top of the data to page the data.  The current page and the total pages are shown.  

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_event_msgs_timeline.png">
</p>


### Table view

A table view of all Event messages that were available in the K8s cluster when the Snapshot was created.  The first 
column is shown with either green, yellow, or red background.  These colors represent Normal, Warning, or Failed messges
respectively.

Use the table __Search__ field to filter the messages that are shown.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_event_msgs_table.png">
</p>

Clicking on a message will either display the resource detail or provide the following message prompt.  This prompt is 
shown when a workload schematic can be shown for the respective message.

If the __'View schematic for involved resource'__ button is pressed view will switch to the Workload Schematic tab and disply the associated schematic.  On the Workload Schematic tab above the schematic will be a 'Return' button.  Press this to return to the 
Events Msgs tab. 

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_event_msgs_action.png">
</p>

<hr style="border:1px solid #aaaaaa">