# LaughingJackalope

> I'm not an enterprising man, I'm an enterprise, man.

Platform engineering looks chaotic from the outside because it is — deliberately. The job is to absorb complexity so researchers and product engineers don't have to. Every weird half-finished repo here is a load-bearing wall in something larger.

I build the substrate: GPU compute platforms, inference gateways, agent scaffolding, GitOps pipelines. The things that make other things possible. If it looks like a junk drawer, you're reading the inside of the engine.

---

## anchor project

### [skyhook](https://github.com/LaughingJackalope/skyhook)
GPU compute-as-a-service on EKS — Karpenter autoprovisioning, EFA for multi-node training, FSx for Lustre with NVMe caching, SkyPilot interface, Flux GitOps. Built so ML researchers can submit a job without knowing what a NodePool is.

---

## also in the engine room

| repo | what it is |
|------|-----------|
| [inferenceGateway](https://github.com/LaughingJackalope/inferenceGateway) | Swift-native inference in a small package |
| [actions-patterns](https://github.com/LaughingJackalope/actions-patterns) | GitHub Actions cookbook — reusable patterns for situations I keep hitting *(coming soon)* |
| [flink-agents](https://github.com/LaughingJackalope/flink-agents) | Working with the Apache Flink agentic AI framework. Part of a larger distributed agent runtime being built in the open. |

---

## what I write about

Platform trickery at [laughingjackalope.github.io](https://laughingjackalope.github.io) — the Karpenter edge cases, the SOCI lazy-loading wins, the things that only make sense after you've been paged at 2am. Also weird esoterics. The two are more related than they appear.
