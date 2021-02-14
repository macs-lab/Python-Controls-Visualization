# Control Systems Visualization

Click the button below to launch the binder repository of notebooks

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/macs-lab/Python-Controls-Visualization/main)

## Individual Modules
[Inverted Pendulum-Cart Control](https://mybinder.org/v2/gh/macs-lab/Python-Controls-Visualization/bdeb35d89f344c499a280fcf606a0be05411694c?filepath=Notebooks%2FInverted_Pendulum_Control_Demo.ipynb)

[Inverted Pendulum-Cart Pole Placement](https://mybinder.org/v2/gh/macs-lab/Python-Controls-Visualization/bdeb35d89f344c499a280fcf606a0be05411694c?filepath=Notebooks%2FInverted_Pendulum_Pole_Placement.ipynb)

[Transition from MATLAB to Python Controls Package](https://mybinder.org/v2/gh/macs-lab/Python-Controls-Visualization/bdeb35d89f344c499a280fcf606a0be05411694c?filepath=Notebooks%2FMatlab-to-Python.ipynb)

## 1 - Visualizing Control Systems in Python

This repository contains the files for creating visualizations using different python packages. 

### 1.1 - Matplotlib

The matplotlib package can be used to create widgets such as sliders, buttons, etc. onto a matplotlib figure. The same package can be used to create animations using the Funcanimation package in matplotlib. See the file **inverted_pendulum_control_demo.ipynb** for instructions and syntax to create widgets and animations

### 1.2 - ipywidgets

Ipywidgets is another package that offers interactive widgets. See the notebook titled **ipywidgets_pendulum.ipynb** for step-by-step guide to using the widgets from ipywidgets

## 2 - Pushing Repository using MyBinder

Mybinder is a tool that allows creating a virtual jupyter environment of your github repository files. It is a fast, free and easy-to-use tool. The following steps show how to publish your repository of files and notebooks. 

### 2.1 - Creating environment files 

The first step is creating a file that contains packages for the jupyter environment. Binder recognizes the file data and installs the required packages for your environment.

**Creating environment.yml**

Create a github repository and make sure that it is **Public**. In the main branch of the repository, create a new file titled environment.yml and in the file, mention the environment type and required packages. A sample environment.yml is present in this repository which is used to create the environment for this project. 

The format for the file is as follows:

>channels:  
>     \- conda-forge  
>  \- defaults  
>dependencies:  
>  \- ipython  
>  \- ipywidgets  
>  \- matplotlib  
>  \- control  
>  \- scipy  
>  \- slycot  
>  \- nbgitpuller  

In the text above, the *dependencies* are the python packages to be installed.

### 2.2 - Creating MyBinder link

Go to the [MyBinder](https://mybinder.org) page and follow these steps: 

- In the "GitHub repository name or URL" field, insert the link to your github repository. Example: https://github.com/username/repository/

- In the "Git Ref" Field, type *main*

- "Path to a notebook" is optional. you can inclue the link to a file in the repository to open on binder launch

This generates a link to your mybinder environment below which can be copied to clipboard. This link will launch the binder. It can be created and shown as a button (as done above with the "launch bidner" button) or directly opened in a browser. 

Press Launch and that's it! You have pushed your repository to an online environment that can be accessed anywhere.

**NOTE:** 

1 - It will take time for initial setup and to build the environment (you can click show logs to see the progress). 

2 - After initial setup, launching again using the link will not take time. 

3 - **Any changes to the repository will require rebuilding the environment and will take time**. Therefore, only click the link once you have all the files/notebooks sorted and in place. To avoid such situations, one can create separate repositories for environment and content. Guide: TBA

A step-by-step guide for the whole process above is available at this [YouTube](https://www.youtube.com/watch?v=owSGVOov9pQ&ab_channel=SerenaBonaretti) Link.

## 3 - Other Resources 

### 3.1 - MATLAB to Python Controls Toolbox Transition Guide

A beginner guide for transition from MATLAB to Python Controls box is available in the file titled **Matlab-to-Python.ipynb**. This guide includes the syntax to use common commands and functions in the controls toolbox. This guide also shows how to install the required packages to your system to run the controls toolbox. 

### 3.2 - Inverted Pendulum Pole Placement

The file **inverted_pendulum_pole_placement.ipynb** is an interactive code that controls an inverted pendulum using Full State Feedback Control. The user can enter the desired closed loop poles and the effects on the system response which are displayed through animations. 
