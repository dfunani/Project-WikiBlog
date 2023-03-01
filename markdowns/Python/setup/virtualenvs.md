# Virtual Environments

> A **virtual environment** ('VENV') is a tool that helps to manage and containerize dependencies required by a project, by creating an isolated python virtual environments for the project.

## Setting up a Virtual Environment

The **virtual environment** tool '**VIRTUALENV**' creates a folder that will maintain the various python packages required by that particular **Python** project.

### Install VIRTUALENV

Using **Python Index Packages** ('PIP'), VIRTUALENV can be installed by running from the command line interface ('**CLI**'):

```python
$ pip install virtualenv
```

### Create VENV/ENV

Using **VIRTUALENV**, a virtual environment ('**venv/env**') can be created:

```python
$ virtualenv name_of_venv_to_create
```

> 🎆 Generally, the name of the virtual environment is '*env*' or '*venv*'\
> 🎆 '*-p*' can be used to specify a a particular Python interpreter: \
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;```virtualenv -p /usr/bin/python3 env```

### Activate VENV/ENV

The virtual environment must be activated:

```Python
$ cd ./folder_containing_venv/
$ ./env/Scripts/Activate
```
> 🎆 Terminal will show venv/env:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;```(env) $```

### Deactivate VENV/ENV

The virtual environment can be deactivated:

```Python
$ deactivate
```
> 🎆 Terminal will no longer show venv/env:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;```$```
