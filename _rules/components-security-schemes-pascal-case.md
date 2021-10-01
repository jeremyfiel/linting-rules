---
components-security-schemes-pascal-case:
  description: All security schemes should be named with UpperCamelCase
  message: '{{property}} is not UpperCamelCase. {{description}}. Fix by renaming the
    definition, eg. object -> Object.'
  given: $.components.securitySchemes
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
components-security-schemes-pascal-case:
  description: All security schemes should be named with UpperCamelCase
  message: '{{property}} is not UpperCamelCase. {{description}}. Fix by renaming the
    definition, eg. object -> Object.'
  given: $.components.securitySchemes
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