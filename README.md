# Cookie Cutter Extension

Cloud AI Platform Notebooks JupyterLab extension cookie cutter project

## Prerequisites

* Python 3.5+
* [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html)
* [Virtualenv](https://virtualenv.pypa.io/en/latest/) (Recommended for local development)
* [NPM](https://nodejs.org/en/) (For local development)

## Quick Start

Install [cookiecutter](https://pypi.org/project/cookiecutter/):

```bash
pip install cookiecutter
```

Generate a new extension from the template. Press enter at each of the prompts to accept the default value or add the `--no-input` flag:

```bash
cookiecutter https://github.com/gclouduniverse/jupyterlab_cookiecutter -o my_extension
```

Change to the generated project directory:

```bash
cd my_extension/jupyterlab_cookiecutter # Change this to the generated project directory
```

To build, install, and launch run:

```bash
virtualenv -p python3 venv && \
source venv/bin/activate && \
pip install . && \
npm install && \
jupyter labextension install . --no-build && \
jupyter lab build && \
npm start
```
