# setlist.fm (setlistfm)

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
