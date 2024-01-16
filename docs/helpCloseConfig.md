

In the upper right-hand corner of the UI there are three icons that provide:

- Help - context based help
- Close - shutdown and close VpK
- Configure - configure options for VpK


<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/help_close_config.png" width="140">
</p>


<hr style="border:1px solid #aaaaaa">

### Help

A build-in help system is available when using VpK.  Select this option to open the help system. When selected the help system will present information related to the currently selected tab.  If the VpK icon in the upper left-hand corner of the home screen is pressed the help Table of Contents is opened.  

Previous, Table of Contents, and Next options are available on all help screens.



<hr style="border:1px solid #aaaaaa">

### Shutdown

VpK can be stopped by selecting the "X" button in the upper right portion of the home screen.  Press the button and confirm the shutdown by pressing the "__Shutdown__" button.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/ui_shutdown_confirm.png">
</p>


!!! Info

    If VpK is running in a Docker container the container will be stopped at this time.


Once the shutdown and close process has completed the following screen is displayed.


<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/ui_shutdown_complete.png">
</p>


<hr style="border:1px solid #aaaaaa">

### Config

From the home screen click the gear in the upper right portion of the screen to open the VpK configuration.   

Multiple items can be configured along with viewing Usage information.  Items that are configurable are:

- managedFields - this controls the displaying of __managedFields__ when a K8s resource information is displayed.  Enabling this 
option will show the managedFields.

- status - controls the displaying of the __status__ section when a K8s resource information is displayed.  Enabling this 
option will show the status information.

- Redact K8s Secret data - controls if the data section of a K8s Secret resource should be redacted. If enabled all items in the 
data section will be replaced with __Content has been REDACTED__.  

!!! Warning

    If this option is modified a complete reload of the selected Snapshot must be performed. The redacting or showing of the data 
    is performed when the Snapshot is processed.

- Snapshot reload - controls if a full reload and re-parse of a Snapshot is performed.  If a selected Snapshot has been processed
and is selected to be processed a second time without loading another Snapshot the default is to perform a soft load of the Snapshot 
data.  Enabling this option will force a complete reload of the selected Snapshot.   

- View usage information - technical information regarding the server and browser are displayed.  See the Usage screen show below.

#### Configuration screen

Several configuration options are available in this portion of VpK.  The configuration options aid in the ability to
control what is displayed when the k8s resource is viewed, the background for the k8s resource view and the 3D cluster view, 
redacting information for k8s secret resources, how data is refreshed, saving the changes, and viewing of VpK resources for the server and browser components.  The following screen is what is shown when the Config option is selected.  The Config option can only be closed by pressing the __Close__ button.


<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/config.png">
</p>

If changes have been made in the configuration and the close button is pressed prior to saving the chaged data the user
is prompted to confirm the desire to not save the changes.  The following message is displayed:

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/config_action.png">
</p>

If the 'Save configuration' button is pressed the following will be shown once the information is saved.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/config_confirm.png">
</p>


#### Resource viewing themes

Two themes are available for viewing the k8s resource source and status information.  These are the light and dark.  Examples
for each follow:

#### Light theme

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/resource_light.png">
</p>

#### Dark theme

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/resource_dark.png">
</p>

#### VpK component usage information

Press the blue circle with an 'i" located in the bottom portion of screen to view the VpK usage information.

<p align="center">
  <img style="float: center;" src="https://raw.githubusercontent.com/k8svisual/vpk-docs/master/docs/images/about.png">
</p>

<hr style="border:1px solid #aaaaaa">

### Tabs

Information for each of the tabs is included in the "__UI TABS__" category of this documentation.  Each tab is listed along with descriptions and instructions on usage.


<hr style="border:1px solid #aaaaaa">