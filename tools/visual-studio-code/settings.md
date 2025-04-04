---
description: >-
  Here are my VS Code settings in JSON format, set up to make development easier
  and boost productivity.
---

# Settings

```json
{
  // Clean and Minimalist
  "breadcrumbs.enabled": false,
  "diffEditor.ignoreTrimWhitespace": false,
  "editor.copyWithSyntaxHighlighting": false,
  "editor.fontFamily": "Fira Code",
  "editor.fontLigatures": true,
  "editor.formatOnSave": true,
  "editor.guides.bracketPairs": "active",
  "editor.inlineSuggest.enabled": true,
  "editor.linkedEditing": true,
  "editor.minimap.enabled": false,
  "editor.mouseWheelZoom": true,
  "editor.quickSuggestions": {
    "comments": "on",
    "strings": "on"
  },
  "editor.renderWhitespace": "none",
  "editor.scrollBeyondLastLine": false,
  "editor.smoothScrolling": true,
  "editor.stickyScroll.enabled": false,
  "editor.tabCompletion": "on",
  "editor.wordWrap": "on",
  "editor.wordWrapColumn": 120,
  "files.autoSave": "afterDelay",
  "files.insertFinalNewline": true,
  "files.trimFinalNewlines": true,
  "files.trimTrailingWhitespace": true,
  "search.collapseResults": "alwaysCollapse",
  "terminal.integrated.defaultProfile.windows": "Git Bash",
  "workbench.startupEditor": "none",
  "workbench.tree.enableStickyScroll": false,
  // Default Formatter
  "[html]": {
    "editor.defaultFormatter": "vscode.html-language-features",
    "editor.tabSize": 2
  },
  "[blade]": {
    // Extension: Laravel Blade formatter
    "editor.defaultFormatter": "shufo.vscode-blade-formatter"
  },
  "[css][javascript]": {
    // Extension: Prettier - Code formatter
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "prettier.printWidth": 80,
    "prettier.singleQuote": true,
    "prettier.tabWidth": 2
  },
  "[php]": {
    // Extension: PHP Intelephense
    "editor.defaultFormatter": "bmewburn.vscode-intelephense-client"
  },
  "[json][jsonc]": {
    "editor.defaultFormatter": "vscode.json-language-features"
  },
  "[markdown]": {
    // Extension: markdownlint
    "editor.defaultFormatter": "DavidAnson.vscode-markdownlint"
  },
  // Extension: CodeSnap
  "codesnap.transparentBackground": true,
  // Extension: DotENV
  "files.associations": {
    "*.env": "dotenv"
  },
  // Extension: Error Lens
  "errorLens.codeLensEnabled": true,
  // Extension: Laravel Blade formatter
  "bladeFormatter.format.indentSize": 2,
  "bladeFormatter.format.sortHtmlAttributes": "code-guide",
  "bladeFormatter.format.sortTailwindcssClasses": true,
  // Extension: markdownlint
  "markdownlint.config": {
    "MD033": false,
    "MD041": false
  },
  // Extension: Material Icon Theme
  "workbench.iconTheme": "material-icon-theme",
  // Extension: One Dark Pro
  "workbench.colorTheme": "One Dark Pro Flat",
  // Extension: PlantUML
  "plantuml.server": "http://www.plantuml.com/plantuml",
  // Extension: Todo Tree
  "todo-tree.highlights.enabled": false
}
```
