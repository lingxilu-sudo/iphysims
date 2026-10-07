# Iphysims

**One interface, all physics.**

Iphysims is a non-profit, open-source project for physics simulations — free to use, no ads, no paid tier.

## The problem

Physics engines are everywhere — finite element, Monte Carlo, molecular dynamics, real-time rigid-body solvers. They often compute the same physics, yet they don't talk to each other. There is no shared way for a fluid solver to hand its state to a particle system, or for two engines to verify each other on the same setup.

## The idea

One shared interface, so simulations built on different methods can **call** and **verify** each other:

- **Call** — a simulation exposes its state, step, and parameters through a common spec, so other tools can drive it or feed it.
- **Verify** — run the same system through two engines built on different methods and compare. Agreement is evidence; disagreement means one of them has a bug worth finding.

## Roadmap

- [ ] v0.1 interface spec draft (state / step / parameters / observables)
- [ ] first adapters from founding builders (fluid / particles / rigid body)
- [ ] cross-verification demo: one system, two engines, side by side
- [ ] public registry of connected simulations
- [ ] long-term: grow into an international non-profit community

## Ways to join

| Path | What it means |
|---|---|
| Founding builder | Shape the first interface spec; your simulation and repo link go on the contributor wall |
| Adapter (main path) | Your simulation stays in your repo — write an adapter that plugs it into the interface; we list it in the registry |
| Code contributor | Fork → branch → pull request (see CONTRIBUTING.md) |
| No code | Open issues, improve docs, or authorize embedding your simulation on the website |

## Registry of connected simulations

| Simulation | Method | Author | Link |
|---|---|---|---|
| *empty — yours could be first* | | | |

## Contact

The fastest way to reach us: open an issue or start a GitHub Discussion on this repo.

---

中文说明（给从小红书来的朋友）：Iphysims 是一个非营利开源物理模拟项目——不收费、不放广告、不设付费版。我们在给散落的各种物理引擎做一个统一接口，让不同方法的模拟互相调用、互相验证。想加入：看上方 Ways to join，或直接提 issue。
