# Microsoft Visual Studio Code - Settings and Preferences



## settings.json
_Overwrite default and User settings_

```
{
  "window.zoomLevel": 0,
  "window.title": "${dirty}${activeEditorMedium}${separator}${rootName}${separator}${appName}",
  "editor.formatOnPaste": false,
  "editor.wordWrap": "on",
  "editor.snippetSuggestions": "top",
  "files.exclude": {
    "**/.git": true,
    "**/.svn": true,
    "**/.hg": true,
    "**/CVS": true,
    "**/.DS_Store": true,
    "**/node_modules": true,
    "**/bower_components": true
  },
  "workbench.editor.enablePreview": true,
  "workbench.activityBar.visible": true,

  // Enable / Disable Telemetry Reporting
  "telemetry.enableTelemetry": false,
  
  // Enable Font Ligatures
  "editor.fontFamily": "Fira Code",
  "editor.fontLigatures": true,
  
  // File explorer sort order (requires vscode ^1.15.0)
  "explorer.sortOrder": "type", // filesFirst | mixed | modified | type
  
  // IndentGuide color customization (requires vscode ^1.23.0)
  "workbench.colorCustomizations": {
    "editorIndentGuide.activeBackground": "#aaa"
  },  
  
  # Indentation
  "editor.autoIndent": true,
  "editor.detectIndentation": true,
  "editor.tabSize": 2,
  "editor.insertSpaces": false,
  
  
  // Terminal Configurations
  "terminal.integrated.fontWeight": "100",
  
  // Additional Terminal Configurations
  // Controls the font family of the terminal, this defaults to editor.fontFamily's value.
  // "terminal.integrated.fontFamily": "",
  // Controls the font size in pixels of the terminal.
  // "terminal.integrated.fontSize": 14,
  // The font weight to use within the terminal for non-bold text.
  // "terminal.integrated.fontWeight": "normal",
  // The font weight to use within the terminal for bold text.
  // "terminal.integrated.fontWeightBold": "bold",
  // Controls the letter spacing of the terminal, this is an integer value which represents the amount of additional pixels to add between characters.
  // "terminal.integrated.letterSpacing": 0,
  // Controls the line height of the terminal, this number is multiplied by the terminal font size to get the actual line-height in pixels.
  // "terminal.integrated.lineHeight": 1,
  
  # Extension Configurations
  # wayou.vscode-todo-highlight
  "todohighlight.keywords": [
        {
            "text": "DONE:",
            "color": "#ffffff",
            "backgroundColor": "green"
        },
        {
            "text": "BACKLOG:",
            "color": "#ffffff",
            "backgroundColor": "gray"
        }
    ],

  # Editor actions on save
  "editor.codeActionsOnSave": {
      "source.organizeImports": true
  }

}
```


## keybindings.json
_User defined key bindings_

```
[
{ "key": "ctrl+shift+a", "command": "HookyQR.beautify", "when": "editorFocus" },
{ "key": "ctrl+shift+w", "command":"editor.emmet.action.wrapWithAbbreviation", "when": "editorFocus" },
{ "key": "ctrl+shift+/", "command": "editor.action.blockComment", "when": "editorTextFocus && !editorReadonly" },
{ "key": "ctrl+shift+v", "command": "editor.action.clipboardPasteAction", "when": "editorTextFocus && !editorReadonly" },
{ "key": "ctrl+shift+l", "command": "editor.action.insertCursorAtEndOfEachLineSelected", "when": "editorTextFocus" },
{ "key": "ctrl+k u", "command": "editor.action.transformToUppercase", "when": "editorTextFocus" },
{ "key": "ctrl+k l", "command": "editor.action.transformToLowercase", "when": "editorTextFocus" },
{ "key": "ctrl+l", "command": "workbench.action.gotoSymbol" },
{ "key": "ctrl+shift+o", "command": "workbench.action.gotoSymbol" },
{ "key": "f7", "command": "workbench.action.navigateEditorGroups" },
{ "key": "ctrl+k ctrl+m", "command": "workbench.action.editor.changeLanguageMode" },
{ "key": "shift+alt+left", "command": "editor.action.smartSelect.grow", "when": "editorTextFocus" },
{ "key": "shift+alt+right", "command": "-editor.action.smartSelect.grow", "when": "editorTextFocus" },
{ "key": "shift+alt+right", "command": "editor.action.smartSelect.shrink", "when": "editorTextFocus" },
{ "key": "shift+alt+left", "command": "-editor.action.smartSelect.shrink", "when": "editorTextFocus" },
{ "key": "ctrl+shift+`", "command": "workbench.action.terminal.toggleTerminal" }
]

```
