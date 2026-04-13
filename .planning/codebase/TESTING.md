# Testing Strategy

- **Automated Tests**: None (No test framework implemented).
- **Manual Testing**: Development driven by direct manual testing in the browser. You can open `index.html` in an internet browser straight from the file system, or via a simple static local server (`npx serve`, VSCode Live Server).
- **Key Test Cases Needed (Manual)**:
  - Filtering interactions by tabs (e.g. click "coding" tab and verify rendering).
  - Search input functionality (real-time filtering).
  - Expanding examples ("See Example" accordion).
  - "Copy" button correctly places the template string on the user clipboard.
