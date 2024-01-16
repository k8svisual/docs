VpK (Visually presented Kubernetes) was created to assist in understanding and learning about Kubernetes cluster.   

VpK is comprised of a server component along with a browser application component.  The server component is a node.js application that can communicate with a running instance of Kubernetes using the __kubectl__ CLI.  The use of other CLI tools other than kubectl is supported.  

VpK requires what is called a 'snapshot'.  This is a collection of files that contain information obtained from a Kubernetes cluster. For VpK to obtain the K8s resource information an existing kubectl CLI connection must be established with the target Kubernetes cluster from where data will be retrieved. 

The kubectl CLI connection must be established by the user outside of VpK. If no kubectl CLI connection has been established then no K8s resource data will be obtained. A series of 'kubectl get' commands are issued to obtain the cluster data.

The output from the kubectl CLI is processed to create multiple files that are collectively called a __snapshot__.  This snapshot is saved in a directory and can be reused without connecting to the K8s cluster for future sessions.  

Once a snapshot has been created VpK no longer requires any communication with the Kubernetes cluster. 

!!! Note

    VpK is designed as read-only and will __not__ modify a Kubernetes cluster and is __not__ a real-time monitoring tool.  


### VpK overview diagram

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/overview_local.png">

</p>

<hr style="border:1px solid #aaaaaa">

### Application features

- VpK will access a Kubernetes cluster via an established kubectl CLI and save query results, called a __snapshot__, in a local directory. 

- The locally stored __snapshot__ can be reused. This supports fully disconnected use of VpK to review the K8s resource data without connecting to the K8s cluster.
 
- A interactive 3D view of the K8s cluster.  This view supports zoom, rotate, tilt, and filtering of resources.

- Timelapse view of the 3D cluster to show the sequence of resource creation and removal.  The timelapse can be stopped
and viewed second-by-second while interacting with the 3D view.

- Schematic views of workloads deployed in the cluster.  Interact with the schematic and view detail resource definitions.

- View storage defined for the cluster by StorageClass, PV, PVC, CSI, and node related storage.  

- View network IP addresses and address ranges for services, pods, and nodes. 

- View defined security roles, bindings, and subjects for the cluster or namespaces.

- View Owner References chains for K8s resources defined in the cluster.

- View event messsages statistics and timeline.

- View container image repositories and associated images.

- Search K8s resources with the ability to filter by namespaces, kinds, labels, resource names, and annotations.

  

<hr style="border:1px solid #aaaaaa">

