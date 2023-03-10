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
- setup.cfg (a initiation file for setup.py)
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
For more information on what sort of code can be put into __init__.py please refer to the example provided. 

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

The list of URLs below shows more information of the license and gives the neccessary documentation to substantiate each type of license.  

1)  https://choosealicense.com/
2)  https://opensource.org/licenses/BSD-2-Clause
3)  https://en.wikipedia.org/wiki/Software_license

You can also take a look at the license file in this repository file to get a better understanding of how a license looks like. 




####  Pythonproj_maddy17.toml file 
This file is a configuration file that shows the meta data of the package that you have created. It also directs "frontend" buidtools to the correct "backend" tools to use to create the distribution packages. 
 
You can refer to the Pythonprof_maddy17.toml file to observe the specific code that should be put in the file. 

In addition,the name of this file should also carry the same name as the package name. 

There are also different representations for the configurations files. For example, the meta data doesnt not neccessarily have to be in one configuration file. it can be split into two different files like how it has been done in this package. 

- Pythonproj_maddy17
  - Pythonproj_maddy17.toml
  - setup.cfg

If you use such a setup, the .toml file would only contain build information as shown in the example code provided in the package. Build information includes information on the modules required to build the package on the frontend and backend. Refer to the .toml for more information. 

Alternatively, you can vist the following websites for more information. 

*URLs*

1)  https://packaging.python.org/en/latest/tutorials/packaging-projects/
2)  https://towardsdatascience.com/how-to-convert-your-python-project-into-a-package-installable-through-pip-a2b36e8ace10 
3)  https://towardsdatascience.com/setuptools-python-571e7d5500f2





####  setup.cfg file
This file is an initiation file for setup.py which will be discussed more in depth in the following sections of this manual. 

It contains metadata information such as personal and contact information, classifiers and options. This information maybe combined with the .toml file in some cases to produce one file which will be the .toml file. However, with the newer release of PEP 517 and 518, it may be required to split the metadata into two files - .toml file and setup.cfg file - as shown in the example. For more information on this detail please refer to the following websites: 

1)  https://towardsdatascience.com/setuptools-python-571e7d5500f2
2)  https://peps.python.org/pep-0517/





####  setup.py file
This file is a python script that contains the package's metadata with the classifiers that would be used in generating and reading the package. Please refer to the example provided to see the specific code that is being input. 

Alternatively you can use the following websites to get a better understanding of what sort of metadata should be inside the file.

*URLs*

1)  https://towardsdatascience.com/make-your-own-python-package-6d08a400fc2d
2)  https://towardsdatascience.com/setuptools-python-571e7d5500f2
3)  https://packaging.python.org/en/latest/tutorials/packaging-projects/
4)  https://betterscientificsoftware.github.io/python-for-hpc/tutorials/python-pypi-packaging/
5)  https://towardsdatascience.com/how-to-convert-your-python-project-into-a-package-installable-through-pip-a2b36e8ace10




### Step 3
Once you have created the folders locally, you would be ready upload the package into PyPI.



