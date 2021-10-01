--- 
security-schemes-jwt: 
  description: |-
      Json Web Tokens RFC7519 is a compact, URL-safe means of representing claims to be transferred between two parties. JWT can be enclosed in encrypted or signed tokens like JWS and JWE. 
  given: 
    - "$.[securitySchemes][?(@.bearerFormat==\"jwt\" || @.bearerFormat==\"JWT\")]"
  message: "JWT usage should be detailed in `description` {{error}}."
  then: 
    - 
      field: description
      function: truthy
    - 
      field: description
      function: pattern
      functionOptions: 
        match: .*RFC8725.*   
...
security-schemes-jwt: 
  description: |-
      Json Web Tokens RFC7519 is a compact, URL-safe means of representing claims to be transferred between two parties. JWT can be enclosed in encrypted or signed tokens like JWS and JWE. 
  given: 
    - "$.[securitySchemes][?(@.bearerFormat==\"jwt\" || @.bearerFormat==\"JWT\")]"
  message: "JWT usage should be detailed in `description` {{error}}."
  then: 
    - 
      field: description
      function: truthy
    - 
      field: description
      function: pattern
      functionOptions: 
        match: .*RFC8725.*  