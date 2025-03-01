---
_build:
  publishResources: false
  render: never
  list: never
---

{{<Aside type="warning">}}

Since Cloudflare validates client certificates with one CA, set at account level, these certificates can be used for validation across multiple zones, as long as the zones are under the same account and mTLS has been enabled for the requested hosts.
This means that (a) if you [bring your own CA](/ssl/client-certificates/byo-ca-api-shield/), you can associate it with hosts in different zones and (b) if you use Cloudflare Managed CA, this is the default behavior.

{{</Aside>}}