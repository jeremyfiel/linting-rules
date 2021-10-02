---
parameters-name-snake-case:
  description: Path and query parmeters must use snake_case.
  given: $.paths.*.*.parameters[?(@.in=='query')].name
  then:
    field: name
    function: casing
    functionOptions:
      type: snake
  x-status: validated
  x-tags:
    - Parameters
    - Casing        
...
parameters-name-snake-case:
  description: Path and query parmeters must use snake_case.
  given: $.paths.*.*.parameters[?(@.in=='query')].name
  then:
    field: name
    function: casing
    functionOptions:
      type: snake
  x-status: validated
  x-tags:
    - Parameters
    - Casing        