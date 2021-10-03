--- 
request-bodies-delete-oas3: 
  description: "DELETE methods must have a request body."
  given: $.paths.*.delete
  message: "Method must not have a request body {{path}}"
  recommended: true
  severity: error
  then: 
    field: "requestBody"
    function: falsy
  x-status: validated
  x-tags:
    - Methods  
...
request-bodies-delete-oas3: 
  description: "DELETE methods must have a request body."
  given: $.paths.*.delete
  message: "Method must not have a request body {{path}}"
  recommended: true
  severity: error
  then: 
    field: "requestBody"
    function: falsy
  x-status: validated
  x-tags:
    - Methods  