---
version-query-parameter-oas2:
  description: Specify API version using api-version query parameter, not in path.
  message: '{{error}}'
  severity: warn
  formats:
  - oas2
  given: $
  then:
    function: version-policy
...
version-query-parameter-oas2:
  description: Specify API version using api-version query parameter, not in path.
  message: '{{error}}'
  severity: warn
  formats:
  - oas2
  given: $
  then:
    function: version-policy