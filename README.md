# ATGU Hail Workshop 2023

As part of a new hire workshop series at the Analytic and Translational Genetics
Unit (ATGU), Massachusetts General Hospital, we decided to introduce Hail as a
genomics analysis tool. This git repo contains the workshop materials for
analysing common (GWAS) using Hail.


Lead: Edmund Higham

TA: Patrick Schultz, PhD


## Installation Instructions

Before we begin, Hail depends on Java 8 or 11. Please ensure you have either
installed. You can download a JDK for your platform [here](https://www.oracle.com/java/technologies/downloads/#java11).

In the following steps, we assume you're using MacOS and ZSH.

We'll start by cloning this repository and then setting up a python 3.9 virtual
environment.

    $ git clone git@github.com:hail-is/ATGU-Hail_Workshop2023.git
    $ cd ATGU-Hail_Workshop2023


We'll then set up a python virtual 3.9 environment and install hail. We'll use
[pyenv](https://github.com/pyenv/pyenv) select the python version

    $ brew install pyenv
    $ eval "$(pyenv init -)"
    $ pyenv install 3.9
    $ pyenv local 3.9


(Optional) Set up a virtual environment for this repository only:

    $ python -m venv .venv
    $ source ./.venv/bin/activate


Then install hail and jupyter

    $ pip install hail jupyter


You can use vscode with the python extension or explore the tutorial notebook
in your browser:

    $ jupyter notebook


## Common Variant Analysis with Hail

&emsp;_Date_: September 12th, 2023

&emsp;_Slide deck_: `CommonVariantAnalysisHail.pdf`

&emsp;_Jupyter notebook_: `ATGUworkshop_CVanalysis.ipynb`


The `resources` folder contains the files needed to run the Jupyter notebooks.
