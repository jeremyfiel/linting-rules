---
check-for-use-of-anyof:
  description: API Connect has a compatibility issue with the anyOf functionality.
    Avoid its use if reasonably possible.
  given: $..
  severity: warn
  then:
    field: anyOf
    function: falsy
  x-status: draft
  x-tags:
    - Tag    
...
check-for-use-of-anyof:
  description: API Connect has a compatibility issue with the anyOf functionality.
    Avoid its use if reasonably possible.
  given: $..
  severity: warn
  then:
    field: anyOf
    function: falsy
  x-status: draft
  x-tags:
    - Tag    