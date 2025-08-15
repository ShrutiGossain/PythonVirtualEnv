# Creating Virtual Environment

### Requirements

- Installing pandas
- Installing virtualenv using `pip install virtualenv`
- Run `virtual env (name of the virtual env)` here wscube. A folder named wscube is created.

### Activate/ Deactivate virtualenv

- Navigate to Scripts folder in wscube (using cmd).
- To activate the wscube, Run `activate`
- To deactivate the wscube, Run `deactivate`

### How to run main.py in virtual environment

- Navigate to Scripts using cmd.
- Run `activate` to activate the wscube.
- Come out of the Script folder using `cd ..` 
- Come out of the wscube using `cd ..`
- Now you are in the root directory
- Run `py main.py` in the terminal. If faced `ModuleNotFound` error for any library, run command `pip install <library>`

### Generating requirement.txt for the wscube.

- Be in the root directory, make sure wscube (virtual environment) is activated.
- Run `pip freeze > requirement.txt`

#### [OPTIONAL] To know which modules are being used in the root directory (virtualEnv) 
- We need to create requirement.txt in virtualEnv.
  - First deactivate the wscube using command `deactivate`.
  - Create a new folder in root directory (say for example demo).
  - Run `cd demo`
  - Run `py -m pip freeze > requirement.txt`.
  

You will have the list of all modules with versions being used in your current project in requirement.txt file.

### Installing the module listed in requirement.txt

- Navigate to Scripts
- Activate the wscube
- Run `pip install <module=-version>`

### Installing all the modules together listed in requirement.txt

- Navigate to Scripts
- Activate the wscube
- Run `pip install -r.\requirement.txt`

## Creating the clone of the existing installed python in the system.

- Deactivate any other python virtual environment created.
- Run `py -m virtualenv --sytem-site-packages`.

