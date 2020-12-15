{{cookiecutter.project_name}}
==============================

{{cookiecutter.description}}

Project Organization
------------
    ├── .gitignore                <- GitHub's excellent Python .gitignore customized for this project
    ├── LICENSE                   <- Your project's license.
    ├── requirements.txt          <- The required packages for reproducing the analysis environment environment.yaml[conda]? pipflie[pipenv]?
    ├── README.md                 <- The top-level README for developers using this project.
    │
    ├── data
    │   ├── raw                   <- The original, immutable data dump.
    │   ├── external              <- Data from third party sources.
    │   ├── interim               <- Intermediate data that has been transformed.
    │   └── final                 <- The final, canonical data sets for modeling.
    │
    ├── docs                      <- Documentations, reports, References, and all other explanatory materials
    │   └── figures
    │
    ├── notebooks                 <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                                the creator's initials, and a short `_` delimited description, e.g.
    │                                `01_cp_exploratory_data_analysis.ipynb`.
    │
    ├── models                    <- Trained and serialized models, model predictions, or model summaries
	│
    ├── serve                     <- Serving codes: Dockerfile, reuqirements.txt, README.md, app.py
    │   ├── Dockerfile            <- Dockerfile for HTTP API
    │   ├── requirements.txt      <- The required packages for the serving environment
    │   └── app.py                <- The entry point of the HTTP API
    │
    ├── pipelines                 <- Pipelines and data workflows. Add subfolder from the used orchestration tool, e.g. airflow, kubeflow
    │
    ├── src                       <- Source folder for training, analyzing codes
    │
    ├── tests                     <- Test codes data folder for dummy testing dataset?             
    │   └── serve                 <- Test serving codes
    │       ├── fixtures          <- Where to put example inputs and outputs
    │       │   ├── input.json    <- Test input data
    │       │   └── output.json   <- Test output data
    │       └── test_app.py       <- Integration tests for the HTTP API
    │
	└── setup.py


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
