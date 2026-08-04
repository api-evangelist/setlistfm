# setlist.fm (setlistfm)

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

setlist.fm is the world's largest crowd-sourced concert setlist database and community, letting fans document, share, and explore which songs artists play at live shows. The setlist.fm REST API gives read-only access to that data - artists (keyed by MusicBrainz MBID), setlists and their revision history, venues, cities, and countries, plus full-text search across each - so developers can build music apps, tour trackers, and research tools. setlist.fm is owned by Live Nation Entertainment through its Ticketmaster subsidiary. The API is free for non-commercial use with an API key sent in the `x-api-key` header; commercial use requires contacting setlist.fm.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/apis.yml)

## Tags

- Music
- Concerts
- Setlists
- Live Music
- Database
- Crowd-Sourced
- Entertainment

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### setlist.fm Artists API

Look up an artist by their MusicBrainz identifier (MBID) and page through every setlist attributed to that artist. Artists are the primary entry point for exploring a performer's live performance history on setlist.fm.

- **Human URL:** [https://api.setlist.fm/docs/1.0/index.html](https://api.setlist.fm/docs/1.0/index.html)
- **Base URL:** `https://api.setlist.fm/rest/1.0`

#### Tags

- Artists
- MusicBrainz
- Setlists

#### Properties

- [Documentation](https://api.setlist.fm/docs/1.0/index.html)
- [API Reference](https://api.setlist.fm/docs/1.0/resource__1.0_artist__mbid_.html)
- [OpenAPI](openapi/setlistfm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/setlistfm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/setlistfm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### setlist.fm Setlists API

Retrieve a single concert setlist by its ID - the ordered songs, sets, encores, tour, artist, and venue - or fetch a specific historical revision of a setlist by its version ID, since setlists are crowd-edited over time.

- **Human URL:** [https://api.setlist.fm/docs/1.0/index.html](https://api.setlist.fm/docs/1.0/index.html)
- **Base URL:** `https://api.setlist.fm/rest/1.0`

#### Tags

- Setlists
- Versions
- Concerts

#### Properties

- [Documentation](https://api.setlist.fm/docs/1.0/index.html)
- [API Reference](https://api.setlist.fm/docs/1.0/resource__1.0_setlist__setlistId_.html)
- [OpenAPI](openapi/setlistfm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/setlistfm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/setlistfm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### setlist.fm Venues API

Look up a venue by its setlist.fm venue ID and page through all setlists performed at that venue. Venues carry the city, and through the city the state, country, and geo-coordinates where each show took place.

- **Human URL:** [https://api.setlist.fm/docs/1.0/index.html](https://api.setlist.fm/docs/1.0/index.html)
- **Base URL:** `https://api.setlist.fm/rest/1.0`

#### Tags

- Venues
- Locations
- Setlists

#### Properties

- [Documentation](https://api.setlist.fm/docs/1.0/index.html)
- [API Reference](https://api.setlist.fm/docs/1.0/resource__1.0_venue__venueId_.html)
- [OpenAPI](openapi/setlistfm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/setlistfm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/setlistfm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### setlist.fm Cities API

Resolve a city by its GeoNames geoId to get its name, state, country, and latitude/longitude. Most of setlist.fm's city data originates from Geonames.org and is the geographic backbone behind venues and setlists.

- **Human URL:** [https://api.setlist.fm/docs/1.0/index.html](https://api.setlist.fm/docs/1.0/index.html)
- **Base URL:** `https://api.setlist.fm/rest/1.0`

#### Tags

- Cities
- Geo
- Geonames

#### Properties

- [Documentation](https://api.setlist.fm/docs/1.0/index.html)
- [API Reference](https://api.setlist.fm/docs/1.0/resource__1.0_city__geoId_.html)
- [OpenAPI](openapi/setlistfm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/setlistfm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/setlistfm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### setlist.fm Countries API

Return the complete list of countries setlist.fm knows about, each with its ISO country code and localized name. This is the reference set used to constrain and interpret geographic filters elsewhere in the API.

- **Human URL:** [https://api.setlist.fm/docs/1.0/index.html](https://api.setlist.fm/docs/1.0/index.html)
- **Base URL:** `https://api.setlist.fm/rest/1.0`

#### Tags

- Countries
- Reference Data
- Geo

#### Properties

- [Documentation](https://api.setlist.fm/docs/1.0/index.html)
- [API Reference](https://api.setlist.fm/docs/1.0/resource__1.0_search_countries.html)
- [OpenAPI](openapi/setlistfm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/setlistfm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/setlistfm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### setlist.fm Search API

Full-text and faceted search across artists, venues, cities, and setlists. Filter setlists by artist, venue, city, country, tour, date, and song, with paginated results - the main discovery surface for finding the exact concert or performer you are after.

- **Human URL:** [https://api.setlist.fm/docs/1.0/index.html](https://api.setlist.fm/docs/1.0/index.html)
- **Base URL:** `https://api.setlist.fm/rest/1.0`

#### Tags

- Search
- Discovery
- Full Text

#### Properties

- [Documentation](https://api.setlist.fm/docs/1.0/index.html)
- [API Reference](https://api.setlist.fm/docs/1.0/resource__1.0_search_setlists.html)
- [OpenAPI](openapi/setlistfm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/setlistfm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/setlistfm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### setlist.fm User API

Look up a community member by user ID and retrieve the concerts they have marked as attended or the setlists they have edited. Surfaces the crowd-sourced contributions that keep the setlist.fm database current.

- **Human URL:** [https://api.setlist.fm/docs/1.0/index.html](https://api.setlist.fm/docs/1.0/index.html)
- **Base URL:** `https://api.setlist.fm/rest/1.0`

#### Tags

- Users
- Community
- Attended

#### Properties

- [Documentation](https://api.setlist.fm/docs/1.0/index.html)
- [API Reference](https://api.setlist.fm/docs/1.0/resource__1.0_user__userId_.html)
- [OpenAPI](openapi/setlistfm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/setlistfm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/setlistfm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/setlist-fm/)
- [Website](https://www.setlist.fm/)
- [Documentation](https://api.setlist.fm/docs/1.0/index.html)
- [Plans](plans/setlistfm-plans-pricing.yml)
- [Rate Limits](rate-limits/setlistfm-rate-limits.yml)
- [Fin Ops](finops/setlistfm-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
