# Repository for template to use Binder and DataLad together via GitHub - from OpenMR Virtual 2021 

## View this example

To open the Jupyter Notebook in a Binder environment (set up using https://mybinder.org) click the following link:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/marianne-aspbury/openmr2021-dataviz-workshop-python/HEAD)

By doing so, everything will be set up for you, without having to worry about
things such as package dependencies. You can start working on the tutorial
notebook right away! :smile:


## How to Set up

### Create virtual environment with conda

The first time

```
conda env create -n dataviz_python -f ./binder/environment.yml
```

To update the environment after changes were made to `./binder/environment.yml`

```
conda env update -n dataviz_pythonv -f ./binder/environment.yml
```

## Download the required data locally

<!-- TODO add more datalad set-up instruction -->

For this example, we are using the fact that the openneuro datasets can be accessed through their siblings on github:

https://github.com/OpenNeuroDatasets

For more info see the handbook:
http://handbook.datalad.org/en/latest/basics/101-180-FAQ.html#how-does-datalad-interface-with-openneuro

```bash
datalad clone https://github.com/OpenNeuroDatasets/ds003542.git inputs/ds003542/
datalad get inputs/ds003542/sub-01/func/sub-01_task-compL1_run-1*
datalad get inputs/ds003542/sub-01/anat/
```
## Instructions on setting-up a binder

<!-- TODO add binder set-up instruction -->
