# sqlb-pca
Python Clean Architecture for sqlg library
## I. The proposed environment setup
- conda as environment manager
- pypi/pip as package repository and manager 
- Poetry as the dependency manager.

https://ealizadeh.com/blog/guide-to-python-env-pkg-dependency-using-conda-poetry


## II. Environment prepare

### 

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


poetry initial
```
$ poetry init
