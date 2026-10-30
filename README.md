# Learnosity

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Learnosity is an Irish-founded assessment infrastructure company whose APIs are embedded into other companies' learning products rather than sold as a finished platform. The surface is split in two: a family of versioned client-side JavaScript APIs - Items, Assess, Questions, Question Editor, Author, Author Aide, Annotations, Events, Reports, Grading, Rubric Editor and Feedback Aide - that render assessment, authoring, grading and reporting experiences inside a host application, and a server-side Data API for Item bank content, learner sessions, responses, scoring, jobs, reports and consumer administration. Learnosity is explicitly not a REST API: every Data API call is an HTTP POST whose operation is chosen by an `action` parameter, and every request across every API carries an HMAC-SHA256 signed `security` object generated server-side by one of six official SDKs. Versions ship on a dated Long Term Support train (vYYYY.X.LTS) pinned in the URL, with regional endpoints in Virginia, Dublin, Sydney, California and Oregon.

**Areas:** Education · Assessment · EdTech · Learning · Analytics · Content Authoring · Artificial Intelligence · Accessibility · Company

## Learnosity on APIs.io

Everything profiled for Learnosity is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/learnosity/](https://apis.io/providers/learnosity/)** — or go straight to one of the APIs or properties below.

### APIs (12)

- [Learnosity Data API](https://apis.io/apis/learnosity/data-api/) — Server-side JSON API for the Learnosity platform. Endpoint families cover Item bank content (Items, Questions, Features, Activities, Tags, Pools, Templates,…
- [Learnosity Items API](https://apis.io/apis/learnosity/items-api/) — Client-side JavaScript API that renders and runs an assessment from an Activity in the Item bank, handling navigation, save and resume, response storage and…
- [Learnosity Assess API](https://apis.io/apis/learnosity/assess-api/) — The assessment player layer used by Items API in assess rendering mode, drivable directly for bespoke player experiences.
- [Learnosity Questions API](https://apis.io/apis/learnosity/questions-api/) — Renders individual Questions and Features inline without the surrounding assessment player - the lowest-level Learnosity rendering component.
- [Learnosity Author API](https://apis.io/apis/learnosity/author-api/) — Full embeddable authoring environment for browsing, creating and editing Items, Questions, Features and Activities in the Item bank.
- [Learnosity Question Editor API](https://apis.io/apis/learnosity/question-editor-api/) — The single-Question editing widget, embeddable on its own inside a custom authoring UI.
- [Learnosity Reports API](https://apis.io/apis/learnosity/reports-api/) — Renders prebuilt learner and aggregate reports - individual reports, live progress and learner-centric reports - into the host application.
- [Learnosity Events API](https://apis.io/apis/learnosity/events-api/) — Real-time client-side event channel used for live progress monitoring across in-flight assessment sessions.
- [Learnosity Annotations API](https://apis.io/apis/learnosity/annotations-api/) — Adds annotation and markup capability - highlighting, notes - over assessment content.
- [Learnosity Grading API](https://apis.io/apis/learnosity/grading-api/) — Embeddable manual grading UI for scoring learner responses.
- [Learnosity Author Aide API](https://apis.io/apis/learnosity/author-aide-api/) — AI-assisted authoring component for generating and improving assessment content inside the host product.
- [Learnosity Feedback Aide](https://apis.io/apis/learnosity/feedback-aide/) — Embeddable AI scoring and feedback surface for open-response work, exposed through feedbackSession and feedbackSessionUI configuration.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [learnosity](https://apis.io/servers/learnosity/learnosity/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Learnosity Authentication](https://apis.io/security/learnosity/learnosity-authentication/)
- [Learnosity Domain Security](https://apis.io/security/learnosity/learnosity-domain-security/)
- [Learnosity Trust Center](https://apis.io/security/learnosity/learnosity-trust-center/)
- [Learnosity Vulnerability Disclosure](https://apis.io/security/learnosity/learnosity-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Learnosity Plans Pricing](https://apis.io/plans/learnosity/learnosity-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Learnosity Rate Limits](https://apis.io/rate-limits/learnosity/learnosity-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://learnosity.com/)
- [Documentation](https://help.learnosity.com/hc/en-us/categories/16266193425053-Developer-Documentation)
- [Getting started](https://help.learnosity.com/hc/en-us/articles/360000758637-Getting-Started-With-the-Data-API)
- [API reference](https://help.learnosity.com/hc/en-us/categories/16266193425053-Developer-Documentation)
- [Pricing](https://learnosity.com/licenses/)
- [Sign up](https://learnosity.com/contact-sales/)
- [Support](https://learnosity.com/platform/support/)
- [Changelog](https://help.learnosity.com/hc/en-us/articles/19629981258653-Developer-Release-Logs)
- [Blog](https://learnosity.com/edtech-blog/)
- [Security](https://learnosity.com/product-security-policy/)
- [Compliance](https://learnosity.com/platform/security/)
- [Terms of service](https://learnosity.com/terms-of-use/)
- [Privacy policy](https://learnosity.com/privacy-policy/)
- [GitHub](https://github.com/Learnosity)
- [Status](https://status.learnosity.com)

## API Evangelist rating

**Kin Score 57.5** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 6.5 |
| Contract governance | 18.2 |
| Operational transparency | 84.2 |
| Developer ergonomics | 71.4 |
| Access clarity | 92.1 |

**Agent readiness 9.2** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 32.7** — Education & Research

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/learnosity/](https://apis.io/providers/learnosity/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Learnosity: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/learnosity/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
