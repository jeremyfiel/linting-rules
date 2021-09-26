---
securitySchemes-oauth-http:
    description: OAuth2 endpoints must use `https://`
    message: OAuth endpoints must use https://
    formats:
        - oas3
    severity: error
    recommended: true
    given:
        - $.[securitySchemes][?(@.type=="oauth2")][*].[?(@property.match(/url$/i))]
    then:
        - field: value
        function: pattern
        functionOptions:
            match: ^https://
...
securitySchemes-oauth-http:
    description: OAuth2 endpoints must use `https://`
    message: OAuth endpoints must use https://
    formats:
        - oas3
    severity: error
    recommended: true
    given:
        - $.[securitySchemes][?(@.type=="oauth2")][*].[?(@property.match(/url$/i))]
    then:
        - field: value
        function: pattern
        functionOptions:
            match: ^https://