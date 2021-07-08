# WatsonAssistantWEB-Hooks-with-NodeRED

Purpose: To see the JSON passed to or got from Watson Assistant in the Node-RED Debug Window

Setup-Steps:

- If you don't have a running and public accesable Node-RED Instance.
  - Go to IBM Cloud and find the Node-RED App in the Cloud Catalog or open this URL
    https://cloud.ibm.com/developer/appservice/create-app?starterKit=59c9d5bd-4d31-3611-897a-f94eea80dc9f&defaultLanguage=undefined
  - Go to the Create Tab and fill in your values.
  - Deploy the code to the cloud with the Tool-Chain (everything will be done automatically.
    
  
  
- Login to the NodeRED Editor and import the File "DebugWebHooks-NodeRED-Flow.json" (Menu in the upper right corner)

- Deploy the Flow

- Go to Watson Assistant and set the WEB-Hook's URL (eg. https://<nodeRedInstanceName>.mybluemix.net/<NodeRED defined function> ), that you want to debug.

where <NodeRED defined function> can be any of the following values:

          preWebHookDebug.json
          postWebHookDebug.json
          logWebHookDebug.json

          skillWebHookDebug.json
  
Hint: The first three functions are only called if the V2 API is used (this is not the case, if you use e.g. the "Try it out" Window in Watson Assistant).
