# PARC 2026 Documentation

This is the documentation repository for the PARC 2026 project. The documentation is written in Markdown and is built using [MkDocs](https://www.mkdocs.org/).

## Installation

### Create Python Virtual Environment

A [Python virtual environment](https://www.geeksforgeeks.org/python/create-virtual-environment-using-venv-python/) enables one to create a space where packages can be installed and managed, without affecting other Python projects on the system that might have different dependencies or package versions.

Install the `venv` Python module used to setup a virtual environment by running this command:

```bash
sudo apt install python3-venv
```

Create a virtual environment called `.venv` (the name is arbitrary) with the following command:

```bash
python3 -m venv .venv
```

Activate the virtual environment

```bash
source .venv/bin/activate
```

***Note:***
*To deactivate the virtual environment, simply run the command, `deactivate`, in the terminal.*

### Install dependencies

With the virtual environment setup, the dependencies for the documentation are installed using the following command:

```bash
pip install -r requirements.txt
```

***Note:*** *The Python package tool, `pip`, is installed automatically when `venv` is installed.*

## Building the documentation

To build the documentation, run the following command:

```bash
mkdocs build
```

***Note:*** *The virtual environment might have to be sourced again if any there are issues encountered when building the documentation.*

## Serving the documentation locally

To serve the documentation locally, run the following command:

```bash
mkdocs serve
```

***Note:*** *Similarly, reactivate the virtual environment if there are any issues encountered when serving the documentation.*

## Deploying the documentation

To deploy the documentation, run the following command:

```bash
mkdocs gh-deploy
```
