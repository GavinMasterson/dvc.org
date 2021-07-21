## Experiments

`dvc exp` commands let you automatically track a variation to an established
[data pipeline](/doc/command-reference/dag). You can create multiple isolated
experiments this way, as well as review, compare, and restore them later, or
roll back to the baseline. The basic workflow goes like this:

- Modify stage <abbr>parameters</abbr> or other dependencies (e.g. input data,
  source code) of committed stages.
- Use `dvc exp run` (instead of `repro`) to execute the pipeline. The results
  are reflected in your <abbr>workspace</abbr>, and tracked automatically.
- Use [metrics](/doc/command-reference/metrics) to identify the best
  experiment(s).
- Visualize, compare experiments with `dvc exp show` or `dvc exp diff`. Repeat
  🔄
- Use `dvc exp apply` to roll back to the best one.
- Make the selected experiment persistent by committing its results to Git. This
  cleans the slate so you can repeat the process.
