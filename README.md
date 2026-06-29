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
11-after after activating the venev we must initalize the git using command -git init
12-add the file README.md using command-git add README.md
13-commit the changes using command-git commit -m "any comment"
Save the current staged changes as a new version of my project
what -m does-It tells Git that you're providing the commit message directly in the command
what if we don't use -m git ask you type the message on terminal
14-to check the git status using command-git status
Here we we git this-On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        venv/

nothing added to commit but untracked files present (use "git add" to track)
as nothing is still commited 
15-next command it to make sure we are in main branch of git hub which one is default 
git branch → Used to create, delete, list, or rename branches.
-M → Rename the branch forcefully.
main → The new branch name.
Why is this command commonly used?
When you create a new Git repository locally:git init
older versions of Git created the default branch as master, while modern Git versions usually create main. 
This ensures your local branch is named main, which matches the default branch used by GitHub for new repositories.
What is mean by branch and why are they used for-
brach is the seprate copy of the project history 
If anyone what add new feature or new code in the project and later he realise that that went wrong 
to handel that problem we create a new brach rater than coding on main brach by uisng command -git branch new-model
If brach is already created we can switch the brach and code over there by using command-git switch new-model
After finishing the code and we got to know we can integrate it with the main brach e do it by using command-git switch new-model
this the same command that merge and switch the branch 
summery-Commit → -m = Message ("What should I call this snapshot?")
Branch → -m = Move/Rename ("Rename this branch.")
Branch → -M = Move/Rename Forcefully ("Rename it even if there's already a branch with that name.")
What is remote -remote is simply another copy of your Git repository that is stored somewhere else (usually on a server like GitHub).
Why we need remote if we our local repo get lost due any problem in system like laptop get lost and more so we keep the safe of copy of 
local repo so that we again edit it on another system taking it from remote repo 
to geting  the repo on git hub to our local system is called as git clone 
step1-open your git hub repo
step2-click on green code button
step3-now there are two ways to clone the repo 
1-HTTPS URL
2-SSH URL
1-copy the https url and run this command terminal -git cloe https_url in the folder on which you want to colne the file 
after colning verify which remote it is connected by using command-git remote -v

