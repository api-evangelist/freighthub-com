---
name: freighthub-com-manage-subscriptions
description: Create, list, and delete event subscriptions.
api: openapi/freighthub-com-forto-platform-api-openapi.yml
operations:
- listSubscriptionsv1
- createSubscriptionv1
- deleteSubscriptionv1
generated: '2026-10-23'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/freighthub-com-forto-platform-api-openapi.yml ; every operationId checked against the contract
---

# freighthub-com-manage-subscriptions

Create, list, and delete event subscriptions.

## Steps

1. 1. `listSubscriptionsv1` – use query parameters `page` and `pageSize` for pagination.
2. 2. `createSubscriptionv1` – provide the subscription payload in the request body.
3. 3. `deleteSubscriptionv1` – specify the subscription `{id}` in the path.

## Rules

- Auth: Include an `Authorization` header with a valid token (http scheme).
- Pagination: Use `page` and `pageSize` query parameters when listing subscriptions.
