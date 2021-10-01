---
components-parameters-prefix-in-query:
  description: Parameters should be in a location matching the prefix (Query.)
  message: '{{value}} does not match the parameter prefix. {{description}}. Fix by
    assigning the correct in value, eg. header -> query.'
  given: $.components.parameters..[?(@property.match(/^Query\./))]
  severity: error
  then:
    field: in
    function: pattern
    functionOptions:
      match: ^query$
  x-status: draft
  x-tags:
    - Tag      
...
components-parameters-prefix-in-query:
  description: Parameters should be in a location matching the prefix (Query.)
  message: '{{value}} does not match the parameter prefix. {{description}}. Fix by
    assigning the correct in value, eg. header -> query.'
  given: $.components.parameters..[?(@property.match(/^Query\./))]
  severity: error
  then:
    field: in
    function: pattern
    functionOptions:
      match: ^query$
  x-status: draft
  x-tags:
    - Tag      