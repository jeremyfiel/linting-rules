---
paths-status-problem-schema:
  x-tags:
    - it
  description: '"/status" schema is not a Problem object.'
  message: "{{error}} {{path}}"
  severity: warn
  recommended: true
  given: $.paths.'/status'.get.responses.200.content.[[schema]]
  then:
    - function: truthy
      field: properties.status
    - function: truthy
      field: properties.title
    - function: truthy
      field: properties.detail     
...
paths-status-problem-schema:
  x-tags:
    - it
  description: '"/status" schema is not a Problem object.'
  message: "{{error}} {{path}}"
  severity: warn
  recommended: true
  given: $.paths.'/status'.get.responses.200.content.[[schema]]
  then:
    - function: truthy
      field: properties.status
    - function: truthy
      field: properties.title
    - function: truthy
      field: properties.detail 