# pre-commit-clang-format

A hook for to run [clang-format] on C++ code using [pre-commit].

[clang-format]: https://clang.llvm.org/docs/ClangFormat.html
[pre-commit]: https://pre-commit.com/

## Prerequisites

A [conda] installation must be present on the `PATH` when `pre-commit` installs the hook's
environment.

[conda]: https://docs.conda.io/en/latest/miniconda.html

## Installation

Add the following to `.pre-commit-config.yaml` to use this hook:

    - repo: https://github.com/glotzerlab/pre-commit-clang-format
      rev: main
      hooks:
      - id: clang-format
