# Software Setup -- alternatives

This document includes ways to install the necessary Python packages for the workshop.
We advise to follow the preferred instructions provided here: https://github.com/gw-odw/odw-2019/master/setup.md
as those alternative methods will be likely deprecated in the future. We give them here for completeness.

## Linux and Mac OS platforms: virtual environment and pip

1) Create a new environment

`python -m virtualenv gw-odw2`

2) Activate the environment

`source gw-odw2/bin/activate`

3) Install the support for Ipython notebooks

`(gw-odw2) $ pip install ipykernel`

4) [optional -- if old Python install] Upgrade your setup tools

`pip install pip setuptools --upgrade`

5) Get the software requirements

`wget -q https://raw.githubusercontent.com/gw-odw/odw-2019/master/requirements.txt -O requirements.txt`

6) Install the software

`pip install -r ./requirements.txt`

7) Create the Jupyter kernel

`ipython kernel install --user --name=gw-odw2`
