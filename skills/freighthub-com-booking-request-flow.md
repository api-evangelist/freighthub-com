---
name: freighthub-com-booking-request-flow
description: Create a new booking request, finalize it, and retrieve its details.
api: openapi/freighthub-com-forto-platform-api-openapi.yml
operations:
- createv1
- finalizev1
- getv1
generated: '2026-10-23'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/freighthub-com-forto-platform-api-openapi.yml ; every operationId checked against the contract
---

# freighthub-com-booking-request-flow

Create a new booking request, finalize it, and retrieve its details.

## Steps

1. 1. Use `createv1` with the request body fields required to create a booking request and include the `Authorization` header.
2. 2. Use `finalizev1` with path parameter `id` of the created request and include the `Authorization` header.
3. 3. Use `getv1` with path parameter `id` to retrieve the finalized booking request, providing the `Authorization` header.

## Rules

- Include an `Authorization` header (HTTP auth scheme) on every request.
- When listing booking requests with `listv1`, use pagination parameters `page` and `pageSize`.
