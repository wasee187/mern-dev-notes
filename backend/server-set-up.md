##Code for server run specific port  

import express from "express";  

const app = express();  
app.listen(5001, ()=>{  
    console.log("Server is running on PORT: 5001")  
});   

##Change in package.json file  
"scripts": {  
    "dev": "node server.js"  
  },  
  "type": "module",  
  
  
nodemon:: for updating any changes in the code and not to restart the server again we need to use this nodemon npm package.  
For deployment we can keep the old node server.js command.  
:::   
 "scripts": {  
    "dev": "nodemon server.js",  
    "start": "node server.js"  
  },  
   
  
// what is Endpoint?
::: An endpoint is a combination of a URL + HTTP method that let the client interact with a specific resource.    