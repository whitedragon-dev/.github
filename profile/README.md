# WhiteDragon-dev

**Minimal software for the open web.**

We build small, single-purpose tools on Cloudflare Workers and Pages — an edge AI worker, a forwarding proxy, a desktop browser, a community forum, and two source-available licenses. Every project favors few dependencies, no build step, and code that's small enough to read in full.

---

## Projects

| Project | What it is |
|---|---|
| [**webcore**](https://github.com/whitedragon-dev/webcore) | A chat assistant that runs entirely on Cloudflare Workers AI. The model answers inside the same request that serves the page — no separate backend to run, scale, or keep online. |
| [**relay**](https://github.com/whitedragon-dev/relay) | A single-file Cloudflare Worker that forwards and rewrites web pages so they load through a domain you control, links and scripts included. For networks on which the open web isn't directly reachable. |
| [**daybreak**](https://github.com/whitedragon-dev/daybreak) | A minimal multi-tab desktop browser built on Electron's `BaseWindow` and `WebContentsView` APIs — a frameless window, a custom tab strip and address bar, and a real registered `daybreak://` protocol. |
| [**whitedragon-forum**](https://github.com/whitedragon-dev/whitedragon-forum) | The community space for the organization, built on git-forums and GitHub Discussions, so threads, issues, and source stay in one place. ([Open the forum](https://whitedragon-dev.github.io/whitedragon-forum)) |
| [**WD-NCL**](https://github.com/whitedragon-dev/WD-NCL) | The White Dragon Non-Commercial License — a non-commercial open-source license written from scratch, with an absolute liability waiver. |
| [**WD-SAL**](https://github.com/whitedragon-dev/WD-SAL) | The White Dragon Source-Available License — adds an explicit patent grant, a no-sublicensing restriction, and a stronger liability disclaimer on top of WD-NCL's terms. |

## Approach

- **Minimal by default** — a single file is used wherever a single file is sufficient. There's no build pipeline, no framework, and no dependency tree requiring continual maintenance.
- **Edge-first** — all projects target Cloudflare Workers and Pages. Deployment occurs on push, no servers require administration, and latency stays low across regions.
- **Open, project by project** — source is available to read, run, and study. Licensing is set per repository and stated there; no project is covered by association with another.

## Licenses

Two licenses are maintained here, [WD-NCL](https://github.com/whitedragon-dev/WD-NCL) and [WD-SAL](https://github.com/whitedragon-dev/WD-SAL). Each applies only where a specific repository states it — neither governs a project by default.

## Feedback and contributions

Feedback, bug reports, and pull requests are welcome, particularly on the experimental projects.

- Browse the organization: [github.com/whitedragon-dev](https://github.com/whitedragon-dev)
- Writing on DEV: [dev.to/whitedragon](https://dev.to/whitedragon)
- Email: [info@whitedragon-dev.com](mailto:info@whitedragon-dev.com)
