# Software Setup

## Option 1: Google co-labs

<img src='https://www.wispresort.com/uploadedImages/Winter/easy.png' width=20 /> Easy (No software installation)

You can open any notebook in the Google Co-labs.

1) Visit https://colab.research.google.com

2) Click the GITHUB tab

3) Enter "gw-odw/odw-2019" in the search bar, and click enter to search

4) Double click the notebook of your choice

5) At the top of the notebook, add these 2 lines to install needed python modules

`! wget -q https://raw.githubusercontent.com/gw-odw/odw-2019/master/requirements.txt -O requirements.txt`
`! pip install -q -r ./requirements.txt`



## Option 2: Use conda

<img src='https://www.wispresort.com/uploadedImages/Winter/intermediate.png' width=20 /> Intermediate (Some software installation)

1) Install miniconda: https://conda.io/en/latest/miniconda.html
You may need to restart your computer after installation

2) Download or clone the git repo
`git clone https://github.com/gw-odw/odw-2019.git`
OR
Click: https://github.com/gw-odw/odw-2019/archive/master.zip

2) Add the conda-forge channel
`conda config --add channels conda-forge`

3) Download the yml file for the enviornment you want (or, find it in the git repo from step 2)
`! wget https://raw.githubusercontent.com/gw-odw/odw-2019/master/enviornment-odw2019.yml`

4) Create the enviornment
`conda env create -f environment-odw2019.yml`

5) Activate the enviornment
`conda activate odw2019`

6) Start the jupyter notebook server
`jupyter notebook`

