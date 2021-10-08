---
schema-description-length:
  description: All schemas descriptions should be shorter than 20 characters.
  message: Description needs to be less than 20 characters {{ property }}.
  severity: warn
  formats:
  - oas3
  given: $.components.schemas.*
  then:
      field: description
      function: length
      functionOptions: 
        max: 20
  x-status: validated
  x-tags:
      - Schema         
...
schema-description-length:
  description: All schemas descriptions should be shorter than 20 characters.
  message: Description needs to be less than 20 characters {{ property }}.
  severity: warn
  formats:
  - oas3
  given: $.components.schemas.*
  then:
      field: description
      function: length
      functionOptions: 
        max: 20
  x-status: validated
  x-tags:
      - Schema  