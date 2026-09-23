# University of Twente (university-of-twente)

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

The University of Twente (Universiteit Twente, UT) is a public technical research university founded in 1961 in Enschede, Netherlands. This repository catalogs the university's publicly confirmable developer and API footprint as an [APIs.json](http://apisjson.org) provider profile, produced under the API Evangelist **university pipeline**, which settles *who operates* each surface before saving any contract.

Unusually for this cohort, the footprint is neither empty nor borrowed: the university operates **one API of its own**. Everything else here is a relationship — a federation membership, a registry membership, or a tenancy on a vendor platform — and is labelled as such rather than credited as the university's engineering.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-twente/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-twente-api-evangelist&utm_content=repo

## Type

- Type: Index (`x-type: university`, `x-category: Technical University`)
- Position: Provider
- Access: Public

## Tags

University, Higher Education, Education, Technical University, Netherlands, Europe, Open Data, Energy, Sustainability, Research Data, Identity Federation, Student Mobility, Open Science

## Surfaces, by operator

Every entry carries an `x-operator` saying who runs the thing it describes.

### `institution` — the university's own

- **University of Twente Energy API** — a public, unauthenticated REST API on the university's own network (`energyapi.utwente.nl`, 130.89.3.170), publishing an **OpenAPI 3.0.1** contract and a Swagger UI. Serves historical electricity, gas, heat, water and solar metering for **103 named campus resources**, at hour/day/week/month/year resolution back to at least 2019, with a CO2-equivalent mode computed against the Dutch national energy mix. It backs the public Energy Data Platform at `energydata.utwente.nl`. Contract: [openapi/university-of-twente-energy-api-openapi.yml](openapi/university-of-twente-energy-api-openapi.yml) · pristine: [openapi/_original/](openapi/_original/university-of-twente-energy-api-openapi.json)
- **llms.txt programme catalog** — a machine-readable study-programme document at `www.utwente.nl/llms.txt`, addressed at language models. Genuinely institution-served, and genuinely defective: despite being JSON-shaped it is *not valid JSON* (it contains JavaScript block comments), and its bachelor and master arrays are elided rather than populated.

### `federation` — shared by definition, the IdP behind it is theirs

- **SAML 2.0 Identity Provider** — entityID `https://sts.windows.net/723246a1-c3f5-43c5-acdc-43adb404ac4d/`, a Microsoft Entra ID tenant registered in **SURFconext**, the Dutch national research and education federation, carrying the Shibboleth metadata extension `shibmd:Scope utwente.nl`. Both its SAML metadata and its OpenID Connect discovery document are public.

### `registry` — a fact about them, not a contract of theirs

- **Crossref membership** — member 2372, *University Library/University of Twente*, DOI prefix **10.3990**, 599 member DOIs. Also registered in ROR as `https://ror.org/006hf6230`. Deliberately **not** recorded as a DataCite member: the university has no DataCite client of its own.

### `tenant` — their data, the vendor's contract

- **UT Research Information (Elsevier Pure)** — `research.utwente.nl` and `ris.utwente.nl` both CNAME to `utwente-pva.elsevierpure.com`.
- **Canvas LMS (Instructure)** — `canvas.utwente.nl` CNAMEs to `utwente-vanity.instructure.com`; its LTI 1.3 platform JWKS is public.
- **OSIRIS student information system (CACI)** — `osiris.utwente.nl` redirects to `utwente.osiris-student.nl`. The authoritative course catalog and timetable live here, behind a login.
- **4TU.ResearchData** — two named UT scopes, groups 28592 (`utwente.nl`) and 28634 (`student.utwente.nl`), in a repository TU Delft operates.
- **Erasmus Without Paper node** — a live discovery manifest declaring **15 EWP student-mobility APIs**, every endpoint scoped to HEI ID `utwente.nl`, served on a UT hostname from SOP's Mobility-Online platform.

## Artifacts

| | |
|---|---|
| OpenAPI (+ pristine original) | [openapi/](openapi/) |
| JSON Schema (8) | [json-schema/](json-schema/) |
| Examples (probed live) | [examples/](examples/) |
| Spectral ruleset | [rules/](rules/) |
| Vocabulary | [vocabulary/](vocabulary/) |
| JSON-LD context | [json-ld/](json-ld/) |
| Authentication | [authentication/](authentication/) |
| Scopes (evidenced empty set) | [scopes/](scopes/) |
| Errors | [errors/](errors/) |
| Conformance (`education` regime) | [conformance/](conformance/) |
| Lifecycle | [lifecycle/](lifecycle/) |
| Plans / Rate Limits / FinOps | [plans/](plans/) · [rate-limits/](rate-limits/) · [finops/](finops/) |
| Per-URL probe log | [review.yml](review.yml) |

## Domain standards (`education` regime)

Probed, not claimed. Full evidence in [conformance/](conformance/university-of-twente-conformance.yml).

- **saml** ✓ · **shibboleth** ✓ · **lti** ✓ · **crossref** ✓ · **orcid** partial
- **oai-pmh** ✗ · **datacite** ✗ · **scim** ✗ · **oneroster** ✗ · **ed-fi** ✗ · **caliper** ✗ · **qti** ✗

## Timestamps

- Created: 2026-06-03
- Modified: 2026-09-01

## Notes

All entries reflect publicly verifiable information only; no endpoints were fabricated, and no vendor contract is saved under this slug.

**Two corrections were made on 2026-09-01.** First, this repo previously carried a *UT Research Information (Pure) OAI-PMH* entry as the university's only API. Re-probing found no working endpoint — `/ws/oai?verb=Identify` returns 500, `/ws/oai/?verb=Identify` returns 404 — and the library page formerly cited as documenting it no longer mentions OAI-PMH at all. The Pure *relationship* was kept and re-labelled `x-operator: tenant`; the endpoint claim was retired. Second, and in the other direction, the university's only institution-operated API was missing from the profile entirely; it was found from the university's own open-data page and confirmed by the `energydata.utwente.nl` JavaScript bundle, which names the API host and its path template.

**Two defects were measured in the Energy API contract** and are recorded rather than smoothed over: the spec declares RFC 7807 `ProblemDetails` on 400 but the service returns a bespoke `{error, results}` envelope, and `GET /api/Dashboard` is documented as 200 but returned 400 when probed. The contract also declares no `servers[]` and no `operationId` on any operation, and `info.contact` routes readers to the contracted developer rather than to the university.

See [review.yml](review.yml) for per-URL probe results.

## Maintainers

- Kin Lane — kin@apievangelist.com
