smlm_cloud_analysis
==============================

Analysis of point cloud SMLM data. Including ...

Project Organization
------------

    ├── LICENSE
    ├── Makefile
    ├── README.md
    ├── config.yaml
    ├── dev_requirements.txt
    ├── docs
    │   ├── Makefile
    │   ├── commands.rst
    │   ├── conf.py
    │   ├── getting-started.rst
    │   ├── index.rst
    │   └── make.bat
    ├── models
    ├── notebooks
    ├── pyproject.toml
    ├── references
    ├── setup.cfg
    ├── src
    │   └── __init__.py
    ├── test_environment.py
    ├── tests
    │   └── test_data
    └── tox.ini
-------------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>

Prerequisites
----------

Recommend installing miniconda.

Details for miniconda installation

Setup linux
-----------

Navigate to where want this repository, clone this repository

```
git clone ...
```

For security reasons we use a .env file to store the path to the data, this is ignored by Git by default.
Therefore, you should add a file called .env to the top level (i.e. same level as License, Makefile, Readme.md,...).
In this file you need ...

```
RAW_DATA_PATH = path/to/data
```

example .env file assuming all your .csv files are in a folder called smlm_csv_folder; note the paths are normally taken as relative to the .env file - so this may take some fiddling around to get it correct (alternatively copy your csv folder into data then path would be = data/smlm_csv_folder) : 

```
RAW_DATA_PATH = ../../smlm_stuff/smlm_csv_folder
```

Create the environment then activate it

```
make create_environment
conda activate ENV_NAME
```

Install dependencies

```
make requirements
```

Install package - this will be depreceated once package is open source

```
pip install git+https://github.com/oubino/package.git
```

Setup windows 
-------------

## On normal windows

Navigate to where want this repository, clone this repository

```
git clone ...
```

For security reasons we use a .env file to store the path to the data, this is ignored by Git by default.
Therefore, you should add a file called .env to the top level (i.e. same level as License, Makefile, Readme.md,...).
In this file you need one line with this
your directory CANNOT HAVE SPACES IN THE NAME i.e. if your directory is named "data/my data folder/" it will not work - you should rename your directory on your computer to something like "data/my_data_folder/"

```
RAW_DATA_PATH = path/to/data
```

example .env file assuming all your .csv files are in a folder called smlm_csv_folder; note the paths are normally taken as relative to the .env file - so this may take some fiddling around to get it correct (alternatively copy your csv folder into data then path would be = data/smlm_csv_folder) : 

```
RAW_DATA_PATH = ../../smlm_stuff/smlm_csv_folder
```


Create the environment then activate it

can't run 

```
make help
```
or
```
make create_environment
```

Therefore setup

```
conda create -n smlm_analysis python=3.9
conda activate smlm_analysis
```

Install dependencies

```
make requirements
```

Install smlm - this will be depreceated once smlm is open source

```
pip install git+https://github.com/oubino/smlm.git
```

## WSL2 

Install wsl2


Usage 
-----

## Linux



## Windows



