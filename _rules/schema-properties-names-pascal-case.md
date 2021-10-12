---
schema-properties-names-pascal-case:
  description: Schema property names should be pascal case.
  message: Schema name should be pascal case.
  severity: error
  given: $..properties.*
  then:
    field: "@key"
    function: casing
    functionOptions:
      type: pascal
  x-status: validated
  x-tags:
      - Schema
      - Casing          
...
schema-properties-names-pascal-case:
  description: Schema property names should be pascal case.
  message: Schema name should be pascal case.
  severity: error
  given: $..properties.*
  then:
    field: "@key"
    function: casing
    functionOptions:
      type: pascal
  x-status: validated
  x-tags:
      - Schema
      - Casing      