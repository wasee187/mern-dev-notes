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

##optimization  
so, for efficiency we need to create a new routes and controller floder where we will store routes and controller section.  
:: in the controller file we will this controller functions and export them  
export function getAllNotes(req,res){  
    res.status(200).send("You have 10 notes")  
};   
export function createNote(req,res){  
    res.status(201).json({ message: "Note created successfully"})  
};     
export function updatreNote(req,res){  
    res.status(201).json({ message: "Note updated successfully"})  
};   
export function deleteNote(req,res){  
    res.status(201).json({ message: "Note delete successfully"})  
};   
  
  
::In the routes file we will add this codes  
import express from "express";  
import { getAllNotes, createNote, updatreNote,deleteNote } from "../controllers/notesControllers.js";  

const router = express.Router();  
router.get("/", getAllNotes);   
router.post("/", createNote);  
router.put("/:id", updatreNote);  
router.delete("/:id",deleteNote);  
  
export default router;  