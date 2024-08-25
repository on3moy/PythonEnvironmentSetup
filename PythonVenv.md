![It Begins](https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExb3d3N2ptNTg2ZjJ4djlxcHQwYnd2bHdkcGJmajBmYnI3a3J2a3ZtaSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/zk0zTXQY5ukCs/giphy.gif)  

# Prerequisites
1. You are working on Windows OS (Not and ancient OS version)
2. [Python](https://python.org/) is installed
3. PATHS are correctly set up (Not needed if you installed checking set up PATHS on Python installation)

# PATHS
You can reach this by going to System > About > Advanced Settings > Environment Variables.  
**Metaphor** - Creating a PATH for exe is like creating a shortcut to a file to access from your desktop. (That way you don't have to dig through folders to open every time)  

## User Variables
If you add a path in this section, the user logged in can only access the path or shortcut.  

## System Variables
If you add a path in this section, every user who has access can use the path or shortcut.

## Adding Python to PATH
For now, stick with user for ease assuming you are the only person using your device. 👌  

Once you install python, the program gets stored on your computer either for a user or for all users depending what option you picked on installation.
- If you already checked add to PATH during the installation then you don't need add Python.exe to PATH to reference.

When using Command Prompt (CMD) or PowerShell (PS), you can reference the executables files as long as they are within the PATH.
- Ex. You want to type in ```python``` in CMD in hopes to start the python interpreter. 
    - You can do this if you let your OS know where to reference that python.exe in PATH.  
- You can also be cool and reference Photoshop (or any .exe) if you wanted to.  
    - Once the location or path of photoshop.exe is located, add this to PATH and now you can type ```photoshop``` to open Photoshop.  
    ![Cool Guy](https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExeHhud2Y4NnBkaWRpem9pOHlxemd0bWllMTd2NXBtcXQ3eDgyeWtzbiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xfD6mEBfQM3wk/giphy.gif)  


# Creating your python virtual environment
- This will keep all your python libraries separate and perfect to keep projects isolated. 
- You can also version control libraries as well, if it supports your current Python version.

## Create Virtual Environment 
First open CMD/PS within your current working directory where you want to create venv.  

Here we say open the python module **venv** with `python -m venv`.  
- Adding a name after will create a venv with that given name.  

`python -m venv [Virtual Environment Name]`  
- Ex. `python -m venv .venv`  
- Ex. `python -m venv venv`  
- Ex. `python -m venv poopenvNameDoesNotMatter`  

## Activate Virtual Environment
To use your environment, you need to activate it every single time.  
`python -m [Virtual Environment Name]\Scripts\activate.ps1`  

- Ex. .venv is the name of virtual environment folder    
`python -m .venv\Scripts\activate.ps1`  

## Deactivate
Type in terminal  
`deactivate`

## Install Packages from Text file
`PIP install -r [filename]`

## Save all your package versions to share
`PIP freeze > [filename].txt`

## Uninstall all current packages
Get all current packages and versions  
`PIP freeze > [filename].txt`  

Uninstall all packages one by one  
`PIP uninstall -r [filename].txt`  

Say yes to uninstalling all packages automatically with -y  
`PIP uninstall -r [filename].txt -y`

Uninstall all packages at once forced in one line (Not recommended)  
`pip freeze | % {pip uninstall -y $_}`