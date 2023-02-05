# Real Intellij Light

Light theme for Visual Studio Code. It uses Intellij-light theme colors and looks almost the same.

![Preview](https://raw.githubusercontent.com/avin/real-intellij-light/master/assets/preview.png)


## Settings recommendations:

```json5
{
    // Theme
    "workbench.colorTheme": "Real IntelliJ Light",
  
    // Show scrollbars
    "editor.scrollbar.verticalScrollbarSize": 10,
    "editor.scrollbar.horizontalScrollbarSize": 10,
    "editor.scrollbar.vertical": "visible",
    "editor.scrollbar.horizontal": "visible",

    // Fonts
    "editor.fontFamily": "'JetBrains Mono'",
    "editor.fontWeight": "500",
    "editor.fontSize": 17,
    "editor.letterSpacing": -0.2,
    "editor.lineHeight": 1.25,

    // Menu
    "workbench.tree.indent": 24,
}
```

## Recommended extensions:

* [Duplicate selection or line](https://marketplace.visualstudio.com/items?itemName=geeebe.duplicate) - duplicate lines like in IntelliJ IDEA
* [JetBrains IDEA Icons](https://marketplace.visualstudio.com/items?itemName=Mostik.JetBrainsIcons) - icons like in IntelliJ IDEA
* [Numbered Bookmarks](https://marketplace.visualstudio.com/items?itemName=alefragnani.numbered-bookmarks) - bookmarks like in IntelliJ IDEA

## Hack internal CSS

Use [Custom CSS and JS Loader](https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-custom-css) with CSS:

```css
/* Disable animations */
.monaco-hover {
    animation: none;
}

/* Cursor on tabs like in IntelliJ IDEA */
.tabs-and-actions-container *,
.monaco-list * {
    cursor: default !important;
}

/* More highlighting active tab */
.tab.active {
    box-shadow: inset 0 -3px #4083c9;
}

/* Change UI font */
.windows {
    font-family: Verdana, sans-serif;
}
```