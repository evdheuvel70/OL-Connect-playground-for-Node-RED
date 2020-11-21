OL-Connect-playground-for-Node-RED
==================================

### About

This project contains various flows to illustrate and test the integration of OL Connect in Node-RED.

 * Pull the playground files from https://github.com/evdheuvel70/OL-Connect-playground-for-Node-RED-files.git
 * In the Node-RED UI locate the Startup tab
 * Open the properties of the **Set Globals** step
    * Set the **workspace** global to the location of the checked out playground files
        * When running a Node-RED in a container this could be something like: /data/projects/OL-Connect-playground-for-Node-RED/workspace
        * Running on a local machine this may look like: C:\Users\{username}\.node-red/projects/OL-Connect-playground-for-Node-RED/workspace
    * Set the **email** global to your email address
 * Open the properties of the **File upload** step in the Startup tab
    * Click the **Edit** button of the Server option and enter the location and credentials of your OL Connect Server. This will update the Connect Server configuration for all flows.

Deploy the flow.