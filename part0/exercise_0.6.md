```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    Note right of browser: payload: {"content": "new-note-spa-v1", "date": "2023-11-29T21:45:16.096Z"}
    activate server
    server-->>browser:
    deactivate server
    Note right of browser: response: {"message":"note created"}
```
