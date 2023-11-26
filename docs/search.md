
Search provides the ability to search all K8s resources in the selected snapshot.  

The Search value input field can be used standalone or in conjunction with the Namespace(s) and/or 
Kind(s) inputs. All data provided in the 'Search value' field is case sensitive.

The Namespace(s) and Kind(s) searches are performed before searching with the 'Search value' input data.


### Search screen

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_search.png">
</p>

---

The following are the options when using the 'Search value' input field.

### Full search

Enter any text in the 'Search value' input field. Kubernetes resource definitions will be searched for the value regardless of where the value is located.

### Limited searches

There are three types of limited searches. Each requires a specific keyword to indicate the associated search is to be performed. 
Keywords must be entered in lowercase followed with a colon.

| Limited Search Type | Search Key |
|---|---|
| Search for a resource by name. | __name:__ |
| Search labels of the metadata section. | __labels:__ |
| Search annotations of the metadata section. | __annotations:__ |

Searching for a specific value in the labels or annotations can be achieved by using an additional parameter of "__::value::__". This key is then followed by a space and the value to locate.  Review the Example searches section of this document for examples of this parameter use.

---

### Search results

The search results are presented in a table format displaying three fields, namespace, kind, and name.     

Information displayed in the table can be clicked on to view the associated resource definition.  

Filtering the results table view is available by entering a value in the "__Search__" field at the top of the table.

---

### Example searches:

| Description | Search value |
|---|---|
| Search all resources for any occurrence of text 'a7be5c9d'. | a7be5c9d |
| Search for resources defined with the name 'bookinfo'. | name: bookinfo |
| Search resource metadata labels that match 'app.kubernetes.io'. | labels: app.kubernetes.io |
| Search resource metadata labels that match 'release' and have the value 'production'. | labels: release ::value:: production |
| Search all resource metadata labels for the value 'server'. | labels: * ::value:: server |
| Search resource metadata annotations that match 'productName'. | annotations: productName |
| Search resource metadata annotations that match 'network' and have the value 'wifi'. | annotations: network ::value:: wifi |
| Search all resource metadata annotations for the value 'click'. | annotations: * ::value:: operational-task |

---

### Search results table controls

The search results table has several controls.  There are identified in the following image.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/tab_search_table.png">
</p>

<hr style="border:1px solid #aaaaaa">

