# Architecture

## High-Level Overview
This is a monolithic, single-file Single Page Application (SPA). All logic, data, structure, and styling exist inside `index.html`.

## Design Patterns
- **Data-Driven UI**: The UI is re-rendered dynamically based on a state (currently active tab and search query) derived from a static source of truth (the `PROMPTS` array).
- **Stateless Rendering**: The `render()` function is called whenever state changes (tab switch or search input), clearing and rebuilding the DOM elements in `<main>`.
- **Event Delegation**: Simple click events for tab toggling and oninput for search are bound directly via HTML attributes, while dynamic elements bind events inside the render logic.
