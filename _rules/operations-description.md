---
operations-description:
  severity: error
  message: Missing {{property}}at {{path}}
  given: $.paths.*[get,post,patch,put,delete]
  then:
  - field: description
    function: truthy
...
operations-description:
  severity: error
  message: Missing {{property}}at {{path}}
  given: $.paths.*[get,post,patch,put,delete]
  then:
  - field: description
    function: truthy