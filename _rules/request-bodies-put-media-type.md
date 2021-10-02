--- 
request-bodies-put-media-type: 
  description: "PUT request bodies must have a application/json media type."
  given: $.paths.*.put[requestBody].content
  message: "application/json is required for PUT requests {{path}}"
  recommended: true
  severity: error
  then: 
    field: "application/json"
    function: truthy
  x-status: validated
  x-tags:
    - Methods  
...
request-bodies-put-media-type: 
  description: "PUT request bodies must have a application/json media type."
  given: $.paths.*.put[requestBody].content
  message: "application/json is required for PUT requests {{path}}"
  recommended: true
  severity: error
  then: 
    field: "application/json"
    function: truthy
  x-status: validated
  x-tags:
    - Methods 