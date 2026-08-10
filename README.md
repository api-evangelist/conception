# Conception

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Conception is a Berkeley, California biotechnology company founded in 2018 (originally as Ovid Research) by CEO Matt Krisiloff. It is building in-vitro gametogenesis (IVG) as a clinical therapy — reprogramming a patient's blood cells into induced pluripotent stem cells, then guiding them through primordial germ cell, oogonia and follicle stages inside engineered three-dimensional ovarian organoids until they mature into viable human eggs. In an update published 2026-08-07 the company reported the first fully stem-cell-derived human ovarian follicles containing early oocytes progressing through meiosis. It has raised roughly USD 38 million.

**Conception publishes no API.** It is a wet-lab therapeutic research company, not a software vendor. Its entire public web presence is a two-page Framer marketing site plus an Ashby job board. Every `/.well-known/` path, `/openapi.json`, `/graphql`, `/mcp` and `/llms.txt` returns a genuine 404 on both `conception.bio` and `www.conception.bio`, and no `api.`, `docs.` or `developer.` subdomain resolves in DNS. That negative result is recorded with status codes in `well-known/conception-well-known.yml`.

- Website: https://www.conception.bio/
- Science and updates: https://www.conception.bio/science-and-updates
- Careers: https://jobs.ashbyhq.com/Conception
- Secondary market: https://forgeglobal.com/conception_stock/

### What is in this repo

| Path | What it holds |
|---|---|
| `well-known/conception-well-known.yml` | Full `/.well-known/` + contract-discovery probe record (all misses, with status codes) |
| `packages/conception-packages.yml` | Registry search record — no first-party packages on npm, PyPI, RubyGems, crates.io or Packagist |
| `conformance/conception-conformance.yml` | FDA/ISSCR regime status; API standards recorded as not-applicable |
| `security/conception-domain-security.yml` | TLS/HSTS/DNSSEC/SPF/DMARC probe of conception.bio |
| `llms/conception-llms.txt` | Generated llms.txt profile of the company |
