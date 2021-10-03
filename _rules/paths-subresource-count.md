---
paths-subresources-limit-number-of:
  message: 'Sub-resource levels should by '
  description: SHOULD limit number of sub-resource levels [147]
  documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#147
  severity: warn
  given: $.paths.*~
  then:
    function: pattern
    functionOptions:
      match: ^\/[^\/]*((\/{[^}]*})*\/[^\/]*(\/{[^}]*})*){0,3}\/?$
  x-status: draft
  x-tags:
      - Tag         
...
paths-subresources-limit-number-of:
  message: 'Sub-resource levels should by '
  description: SHOULD limit number of sub-resource levels [147]
  documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#147
  severity: warn
  given: $.paths.*~
  then:
    function: pattern
    functionOptions:
      match: ^\/[^\/]*((\/{[^}]*})*\/[^\/]*(\/{[^}]*})*){0,3}\/?$
  x-status: draft
  x-tags:
      - Tag           