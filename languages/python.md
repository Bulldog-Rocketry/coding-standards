# Python Guidelines

## Table of Contents

-   [Python Guidelines](#python-guidelines)
    -   [Table of Contents](#table-of-contents)
    -   [Dependencies](#dependencies)
    -   [Formatting](#formatting)
    -   [Documentation](#documentation)
    -   [Testing](#testing)

## Dependencies

-   Store dependencies in a virtual environment (referred to as `venv`)
    -   `python3 -m venv $VENV` where `$VENV` is the name of the virtual environment (typically `venv` or `.venv`)
-   Use the `pip` in the virtual environment to manage dependencies.
-   The `venv` directory should be ignored in the `.gitignore` file.
-   The `requirements.txt` file should be included in the repository.

## Formatting

-   Use [`Black`](https://github.com/psf/black) to format your code.
-   Use [`isort`](https://github.com/PyCQA/isort) to sort your imports.
    -   So that `isort` and `black` don't conflict, run it with `isort --profile black`.
-   Use clean coding practices in accordance with PEP: https://peps.python.org/
-   These can and should all be configured with a `pyproject.toml` - [example](examples/python/pyproject.toml)

## Documentation

-   Docstrings should be used for documentation, PEP 484 covers how to document code with docstrings: https://peps.python.org/pep-0484/
-

## Testing

-   The writing of unit tests may be done with unittest or pytest
-   Coverage can be used to see how well you have written your tests. Its documentation can be found here: https://coverage.readthedocs.io/en/7.2.1/#quick-start
