# WhiteDragon-dev

**Small, sharp tools for the open web.**

WhiteDragon-dev builds minimal software on Cloudflare Workers and Pages — edge AI, a
forwarding proxy, an experimental browser, a community forum, and a license of its own.
Few dependencies, no build steps, readable in one sitting.

| | |
| --- | --- |
| **Focus** | Edge software |
| **Runtime** | Cloudflare Workers & Pages |
| **Languages** | JavaScript · TypeScript · HTML |
| **Source** | Public on GitHub |

## Projects

Five things worth looking at.

### 01 · [webcore](https://github.com/whitedragon-dev/webcore) · Active

An AI chat worker built directly on Cloudflare Workers AI. Inference happens in the same
request that serves the response — no origin server, no queue, nothing to keep alive
between messages.

`Workers AI` `JavaScript` `Edge inference`

### 02 · [relay](https://github.com/whitedragon-dev/relay) · Active

A single-file Cloudflare Worker that forwards and rewrites web pages so they load through
your own domain — links, forms, scripts and stylesheets included. Built for networks where
the open web is not reachable directly.

`Cloudflare Workers` `Proxy` `Single file`

### 03 · [whitedragon-browser](https://github.com/whitedragon-dev/whitedragon-browser) · Experimental

An experimental browser written in pure HTML. The constraint is the point: how much of a
real browsing surface can exist with no framework, no bundler, and no install step?

`HTML` `Experiment` `No build step`

### 04 · [whitedragon-forum](https://github.com/whitedragon-dev/whitedragon-forum) · Live

The community space for the organization, built on git-forums and GitHub Discussions — so
threads, issues and code all live in the same place instead of a separate platform.

**→ [Open the forum](https://whitedragon-dev.github.io/whitedragon-forum)**

`GitHub Discussions` `git-forums` `Community`

### 05 · [WD-NCL](https://github.com/whitedragon-dev/WD-NCL) · Stable

A non-commercial open-source license written from scratch, with an absolute liability
waiver. Short identifier: WD-NCL v1.0.

`License` `v1.0`

## Approach

- **◆ Minimal by default** — One file when one file will do. No build pipeline, no
  framework, no dependency tree to rot over a weekend.
- **■ Edge-first** — Everything targets Cloudflare Workers and Pages. Deploys are a push,
  there are no servers to babysit, and latency stays low everywhere.
- **▲ Open, project by project** — Source is there to read, run and learn from. Licensing
  is decided per repository and stated there — nothing is covered by association.

## WD-NCL v1.0

The White Dragon Non-Commercial License — a custom non-commercial open-source license with
an absolute liability waiver, written from scratch rather than borrowed.

It is one of the projects above, not a blanket policy: it applies only where a repository
says so, and it does not govern the other projects by default.

- ◆ Non-commercial use
- ◆ Source available to read and modify
- ◆ Absolute liability waiver

[Read the full text →](https://github.com/whitedragon-dev/WD-NCL)

## Poke around. Open an issue.

Blunt feedback, bug reports and pull requests are all welcome — especially on the
experimental things.

[GitHub](https://github.com/whitedragon-dev) ·
[Forum](https://whitedragon-dev.github.io/whitedragon-forum) ·
[License](https://github.com/whitedragon-dev/WD-NCL) ·
[DEV](https://dev.to/whitedragon)

---

Each project is licensed in its own repository.
