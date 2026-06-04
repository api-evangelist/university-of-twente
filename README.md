# University of Twente (university-of-twente)

The University of Twente (Universiteit Twente, UT) is a public technical research university founded in 1961 in Enschede, Netherlands, ranked #233 in the QS World University Rankings 2025. This repository catalogs the university's publicly confirmable developer and API footprint as an [APIs.json](http://apisjson.org) provider profile. That footprint is modest: a Pure-based research information system documented to offer OAI-PMH harvesting, official GitHub organizations, and participation in the 4TU.ResearchData repository.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-twente/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-twente-api-evangelist&utm_content=repo

## Type

- Type: Index
- Position: Consumer
- Access: 3rd-Party

## Tags

Education, Higher Education, University, Research Data, Netherlands, Open Science

## APIs

- **UT Research Information (Pure) OAI-PMH** — OAI-PMH metadata harvesting endpoint documented for the UT Research Information Pure system (research.utwente.nl). Cataloged on documented evidence only; no live public OAI-PMH endpoint was confirmed at review time. Docs: https://www.utwente.nl/en/service-portal/university-library/publication-archiving/ut-research-information-pure

## Plans, Rate Limits & FinOps

- Plans / Pricing: [plans/university-of-twente-plans-pricing.yml](plans/university-of-twente-plans-pricing.yml)
- Rate Limits: [rate-limits/university-of-twente-rate-limits.yml](rate-limits/university-of-twente-rate-limits.yml)
- FinOps: [finops/university-of-twente-finops.yml](finops/university-of-twente-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.utwente.nl/en/
- GitHub: https://github.com/utwente
- LinkedIn: https://www.linkedin.com/school/university-of-twente/
- SourceCode: https://github.com/utwente-fmt
- Plans: plans/university-of-twente-plans-pricing.yml
- RateLimits: rate-limits/university-of-twente-rate-limits.yml
- FinOps: finops/university-of-twente-finops.yml
- Review: review.yml

## Notes

All entries reflect publicly verifiable information only; no endpoints were fabricated. The official website, the Pure portal (research.utwente.nl), the GitHub org, and the 4TU.ResearchData institution page resolved live (HTTP 200). The Pure OAI-PMH endpoint is documented by the UT library but every OAI base-URL variant probed returned an error/500 (not openly accessible), so it is listed without a baseURL. 4TU.ResearchData (data.4tu.nl) is co-founded by UT but hosted and governed by TU Delft, so it is referenced rather than claimed as a UT-operated API. See [review.yml](review.yml) for per-URL probe results.

## Maintainers

- Kin Lane — kin@apievangelist.com
