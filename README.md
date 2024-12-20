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

## CI/CD in GitLab

Take a look at the `.gitlab-ci.yml` file. It configures pipelines to run in [GitLab](https://code.ornl.gov/ndip/project-templates/python/-/pipelines).
Some jobs will run automatically on each commit, jobs to
build packages and Docker images need to be trigerred manually. Don't forget to set versions properly:
in `pyproject.toml` for python package and in `.gitlab-ci.yml` for Docker tag.
