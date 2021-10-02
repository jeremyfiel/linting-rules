---
parameters-name-camel-case:
  description: Path and query parmeters must use camelCase.
  given: $.paths.*.*.parameters[?(@.in=='query')].name
  then:
    field: name
    function: casing
    functionOptions:
      type: camel
  x-status: validated
  x-tags:
    - Parameters
    - Casing        
...
parameters-name-camel-case:
  description: Path and query parmeters must use camelCase.
  given: $.paths.*.*.parameters[?(@.in=='query')].name
  then:
    field: name
    function: casing
    functionOptions:
      type: camel
  x-status: validated
  x-tags:
    - Parameters
    - Casing        