# PYPI python package template

## Steps to create a project structure using this template

## 1. Run template.py

This creates a project folder in the root folder pypi-template. Enter the project name when asked in terminal.

If you want to add more files/folders   to the project, add its path in list_of_files in template.py.

Run *python template.py* and *enter the name of the project*.

```
$ python template.py
Enter the Project Name: test_project
[2022-10-20 15:36:34,102: INFO]: Creating project by name: test_project
[2022-10-20 15:36:34,103: INFO]: Creating a directory at: src\test_project for file: __init__.py       
[2022-10-20 15:36:34,104: INFO]: Creating a new file: __init__.py at path: src\test_project\__init__.py
```

## 2. Fill setup.py

Fill this part with your github repo name, username and email.

```
REPO_NAME = "<YOUR REPO NAME>"
AUTHOR_USER_NAME = "<YOUR USERNAME>"
SRC_REPO = "<YOUR REPO NAME>"
AUTHOR_EMAIL = "<YOUR EMAIL ID>"
```

## 3.Run script init_setup.sh

This script will create a virtual environment and activates it. Here, I am going to install python with version 3.8. This can be changed as needed.
After creating the virtual environment, all packages mentioned in requirements_dev.txt file will be installed into the environment.

In the end of requirements_dev.txt, **-e .** is given inorder to install all local packages. This will check for setup.py file. 

Note: This script is running in a different terminal. So, after the run, activate the virtual environment in vscode terminal. 
```
conda activate ./env
```


## References
This work is refered from **Sunny Bhaveen Chandra's work - Pypi Packages: Project setup**

You can find the source [here](https://www.youtube.com/watch?v=X868cWGsrVY&list=PLrdaCCBhU_hlLUujFA5KUjb3yathXilut&index=2).
