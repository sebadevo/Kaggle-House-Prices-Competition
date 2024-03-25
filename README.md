# Kaggle-House-Prices-Competition

Kaggle competition of House Prices prediction (House Prices - Advanced Regression Techniques)

## Environement installation

First you at least need a python version on your computer. If your on ubuntu you should have one out of the box, but if your on mac and/or windows you will want to install one. So first make sure you install python ([download python](https://www.python.org/downloads/)).

You will then need to install pyenv to manage the python version ([windows installation](https://github.com/pyenv-win/pyenv-win), [linux & mac installation](https://github.com/pyenv/pyenv)), it is actually a nice tool to have as later on for the creation of new environment you will easily be able to manage the python verison you will need. Once pyenv is install you will also need to install poetry (this project was created with poetry version 1.7.1). For that you can simply open your terminal and run the following command.

```
pip install poetry
```

```
cd *path_to_project*
```

Once poetry and pyenv are installed, the next step is to create an environment with the correct version of python. For that pyenv first need to install the python version needed.

```
pyenv install 3.10.13
pyenv local 3.10.13
```

Then we will make poetry use the environment just created by running

```
poetry env use 3.10.13
```

Finally, everything is set and we can let poetry install everything by running (this can take minutes to install depending on the internet connection):

```
poetry install
```
It can also be used directly in vs-code by selecting the interpreter and using 'your_project_name-XXX-py3.10.13'.
To select the interpreter enter <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> on Windows and Linux (<kbd>Cmd</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> on macOS) to open the Command Palette and click Python: Select Interpreter > + Enter interpreter path

## Environement creation

If eventually you want to create your own environment and install whatver you want, for example you create a completely new project here is how you want to proceed. First install pyenv and poetry (same way as in the [Environement installation](#environement-installation))

Once poetry and pyenv are installed, the next step is to create an environment with the correct version of python. For that pyenv first need to install the python version needed. In this case set the version to the one you wish, in this example it is set to 3.10.13 .

```
pyenv install 3.10.13
pyenv local 3.10.13
```

Then we will create the poetry environment.

```
poetry init
```

from here follow the instruction set by poetry, set the same python version as the one you installed with pyenv, and add all the library you wish. (Don't worry, even if you forget some libraries, you can add them later on)

Once you finished the poetry init creation, you will make poetry use the python version you installed with pyenv by running the following (remember to use the version you chose in the first step)

```
poetry env use 3.10.13
```

Then you can install the environment using

```
poetry install
```

and use the environment in the terminal with

```
poetry shell
```

(side note, if you want to add a library you forgot to add, now is the moment you can run)

```
poetry add *my_library*
```

It can also be used directly in vs-code by selecting the interpreter and using 'your_project_name-XXX-py3.10.13'.
To select the interpreter enter <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> on Windows and Linux (<kbd>Cmd</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> on macOS) to open the Command Palette and click Python: Select Interpreter > + Enter interpreter path
