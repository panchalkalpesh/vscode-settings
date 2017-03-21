# Microsoft Visual Studio Code - Settings and Preferences



## settings.json
_Overwrite default and User settings_

```
{
  "editor.snippetSuggestions": "top"
}
```


## keybindings.json
_User defined key bindings_

```
[
{ "key": "ctrl+shift+a", "command": "HookyQR.beautify", "when": "editorFocus" },
{ "key": "ctrl+shift+w", "command":"editor.emmet.action.wrapWithAbbreviation", "when": "editorFocus" },
{ "key": "ctrl+shift+/", "command": "editor.action.blockComment", "when": "editorTextFocus && !editorReadonly" }
]

```
