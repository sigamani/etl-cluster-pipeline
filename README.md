## What is this repository for?

This is a [Dagster](https://dagster.io/) project scaffolded with [`dagster project scaffold`](https://docs.dagster.io/getting-started/create-new-project).



## Getting started

First, install your Dagster code location as a Python package. By using the --editable flag, pip will install your Python package in ["editable mode"](https://pip.pypa.io/en/latest/topics/local-project-installs/#editable-installs) so that as you develop, local code changes will automatically apply.

```bash
cd src
pip install -e ".[dev]"
```

Then, start the Dagster UI web server:

```bash
cd src
dagster dev
```

Open http://localhost:3000 with your browser to see the project.

You can start writing assets in `src/kraken/assets.py`. The assets are automatically loaded into the Dagster code location as you define them.

## Development


### Adding new Python dependencies

You can specify new Python dependencies in `src/setup.py`.

### Unit testing

Tests are in the `src/kraken_tests` directory and you can run tests using `pytest`:

```bash
pytest
```
