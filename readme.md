# Study AI from zero to mastery

This is a simplified version of the original ZTM project on github, which does not require that\
Anaconda, Conda and jupterbook pre-installed.

It uses Python3 as interpreter to run the code in `.ipynb` files, and uses poetry to manage dependencies.

Those are the steps to create a project like this on your laptop.

## Install Python
Download latest stable version of python3 installer and install or use `brew install`.
I prefer brew.
```bash
# install python3
brew install python
# check version
python3 --version
# export Path in your $HOME/.bash_profile
alias python="/usr/local/bin/python3.13"
export PATH="/usr/local/bin/python3.13:${PATH}"
# source your profile to make the executive path effective
source $HOME/.bash_profile
```

## Create VirtualEnv & Activate it
```bash
# create a project directory
mkdir <project-name>
# cd into the dir
cd <project-name-dir-path>
# create venv
python -m venv myenv
# acitvate venv
source myenv/bin/activate
```

## Install poetry
```bash
# upgrade pip
python -m pip install --upgrade pip
# install poetry
pip install poetry
```

## Poetry config project
Use poetry to configure your project and manage the dependencies.
```bash
# add dependency
poetry add <dependency-name>
```