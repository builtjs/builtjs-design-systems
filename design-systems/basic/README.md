# Basic Built.js Design System

Welcome to the Basic Design System. This design system provides a set of reusable styles. It doesn't include a component library.

## Table of Contents

- [Overview](#overview)
- [Installation and usage](#installation)
- [Contributing](#contributing)

## Overview

This design system includes:

- A customized `tailwind.config.ts` file for consistent design tokens and utility classes.
- A set of global styles in `globals.css` for color, typography, corners and resets.

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

## Contributing

If you’d like to contribute to this design system, please follow the guidelines in the [CONTRIBUTING.md](../CONTRIBUTING.md).
