# {{ cookiecutter.project_name }}

## Index
- [Quick Start](#quick_start)
    - [Set up the environment](#environment_setup)
    - [Install new packages](#install_packages)
    - [Auto-generate Project documentation](#generate_docs)

- [Structure Description](#structure_description)
    - [data](#data_directory)
        - [external](#external_data)
        - [final](#final_data)
        - [processed](#processed_data)
        - [raw](#raw_data)

<a name="quick_start"/>

## Quick Start

<a name="environment_setup"/>

### Set up the environment

To set up the environment there are two options:

1. The project is new:
    1. Install [Poetry](https://python-poetry.org/docs/#installation) and initialize git
    2. Set up the environment:
    ```bash
    make setup
    make activate
    ```

2. Project is already created on Git:
    1. Install [Poetry](https://python-poetry.org/docs/#installation)
    2. Set up the environment:
    ```bash
    make install
    make activate
    ```

<a name="install_packages"/>

### Install new packages

To install new PyPI packages, run:
```bash
poetry add <package-name>
```

<a name="generate_docs"/>

### Auto-generate Project documentation

To auto-generate Project documentation for your project, run:

1. To save documentation under the docs folder:
```bash
make docs_save
```

2. To visualize documentation on local server:
    1. Run:
    ```bash
    make docs_view
    ```
    2. Access [Localhost](http://localhost:8080)


<a name="structure_description"/>

## Structure Description

<a name="data_directory"/>

### data
Data folder that includes different directories for different stages of data

<a name="external_data"/>

#### external
Put here external data sources files

<a name="final_data"/>

#### final
Put here model ready data sources 

<a name="processed_data"/>

#### processed
Put here processed data sources

<a name="raw_data"/>

#### raw
Put here raw data sources
