# nitpick-style

Nitpick style configuration for python projects

## How to use

### Local

Add the following to `pyproject.toml`. Change the version if needed.

```toml
[tool.nitpick]
style = [
    "https://raw.githubusercontent.com/invian/nitpick/master/nitpick-38.toml",
]
```

### Pre-commit hook

Add the following to `repos` in `.pre-commit-config.yaml`.

```yaml
  - repo: https://github.com/andreoliwa/nitpick
    rev: v0.35.0
    hooks:
      - id: nitpick
```

Now simply run it as a pre-commit hook, or directly via `python -m nitpick`
