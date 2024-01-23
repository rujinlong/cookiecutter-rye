# Cookiecutter Rye

## Usage

```shell
cookiecutter https://github.com/rujinlong/cookiecutter-rye.git

# assume package name is `myapp`
cd myapp
rye sync
git init && gaa && gcam "init"

# run app (default: `mycli`)
mycli
```

## TODO

- [ ] Fix `makefile` to use `ruff`
- [ ] Fix `-pre-commit-config.yaml` to use `ruff`
- [ ] Add mkdocs config
- [ ] Add docker config
- [ ] Add github actions config

## Features

This tool will create Python project with the following features:

- [Rye](https://rye-up.com/): Manage dependency, build and release
- [Mkdocs](https://www.mkdocs.org): Writing your docs in markdown style
- Testing with [Pytest](https://pytest.org) (unittest is still supported out of the box)
- Code coverage report and endorsed by [Codecov](https://codecov.io)
- [Tox](https://tox.readthedocs.io): Test your code against environment matrix, lint and artifact check
- Format with [Black](https://github.com/psf/black) and [Isort](https://github.com/PyCQA/isort)
- Lint code with [Flake8](https://flake8.pycqa.org) and [Flake8-docstrings](https://pypi.org/project/flake8-docstrings/)
- Check static type with [Mypy](http://mypy-lang.org/) (optional)
- [Pre-commit hooks](https://pre-commit.com/): Formatting/linting anytime when commit your code
- [Mkdocstrings](https://mkdocstrings.github.io/): Auto API doc generation
- Command line interface using [Click](https://click.palletsprojects.com/en/8.0.x/) (optional)
- [bump2version](https://github.com/c4urself/bump2version): Pre-configured version bumping with a single command
- Continuous Integration/Deployment by [GitHub actions](https://github.com/features/actions), includes:
  - publish dev build/official release to TestPyPI/PyPI automatically when CI success
  - publish documents automatically when CI success
  - extract changelog from CHANGELOG and integrate with release notes automatically
- Host your documentation from [GitHub Pages](https://pages.github.com) with zero-config
