# Contributing to WhiteDragon-dev

Thank you for your interest in contributing to WhiteDragon-dev.

WhiteDragon-dev develops minimal software for the open web. Our projects are intentionally small, focused, and designed to remain understandable without unnecessary frameworks, build systems, services, or dependency trees.

Contributions are welcome when they improve a project while preserving these principles.

---

## 1. Scope

This document provides the general contribution guidelines for repositories maintained by WhiteDragon-dev.

Individual repositories may contain additional contribution instructions specific to that project. Where repository-specific instructions exist, they take precedence for work within that repository.

Before contributing, please read:

- the repository's `README.md`;
- the repository's license;
- any repository-specific documentation or development instructions;
- the WhiteDragon-dev `CODE_OF_CONDUCT.md`;
- the WhiteDragon-dev `SECURITY.md` when your contribution involves security-sensitive functionality.

The absence of a project-specific document does not remove the general standards described here.

---

## 2. What We Value

Contributions should generally support the following principles.

### 2.1 Minimal by default

Prefer the smallest implementation that correctly solves the problem.

Avoid adding:

- frameworks where platform APIs are sufficient;
- dependencies where a small local implementation is reasonable;
- build systems where source can be deployed directly;
- abstractions that do not solve a demonstrated problem;
- configuration that exists only for convention.

Complexity should have a reason.

### 2.2 Readable source

Code should remain understandable to someone reading the project for the first time.

Prefer:

- straightforward control flow;
- descriptive names;
- small, comprehensible files;
- comments that explain why rather than restating what code does;
- platform-native APIs where practical.

Do not optimize for cleverness at the expense of clarity.

### 2.3 Project independence

WhiteDragon-dev maintains multiple projects with different purposes and licenses.

Do not assume that a policy, dependency, license, architecture, or implementation detail from one repository automatically applies to another.

Each project should remain understandable and maintainable on its own terms.

### 2.4 Open development

Issues, discussions, and pull requests should contain enough context for another contributor to understand what is being proposed and why.

Where practical, design decisions should be discussed openly rather than made through private communication.

### 2.5 Security and responsible operation

Contributions must not knowingly introduce unnecessary security, privacy, reliability, or operational risks.

Security vulnerabilities should **not** be disclosed through public issues or pull requests. Follow `SECURITY.md` for security-sensitive reports.

---

## 3. Before You Start

For substantial changes, please open an issue or discussion before beginning implementation.

This is especially useful for:

- architectural changes;
- new features;
- changes affecting multiple repositories;
- changes to public behavior or interfaces;
- changes to licensing;
- changes that introduce a new dependency;
- changes that materially increase project complexity.

Small fixes do not necessarily require prior discussion.

Examples include:

- correcting a typo;
- fixing an obvious bug;
- improving documentation;
- correcting an existing test;
- making a narrowly scoped compatibility fix.

Opening an issue first does not guarantee that a proposed change will be accepted. It provides an opportunity to establish whether the change fits the project's direction before significant work is undertaken.

---

## 4. Finding Work

Issues and discussions are the primary places to identify work that is suitable for public contribution.

When selecting an issue, consider whether:

1. the issue is still relevant;
2. it has not already been assigned or actively addressed;
3. the proposed solution is consistent with the project's existing design;
4. the change can be implemented without unnecessary complexity.

If you intend to work on a larger issue, leave a comment indicating that you are working on it when appropriate. This helps prevent duplicated effort.

---

## 5. Making Changes

Keep changes focused.

A pull request should normally address one coherent problem or improvement. Avoid combining unrelated refactoring, formatting changes, dependency changes, or feature work with an otherwise focused fix.

### 5.1 Preserve existing behavior

Unless a change intentionally modifies behavior, existing functionality should continue to work.

When changing behavior intentionally, document:

- what changes;
- why it changes;
- what users should expect afterward;
- any compatibility implications.

### 5.2 Avoid unnecessary dependencies

Before adding a dependency, consider whether the requirement can reasonably be met using:

- the language standard library;
- the runtime;
- browser APIs;
- Cloudflare APIs;
- Electron APIs;
- existing project code.

