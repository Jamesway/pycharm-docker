# Getting Pycharm (OS X) to work with Docker

## The Problem

When you start a project with your nice shiny docker image selected as the remote interpreter you'll probably see...  

![alt text](IMG/new_project.png)  

You might even try to add a path for the project location. It won't work.  
You'll get a "This interpreter type..." error instead of the "Remote path" error.

## The Hack

### 1) Start the project with a virtual environment  

![alt text](IMG/new_project_with_venv.png)

### 2) Delete out the venv directory after the scans finish
![alt text](IMG/scans.png)  

![alt text](IMG/venv_dir.png)

### 3) In preferences, select your docker image as the interpreter
- make sure to add the paths
- wait for Pycharm to find the packages

![alt text](IMG/paths.png)  

![alt text](IMG/paths_and_packages.png)

### 4) Success

Your project is using a python docker image.  

![alt text](IMG/test.png)  

if you see the container id, you're set
