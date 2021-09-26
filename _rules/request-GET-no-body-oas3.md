---
request-GET-no-body-oas3:
  description: A `GET` request MUST NOT accept a request body
  severity: error
  format: [oas3]
  given: $.paths..get.requestBody
  then:
    function: undefined    
...
request-GET-no-body-oas3:
  description: A `GET` request MUST NOT accept a request body
  severity: error
  format: [oas3]
  given: $.paths..get.requestBody
  then:
    function: undefined     