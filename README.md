# grid1q

This is a Python 3.12 app called grid1q. The project includes Docker, Pyright, Ruff, GitHub Actions, Black, pre-commit, and Sphinx.

## Project Structure

The project structure is as follows:

```sh
grid1q
├── .dockerignore
├── .github
│   └── workflows
│       └── python-app.yml
├── .gitignore
├── .pre-commit-config.yaml
├── Dockerfile
├── Makefile
├── README.md
├── docs
│   ├── Makefile
│   └── source
│       ├── conf.py
│       └── index.rst
├── pyproject.toml
├── grid1q
│   ├── __init__.py
│   ├── main.py
│   └── utils.py
├── requirements.txt
├── ruff.toml
└── tests
    ├── test_main.py
    └── test_utils.py
```

The source code is located in the `grid1q` folder, which contains the `__init__.py`, `main.py`, and `utils.py` files. The tests are located in the `tests` folder, which contains the `test_main.py` and `test_utils.py` files.

The project uses toml for configuration instead of `setup.py`. The configuration file is located in `pyproject.toml`.

The project includes Docker, with a `Dockerfile` located in the root directory. The `.dockerignore` file is also located in the root directory.

The project includes Pyright for static type checking, pre-commit for code formatting, Black for code formatting and Ruff for linting. The configuration for these tools is located in the `.pre-commit-config.yaml` and `ruff.toml` files.

The project includes Sphinx for documentation, with the documentation located in the `docs` folder. The `source/conf.py` file contains the configuration for Sphinx.

The project includes GitHub Actions for continuous integration, with the configuration located in the `.github/workflows/python-app.yml` file.

## Installation

To install the project, clone the repository and run:

```sh
python3.12 -m venv .venv
source .venv/bin/activate
pip install -U pip setuptools
pip install -r requirements.txt
pre-commit install
```

Then install the project using:

```sh
pip install -e .
```

See `Makefile` for other useful commands.

## Testing

Just issue `pytest` from the root directory.
