# Documentation
An instruction manual on how to create your own pip installable package and on how to upload into PyPI

##  Author
- Maathavan Manimaran

##  Steps

### Step 1
Make sure you have created the following file structure locally:

Pythonproj_maddy17 (Name of your package)
- src (Contains the source code and initiation files)
- README.md (Contains documentation and instruction on how the package works)
- LICENSE (Contains the License details as to prevent infringement of copyrights)
- setup.py (A python script that enables the execution of packaging commands)
- Pythonproj_maddy17.toml (a configuration file that follows the same name as the package and contains the metadata about the package)


These files are important to ensure that your package uploads correctly. Once you have created these files we will look into each one of them to see the components needed to make each of the file work correctly. I will be presenting alternative forms of structure as well in case one solution does not work. If none of the structures work please refer to the sources above to troubleshoot the exact problem. 

### Step 2
Observing each component of the structure and creating the correct file structure of each internal component so that the package is able to compile properly. 

####  src folder
This folder should contain another folder that shares the same name as the package folder. 

- src
  - Pythonproj_maddy17

Under src/Pythonproj_maddy17 folder, there should be mainly two types of files. 

1)  Your source scipt (Python)
2)  A Python Initiation file

So your file sturcture for the src folder will look something like this 

- src
  - Pythonproj_maddy17
    - Source_code.py
    - __init__.py

The source script here refers to the code you have created using python to make your application of robot run. It also the module of your package that contains all the logic functions of your package. 

The python initiation file is a very important piece of file. It is required to import the directory as a package and it should be empty. However, it does not have to strictly be empty.

If your module have multiple source codes then you can create a folder for each script with a python initiation script in it. The structure for such a module would look like this: 

- src
  - Pythonproj_maddy17
    - __init__.py
    - source_code_1.py
    - source_code_2.py

If you want a more organised and full proof but tedious srtucutres there are also other alternative structure like the one below. 

- src
  - Pythonproj_maddy17
  
    - Package 1
      - source_code_1.py
      - __init__.py
  
    - Package 2
      - source_code_2.py
      - __init__.py



If you have any questions or issues on how to organise the source code files locally you can visit the following websites to obereve and learn what you can do. 

*URLs*

1)  https://towardsdatascience.com/how-to-convert-your-python-project-into-a-package-installable-through-pip-a2b36e8ace10

2)  https://betterscientificsoftware.github.io/python-for-hpc/tutorials/python-pypi-packaging/

3)  https://towardsdatascience.com/make-your-own-python-package-6d08a400fc2d


####  LICENSE
This file contains the information on which License you are using to prevent the package from being flagged for infringement. 

The list of URL below shows more information of the license and gives the neccessary documentation to substantiate each type of license.  








# package_template
A Template to build a Hello World PIP package

## Authors
- Maathavan Manimaran
## Installation

Install Pythonproj_maddy17 with pip
```bash
  pip install Pythonproj_maddy17
```
## Requirements
* nothing its just a python script
