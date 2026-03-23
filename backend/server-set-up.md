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