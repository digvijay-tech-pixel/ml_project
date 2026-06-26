#FIRST STE UP:
1-creat an github repo
2-create a folder in system and open with anaconda prompt with
first changeing the directory to project directory and then open it in vs code using command-code .
3-creteing an virtual envorment on terminal either by simple python command or conda prompt 
here in this project we we are using conda command-conda create -p venv python==3.24 -y
Here is what command mean -saying to conda that create a virtual environment with name venv and python version=3.14 and -y saying saying that giving permission to install the requrments in venv
4-As this command given the 3 channels activates which are used to install package :
1-defalut -package given by comapany
2-conda -forge-which is an community store which is public and we anyone can give public the there own package 
3-bioconda-Made for biology and data science packagesHas specialized scientific tools
Like a specialized store for scientists
5-command to update the conda-conda update -n base -c defaults conda
6-command to see the channels-conda chanel confiuration -conda config --show channels
7-How does this works actually -
You type: conda install numpy
              ↓
Conda checks channel 1 (defaults) → found? download it
              ↓
Not found? Check channel 2 (conda-forge) → found? download it
              ↓
Not found? Check channel 3 (bioconda) → found? download it
              ↓
Not found anywhere? → Error!
8-How to create own new channel-conda config --add channels conda-forge
creating new channel doesn't help at all as we are installing it from conda default only 
9- How do we install packages forom speacific channel-conda install -c conda-forge numpy
For default we don't write it or not write it both are same 
10-Jumping back to venv now we actiate it using command-conda actiavate 

