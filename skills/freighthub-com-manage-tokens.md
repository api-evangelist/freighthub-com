---
name: freighthub-com-manage-tokens
description: Create a token, list existing tokens, and delete a token.
api: openapi/freighthub-com-forto-platform-api-openapi.yml
operations:
- createTokenv1
- getTokensv1
- deleteTokenv1
generated: '2026-10-23'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/freighthub-com-forto-platform-api-openapi.yml ; every operationId checked against the contract
---

# freighthub-com-manage-tokens

Create a token, list existing tokens, and delete a token.

## Steps

1. 1. Call `createTokenv1` with the required request body fields and include the `Authorization` header.
2. 2. Call `getTokensv1` with query parameters `page` and `pageSize` to paginate the list of tokens, also including the `Authorization` header.
3. 3. Call `deleteTokenv1` with path parameter `id` of the token to remove, and include the `Authorization` header.

## Rules

- Include an `Authorization` header (HTTP auth scheme) on every request.
- Use `page` and `pageSize` query parameters for pagination when calling `getTokensv1`.
