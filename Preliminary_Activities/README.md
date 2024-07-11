# Introduction and preliminary activities

Please read carefully all the information given below.

This School focuses mainly on python, but there are a few lectures on Matlab and R too (https://www.r-project.org/).  All the code will be shared on github, so we recommend reading the basics on using GIT:

https://github.com/ciencialatitud0/EPIC_4/blob/main/Preliminary_Activities/1_introgit.pdf

We will use python 3.x and jupyter notebooks (.ipynb) for the courses taught at this School.

- Jupyter notebooks are very useful tools for learning programming because they provide a nice visual and interactive interface.

- You can see the results of your code live, instead of waiting till your script (.py) finishes running in a terminal.

To be able to use python and jupyter notebooks in your laptop, there are several options:

## OPTION 1: Google Colab (see https://colab.research.google.com/):

**Important Note: We highly recommend this option for participants with little programming experience.**

One option is to use Google Colab, for which you would need a Google account, which can be a personal gmail account or an institutional email account supported by Google. The advantage of using Google Colab is that all libraries are installed in a Linux server remotely, so we don't need to worry about compatibility issues, different operating systems, etc. The disadvantage is that Colab provides limited RAM memory, limited space, and computing resources as everything runs in a cloud, so you can only use it to process small datasets. Google Colab will be sufficient to follow all the exercises developed in the School.

## How do I test Google Colab?

1. Log into your Google account.

2. Open this notebook: https://github.com/ciencialatitud0/EPIC_4/blob/main/Preliminary_Activities/2_notebook.ipynb

3. Clic on "Open in Google Colab".

4. Run all the cells in this notebook. You can place the image of the worked example (which you can find here: https://github.com/ciencialatitud0/EPIC_4/blob/main/Preliminary_Activities/images/Cotopaxi_volcano.jpeg) or any other image into your "Colab Notebooks" folder in Google Drive.

5. If you see a plot of sin(x) vs. x and the image of the Cotopaxi volcano, your local Google Colab works.

6. Congrats, you are ready to follow all the python tutorials of the School.


## OPTION 2: Anaconda/Miniconda (see https://anaconda.org/):

**Important Note: We recommend this option only for participants with substantial Linux and programming experience.**

Another option is to have python (and all the libraries you need to analyse your datasets) installed in your laptop. This can also be done in many ways, but anaconda is now very popular because it provides good portability and an interface that allows the user to include extra kernels for other programming languages. Anaconda has the advantage that you have all the code you need locally in your laptop. **In the long term, using Anaconda will be much more advantageous for you.**

# Installation instructions

## How to install Anaconda?
Download Anaconda from this website: https://www.anaconda.com/products/individual. Choose the package version that best suits the operating system (OS) of your laptop.

### On Linux and MacOSX:
For testing and customising your installation on Linux/MaxOSX laptops/PCs, follow these instructions:

#### Option A: Installation from a terminal (recommended)

1. Open a terminal window.<br>

2. Type the command below:<br>
~~~~html
  $ conda --version
  conda 24.1.2
~~~~

3. That means you have anaconda 24.1.2 installed.<br>

4. Now, let us check which environment you have:<br>
~~~~html
  $ conda env list
  conda environments:
  base                  *  /Users/webb/opt/anaconda3
~~~~

5. Let us know create a new environment with:<br>
~~~~html
  $ conda create -n py39 python=3.9
  $ conda env list
  conda environments:
  base                  *  /Users/webb/opt/anaconda3
  py39                     /Users/webb/opt/anaconda3/envs/py39
~~~~

6. Now, we activate the environment:<br>
~~~~html
  $ conda activate py39
  $ conda env list
  conda environments:
  base                     /Users/webb/opt/anaconda3
  py39                  *  /Users/webb/opt/anaconda3/envs/py39
~~~~

7. Let us check with libraries are installed by default:<br>
~~~~html
  $ conda list
~~~~

8. Let's install a few extra libraries:<br>
~~~~html
  $ conda install jupyter numpy scipy matplotlib mpi4py git
~~~~

9. Type 'yes' to accept changes, and check that the new libraries are present.<br>
~~~~html
  $ conda list
~~~~

10. Let's now open a jupyter notebook, and we are ready to work.<br>
~~~~html
  $ jupyter notebook
~~~~

10. Once the notebook is open, you can start coding your notebook:<br>

https://github.com/ciencialatitud0/EPIC_4/blob/main/Preliminary_Activities/2_notebook.ipynb

### On Windows:
If you are using Windows, we highly recommend either:

1. setting up a dual partition in your hard drive with both Windows and Linux, or
2. setting up a Virtual Machine (VM) with a linux distribution. For this:

- Download VirtualBox from: https://www.virtualbox.org/
- Follow the instructions here: https://itsfoss.com/install-linux-in-virtualbox/

After the installation of the VM is successful, follow the instructions provided above for Linux/MacOSX systems to set up your Anaconda installation.

In the long term, you may want to fully switch to Unix-based operating systems. Ubuntu is a popular and user-friendly option.


## How do I test and use Anaconda?
Assumming all the steps above went well, and you were able to create your first jupyter notebook, open a new notebook and follow these two tutorials on jupyter notebooks and basic python:

- https://datacarpentry.org/python-ecology-lesson/jupyter_notebooks/
- https://swcarpentry.github.io/python-novice-gapminder/

Please note that we will **NOT** have time to cover the basics in the School, so make sure you are familiar with the material above.

# Highly recommended preliminary tutorials:

If you have little or no python programming experience, we highly recommend to follow all these tutorials before EPIC starts:

- https://github.com/wbandabarragan/computational-physics-1/blob/main/unit-1/104-python-basics-review.ipynb
- https://github.com/wbandabarragan/computational-physics-1/blob/main/unit-1/105-Numpy-Arrays.ipynb
- https://github.com/wbandabarragan/computational-physics-1/blob/main/unit-1/106-Plotting-in-Python.ipynb
- https://github.com/wbandabarragan/computational-physics-1/blob/main/unit-1/107-Python-Functions.ipynb
- https://github.com/wbandabarragan/computational-physics-1/blob/main/unit-1/108-Data-Input-Output.ipynb
- https://github.com/wbandabarragan/computational-physics-1/blob/main/unit-1/109-Data-IO-Pandas.ipynb
