# Quarkloop

A universal runtime for programmable nodes — declare systems in TypeScript, execute them across a three-service architecture, and manage everything through autonomous AI workspaces.

## What is Quark?

Quark is a platform where everything — timers, profilers, parsers, writers, endpoints, policies — is a **Node** identified by a Docker-style URI. Users declare nodes and their communication patterns in `.quark.ts` files. The control plane persists these declarations and forwards them to the data plane, where GraalJS evaluates TypeScript node logic natively over NATS.

**Multi-tenant by construction**: NATS subjects encode the namespace. Two tenants can deploy same-named systems simultaneously with zero data leakage.

## Repositories

| Repository | Description |
|---|---|
| [**quark**](https://github.com/quarkloop/quark) | Main platform — three-service architecture (Go control plane + Java/GraalJS data plane + Go Catalog) |
| [**agent**](https://github.com/quarkloop/agent) | Local operating environment for autonomous AI workspaces (supervisor, runtime, plugins, services) |
| [**quark-js**](https://github.com/quarkloop/quark-js) | TypeScript SDK — execute nodes, chain pipelines, browse the catalog |
| [**docs**](https://github.com/quarkloop/docs) | Unified documentation portal — Fuma Docs (Next.js) aggregating markdown from product repos |
| [**guidelines**](https://github.com/quarkloop/guidelines) | Specifications, templates, and tooling for consistent configuration across repos |

---

<div align="center">

**[🌐 quarkloop.com](https://quarkloop.com)** · **[📚 Documentation](https://quarkloop.com/docs)** · **[📋 Guidelines](https://github.com/quarkloop/guidelines)**

</div>
