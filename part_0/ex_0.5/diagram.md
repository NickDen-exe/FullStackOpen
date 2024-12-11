```mermaid
sequenceDiagram
    browser->>+server:GET https://studies.cs.helsinki.fi/exampleapp/spa
    server-->>-browser: HTML document file

    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    server-->>-browser: CSS stylesheets file 

    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/spa.js
    server-->>-browser: JavaScript file

    browser->>+server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
    server-->-browser: data JSON [{"content": "...", "data": "..."}]

        Note right of browser: Browsers render the notes
    
```