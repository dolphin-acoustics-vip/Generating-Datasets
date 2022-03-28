# CNN classifier for dolphin whistle spectrograms

The easiest way to set up and run the jupyter notebook files in this folder is by creating a virtual environment for this project. This way you can avoid the so-called "dependency-hell".
But you can obviously choose your own preferred way of getting everything set up, just know that it will be more work.

The Python version used in this project is Python 3.9.10

## First step: creating a virtual environment using virtualenv

First, check that you have virtualenv installed:
`which virtualenv`
if you don't have virtualenv installed enter the following in terminal:
`pip install virtualenv`

Now create a virtual environment:
`virtualenv <virtual_env_name>` (replace <virtual_env_name> with any name. For example you could type: `virtualenv dolphin_acoustics`)

Activate your virtual environment:
`source <virtual_env_name>/bin/activate`

You can verify that you are in the correct virtual environment by typing:
`which python`
`which pip`
The terminal/command-prompt usually shows that you have activated a virtualenv by displaying `(<virtual_env_name)` before the prompt.

Install all the necessary libraries and modules of the correct versions by typing:
`pip install -r requirements.txt`

### Deactivating or deleting your virtual environment

To deactivate the virtual environment:
`deactivate`

To delete an environment enter the following command:
`sudo rm -rf <virtual_env_name>`

## Second step: add virtual enviroment to jupyter notebook

1. activate your venv if you haven't already
2. install ipykernel (this provides the ipython kernel for jupyter, ie allows jupyter to change a kernel based on a virtual enviroment)
3. add the virtual environment to Jupyter by typing:
`python -m ipykernel install --user --name=<virtual_env_name>`
or you can change the kernel with the GUI in the jupyter notebook interface:

## Deleting your virtual environment from the jupyter notebook

if you delete your virtual environment you would need to remove it from the list of kernels:
`jupyter kernelspec list`
`jupyter kernelspec uninstall <my_env_name>`