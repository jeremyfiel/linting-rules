---
components-request-and-response-body-oas3:
  description: Response and requestBody content schema $ref may only point to elements in the components object within document.
  severity: error
  resolved: false
  given:
  - $..responses.*.content..*.schema.$ref
  - $..requestBody.content..*.schema.$ref
  then:
    function: pattern
    functionOptions:
      match: '#/components/'
  x-status: draft
  x-tags:
    - Tag      
...
components-request-and-response-body-oas3:
  description: Response and requestBody content schema $ref may only point to elements in the components object within document.
  severity: error
  resolved: false
  given:
  - $..responses.*.content..*.schema.$ref
  - $..requestBody.content..*.schema.$ref
  then:
    function: pattern
    functionOptions:
      match: '#/components/'
  x-status: draft
  x-tags:
    - Tag      