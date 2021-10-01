--- 
responses-headers-rate-limits-oas3: 
  description: Must posses rate limiting headers.
  formats: 
    - oas3
  given: "$.[responses][?(@property[0] == \"2\" )][headers]"
  message: "Missing ratelimit headers. {{property}} {{error}} {{path}}"
  recommended: true
  severity: warn
  then: 
    - 
      function: xor
      functionOptions: 
        properties: 
          - X-RateLimit-Limit
          - RateLimit-Limit
    - 
      function: xor
      functionOptions: 
        properties: 
          - X-RateLimit-Remaining
          - RateLimit-Remaining
    - 
      function: xor
      functionOptions: 
        properties: 
          - X-RateLimit-Reset
          - RateLimit-Reset
  x-tags: 
    - Rate Limits 
...
responses-headers-rate-limits-oas3: 
  description: Must posses rate limiting headers.
  formats: 
    - oas3
  given: "$.[responses][?(@property[0] == \"2\" )][headers]"
  message: "Missing ratelimit headers. {{property}} {{error}} {{path}}"
  recommended: true
  severity: warn
  then: 
    - 
      function: xor
      functionOptions: 
        properties: 
          - X-RateLimit-Limit
          - RateLimit-Limit
    - 
      function: xor
      functionOptions: 
        properties: 
          - X-RateLimit-Remaining
          - RateLimit-Remaining
    - 
      function: xor
      functionOptions: 
        properties: 
          - X-RateLimit-Reset
          - RateLimit-Reset
  x-tags: 
    - Rate Limits 