---
schema-properties-descriptions-words:
  description: Some words should not exist within the property description.
  message: Words should not exist within description {{ property }}.
  severity: warn
  formats:
  - oas3
  given: $..properties.*
  then:
    field: description
    function: pattern
    functionOptions:
        notMatch: \b(word|word|word)\b
  x-status: validated
  x-tags:
      - Schema         
...
schema-properties-descriptions-words:
  description: Some words should not exist within the property description.
  message: Words should not exist within description {{ property }}.
  severity: warn
  formats:
  - oas3
  given: $..properties.*
  then:
    field: description
    function: pattern
    functionOptions:
        notMatch: \b(word|word|word)\b
  x-status: validated
  x-tags:
      - Schema 