---
no-default-additionalProperties:
  description: |-
    By default, jsonschema allows additionalProperties. This means
    that schema validators can be bypassed using further, unspecified
    fields.

    While forbidding additionalProperties can create rigidity and hinder
    the evolution of an API - eg making it hard to accept new parameters
    or fields - it is possible that this flexibility can be used
    to bypass the schema validator and force the application to process
    unwanted information.

    Disable `additionalProperties` with `false`

    ```
    Person:
      type: object
      additionalProperties: false
      properties:
        given_name:
          type: string
          pattern: [a-zA-Z ]{24}
    ```
    Or constraint them using `maxProperties`
    ```
    Person:
      type: object
      additionalProperties:
        type: string
        pattern: /+39[0-9]{,14}/
      maxProperties: 3
      properties:
        given_name:
          type: string
          pattern: [a-zA-Z ]{24}
    ```
    - no additionalProperties
    - constrained additionalProperties
  message: "Objects should not allow additionalProperties. Disable them with
    `additionalProperties: false` or constraint them."
  formats:
    - oas3
  severity: warn
  recommended: true
  given:
    - $.[?(@.type=="object" && ! @.additionalProperties)]
  then:
    - field: additionalProperties
      function: defined   
...
no-default-additionalProperties:
  description: |-
    By default, jsonschema allows additionalProperties. This means
    that schema validators can be bypassed using further, unspecified
    fields.

    While forbidding additionalProperties can create rigidity and hinder
    the evolution of an API - eg making it hard to accept new parameters
    or fields - it is possible that this flexibility can be used
    to bypass the schema validator and force the application to process
    unwanted information.

    Disable `additionalProperties` with `false`

    ```
    Person:
      type: object
      additionalProperties: false
      properties:
        given_name:
          type: string
          pattern: [a-zA-Z ]{24}
    ```
    Or constraint them using `maxProperties`
    ```
    Person:
      type: object
      additionalProperties:
        type: string
        pattern: /+39[0-9]{,14}/
      maxProperties: 3
      properties:
        given_name:
          type: string
          pattern: [a-zA-Z ]{24}
    ```
    - no additionalProperties
    - constrained additionalProperties
  message: "Objects should not allow additionalProperties. Disable them with
    `additionalProperties: false` or constraint them."
  formats:
    - oas3
  severity: warn
  recommended: true
  given:
    - $.[?(@.type=="object" && ! @.additionalProperties)]
  then:
    - field: additionalProperties
      function: defined  