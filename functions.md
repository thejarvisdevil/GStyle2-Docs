# Functions

**This explains the `<::functions::>` you can use inside commands.**  
  
To use a function inside a command, add `<::function::>` anywhere in an argument for a command.  
**Example:**
```
text.create "Pack: <::pack.info.name::>" 1.0 10 10 Roboto titletext

# The arguments for text.create being [text, scale, x, y, font, id]
```
  
You can also use expressions inside functions **(IMPORTANT: You need to have spaces around the expression)**.  
**Example:** `< ::display.width:: / 2 >` = Gets the center of the screen width so you can place stuff there.  
  
**Full Example:**
```
text.create "Hello from <::pack.info.name::>" 1.0 < ::display.width:: / 2 > < ::display.height:: / 2 > bigFont hellotext
```

## List of functions

- `display` or `display.screen` -- returns `widthxheight`. Example: `1920x1080`.
- `display.width` -- the width of the screen. Example: `1920`.
- `display.height` -- the height of the screen. Example: `1080`.
- `pack` or `pack.name` -- the pack folder name (e.g. `testpack`).
- `pack.info.<key>` -- the value of `<key>` from `packs/<pack>/info.txt`.
  - Keys in `info.txt` are usually: `name`, `author`, `version`, `description`.
  - Example: `<::pack.info.name::>` -> `Test Pack`