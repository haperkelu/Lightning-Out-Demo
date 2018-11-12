# Steps to run
### Step 1
Create account list as per https://trailhead.salesforce.com/en/content/learn/projects/slds-lightning-components-workshop/slds-lc-4

Create below Lightning application in your Salesforce instance and name it as **LightningOutDemo**

`<aura:application access="Global" extends="ltng:outApp">`

`<c:AccountList />`

`</aura:application>`

### Step 2
Create Connected App in your Salesforce instance with callback URL - `https://localhost:8081/oauthcallback.html`
Copy Consumer Key created in connected app and update clientId variable defined in [OAuth.js](/Lightning-Out-Demo/blob/master/client/js/OAuth.js) file.

### Step 3 
Save `https://localhost:8081` in **CORS** setting of Salesforce.

### Step 4
Run `npm install` command in the directory where this code is downloaded. It will download all the required node modules.
Then run `npm start`, it will start the server

### Step 5
Navigate to `https://localhost:8081/` in your browser and you would see **Lightning Out** in Action
