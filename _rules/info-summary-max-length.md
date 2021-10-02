---
info-summary-max-length:
  description: "The summary must not be greater than 20 characters."
  given: "$.info"
  severity: error
  recommended: true
  type: style
  formats:
      - oas3
  then:
      field: summary
      function: length
      functionOptions: 
        max: 20      
  x-status: validated
  x-tags:
    - Info
    - Length
...
info-summary-max-length:
  description: "The summary must not be greater than 20 characters."
  given: "$.info"
  severity: error
  recommended: true
  type: style
  formats:
      - oas3
  then:
      field: summary
      function: length
      functionOptions: 
        max: 20      
  x-status: validated
  x-tags:
    - Info
    - Length 