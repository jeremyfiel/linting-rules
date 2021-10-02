--- 
request-bodies-post-media-type: 
  description: "POST request bodies must have a application/json media type.";
  given: "$.post.requestBody.content"
  message: "application/json is required for POST requests {{path}}"
  recommended: true
  severity: error
  then: 
    field: "application/json"
    function: truthy
  x-status: draft
  x-tags:
    - Tag  
...
request-bodies-post-media-type: 
  description: "POST request bodies must have a application/json media type.";
  given: "$.post.requestBody.content"
  message: "application/json is required for POST requests {{path}}"
  recommended: true
  severity: error
  then: 
    field: "application/json"
    function: truthy
  x-status: draft
  x-tags:
    - Tag  