A dependency should provide sufficient value to justify its maintenance, security, size, and operational cost.

### 5.3 Respect the project's architecture

Do not introduce a new architectural layer merely because it is common in other projects.

For example, projects intentionally designed around a single Worker file or direct deployment should not acquire a framework or build pipeline without a clear technical reason.

### 5.4 Preserve deployment simplicity

Where a project is designed for direct deployment, contributions should preserve that property unless there is a documented reason to change it.

For Cloudflare projects, contributors should understand the project's Workers/Pages configuration and test deployment-sensitive changes appropriately.

For desktop projects, contributors should follow the project's existing Electron architecture and platform requirements.

---

## 6. Local Development

Each repository is responsible for documenting its own development and deployment requirements.

Before submitting a pull request:

1. install only the dependencies required by the project;
2. run the project's documented development workflow;
3. test the affected functionality;
4. run available automated checks;
5. review the final diff for unrelated changes;
6. remove local configuration, credentials, generated files, and debugging code that should not be committed.

If a project intentionally has no build step, do not introduce one merely to satisfy a conventional workflow.

---

## 7. Testing

Changes should be tested to an extent appropriate to their risk and scope.

At minimum, contributors should verify the behavior directly affected by their change.

For changes involving:

- routing;
- persistence;
- authentication or authorization;
- security;
- network requests;
- AI or model interaction;
- browser behavior;
- desktop navigation;
- deployment;
- database behavior;

additional testing should be performed where practical.

If a project provides a testing checklist, use it.

When automated tests do not exist, describe the manual verification performed in the pull request.

---

## 8. Documentation

Documentation is part of a contribution, not an afterthought.

Update relevant documentation when a change affects:

- installation;
- configuration;
- usage;
- commands;
- public behavior;
- APIs;
- deployment;
- limitations;
- supported platforms;
- security considerations.

Documentation should be concise and accurate.

Do not document functionality that does not actually exist.

---

## 9. Commit Practices

Use clear, descriptive commit messages.

A commit should describe the change it introduces rather than the process used to create it.

Examples:

```text
Fix conversation branch restoration
```

```text
Add mobile navigation handling
```

```text
Document local Worker configuration
```

Avoid commit messages that provide little information, such as:

```text
update
```

```text
changes
```

```text
fix stuff
```

Contributors may use whatever reasonable local Git workflow they prefer. Pull requests should ultimately present a coherent and reviewable set of changes.

---

## 10. Pull Requests

Pull requests should explain the change sufficiently for a maintainer to review it without reconstructing the author's intent.

A useful pull request normally includes:

- a concise description of the problem;
- a summary of the solution;
- relevant implementation details;
- testing performed;
- known limitations or follow-up work;
- links to related issues or discussions, when applicable.

For larger changes, explain important design decisions and alternatives considered.

### Pull request checklist

Before requesting review, confirm that:

- [ ] the change addresses a defined problem or useful improvement;
- [ ] the implementation is appropriately scoped;
- [ ] existing functionality has been considered;
- [ ] relevant tests or manual checks have been performed;
- [ ] documentation has been updated where necessary;
- [ ] no secrets or credentials are included;
- [ ] unrelated changes have been removed;
- [ ] the repository's license and existing project conventions have been respected.

---

## 11. Review

Pull requests are reviewed based on the needs and direction of the affected project.

Review may consider:

- correctness;
- security;
- maintainability;
- readability;
- compatibility;
- performance;
- operational simplicity;
- dependency impact;
- consistency with project goals;
- documentation and testing.

Review comments are intended to improve the contribution and the project.

Contributors are expected to respond to review comments constructively. Maintainers may request changes, ask for additional information, or decline a contribution when it does not fit the project's direction.

Approval of a pull request does not imply that every implementation detail is preferred indefinitely. Maintainers may revise implementation decisions as the project evolves.

---

## 12. Changes to Scope

A contribution may be declined or deferred when it would:

- substantially increase unnecessary complexity;
- introduce an avoidable dependency;
- duplicate functionality already present;
- conflict with the project's stated purpose;
- create disproportionate maintenance requirements;
- introduce unacceptable security or privacy risks;
- require infrastructure that is inconsistent with the project's design;
- change licensing or legal terms without appropriate consideration.

