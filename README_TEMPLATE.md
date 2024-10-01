# **[Design System Name]** Built.js Design System

Welcome to the **[Design System Name]** Design System. This design system provides a set of reusable components and styles, using [**[framework/external-library-name]**](**[external-link-toframework/external-library]**).

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)

## Overview

This design system includes:

- A customized `tailwind.config.ts` file for consistent design tokens and utility classes.
- A set of global styles in `globals.css` for typography, resets, and utility classes.
- Predefined components from [framework], ready to be used in your project.

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

```json title="" copy
"config": {
    "dependencies": {
        "**[npm-dependency-1-name]**", <--Replace with the required NPM dependencies
    },
    "devDependencies": {
        "**[npm-devdependency-1-name]**", <--Replace with the required NPM devDependencies
    }
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

## Usage
1. Set up **[framework/external-library-name]** in your project:
- Install the dependencies:
```bash copy
npm install -S **[npm-dependency-1-name]** <--Replace with the required NPM dependencies (seperated by spaces)
```
- Install the devDependencies:
```bash copy
npm install -D **[npm-devdependency-1-name]** <--Replace with the required NPM devDependencies (seperated by spaces)
```

2. Run the app:
```bash copy
npm run dev
```

## Contributing
If you’d like to contribute to this design system, please follow the guidelines in the [CONTRIBUTING.md](../CONTRIBUTING.md).