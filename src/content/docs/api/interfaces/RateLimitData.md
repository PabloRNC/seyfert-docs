---
editUrl: false
next: false
prev: false
title: "RateLimitData"
---

Data emitted on `RESTEvents.RateLimited`

## Properties

| Property | Type | Description |
| :------ | :------ | :------ |
| `global` | `boolean` | Whether the rate limit that was reached was the global limit |
| `hash` | `string` | The bucket hash for this request |
| `limit` | `number` | The amount of requests we can perform before locking requests |
| `majorParameter` | `string` | The major parameter of the route
| `method` | `string` | The HTTP method being performed |
| `retryAfter` | `number` | The time, in milliseconds, that will need to pass before this specific request can be retried |
| `route` | `string` | The route being hit in this request |
| `scope` | `"shared"` \| `"global"` \| `"user"` | The scope of the rate limit that was hit.
| `sublimitTimeout` | `number` | The time, in milliseconds, that will need to pass before the sublimit lock for the route resets, and requests that fall under a sublimit
| `timeToReset` | `number` | The time, in milliseconds, until the route's request-lock is reset |
| `url` | `string` | The full URL for this request |