---
info-contact-name-and-url:
  description: Contact should have name and url properties.
  given: $.info.contact
  severity: error
  then:
  - field: name
    function: truthy
  - field: url
    function: truthy
  x-status: validated
  x-tags:
    - Contact
    - Communication    
...
info-contact-name-and-url:
  description: Contact should have name and url properties.
  given: $.info.contact
  severity: error
  then:
  - field: name
    function: truthy
  - field: url
    function: truthy
  x-status: validated
  x-tags:
    - Contact
    - Communication    