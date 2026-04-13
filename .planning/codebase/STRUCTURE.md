# Codebase Structure

Since the application is exceptionally minimal, the directory structure is flat:

```text
/
├── .planning/       # GSD project context and mapping documents
├── README.md        # Project documentation and setup instructions
├── favicon.png      # Application logo / favicon
└── index.html       # The single-file SPA (HTML structure, CSS, JS logic, and Data)
```

## File Breakdown (`index.html`)
- **Lines 1-400**: CSS Styles (CSS Variables for theming, responsive design, grid layout)
- **Lines 400-432**: HTML Structure (Header, Tabs, Search Box, Main Container)
- **Lines 434+**: JavaScript Logic (The `PROMPTS` array data store, `render()` function, event listeners)
