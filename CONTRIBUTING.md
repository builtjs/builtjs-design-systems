# Contributing to the Design Systems Repository

Thank you for your interest in contributing! Please take a moment to read through the following guidelines before submitting your contribution.

## Table of Contents

- [Getting Started](#getting-started)
- [Creating a New Branch](#creating-a-new-branch)
- [Tailwind Configuration](#tailwind-configuration)
- [Styles Directory](#styles-directory)
- [Testing Your Changes](#testing-your-changes)
- [Creating a Pull Request](#creating-a-pull-request)
- [Code of Conduct](#code-of-conduct)

## Getting Started

1. Fork this repository to your own GitHub account.
2. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/[your-username]/builtjs-design-systems.git
   ```
## Creating a New Branch
To create a new version of a design system:
1. Branch naming convention: Follow this naming format when creating a new branch:
```
[design-system-name]_[version]
```
Example:
```
shadcn_0.1.0
```
2. To create and switch to your new branch:
 ```bash
git checkout -b [design-system-name]_[version]
```
## Creating a new design system
To create a new design system, create a new folder in the ```design-systems``` with the name of your design system (lowercase with dashes). Include a ```README.md``` file to introduce the design system.

## Tailwind Configuration
Each design system should include a ```tailwind.config.ts``` file. This file defines the custom configurations for TailwindCSS, including theme extensions, variants, and plugins.

1. Ensure that your ```tailwind.config.ts``` file follows the project standards.
2. Test your configurations to ensure compatibility across different styles and components.

## Styles Directory
Each design system should contain a ```styles``` directory, which should include the following:

- ```index.css```: This file should import all the necessary styles for the design system.
- ```globals.css```: This file should include global styles such as typography, resets, or any custom utility classes.

## Testing Your Changes
Before submitting a pull request:

1. Run the design system locally in your Built.js theme or plugin to ensure your changes work as expected.
2. Verify that there are no errors in your styles or configuration files.
3. Ensure that your design system is compatible and doesn't break functionality.

# Creating a Pull Request
Once you're ready to submit your changes:

1. Push your branch to your fork:

```bash
git push origin [design-system-name]_[version]
```

2. Open a pull request from your fork to the main repository:

- Base branch: ```main```
- Compare branch: ```[design-system-name]_[version]```

Include the following information in your pull request description:

- A summary of the changes you made.
- Why these changes are needed or what issues they address.
- Any additional context or instructions for testing.

3. Your pull request will be reviewed by one or more maintainers. We may ask for changes before merging, so please be prepared to respond to feedback.

## Code of Conduct
We expect all contributors to foster an inclusive, welcoming, and respectful environment.