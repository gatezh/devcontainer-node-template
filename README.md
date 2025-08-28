# Devcontainer node template

> ℹ️ Using current LTS version `22.18.0`
Minimal template repo containing only a `.devcontainer` that boots an **Alpine** image with **node** installed.
`NODE_VERSION` is set in the Dockerfile as:

```
ARG NODE_VERSION=22.18.0
```



## Purpose

Starter container for creating Node apps (React, Vite, Next, etc.) — safe, fast, minimal.



## Quick start

1. Clone this repo.
  > The most convenient way is to use `gh`: 
  > ```
  > gh repo create my-node-project --template gatezh/devcontainer-node-template --private --clone
  > ```
  > This will create a private GitHub repository name `my-node-project` and clone it to your local machine
2. Open in VS Code and choose **Reopen in Container** (or use *Remote - Containers*).
3. The container installs node (version defined by `ARG NODE_VERSION`) and the listed extensions.



## Change node version

Edit the Dockerfile `ARG NODE_VERSION=...` and rebuild the container.



## VS Code extensions (auto-installed via `customizations.vscode.extensions`)



```
// **General**
// Prettier - Code Formatter - General code formatting
"esbenp.prettier-vscode",
// Code Spell Checker - Spell checking
"streetsidesoftware.code-spell-checker",
// YAML - YAML support
"redhat.vscode-yaml",
// Markdown Preview Github Styles - Markdown preview
"bierner.markdown-preview-github-styles",

// **JS**
// ESLint - JavaScript linting
"dbaeumer.vscode-eslint",
// NPM Intellisense - NPM package intellisense
"christian-kohler.npm-intellisense",
// TS Error Translator - Translates TypeScript errors into readable suggestions
"mattpocock.ts-error-translator",

// **CSS**
// Color Info - Provides color information (names, values)
"bierner.color-info",
// Colorize - Colorizes code with visual swatches
"kamikillerto.vscode-colorize",
// Tailwind Fold - Fold Tailwind utility classes for readability
"stivo.tailwind-fold",
// Tailwind CSS IntelliSense - Tailwind CSS completions & linting
"bradlc.vscode-tailwindcss"
```
