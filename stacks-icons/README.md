
# Stacks Icons Generation tool

This tool will take icons then resize and rename them to create the 4 icons required for Stacks 2 & RapidWeaver 6. 

**Warning**: This workflow will overwrite the icons that you pass to it.

### Installation

Copy the workflow file into the /Library/Services folder inside your home folder

### How to Use

1. Right click on one or more icons that are at least 256px in size. 
2. Go to Services->Stack Icons
3. Done

The images created are based on the name of the icon that the service processes. So if we take **icon.png** as an example. The service will generate the following icons:

* icon.png (*128px*)
* icon@2x.png (*256px*)
* icon@58.png (*58px*)
* icon@50.png (*50px*)