A technically functional change is not necessarily an appropriate change for a particular project.

---

## 13. Dependencies

New dependencies require particular care.

When proposing a dependency, contributors should consider:

- whether it is necessary;
- whether an existing platform capability can replace it;
- maintenance activity;
- license compatibility;
- security history;
- package size and runtime impact;
- transitive dependencies;
- long-term maintenance cost.

A pull request introducing a dependency should explain why the dependency is justified when the reason is not self-evident.

---

## 14. Licensing

WhiteDragon-dev does not apply one license to every repository by association.

Each project is licensed according to the license explicitly stated in that repository.

WhiteDragon-dev maintains the following licenses as separate projects:

- **WD-NCL â€” White Dragon Non-Commercial License**
- **WD-SAL â€” White Dragon Source-Available License**

The existence of these licenses does not cause them to apply automatically to other WhiteDragon-dev repositories.

Contributors must review the license of the repository to which they are contributing and must not assume that another WhiteDragon-dev project has the same licensing terms.

If a proposed contribution raises a material licensing or copyright question, discuss it with the maintainers before submitting the contribution.

---

## 15. Copyright and Third-Party Material

Do not submit code, documentation, assets, or other material that you do not have the right to contribute.

Contributors are responsible for ensuring that third-party material is appropriately licensed and attributed where required.

Do not copy substantial portions of code from another project into a WhiteDragon-dev repository without verifying that its license permits the intended use.

If licensing is unclear, raise the issue before submitting the material.

---

## 16. Security-Sensitive Contributions

Do not disclose security vulnerabilities through public issues, discussions, or pull requests.

If you discover a potential vulnerability, follow the reporting procedure in `SECURITY.md`.

Security-sensitive changes should receive appropriate review before being merged.

Examples include changes involving:

- authentication;
- authorization;
- secrets;
- credentials;
- user data;
- database access;
- network proxying;
- external requests;
- HTML or script rewriting;
- command execution;
- sandbox boundaries;
- browser security;
- content isolation.

---

## 17. Community Conduct

All contributors, maintainers, reviewers, and participants are expected to follow the WhiteDragon-dev `CODE_OF_CONDUCT.md`.

Technical disagreement is acceptable and often useful. Personal attacks, harassment, intimidation, discrimination, or other conduct prohibited by the Code of Conduct is not.

Technical criticism should address the implementation, proposal, or idea rather than the person making it.

---

## 18. Maintainer Discretion

Maintainers are responsible for protecting the project's purpose, quality, security, and long-term maintainability.

Maintainers may:

- request changes;
- ask for additional testing;
- close duplicate or obsolete issues;
- defer proposals;
- decline changes that do not fit the project;
- prioritize work according to project needs;
- modify implementation details during review;
- archive or discontinue projects when appropriate.

Maintainer decisions should be exercised consistently with the project's documentation and the WhiteDragon-dev governance framework.

For organization-level questions concerning authority, project ownership, or decision-making, refer to `GOVERNANCE.md`.

---

## 19. Becoming a Maintainer

Contributing to a project does not automatically grant maintainer access.

Maintainer responsibilities require demonstrated familiarity with the relevant project, its architecture, its operational requirements, and its community standards.

Maintainer appointments and permissions are governed by the WhiteDragon-dev governance process.

Details concerning current maintainers and project ownership are maintained separately in `MAINTAINERS.md`.

---

## 20. Questions and General Discussion

For general questions, project discussion, ideas, and non-sensitive feedback, use the appropriate public GitHub issue or discussion area.

WhiteDragon-dev also maintains a community forum through the `whitedragon-forum` project.

For general organizational contact, the public organization contact address is:

**info@whitedragon-dev.com**

Do not use public issues or discussions to disclose private information, credentials, security vulnerabilities, or other sensitive material.

---

## 21. Final Principle

The goal of contribution is not simply to add more code.

A successful contribution should leave the project clearer, more useful, more reliable, or easier to maintain without adding complexity that the project does not need.

When in doubt:

> Prefer the smallest clear solution that solves the real problem.

Thank you for contributing to WhiteDragon-dev.
