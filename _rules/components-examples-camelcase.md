---
components-examples-camelcase:
  description: All examples should be named with UpperCamelCase
  message: '{{property}} is not UpperCamelCase. {{description}}. Fix by renaming the
    example, eg. object -> Object.'
  given: $.components.examples
  severity: error
  then:
    field: '@key'
    function: casing
    functionOptions:
      type: pascal
      separator:
        char: .
        allowLeading: false
  x-status: draft
  x-tags:
    - Tag        
...
components-examples-camelcase:
  description: All examples should be named with UpperCamelCase
  message: '{{property}} is not UpperCamelCase. {{description}}. Fix by renaming the
    example, eg. object -> Object.'
  given: $.components.examples
  severity: error
  then:
    field: '@key'
    function: casing
    functionOptions:
      type: pascal
      separator:
        char: .
        allowLeading: false
  x-status: draft
  x-tags:
    - Tag        