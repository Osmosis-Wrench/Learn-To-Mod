# Automating MCM Menu's and an introduction to Scripting

## Intro

Are you the sort of person who starts a new character regularly? Or perhaps you're an Modlist Author who wants to make things easier for their users, or perhaps you're curious about learning scripting and want a way to get your feet wet? Well, if you're any of the above you've come to the right place.  
In this guide I'll be walking you through how to:  

- Decompile scripts.
- Modify existing scripts.
- Basic MCM automation.
- How to move beyond this to more complex scripting.  

## What you will need

- Any text editor. I personally recommend [Visual Studio Code](https://code.visualstudio.com/download), however [Notepad++](https://notepad-plus-plus.org/downloads/), [Sublime](https://www.sublimetext.com/) or even the venerable Notepad are all perfectly acceptable.
- The [Creation Kit](https://www.creationkit.com/index.php?title=Category:Getting_Started#Installing_the_Creation_Kit)
- [Champollion](https://www.nexusmods.com/skyrim/mods/35307/?tab=files)
- [My Example Mod](FIXME)

## Before we begin

### A basis for understanding

So, for the groundwork of this I'll cover the absolute basics of Skyrim scripting. All scripts are written in a scripting language called **Papyrus**, scripts that are written in this language are run inside something called the **Papyrus Virtual Machine**. You can think of this as a second, separate game engine that is able to send instructions and receive data and updates from the "actual" Skyrim game engine.  

For the Papyrus VM to be able to understand the instructions in the script, it must first be **Compiled**.  This compilation is done with the appropriately named **Papyrus Compiler** which is used to convert the human readable papyrus script into something that a computer can read more efficiently.  

An uncompiled "Source" script will have the **.PSC** file extension, while a compiled script will have the **.PEX** file extension. To be able to make any changes to a script, you'll need to be able to access the PSC source file. And that leads onto our next subject.

### From PEX to PSC, and back again

Unfortunately, some mod authors do not include their source files with their mods. Instead choosing to only include the compiled PEX files. This is where script **Decompilation** comes in. By making use of a tool called **Champollion** we are able to convert a compiled PEX script back to a editable PSC source file.  

How this is done will be covered in more detail in the FIXME section of this guide.

### Source Scripts and Scripts Source

For reasons beyond the ken of us mere mortals, Bethesda decided to change the default location of the source files for scripts in SE compared to LE. Because of this decision some mods will have their script source files in ``/Source/Scripts``(SE default) while other mods will have their scripts in ``/Scripts/Source``(LE default). Any time you're looking through a mod for it's source files make sure you check both folders before you try to decompile any scripts.

## Time to get started

### Installing the Creation Kit

Download and install the creation kit, and then make sure you unzip the file called "Scripts.rar" to the skyrim root folder. 

### Downloading my example mod.