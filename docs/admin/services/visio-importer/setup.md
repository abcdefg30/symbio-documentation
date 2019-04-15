# Setting the Visio importer up

## URI und Token

First, navigate to the 'Automation Tasks' overview. (Admin settings panel > Services > Automation Tasks)  
Select the 'data, Rest API endpoint' task and create a new 'Authentication token' for it.  
![automation](media/createAutomation.png)

Select the token and copy the ID displayed on the right.  
Then scroll down to 'Application roles'. Expand it and check the 'Administrator' box.  
If you want to change the token's lifespan (default is 3 months), you can do so in the collapsed 'Validity' field further down below the ID field.

Besides the token an URL is needed for the import. The URL is the base URL to your Symbio instance appended with "_api". (In our case "https://pz-1904.symbioweb.com/Test/visio-importer/_api".)  
The Token and the URL are added to the Tool using the Website.  
This returns a GUID which is needed by the user to complete an import.
