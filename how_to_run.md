#Step 1: Download miniconda
##These four commands download the latest M1 version of the MacOS installer, rename it to a shorter filename, install it silently, and then delete the installer.(If you are other version please follow the official website tips to download.)


mkdir -p ~/miniconda3
curl https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh -o ~/miniconda3/miniconda.sh
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
rm ~/miniconda3/miniconda.sh


##After installing, close and reopen your terminal application or refresh it by running the following command:

source ~/miniconda3/bin/activate

###IF you want
###To initialize conda on all available shells, run the following command:

conda init --all

#Step 2: To re-create the environment from the file, run:

conda env create -f environment.yml

#Then activate the environment:

conda activate myenv

#Step 3: Run the Script

python Q19.py

