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
    "**/.DS_Store": true,
    "**/node_modules": true,
    "**/bower_components": true
  },
  "workbench.editor.enablePreview": true,
  "workbench.activityBar.visible": true,

  
  // Enable Font Ligatures
  "editor.fontFamily": "Fira Code",
  "editor.fontLigatures": true,
  
  // File explorer sort order (requires vscode ^1.15.0)
  "explorer.sortOrder": "type" // filesFirst | mixed | modified | type
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
{ "key": "ctrl+k ctrl+m", "command": "workbench.action.editor.changeLanguageMode" }
]

```
