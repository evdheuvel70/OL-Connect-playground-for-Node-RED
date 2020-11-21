OL-Connect-playground-for-Node-RED
==================================

## About

This Node-RED project contains various flows to illustrate and test the integration of OL Connect in Node-RED.

The easiest way to grab a copy is to enable the [Node-RED's project feature|https://nodered.org/docs/user-guide/projects/] and clone the repository. Enter the following web URL in the Git repository URL field: https://github.com/evdheuvel70/OL-Connect-playground-for-Node-RED-files.git


## Setting up the flow
There isn't much needed to get the project running. One needs to define the path to the project and optionally change the email address to match yours. OL Connect resources (like sample templates etc) are automatically deployed.

To change the base parameters of the project:
 * In the Node-RED UI locate the Startup tab of the project
 * Open the properties of the **Set Globals** step
    * Set the **project** global to the location of the checked out playground files
        * When running a Node-RED in a container this could be something like: /data/projects/OL-Connect-playground-for-Node-RED
        * Running on a local machine this may look like: C:\Users\{username}\.node-red/projects/OL-Connect-playground-for-Node-RED
    * Set the **email** global to your email address
 * Open the properties of the **File upload** step
    * Click the **Edit** button of the Server option and enter the location and credentials of your OL Connect Server. This will update the Connect Server configuration for all flows.
    * The same can be done via the Configuration Nodes option located in the Node-RED menu (hamburger icon in the upper right corner of the editor).

Deploy the flow.