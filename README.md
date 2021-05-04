# pre-commit-clang-format

A hook for to run [clang-format] on C, C++, CUDA code, and template `inc` files using [pre-commit].

[clang-format]: https://clang.llvm.org/docs/ClangFormat.html
[pre-commit]: https://pre-commit.com/

## Prerequisites

A [conda] installation must be present on the `PATH` when [pre-commit] installs the hook's
environment.

[conda]: https://docs.conda.io/en/latest/miniconda.html

## Installation

Add the following to `.pre-commit-config.yaml` to use this hook:

```yaml
- repo: https://github.com/glotzerlab/pre-commit-clang-format
  rev: v0.0.0
  hooks:
  - id: clang-format
```

You can make [conda] an optional requirement by using the `manual` stage:

```yaml
    stages: [manual]
```

Then developers can opt-in to running [clang-format] with:

```bash
$ pre-commit run --hook-stage manual clang-format
```
