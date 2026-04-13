# Concerns & Limitations

## Technical Debt & Scalability
- **Single File Monolith**: As the `PROMPTS` array continuously grows, `index.html` will become very large and difficult to manage.
  - *Recommendation*: Extract the JS logic into an `app.js` file and move data to `data.js` or `data.json`.
- **Rendering Performance**: The current architecture relies on modifying `innerHTML` upon every keystroke (for search functionality).
  - *Recommendation*: If the prompt collection scales to hundreds of items, this `oninput="render()"` approach could cause UI stuttering. Implement a debounced search function or simple DOM hiding/showing instead of complete re-rendering.

## Security
- The app requires the Browser's `navigator.clipboard` API to copy the prompts, which mandates a secure context (the app must be hosted on `HTTPS` or accessed over `localhost`).
