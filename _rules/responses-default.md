---
responses-default:
  message: Operation does not contain a default response
  description: MUST specify success and error responses [151]
  documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#151
  severity: error
  given: $.paths.*.*.responses
  then:
    field: default
    function: truthy
...
responses-default:
  message: Operation does not contain a default response
  description: MUST specify success and error responses [151]
  documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#151
  severity: error
  given: $.paths.*.*.responses
  then:
    field: default
    function: truthy