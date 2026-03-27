MongoDB: is the database, place where you store your data.  
Express: A web framework is a ready-to-use toolbox for building the web apps faster and more easily. It will handle routing, error handling etc.  
NodeJS: JavaScript Runtime that allow to run JS on server  
ReacJS: front end library.    
##API:: Application Programming Interface. It will connect backend with frontend.   
REST API:: It uses HTTP methods. Like GET, POST, PUT, DELETE   
  
:: File formation  
It is good practise to keep all the application files like folders of routes, controllers and server.js file in source/src file. By this we need to adjust the scripts command in pacage.json file  
"scripts": {   
    "dev": "nodemon src/server.js",  
    "start": "node src/server.js"  
  },  