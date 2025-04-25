# Vim-Style CapsLock+

English | [中文](README_zh-CN.md)

---

master branch: v3.0+

v2 branch: v2.x

[Docs](https://capslox.com/capslock-plus/en.html)

## New Vim-Style Key Mappings

This fork of CapsLock+ uses Vim-style key mappings for more intuitive navigation:

| Action | New Key | Original Key |
|--------|---------|--------------|
| Move cursor left | `CapsLock+h` | `CapsLock+s` |
| Move cursor down | `CapsLock+j` | `CapsLock+d` |
| Move cursor up | `CapsLock+k` | `CapsLock+e` |
| Move cursor right | `CapsLock+l` | `CapsLock+f` |
| Move cursor left by word | `CapsLock+b` | `CapsLock+a` |
| Move cursor right by word | `CapsLock+w` | `CapsLock+g` |
| Delete | `CapsLock+d` | `CapsLock+w` |
| Delete character | `CapsLock+x` | `CapsLock+r` |
| Copy to clipboard 1 | `CapsLock+q` | `CapsLock+c` |
| Cut to clipboard 1 | `CapsLock+c` | `CapsLock+x` |
| Paste from clipboard 1 | `CapsLock+m` | `CapsLock+v` |

More mappings can be found in the CapsLock+settings.ini file.

## How to run the source code?
1. Download and install [AutoHotkey (v1.1.+)](http://www.ahkscript.org/)
2. Clone the Capslock+ source code
3. Run `Capslock+.ahk`

## How to set a custom function to a hotkey?
1. There is a key function `keyFunc_example2` in demo.ahk.
2. Add below setting under the [Keys] section in `CapsLock+settings.ini`:
    `caps_f7=keyFunc_example2`
3. Save, reload Capslock+ (CapsLock+F5)
4. Press `CapsLock+F7` to invoke the function

* In order to avoid calling the internal functions, all the key functions are restricted to start with `keyfunc_`

An example here:

### Creating a Custom Function
Let's create a custom Listary launcher:

1. Copy the following code to `/userAHK/main.ahk`:
