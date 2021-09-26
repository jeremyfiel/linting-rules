---
paths-http-method:
  x-tags:
    - it
  description: >-
    When you design a REST API, you don't usually need to mention terms like `get`, `delete` and so on in your `paths`, because this information is conveyed by the HTTP method. Instead of using
    ```
    POST /books/1234/delete HTTP/1.1

    Host: api.example
    ```
    You can simply call
    ```
    DELETE /books/1234 HTTP/1.1

    Host: api.example

    ```
    Similarly you don't need verbs like `list` or `create` because the HTTP Semantics RFC7231 supports this kind of actions natively with proper methods and status code. Instead of
    ```

    POST /create/user HTTP/1.1

    Host: api.example

    Content-Type: application/json

    {"given_name": "Mario"}

    ```
    You can use
    ```

    POST /create/user HTTP/1.1

    Host: api.example

    Content-Type: application/json

    {"given_name": "Mario"}

    ```
    returning a proper response
    ```
    HTTP/1.1 201 Created

    Location: /users/1234
    ```
    This simplifies securing your API as you know beforehand the kind of action which is going to be performed.
  message: API "path" contains a name of an http method. {{error}}
  severity: hint
  recommended: true
  given:
    - $.paths[?(@property.match( /\/(get|post|put|delete|patch)[\/A-Z_\-]?/
      ))]~
    - $.paths[?(@property.match( /\/(create|remove|list)[\/A-Z_\-]?/ ))]~
  then:
    field: "@key"
    function: undefined 
...
paths-http-method:
  x-tags:
    - it
  description: >-
    When you design a REST API, you don't usually need to mention terms like `get`, `delete` and so on in your `paths`, because this information is conveyed by the HTTP method. Instead of using
    ```
    POST /books/1234/delete HTTP/1.1

    Host: api.example
    ```
    You can simply call
    ```
    DELETE /books/1234 HTTP/1.1

    Host: api.example

    ```
    Similarly you don't need verbs like `list` or `create` because the HTTP Semantics RFC7231 supports this kind of actions natively with proper methods and status code. Instead of
    ```

    POST /create/user HTTP/1.1

    Host: api.example

    Content-Type: application/json

    {"given_name": "Mario"}

    ```
    You can use
    ```

    POST /create/user HTTP/1.1

    Host: api.example

    Content-Type: application/json

    {"given_name": "Mario"}

    ```
    returning a proper response
    ```
    HTTP/1.1 201 Created

    Location: /users/1234
    ```
    This simplifies securing your API as you know beforehand the kind of action which is going to be performed.
  message: API "path" contains a name of an http method. {{error}}
  severity: hint
  recommended: true
  given:
    - $.paths[?(@property.match( /\/(get|post|put|delete|patch)[\/A-Z_\-]?/
      ))]~
    - $.paths[?(@property.match( /\/(create|remove|list)[\/A-Z_\-]?/ ))]~
  then:
    field: "@key"
    function: undefined 