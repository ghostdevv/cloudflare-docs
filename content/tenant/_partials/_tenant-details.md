---
_build:
  publishResources: false
  render: never
  list: never
---

{{<definitions>}}

To retrieve tenant details, send a `GET` request to the `/user/tenants` endpoint:

{{</definitions>}}

```bash
---
header: Request
---
curl 'https://api.cloudflare.com/client/v4/user/tenants' \
--header "x-auth-email: <EMAIL>" \
--header "x-auth-key: <API_KEY>"
```

A successful request will return an HTTP status of `200` and a response body containing tenant information, unit information, memberships, and tenant entitlements for all tenants administered by the user.