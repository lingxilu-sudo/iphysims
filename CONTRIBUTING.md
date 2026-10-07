# Contributing to Iphysims

Thanks for considering a contribution — this project is early, so the bar is "interesting physics, honest code", nothing more.

## Pull requests

1. Fork the repo, create a branch (`feat/your-simulation`, `fix/...`)
2. Commit with a short message saying **what physics / method** the change covers
3. Open a Pull Request; describe what it does and, if it's a simulation, which method it uses
4. By submitting, you agree your contribution is licensed under the project license

## Writing an adapter (main path)

Your simulation stays in your repo. An adapter plugs it into the shared interface:

- expose the simulation's **state**, **step function**, **parameters**, and **observables** per the interface spec
- keep your own license — the adapter only calls your code, it doesn't absorb it
- open a PR adding a row to the registry in README (simulation / method / author / link)

The interface spec draft will be published in this repo (docs/interface-spec.md) once v0.1 lands.

## Good first issues

Issues labeled `good first issue` are picked to be doable in an evening.

## Non-code contributions

Bug reports, doc fixes, and permission to embed your simulation on the website all count.
