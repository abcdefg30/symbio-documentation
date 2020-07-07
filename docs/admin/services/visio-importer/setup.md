# Setting the Visio importer up

## URI und Token

First, navigate to the 'Automation Tasks' overview. (Admin settings panel > Services > Automation Tasks)  
Select the 'data, Rest API endpoint' task and create a new 'Authentication token' for it.

![automation](media/createAutomation.png)

Select the token and copy the ID displayed on the right.  
Then scroll down to 'Application roles'. Expand it and check the 'Architect' box.  
If you want to change the token's lifespan (default is 3 months), you can do so in the collapsed 'Validity' field further down below the ID field.

Besides the token an URL is needed for the import. The URL is the base URL to your Symbio instance appended with '_api'. (In our case "https://pz-1904.symbioweb.com/Test/visio-importer/_api".)  
You can also retrieve the URL from token's 'Information' section, just remove everything after '_api' from the URL.

The last thing we need is the GUID for the category in Symbio we want the import to end up in.
Go to your Symbio installation and create a new category or select an existing one and press `ctrl + alt + d`.

![categoryGUID](media/categoryGUID.png)

Select the 'ContextKey' GUID from there and copy it.

The Token, the URL and category GUID are added to the Tool using the [Website](https://visio.symbioweb.com/pzdebug).  
This returns a GUID which is needed by the user to complete an import.

![guidGeneration](media/guidGeneration.png)
