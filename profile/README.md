# WhiteDragon-dev

**Minimal software for the open web.**

WhiteDragon-dev is an open-source organization that develops minimal software on Cloudflare
Workers and Pages: an edge AI worker, a forwarding proxy, an experimental browser, a
community forum, and a non-commercial license. Each project uses few dependencies, requires
no build step, and is small enough to be read in full.

| | |
| --- | --- |
| **Focus** | Edge software |
| **Runtime** | Cloudflare Workers & Pages |
| **Languages** | JavaScript · TypeScript · HTML |
| **Source** | Public on GitHub |

## Projects

The five principal projects maintained by the organization.

### 01 · [webcore](https://github.com/whitedragon-dev/webcore) · Active

A chat assistant that runs entirely on Cloudflare Workers AI. The model answers inside the
same request that serves the page, so there is no separate backend to run, scale or keep
online.

`Workers AI` `JavaScript` `Edge inference`

### 02 · [relay](https://github.com/whitedragon-dev/relay) · Active

A single-file Cloudflare Worker that forwards and rewrites web pages so that they load
through a domain you control, including links, forms, scripts and stylesheets. Intended for
networks on which the open web is not directly reachable.

`Cloudflare Workers` `Proxy` `Single file`

### 03 · [whitedragon-browser](https://github.com/whitedragon-dev/whitedragon-browser) · Experimental

An experimental browser implemented entirely in HTML, with no framework, no bundler and no
installation step.

`HTML` `Experiment` `No build step`

### 04 · [whitedragon-forum](https://github.com/whitedragon-dev/whitedragon-forum) · Live

The community space for the organization, built on git-forums and GitHub Discussions, so
that discussion threads, issues and source code remain in a single location rather than on a
separate platform.

**→ [Open the forum](https://whitedragon-dev.github.io/whitedragon-forum)**

`GitHub Discussions` `git-forums` `Community`

### 05 · [WD-NCL](https://github.com/whitedragon-dev/WD-NCL) · Stable

A non-commercial open-source license written from scratch, incorporating an absolute
liability waiver. Short identifier: WD-NCL v1.0.

`License` `v1.0`

## Approach

Engineering principles.

- **◆ Minimal by default** — A single file is used wherever a single file is sufficient.
  There is no build pipeline, no framework, and no dependency tree requiring continual
  maintenance.
- **■ Edge-first** — All projects target Cloudflare Workers and Pages. Deployment occurs on
  push, no servers require administration, and latency remains low across regions.
- **▲ Open, project by project** — Source code is available to read, run and study.
  Licensing is determined per repository and stated there; no project is covered by
  association.

## WD-NCL v1.0

The White Dragon Non-Commercial License — a custom non-commercial open-source license with
an absolute liability waiver, written from scratch rather than borrowed. It is one of the
projects above, not a blanket policy: it applies only where a repository says so, and it does
not govern the other projects by default.

- ◆ Non-commercial use
- ◆ Source available to read and modify
- ◆ Absolute liability waiver

[Read the full text →](https://github.com/whitedragon-dev/WD-NCL)

## Feedback and contributions

Feedback, bug reports and pull requests are welcome, particularly on the experimental
projects.

[GitHub](https://github.com/whitedragon-dev) ·
[Forum](https://whitedragon-dev.github.io/whitedragon-forum) ·
[License](https://github.com/whitedragon-dev/WD-NCL) ·
[DEV](https://dev.to/whitedragon)

---

Each project is licensed in its own repository.
