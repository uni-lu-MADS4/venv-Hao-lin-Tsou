# Doenload conda mini
#These four commands download the latest M1 version of the MacOS installer, rename it to a shorter file name, silently install, and then delete the installer:

mkdir -p ~/miniconda3
curl https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh -o ~/miniconda3/miniconda.sh
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
rm ~/miniconda3/miniconda.sh
#Check the installation by running 

conda --version.

#Update conda by running 

conda update conda.

#Creating a conda environment
conda create --name myenv python=3.9

to activate the environment, run:
conda activate myenv

# How to Run

## Step 1: Create and Activate the Environment
To create a new conda environment, run:
```bash
conda env create -f environment.yml

## Step 2: Then activate the environment:

conda activate myenv

## Step 3: Run the Script

python Q19.py

##note
#Add clone
git clone
cd [your clone name]
ls

#Create a Conda virtual environment: Run the following command to create a new Conda environment and specify Python version 3.9:

conda create --name myenv python=3.9

#to activate the environment, run:
conda activate myenv


#to install a package in the environment, run:
conda install PACKAGE_NAME

conda install faker


