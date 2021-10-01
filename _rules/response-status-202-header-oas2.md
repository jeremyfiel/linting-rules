---
response-status-202-header-oas2:
  description: A 202 response should include an Operation-Location response header.
  severity: warn
  formats:
  - oas2
  given: $.paths[*][*].responses[?(@property == '202')]
  then:
    field: headers.Operation-location
    function: truthy
...
response-status-202-header-oas2:
  description: A 202 response should include an Operation-Location response header.
  severity: warn
  formats:
  - oas2
  given: $.paths[*][*].responses[?(@property == '202')]
  then:
    field: headers.Operation-location
    function: truthy