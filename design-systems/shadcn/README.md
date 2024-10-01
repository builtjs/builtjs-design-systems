# ShadCN Built.js Design System

Welcome to the ShadCN Design System. This design system provides a set of reusable components and styles, using [ShadCN](https://ui.shadcn.com/).

## Table of Contents

- [Overview](#overview)
- [Installation and usage](#installation)
- [Contributing](#contributing)

## Overview

This design system includes:

- A customized `tailwind.config.ts` file for consistent design tokens and utility classes.
- A set of global styles in `globals.css` for typography, resets, and utility classes.
- Predefined components from [ShadCN](https://ui.shadcn.com/), ready to be used in your project.

## Installation

To install the design system into your Built.js plugin or theme, follow these steps:

1. Replace the code in your project's `tailwind.config.js` file with the code in [/tailwind.config.js](/tailwind.config.js).
2. In the `styles/index.css` replace the code beneath the plugin imports (if any) with the code in [/index.css](/index.css):

```css
@import "./plugins/plugin_one/index.css";
@import "./plugins/plugin_two/index.css";

/* Paste here */
```

3. Replace the code in your `styles/globals.css` file with the code in [/globals.css](/globals.css).
4. Copy this code into your `theme.json` or `plugin.json`:

```json copy
"config": {
    "dependencies": [
        "tailwindcss-animate",
        "class-variance-authority",
        "clsx",
        "tailwind-merge",
        "@radix-ui/react-icons"
    ]
}
```

If you're installing this into a theme, copy it into your `public/data/theme.json`:

```json title="public/data/theme.json" copy
{
  "theme": {
    "title": "Your Theme Name",
    ...,
    <-- Paste here
  }
}
```

Or if it's for a plugin, copy it into the `public/data/plugin.json` file:

```json title="public/data/plugin.json" copy
{
  "plugin": {
    "title": "Your Plugin Name",
    ...,
    <-- Paste here
  }
}
```

5. Set up and use ShadCN in your project:

- Add the following dependencies to your project:

```bash copy
npm install tailwindcss-animate class-variance-authority clsx tailwind-merge
```

- Add the `New York` icon libraries:

```bash copy
npm install @radix-ui/react-icons
```

## Contributing

If you’d like to contribute to this design system, please follow the guidelines in the [CONTRIBUTING.md](../CONTRIBUTING.md).
