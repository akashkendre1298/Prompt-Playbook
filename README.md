# Prompt Playbook — Engineer Edition 🚀

[![Live Demo](https://img.shields.io/badge/Live_Website-View_Playbook-2ea44f?style=for-the-badge)](https://akashkendre1298.github.io/Prompt-Playbook/)

A sleek, premium, developer-focused interface that serves as a high-value collection of AI prompt templates. Designed specifically for software engineers, this playbook provides proven, copy-paste ready prompt structures to help you get the absolute best output from tools like ChatGPT, Claude, and Gemini.

Stop writing generic prompts and start getting professional, targeted results for your complex engineering tasks!

![Prompt Playbook Screenshot](favicon.png) <!-- Note: This assumes the favicon serves as a temporary logo placeholder if an actual screenshot is absent -->

## 🛠️ Features

- **Categorized Prompts:** Organized neatly into *Prompt Craft, Coding & Tech, Work & Productivity, and Creative Projects*.
- **Deep Technical Scenarios:** Includes advanced prompts for:
  - Architecture Decision Records (ADRs)
  - Surgical Bug Debugging & Stack Trace decoding
  - Accessibility (a11y) refactoring
  - React/Vue Frontend Re-render optimization
  - Race condition & Concurrency auditing
- **Instant Copy-to-Clipboard:** Get the exact prompt you need with a single click.
- **Example Use-Cases:** Every template comes with a "See Example" toggle, allowing you to see exactly how to fill out the bracketed `[VARIABLES]` and what output to expect.
- **Zero Dependencies:** Pure HTML, vanilla CSS, and raw JavaScript. Lightning-fast and infinitely customizable.

## 🚀 Live Demo

You can view the live site running directly on GitHub pages here:
👉 **[https://akashkendre1298.github.io/Prompt-Playbook/](https://akashkendre1298.github.io/Prompt-Playbook/)**

## 💻 Local Usage

Because the Prompt Playbook is built with vanilla web technologies and has absolutely zero build steps, using and modifying it is incredibly easy.

1. Clone the repository:
   ```bash
   git clone https://github.com/akashkendre1298/Prompt-Playbook.git
   ```
2. Navigate into the directory:
   ```bash
   cd Prompt-Playbook
   ```
3. Open `index.html` directly in your favorite browser.
   *(Or spin up a quick local server using `npx serve` or the VSCode Live Server extension).*

## 🧩 Adding Your Own Prompts

You can easily extend the library with your own prompt templates. Open `index.html`, locate the `PROMPTS` array (around line 625), and add a new object in this format:

```javascript
{
  tab: "coding",          // "prompt-craft", "coding", "productivity", or "creative"
  iconClass: "icon-code", // "icon-craft", "icon-code", "icon-prod", or "icon-creative"
  badge: "badge-code",    // badge color matching the tab
  badgeLabel: "coding",   
  icon: "⌖",             // Insert a cool unicode symbol
  title: "Your Prompt Title",
  desc: "A brief, one sentence description of what the prompt accomplishes.",
  template:`Paste your Prompt here. 
You can use [BRACKETS] for variables.`,
  examples:[
    { filled: "Write how the prompt looks when filled out by the user." }
  ]
}
```

## 🤝 Contributing

Have an amazing, hardcore engineering prompt that saves you hours of time? Feel free to submit a Pull Request to expand the playbook!

## 📜 License

This project is open-source and free to use. Modify it, share it, and use it to engineer better software!
