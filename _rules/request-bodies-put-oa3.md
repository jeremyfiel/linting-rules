--- 
request-bodies-put-oas3: 
  description: "PUT methods must have a request body."
  given: $.paths.*.put
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
request-bodies-put-oas3: 
  description: "PUT methods must have a request body."
  given: $.paths.*.put
  message: "Method must have a request body {{path}}"
  recommended: true
  severity: error
  then: 
    field: "requestBody"
    function: truthy
  x-status: validated
  x-tags:
    - Methods  