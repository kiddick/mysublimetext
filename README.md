### There is some stuff about sublimetext: some tips and tweaks


#### Search oprtion `Wrap`
It is very easy, so it allows perform cyclic navigation between search results.

If that option disabled we'll stuck up to top/bottom of document.

#### Clipboard copy/paste history
```
Ctrl+K, Ctrl+V
```

#### Delete to beginning of the line
```
Ctrl + Shift + Backspace
```

#### Delete to end of the line
```
Ctrl + K K (press K twice while Ctrl is pressed)
```

#### Go to mathing bracket
```
Ctrl + M
```

#### Select content in brackets
```
Ctrl + Shift + M
```

#### Insert new line before/after immediately
```
Crtl + Enter
Crtl + Shift + Enter
```

#### MoveTab to first/last position
For some reason there is no file with settings for `MoveTab` plugin.
So we need to use great [PackageResourceViewer](https://github.com/skuroda/PackageResourceViewer) package and manually edit default file with `sublime-keymap`. Just uncomment required fields. And enjoy tabs moving!

```
[
    // Uncomment to enable.
    // {
    //  "keys": ["ctrl+shift+end"],
    //  "command": "move_tab",
    //  "args": { "position": "999" }
    // },
    // {
    //  "keys": ["ctrl+shift+home"],
    //  "command": "move_tab",
    //  "args": { "position": "0" }
    // },
    {
        "keys": ["ctrl+shift+pageup"],
        "command": "move_tab",
        "args": { "position": "-1" }
    },
    {
        "keys": ["ctrl+shift+pagedown"],
        "command": "move_tab",
        "args": { "position": "+1" }
    }
]
```

#### Focus on sidebar
```
Ctrl + 0
```