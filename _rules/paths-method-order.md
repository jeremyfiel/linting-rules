---
paths-method-order:
  severity: error
  given: $.paths[?(@.get || @.post || @.patch || @.put || @.delete)]
  then:
    function: operationOrdering
...
paths-method-order:
  severity: error
  given: $.paths[?(@.get || @.post || @.patch || @.put || @.delete)]
  then:
    function: operationOrdering