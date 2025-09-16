# nova-top-level-docs
=======================

# Introduction

This is the repository for the nova-top-level-docs. This project creates the documentation at https://nova-application-development.readthedocs.io/en/latest


## Formatting
```commandline
poetry run ruff format
```

## Linting
```commandline
poetry run ruff check
poetry run mypy .
```

## Build docs
```commandline
docker build -f dockerfiles/Dockerfile --target source -t image .
docker run -u `id -u`:`id -g` image bash build_docs.sh
```

## CI/CD in GitHub

Take a look at the [`.github/workflows`](.github/workflows) folder.
Actions to lint and test your code will run automatically on each commit.
The action for building and releasing this package needs to be triggered manually.

### Publishing docs to readthedocs.io

This repo has a [webhook](https://github.com/nova-model/nova-docs/settings/hooks) that automatically triggers documentation builds on readthedocs.
