---
components-links-pascal-case:
  description: All links should be named with UpperCamelCase
  message: '{{property}} is not UpperCamelCase. {{description}}. Fix by renaming the
    link, eg. object -> Object.'
  given: $.components.links
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
components-links-pascal-case:
  description: All links should be named with UpperCamelCase
  message: '{{property}} is not UpperCamelCase. {{description}}. Fix by renaming the
    link, eg. object -> Object.'
  given: $.components.links
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