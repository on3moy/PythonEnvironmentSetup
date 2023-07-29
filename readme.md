# Creating your python virtual environment
![Bear](https://i.pinimg.com/originals/33/82/cc/3382cc9cfac5588e571d51a8bbee69f3.gif)
## Create Virtual Environment 
`python -m venv [ProjectName]`

### Example
venv is the name of virtual environment folder    
`python -m venv venv`  

## Activate Virtual Environment
`python -m [vevn folder]\Scripts\activate.ps1`

### Example
venv is the name of virtual environment folder    
`python -m venv\Scripts\activate.ps1`  

## Deactivate
Type in terminal  
`deativate`

## Install Packages from Text file
`PIP install -r [filename]`

## Save all your package versions to share
`PIP freeze > [filename].txt`

## Uninstall all current packages
Get all current packages and versions  
`PIP freeze > [filename].txt`  

Uninstall all packages one by one  
`PIP unintall -r [filename].txt`  

Say yes to uninstalling all packages automatically with -y  
`PIP unintall -r [filename].txt -y`
