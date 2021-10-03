---
response-get-500-status-code:
  description: A get operation should have a 500 response.
  message: A GET operation should have a 500 response.
  severity: warn
  formats:
  - oas2
  - oas3
  given: $.paths[*].get.responses
  then:
    field: "500"
    function: truthy
  x-status: validated
  x-tags:
      - Methods
      - Status Codes       
...
response-get-500-status-code:
  description: A get operation should have a 500 response.
  message: A GET operation should have a 500 response.
  severity: warn
  formats:
  - oas2
  - oas3
  given: $.paths[*].get.responses
  then:
    field: "500"
    function: truthy
  x-status: validated
  x-tags:
      - Methods
      - Status Codes    