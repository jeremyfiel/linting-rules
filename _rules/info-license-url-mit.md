---
info-license-url-mit:
  description: Should have a MIT license.
  given: $.info.license.url
  severity: error
  then:
    function: pattern
    functionOptions:
      match: mit.edu
  x-status: validated
  x-tags:
    - License
    - Legal     
...
info-license-url-mit:
  description: Should have a MIT license.
  given: $.info.license.url
  severity: error
  then:
    function: pattern
    functionOptions:
      match: mit.edu
  x-status: validated
  x-tags:
    - License
    - Legal  