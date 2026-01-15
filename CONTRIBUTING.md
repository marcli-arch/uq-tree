# Contributing to UQ Decision Tree

Thank you for your interest in contributing to the UQ Decision Tree project!

## Getting Started

### Prerequisites

- Python 3.8 or higher
- Git
- (Optional) pandoc and LaTeX for local PDF generation

### Setting Up Your Development Environment

1. Clone the repository:

```bash
git clone https://github.com/thawn/uq-tree.git
cd uq-tree
```

2. Install Python dependencies:

```bash
pip install -r docs/requirements.txt
```

3. Install pre-commit hooks:

```bash
pip install pre-commit
pre-commit install
```

## Working with Documentation

### Building HTML Documentation

To build the Sphinx documentation locally:

```bash
cd docs
make html
```

View the documentation by opening `docs/_build/html/index.html` in your browser.

### Markdown Files

The paper content is organized into separate markdown files in the `docs/` directory:

- `introduction.md` - Background and motivation
- `methodology.md` - Approach and decision factors
- `decision-tree.md` - Core decision tree framework
- `case-studies.md` - Real-world examples
- `conclusions.md` - Summary and future work
- `references.md` - Bibliography and resources

### Editing Content

When editing markdown files:

1. Use clear, concise language
2. Follow the existing structure and style
3. Add citations where appropriate
4. Test that the documentation builds successfully
5. Run pre-commit hooks before committing

## Pre-commit Hooks

Pre-commit hooks automatically run checks when you commit:

- Trailing whitespace removal
- End-of-file fixing
- YAML syntax checking
- Markdown linting
- Python code formatting (Black)
- Python import sorting (isort)
- Python linting (flake8)

To manually run all hooks:

```bash
pre-commit run --all-files
```

## GitHub Workflows

### Documentation Deployment

The `.github/workflows/docs.yml` workflow automatically:

1. Builds the Sphinx documentation
2. Deploys to GitHub Pages (on main branch)
3. Runs on every push and pull request

### PDF Generation

The `.github/workflows/pdf.yml` workflow automatically:

1. Combines all markdown files
2. Converts to LaTeX using pandoc
3. Generates a PDF
4. Stores LaTeX and PDF as artifacts

Artifacts can be downloaded from the GitHub Actions workflow run page.

## Submitting Changes

1. Create a new branch for your changes
2. Make your edits
3. Ensure all pre-commit hooks pass
4. Test that documentation builds successfully
5. Commit your changes with a descriptive message
6. Push to your branch and create a pull request

### Pull Request Guidelines

- Provide a clear description of your changes
- Reference any related issues
- Ensure all CI checks pass
- Be responsive to feedback

## Code of Conduct

- Be respectful and inclusive
- Focus on constructive feedback
- Help create a welcoming environment

## Questions?

If you have questions or need help, please:

1. Check the README.md
2. Review existing issues
3. Open a new issue if needed

Thank you for contributing!
