# Python API Quickstart - Kegstand project template

[Kegstand](https://kegstand.dev/) is a free and open-source framework for creating Python APIs and services. It allows you to rapidly build and deploy services on AWS. We all have better things to do than print(json.dumps(event)) all day long, and Kegstand is here to help you get to the party — and into Prod — a lot faster.

This template lets you create a Python API on AWS Lambda / API Gateway with CDK in a matter of minutes.

## Features

- Python 3.12+
- Choice of [uv](https://docs.astral.sh/uv/) or [Poetry](https://python-poetry.org/) for dependency management
- File-based routing
- Decorator-based endpoint definitions
- Public and private endpoints
- Easy authorization integration with an existing Cognito user pool
- Automated deployment with AWS CDK

## Usage

First, create a new project using the Kegstand CLI or Copier:

```shell
# Using the Kegstand CLI
> pipx install kegstandcli
> keg new my-service

# Using Copier
> copier copy -d project_name=my-service gh:JensRoland/kegstand-project-template .
```

This will create a new subfolder, `my-service`, inside the current folder.

Then, to build and deploy your service, run the following commands:

```shell
# Using uv
> cd my-service
> uv run keg deplpy

# Using Poetry
> cd my-service
> poetry install
> poetry run keg deploy
```

## Learn more

Visit the [official Kegstand repo](https://github.com/JensRoland/kegstand) to learn more about the framework and how to use it.
