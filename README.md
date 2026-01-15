# uq-tree

A decision tree for practitioners needing uncertainty quantification for their deep learning project

## Documentation

The paper is written using Sphinx with Markdown files. The documentation is automatically built and deployed to GitHub Pages.

### Building the Documentation Locally

1. Install Python dependencies:

```bash
pip install -r docs/requirements.txt
```

2. Build the HTML documentation:

```bash
cd docs
make html
```

3. View the documentation by opening `docs/_build/html/index.html` in your browser.

### PDF Generation

The workflow automatically generates a PDF version of the paper from the markdown files. The PDF is available as an artifact in the GitHub Actions workflow runs.

## Development

### Pre-commit Hooks

This repository uses pre-commit hooks for linting and formatting. To set up:

1. Install pre-commit:

```bash
pip install pre-commit
```

2. Install the git hook scripts:

```bash
pre-commit install
```

3. (Optional) Run against all files:

```bash
pre-commit run --all-files
```

The hooks will automatically run on `git commit` and will check:

- Trailing whitespace
- End-of-file fixers
- YAML syntax
- Large files
- Markdown linting and formatting
- Python code formatting (Black)
- Python import sorting (isort)
- Python linting (flake8)

## Contributing

Contributions are welcome! Please ensure that:

1. Pre-commit hooks pass
2. Documentation builds successfully
3. Changes follow the existing structure and style

## License

See [LICENSE](LICENSE) file for details.
