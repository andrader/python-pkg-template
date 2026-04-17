# Python Package Template

A modern, production-ready Python package template using `uv`, `copier`, and `just`.

## Features

- ⚡ **[uv](https://github.com/astral-sh/uv)** for fast dependency management and packaging.
- 🛠 **[just](https://github.com/casey/just)** for automated tasks.
- ✨ **[Ruff](https://github.com/astral-sh/ruff)** for linting and formatting.
- ✅ **[pytest](https://github.com/pytest-dev/pytest)** for testing.
- 🏗 **[hatchling](https://hatch.pypa.io/)** as the build backend.
- 🛠 **Optional Features** (via Copier prompts):
    - **MkDocs** documentation setup with Material theme.
    - **ty** for high-performance type checking.
    - **Python Semantic Release** for automated versioning and changelogs.
    - **GitHub Actions** release workflows.
    - **Typer** CLI entry point boilerplate.

## Usage

To generate a new project from this template, ensure you have `uv` and `copier` installed, then run:

```bash
uvx copier copy https://github.com/andrader/python-pkg-template.git path/to/your-project
```

### Prompts

Copier will ask you several questions to customize your project:

1. **Project Name**: The display name of your project.
2. **Package Name**: The Python package name (slugified).
3. **Description**: A short description of the project.
4. **Author Details**: Your name and email.
5. **Optional Features**: Toggle on/off Documentation, Type Checking, Semantic Release, GitHub Workflows, and CLI setup.

## Development

After generating the project, follow the `CONTRIBUTING.md` instructions within the generated folder to set up your development environment:

```bash
just setup
```

Run all quality checks:

```bash
just qa
```
