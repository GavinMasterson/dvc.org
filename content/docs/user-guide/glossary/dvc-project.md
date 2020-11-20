---
name: 'DVC Project'
match:
  [
    'DVC project',
    'DVC projects',
    project,
    projects,
    'DVC repository',
    'DVC repositories',
    repository,
    repositories,
  ]
tooltip: >-
  Initialized by running `dvc init` in the **workspace** (typically a Git
  repository). It will contain the [`.dvc/`
  directory](/doc/user-guide/dvc-files-and-directories), as well as `dvc.yaml`
  and `.dvc` files created with commands such as `dvc add` or `dvc run`.
---

Initialized by running `dvc init` in the **workspace** (typically a Git
repository). It will contain the
[`.dvc/` directory](/doc/user-guide/dvc-files-and-directories), as well as
`dvc.yaml` and `.dvc` files created with commands such as `dvc add` or
`dvc run`.

This page extends for a _while_, elaborating on what a DVC Project is in a way
where it doesn't make sense to put **all** this stuff in a tooltip.