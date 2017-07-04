# SublimeText3Setup

## Layout
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

## Key bindings
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
    },
    { 
        "keys": ["ctrl+/"],
        "command": "toggle_comment",
        "args": {
            "block": false
        } 
    },
    {
        "keys": ["ctrl+shift+/"],
        "command": "toggle_comment",
        "args": {
            "block": true
        }
    },
    { 
        "keys"    : ["f5"], 
        "command" : "refresh_folder_list" 
    }
]
```

## User Settings
```json
{
    "always_show_minimap_viewport": true,
    "bold_folder_labels": true,
    "color_scheme": "Packages/User/SublimeLinter/Material One Dark (SL).tmTheme",
    "font_face": "menlo",
    "font_options":
    [
        "gray_antialias",
        "subpixel_antialias"
    ],
    "font_size": 15,
    "ignored_packages":
    [
        "Vintage"
    ],
    "indent_guide_options":
    [
        "draw_normal",
        "draw_active"
    ],
    "line_padding_bottom": 3,
    "line_padding_top": 3,
    "material_theme_big_fileicons": true,
    "material_theme_bold_tab": true,
    "material_theme_bright_scrollbars": true,
    "material_theme_small_statusbar": true,
    "material_theme_tree_headings": true,
    "overlay_scroll_bars": "enabled",
    "theme": "Material-Theme-Darker.sublime-theme"
}
```

## Serial

```
—– BEGIN LICENSE —–
Michael Barnes
Single User License
EA7E-821385
8A353C41 872A0D5C DF9B2950 AFF6F667
C458EA6D 8EA3C286 98D1D650 131A97AB
AA919AEC EF20E143 B361B1E7 4C8B7F04
B085E65E 2F5F5360 8489D422 FB8FC1AA
93F6323C FD7F7544 3F39C318 D95E6480
FCCC7561 8A4A1741 68FA4223 ADCEDE07
200C25BE DBBC4855 C4CFB774 C5EC138C
0FEC1CEF D9DCECEC D3A5DAD1 01316C36
—— END LICENSE ——
```