# Cookiecutter Data Science

_A logical, reasonably standardized, but flexible project structure for doing and sharing data science work._


#### [Project homepage](Modify from http://drivendata.github.io/cookiecutter-data-science/)


### Requirements to use the cookiecutter template:
-----------
 - Python 2.7 or 3.5
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0: This can be installed with pip by or conda depending on how you manage your Python packages:

``` bash
$ pip install cookiecutter
```

or

``` bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```


### To start a new project, run:
------------

    cookiecutter https://github.com/syhsu/cookiecutter-data-science


### The resulting directory structure
------------

The directory structure of your new project looks like this: 

```
{{cookiecutter.repo_name}}
├── .gitignore                          <- GitHub's excellent Python .gitignore customized for this project
├── LICENSE                             <- Your project's license. 
├── requirements.txt                    <- The required packages for reproducing the analysis environment
├── README.md                           <- The top-level README for developers using this project.
├── Dockerfile                          <- The Dockerfile for running the codes in src
│
├── data 
│   ├── raw                             <- The original, immutable data dump; .json/.yaml pointing to the raw data dump 
│   │   └── metadata.json               <- Format still requires to define but just update from the previous version, i.e. only-one record is kept.
│   ├── external
│   │   └── metadata.json     
│   ├── interim                         <- Intermediate data that has been transformed.
│   │   └── metadata.json
│   └── final                           <- The final, canonical data sets for modeling.
│       └── metadata.json
│
├── docs                                <- Documentations, reports, References, and all other explanatory materials
│   
│
├── notebooks                           <- Jupyter notebooks. Naming convention is a number (for ordering),
│                                          the creator's initials, and a short `_` delimited description, e.g.
│                                          `01_cp_exploratory_data_analysis.ipynb`. NOTE: clean outputs before pushing to git!!
│
├── models                              <- Trained and serialized models, model predictions, or model summaries
│   └── metadata.json
│
├── pipelines                           <- Pipelines and data workflows. Add subfolder from the used orchestration tool, e.g. airflow, kubeflow
│   ├── kubeflow
│   │   ├── {{cookiecutter.repo_name}}  <- compiled kubeflow pipelines    
│   └── airflow
│
├── src                                 <- Source folder for training, analyzing codes
│   └── components                      <- kubeflow components or airflow custom operators [Align with Dbox design]
│
├── tests                               <- Testing codes        
│   └──components                      
└── setup.py
```

### Installing development requirements
------------

    pip install -r requirements.txt

### Running the tests
------------

    py.test tests
