---
info-title:
  description: "Must have a #/info/title."
  given: "$.info"
  severity: error
  recommended: true
  type: style
  formats:
      - oas3
  then:
      field: title
      function: truthy  
  x-status: validated
  x-tags:
    - Info
...
info-title:
  description: "Must have a #/info/title."
  given: "$.info"
  severity: error
  recommended: true
  type: style
  formats:
      - oas3
  then:
      field: title
      function: truthy  
  x-status: validated
  x-tags:
    - Info    