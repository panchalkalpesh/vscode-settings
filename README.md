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
  
  # Terminal Configurations
  "terminal.integrated.fontWeight": "100",
  
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
    ]

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
