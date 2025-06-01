# action-black

A composite action that checks file formatting with [black](https://black.readthedocs.io/)

This repository is not meant to be referenced in third-party workflows; please fork the repository if you would like to use it in your project.

## Inputs

| Name              | Description                                       | Default |
| ----------------- | ------------------------------------------------- | ------- |
| cache             | Whether to cache project dependencies.            | "true"  |
| package_manager   | The package manager to use ("poetry" or "uv").    | "uv"    |
| python_version    | The python version to use in SemVer range syntax. | "3.13"  |
| working_directory | The working directory for the action.             | "."     |

## Examples

```
jobs:
  black:
    runs-on: ubuntu-latest
    steps:
      - uses: lojoja/action-black@main
        with:
          cache: "true"
          package_manager: uv
          python_version: "3.13"
```

## License

action-black is released under the [MIT License](./LICENSE)
