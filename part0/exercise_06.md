
```
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server

    Note right of browser: Payload: {content: "Note", date: "2025-01-26T10:59:26.633Z"}

    server-->>browser: Status code: 201 Created {message: "note created"}
    deactivate server

    Note right of browser: The browser executes the event handler (callback function) that renders the notes content (including the new note)
```
![exercise_06](https://github.com/user-attachments/assets/28be3773-c7c1-4928-9539-85568a32680c)
