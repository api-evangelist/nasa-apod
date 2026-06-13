# NASA APOD

APIs.json 0.19 provider profile for the NASA Astronomy Picture of the Day (APOD) API.

## Overview

The NASA APOD API delivers daily astronomy images and explanations curated by
NASA scientists. Each entry includes a title, a written explanation, image URLs
(standard and HD), media type, and optional copyright attribution. The archive
extends back to 1995-06-16.

**Base URL:** `https://api.nasa.gov`  
**Endpoint:** `GET /planetary/apod`

## Key Parameters

| Parameter | Description |
|-----------|-------------|
| `api_key` | NASA API key (use `DEMO_KEY` for testing) |
| `date` | YYYY-MM-DD — specific APOD date (default: today) |
| `start_date` | Beginning of a date range |
| `end_date` | End of a date range (default: today) |
| `count` | Number of random APODs to return (max 100) |
| `thumbs` | Return video thumbnail URL when media type is video |

## Authentication

Register for a free API key at https://api.nasa.gov/#signUp.  
Use `DEMO_KEY` for low-volume exploration (30 req/hour, 50 req/day per IP).

## Rate Limits

| Key Type | Hourly | Daily |
|----------|--------|-------|
| DEMO_KEY | 30 / IP | 50 / IP |
| Registered | 1,000 / key | — |

## Files

- `apis.yml` — APIs.json 0.19 provider index
- `plans/nasa-apod-plans-pricing.yml` — access plans
- `rate-limits/nasa-apod-rate-limits.yml` — rate limit details
- `finops/nasa-apod-finops.yml` — financial operations guidance

## Links

- Developer portal: https://api.nasa.gov/
- Source code: https://github.com/nasa/apod-api
- APOD website: https://apod.nasa.gov/apod/

## Maintainer

Kin Lane &lt;kin@apievangelist.com&gt;
