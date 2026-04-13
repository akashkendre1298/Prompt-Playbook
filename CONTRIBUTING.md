# Contributing to Prompt Playbook

First off, thank you for considering contributing to the **Prompt Playbook — Engineer Edition**! We want this to be the ultimate collection of high-value AI prompts for developers, and community contributions are the best way to get there.

## How to Contribute

To protect the main application from breaking, we use the standard open-source "Fork & Pull Request" workflow. Direct pushes to the `main` branch are blocked.

### 1. Fork the Repository
1. Click the **Fork** button at the top right of the [repository page](https://github.com/akashkendre1298/Prompt-Playbook).
2. Clone your fork locally to your machine:
   ```bash
   git clone https://github.com/YOUR_USERNAME/Prompt-Playbook.git
   cd Prompt-Playbook
   ```
3. Create a new branch for your changes:
   ```bash
   git checkout -b add-new-prompt
   ```

### 2. Add Your Prompt
The entire application is contained in the `index.html` file. To add your prompt:
1. Open `index.html` in your code editor.
2. Locate the `PROMPTS` array (starts around line 434).
3. Add your new prompt object to the appropriate category. Your object must follow this exact schema:

```javascript
{
  tab: "coding",          // Choose from: "prompt-craft", "coding", "productivity", or "creative"
  iconClass: "icon-code", // Choose from: "icon-craft", "icon-code", "icon-prod", or "icon-creative"
  badge: "badge-code",    // Choose from: "badge-craft", "badge-code", "badge-prod", or "badge-creative"
  badgeLabel: "coding",   // The text displayed on the badge
  icon: "⌖",             // Insert a distinct unicode symbol
  title: "Your Prompt Title",
  desc: "A brief, one sentence description of what the prompt accomplishes.",
  template:`Paste your Prompt here. 
You can use [BRACKETS] for variables.`,
  examples:[
    { filled: "Write how the prompt looks when filled out by the user." }
  ]
}
```

**Important Guidelines:**
- Ensure your prompt is highly relevant to software engineers, developers, or tech professionals.
- Keep the `template` clean and structured.
- Always provide at least one clear example in the `examples` array so users know exactly how to fill out the bracketed variables.
- Test your changes locally simply by opening `index.html` in your web browser!

### 3. Commit and Push
Once you've tested your prompt and verified that it renders properly on the page:
1. Stage and commit your changes:
   ```bash
   git add index.html
   git commit -m "feat: add [Title of Your Prompt]"
   ```
2. Push your branch to your forked repository:
   ```bash
   git push origin add-new-prompt
   ```

### 4. Create a Pull Request (PR)
1. Navigate back to the original repository page.
2. You will see a banner prompting you to **"Compare & pull request"**. Click it!
3. Add a brief title and description explaining what your prompt does and why it's useful.
4. Click **Create pull request**.

The maintainers will review your PR to ensure it doesn't break the application. Once approved and merged, your prompt will be live on the site! 🎉
