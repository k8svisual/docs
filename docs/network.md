

Network provides two views of the related network IPs and components. 

### Node & Pod IPs

The default view when opening the tab is the Node & PodIPs.  This view provides the node IP along with the Pod IP ranges
that are in use within the associated Pods.he associated resource definition will be displayed.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_network_nodes.png">
</p>

Click the node icon to view node related information.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_network_nodes_detail2.png">
</p>


Click the Pod IP ranges to view each Pod and associated IPs.  Once displayed select any of the rows to view the 
associated resource definition.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_network_nodes_detail.png">
</p>

<hr style="border:1px solid #aaaaaa">

### Services to Pods

The second view is the Services to Pods view.  This is a view of the Service to the associated Node and Pods.  Click any of the 
icons to view the related resource definition.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_network_services.png">
</p>

<hr style="border:1px solid #aaaaaa">


### Filter view

Each view can have a filter applied.  Press the __Filter__ button to open the filter capability.  Once open selected the type
of filter to be applied and then selected the associated data for the selected filter type.  Press the button labeled 
__Apply filter__ and the filter will be applied and the filter screen closed.

The drop down for the filter type will have different options based on the view.  Node view has two filter types: Node name and Node ip.  While the Services view has five filter types: Service name, Service ip, Pod name, Pod ip, and Namespace.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_network_services.png">
</p>


<hr style="border:1px solid #aaaaaa">


