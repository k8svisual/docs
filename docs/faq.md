
The following questions and answers hopefully provide aid in understanding and working with VpK software.  

<hr style="border:1px solid grey">

!!! Question 

    Is the kubectl CLI required or can another command CLI be used to connect to the Kubernetes cluste?

??? Answer

    The default CLI is kubectl is not required.  For example when using Red Hat(r) OpenShift(r) the "__oc__" command CLI is used.
    If the default command CLI is not used the optional command CLI must be connected to the target K8s cluster before VpK can 
    query and retrieve resource data.  The optional command CLI must also be provide in the UI when quering to the cluster.

<hr style="border:1px solid grey">

!!! Question 

    Can I modify the displayed resource information?

??? Answer

    VpK is read-only and does not modify the K8s cluster.   

<hr style="border:1px solid grey">

