# SublimeText3Setup

##Layout
On Linux save the file `Main.sublime-menu` in
`~/.config/sublime-text-3/Packages/User/Main.sublime-menu`
```json
[{
    "id": "view",
    "children": [{
        "id": "layout",
        "children": [{
            "command": "set_layout",
            "caption" : "Custom: 1 Pane (1C 2R)",
            "keys": ["super+alt+shift+5"],
            "args":
            {
                "cols": [0.0, 0.5, 1.0],
                "rows": [0.0, 0.5, 1.0],
                "cells":
                [
                    [0, 0, 1, 2], [1, 0, 2, 1],
                    [1, 1, 2, 2]
                ]
            }
        },
        {
            "command": "set_layout",
            "caption" : "Custom: 2 Pane (2R 1C)",
            "keys": ["super+alt+shift+6"],
            "args":
            {
                "cols": [0.0, 0.5, 1.0],
                "rows": [0.0, 0.5, 1.0],
                "cells":
                [
                    [0, 0, 1, 1], [1, 0, 2, 2],
                    [0, 1, 1, 2]
                ]
            }
        },
        {
            "command": "set_layout",
            "caption" : "Custom: 3 Pane (2R 1C 1C)",
            "keys": ["super+alt+shift+7"],
            "args":
            {
                "cols": [0.0, 0.44, 0.72, 1.0],
                "rows": [0.0, 0.5, 1.0],
                "cells":
                [
                    [0, 0, 1, 1],
                    [0, 1, 1, 2],
                    [1, 0, 2, 2],
                    [2, 0, 3, 2]
                ]
            }
        },
        {
            "command": "set_layout",
            "caption" : "Custom: 4 Pane (2T 1B)",
            "mnemonic": "C",
            "args": {
                "cols": [0.0, 0.5, 1.0],
                "rows": [0.0, 0.5, 1.0],
                "cells": [
                    [0, 0, 1, 1],
                    [1, 0, 2, 1],
                    [0, 1, 2, 2]
                ]
            }
        },
        {
            "command": "set_layout",
            "caption" : "Custom: 5 Pane (1T 2B)",
            "mnemonic": "C",
            "args": {
                "cols": [0.0, 0.5, 1.0],
                "rows": [0.0, 0.5, 1.0],
                "cells": [
                    [0, 0, 2, 1],
                    [0, 1, 1, 2],
                    [1, 1, 2, 2]
                ]
            }
        }]
    }]
}]
```

##Key bindings
```json
[
    {
        "keys": ["ctrl+shift+y"],
        "command": "unexpand_tabs",
        "args": {
            "set_translate_tabs": true
        }
    },
    {
        "keys": ["ctrl+alt+y"],
        "command": "expand_tabs",
        "args": {
            "set_translate_tabs": true
        }
    },
    {
        "keys": ["ctrl+alt+k"],
        "command": "delete_trailing_spaces"
    },

    {
        "keys": ["alt+shift+f"],
        "command": "reindent",
        "args": {
            "single_line": false
        }
    },
    {
        "keys": ["ctrl+k", "ctrl+j"],
        "command": "title_case"
    },
    {
        "keys": ["ctrl+shift+w"],
        "command": "toggle_setting",
        "args": {
            "setting": "word_wrap"
        }
    }
]
```


