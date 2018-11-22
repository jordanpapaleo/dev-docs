# Key bindings

Create a custom key map file in VSC and add the following

```json
[
  {
    "key": "shift+backspace",
    "command": "editor.action.deleteLines",
    "when": "editorTextFocus"
  },
  {
    "key": "shift+delete",
    "command": "editor.action.deleteLines",
    "when": "editorTextFocus"
  },
  {
    "key": "alt+cmd+/",
    "command": "editor.action.blockComment",
    "when": "editorTextFocus"
  },
  {
    "key": "cmd+shift+up",
    "command": "editor.action.moveLinesUpAction",
    "when": "editorTextFocus"
  },
  {
    "key": "cmd+shift+down",
    "command": "editor.action.moveLinesDownAction",
    "when": "editorTextFocus"
  },
  {
    "key": "cmd+shift+j",
    "command": "editor.action.joinLines"
  },
  {
    "key": "shift+cmd+d",
    "command": "editor.action.copyLinesDownAction",
    "when": "editorTextFocus"
  },
  {
    "key": "f5",
    "command": "editor.action.sortLinesAscending"
  },
  {
    "key": "cmd+v",
    "command": "pasteAndIndent.action",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "cmd+v",
    "command": "editor.action.clipboardPasteAction",
    "when": "!editorTextFocus"
  },
  {
    "key": "cmd+shift+v",
    "command": "editor.action.clipboardPasteAction",
    "when": "editorTextFocus && !editorReadonly"
  }
]

```
