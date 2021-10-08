--- 
request-bodies-patch-oas3: 
  description: "PATCH methods must have a request body."
  given: $.paths.*.patch
  message: "Method must have a request body {{path}}"
  recommended: true
  severity: error
  then: 
    field: "requestBody"
    function: truthy
  x-status: validated
  x-tags:
    - Methods  
...
request-bodies-patch-oas3: 
  description: "PATCH methods must have a request body."
  given: $.paths.*.patch
  message: "Method must have a request body {{path}}"
  recommended: true
  severity: error
  then: 
    field: "requestBody"
    function: truthy
  x-status: validated
  x-tags:
    - Methods 