##get Route:  
  app.get("/api/notes", (req,res)=>{
  console.log("You have 5 notes");
  });  
##post route:  
app.post("/api/notes", (req,res)=>{  
    res.status(201).json({ message: "Note created successfully"})  
});  
##put route:  
app.put("/api/notes/:id", (req,res)=>{  
    res.status(200).json({ message: "Note updated successfully"})  
});  
##delete route:  
app.delete("/api/notes/:id", (req,res)=>{  
    res.status(201).json({ message: "Note deleted successfully"})  
});  
