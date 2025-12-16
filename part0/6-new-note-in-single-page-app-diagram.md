```mermaid
sequenceDiagram
    participant browser
    participant server

    Note right of browser: The browser executes the JavaScript code that updates the local list of elements and redraws them

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: Status 201
    deactivate server
```