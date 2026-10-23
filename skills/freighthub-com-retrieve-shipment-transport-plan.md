---
name: freighthub-com-retrieve-shipment-transport-plan
description: Retrieve a shipment's transport plan and related events.
api: openapi/freighthub-com-forto-platform-api-openapi.yml
operations:
- getShipmentv1
- getShipmentTransportPlanv2
- getShipmentTransportPlanEventsv2
generated: '2026-10-23'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/freighthub-com-forto-platform-api-openapi.yml ; every operationId checked against the contract
---

# freighthub-com-retrieve-shipment-transport-plan

Retrieve a shipment's transport plan and related events.

## Steps

1. 1. Call `getShipmentv1` with the `shipmentId` path parameter to obtain basic shipment details.
2. 2. Call `getShipmentTransportPlanv2` with the same `shipmentId` to fetch the transport plan.
3. 3. Call `getShipmentTransportPlanEventsv2` with the `shipmentId` to list transport‑plan events.

## Rules

- Include an `Authorization` header with a valid bearer token for all requests.
- Use the `pageSize` and `page` query parameters for pagination when listing events.
