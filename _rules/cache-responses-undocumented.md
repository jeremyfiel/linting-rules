---
cache-responses-undocumented:
  description: >-
    Cache usage SHOULD be extensively detailed in the `description` property to avoid data leaks or the usage of stale data. This rule should ensure in some way that the api provider documented extensively the cache usage to avoid data leaks or usage of stale data.

    For now this ruleset tests:

    * the presence of following keywords
      in the `description`: `max-age`, `private`, `no-store`, `no-cache`.
    * that one and only one between Expires and Cache-Control is used.

    `Cache-Control` and `Expires` should not be used in conjuction, because `Cache-Control` overrides `Expires` when `max-age` is set. Instead if neither `Cache-Control` or `Expires` are set, clients MAY use euristic cache like described in RFC7234.
  message: Cache usage in responses SHOULD be documented in Cache-Control and/or
    Expires. {{error}}
  formats: *a1
  severity: info
  recommended: true
  given: $.[responses][?(@property[0] == "2"
    )][headers].[?(@property.match(/Cache-Control|Expires/i))]]
  then: *a2    
...
cache-responses-undocumented:
  description: >-
    Cache usage SHOULD be extensively detailed in the `description` property to avoid data leaks or the usage of stale data. This rule should ensure in some way that the api provider documented extensively the cache usage to avoid data leaks or usage of stale data.

    For now this ruleset tests:

    * the presence of following keywords
      in the `description`: `max-age`, `private`, `no-store`, `no-cache`.
    * that one and only one between Expires and Cache-Control is used.

    `Cache-Control` and `Expires` should not be used in conjuction, because `Cache-Control` overrides `Expires` when `max-age` is set. Instead if neither `Cache-Control` or `Expires` are set, clients MAY use euristic cache like described in RFC7234.
  message: Cache usage in responses SHOULD be documented in Cache-Control and/or
    Expires. {{error}}
  formats: *a1
  severity: info
  recommended: true
  given: $.[responses][?(@property[0] == "2"
    )][headers].[?(@property.match(/Cache-Control|Expires/i))]]
  then: *a2 