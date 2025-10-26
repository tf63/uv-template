# uv template

This repository provides a template for managing Python environments and dependencies using [uv](https://docs.astral.sh/uv/getting-started/installation/).

| Feature                             | Tool         | Description                                        |
| ----------------------------------- | ------------ | -------------------------------------------------- |
| **Tool Management**                 | `mise`       | Manage development tools and their versions.       |
| **Task Automation**                 | `mise`       | Automate common development tasks.                 |
| **Python Version Management**       | `uv`         | Manage multiple Python versions seamlessly.        |
| **Dependency Management**           | `uv`         | Handle project dependencies efficiently.           |
| **Jupyter Notebook Support**        | `uv`         | Integrate Jupyter notebooks into your workflow.    |
| **Formatter and Linter for Python** | `ruff`       | Ensure code quality with automated linting.        |
| **Formatting for other Languages**  | `prettier`   | Apply consistent code formatting across languages. |
| **Type Checking for Python**        | `mypy`       | Perform static type checking for Python code.      |
| **Git Hooks Management**            | `lefthook`   | Manage and maintain Git hooks easily.              |
| **Git Commit Standardization**      | `commitlint` | Standardize Git commit messages.                   |

## Setup

### Setup mise

Install [mise](https://mise.jdx.dev/getting-started.html)

```shell
curl https://mise.run | sh
```

Install uv and other tools

```shell
mise install
```

### Setup Python and Dependencies

```shell
uv sync
```

## Using uv

### Checking Available Python Versions with uv

```shell
uv python list --all-versions
```

### Specifying a Python Version (refer to `.python-version`)

```shell
uv python pin x.x.x
```

### Installing Python and Dependencies

```shell
uv sync
```

### Running a Python File

```shell
uv run src/sample/main.py
```

### Starting a REPL

```shell
uv run python
```

### Adding Dependencies

```shell
uv add <package>
uv add --dev <package>
```
