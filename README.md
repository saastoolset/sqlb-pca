# sqlb-pca
Python Clean Architecture for sqlg library
## I. The proposed environment setup
- conda as environment manager
- pypi/pip as package repository and manager 
- Poetry as the dependency manager.

https://ealizadeh.com/blog/guide-to-python-env-pkg-dependency-using-conda-poetry


## II. Environment prepare

### Virtual environment 

```
$ conda env create -n sqlb-pca
$ conda activate sqlb-pca

```

### Install Poetry

```
conda install -c conda-forge poetry
```

Setup path 
```
$HOME/.local/bin for Unix
%APPDATA%\Python\Scripts on Windows
```


### poetry initial
```
$ poetry init
```

## III. PCA installation

### pca-scaffold
#### Step 1: Install Cookiecutter

Install cookiecutter:

``` bash
$ conda deactivate sqlb-pca
(base) $ pip install cookiecutter
$ conda activate sqlb-pca
```

#### Step 2: Generate Your Package

Now it's time to generate your Python package.

Run the following command and feed with answers, If you don’t know what to enter, stick with the defaults:

```bash
cookiecutter https://github.com/pcah/pca-scaffold.git
```

Finally, a new folder will be created under current folder, the name is the answer you
provided to `sqlb-pca`.

Go to this generated folder, the project layout should look like:

```text
.
├── .bumpversion.cfg
├── .editorconfig
├── .github
│   ├── ISSUE_TEMPLATE.md
│   └── workflows
│       ├── dev.yml
│       ├── preview.yml
│       └── release.yml
├── .gitignore
├── .pre-commit-config.yaml
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
├── docs
│   ├── api.md
│   ├── changelog.md
│   ├── contributing.md
│   ├── index.md
│   ├── installation.md
│   └── usage.md
├── makefile
├── mkdocs.yml
├── my_package
│   ├── __init__.py
│   ├── cli.py
│   └── my_package.py
├── pyproject.toml
├── setup.cfg
└── tests
    ├── __init__.py
    └── test_my_package.py

```
