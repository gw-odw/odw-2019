# Software Setup

All tutorials are Python-based Jupyter notebooks. The instructions below explain how to install the necessary Python packages depending on the type of platform. The tutorial 2.6 on gravitational-wave skymap also requires the installation of the Aladin GUI ; installation instructions are provided at the bottom of this page for all platforms.

## Option 1: Google co-labs

<img src='https://www.wispresort.com/uploadedImages/Winter/easy.png' width=20 /> Easy (No software installation; Works for any OS)

You can open any notebook in the Google Co-labs.

1) Visit https://colab.research.google.com

2) Click the GITHUB tab

3) Enter "gw-odw/odw-2019" in the search bar, and click enter to search

4) Double click the notebook of your choice

5) At the top of the notebook, there are 2 lines to install the needed Python modules

`! wget -q https://raw.githubusercontent.com/gw-odw/odw-2019/master/requirements.txt -O requirements.txt` <br/>
`! pip install -q -r ./requirements.txt`

## Option 2: Run in mybinder

<img src='https://www.wispresort.com/uploadedImages/Winter/easy.png' width=20 /> Easy (No software installation; Works for any OS)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gw-odw/odw-2019/master)


## Option 2: You have a Linux or Apple/Mac computer -- Use conda

<img src='https://www.wispresort.com/uploadedImages/Winter/intermediate.png' width=20 /> Intermediate (Some software installation; Will not work on Windows PC)

Note: this workshop will use Python version 2.7.

1) Install miniconda: https://conda.io/en/latest/miniconda.html <br/>
Choose the version for Python 2.7. 
See the installation instructions here: https://conda.io/projects/conda/en/latest/user-guide/install/
You may need to restart your computer after installation.

2) Download or clone the git repo: https://github.com/gw-odw/odw-2019/archive/master.zip <br/>
`git clone https://github.com/gw-odw/odw-2019.git`

3) Add the conda-forge channel <br/>
`conda config --add channels conda-forge`

4) Move into the directory with the workshop git repo <br/>
`cd odw-2019`

5) Create the environment <br/>
`conda create --name odw2019 python=2.7`

6) Install the software <br/>
`conda install --name odw2019 --file requirements.txt` <br/>
`conda install --name odw2019 -c conda-forge jupyter` <br/>

7) Activate the enviornment <br/>
`conda activate odw2019`

8) Start the jupyter notebook server <br/>
`jupyter notebook`

## Option 3: You use Windows 10 -- Easy Linux install on Windows 10 with dedicated app

<img src='https://www.wispresort.com/uploadedImages/Winter/hard.png' width=20 /> Intermediate (For Windows 10)

Install a Linux distribution on your Windows system. 
See instructions here: https://docs.microsoft.com/en-us/windows/wsl/install-win10

We suggest you install Debian GNU/Linux, which is the closest distribution to what is 
used currently by LIGO/Virgo. Once you have Linux installed, follow the instructions 
in Option 2.

## Visualization tool for gravitational-wave skymaps 

To install the Aladin GUI, follow the instructions here: https://aladin.u-strasbg.fr/java/nph-aladin.pl?frame=downloading
