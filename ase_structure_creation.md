# Creating and editing structures with Atomic Simulation Environment (ASE)

[ASE](https://ase-lib.org/) "is a set of tools and Python modules for setting up, manipulating, running, visualizing and analyzing atomistic simulations."

Today we will focus on some python modules that are useful for creating and manipulating atomic structures, but keep in mind that you can also use it for much more (like actually setting up and running calculations)!

## Installation

ASE can be installed just like any other python module. The most straight-forward way is to use `pip install ase`. If you're using Anaconda, it's best to install ASE within a conda environment. To create a new conda environment with ASE installed, you can type `conda create -n <your_chosen_env_name> ase`. Anaconda will install any other packages that ASE depends on. 

## Use

ASE is used within python code, but it does have some good graphical user interfaces for editing and visualising structures. Today we will run it using a Jupyter Notebook, but you can use many different editors to write and run python scripts. I recommend [Visual Studio Code](https://code.visualstudio.com/).

To use ASE within any python script, use import statements to access the functions you need. Today, our code will start with 
```python
from ase.io import write
from ase.visualize import view
from ase.build import graphene, sort
```

## Next

Next, let's start coding! [Click here](structure_build_example.ipynb) for the Jupyter Notebook. [download](https://qckenny.github.io/structure_build_example.ipynb)
