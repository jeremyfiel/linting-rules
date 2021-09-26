---
has-x-summary:
    x-tags:
        - it
        - metadata
    message: "API MUST have an one-liner #/info/x-summary field containing a brief
        description."
    description: >-
        The `#/info/x-summary` can be used to specify a brief, one-liner description of your API: this is very useful for catalog purposes (eg. this can be shown as your API subtitle in catalogs and developer portals). In OAS3.1 you can use the standard `#/info/summary` field.
    given: $
    severity: error
    recommended: true
    type: style
    formats:
        - oas3
    then:
        field: info.x-summary
        function: truthy    
...
has-x-summary:
    x-tags:
        - it
        - metadata
    message: "API MUST have an one-liner #/info/x-summary field containing a brief
        description."
    description: >-
        The `#/info/x-summary` can be used to specify a brief, one-liner
        description of your API: this is very useful for catalog purposes (eg.
        this can be shown as your API subtitle in catalogs and developer portals).

        In OAS3.1 you can use the standard `#/info/summary` field.
    given: $
    severity: error
    recommended: true
    type: style
    formats:
        - oas3
    then:
        field: info.x-summary
        function: truthy 