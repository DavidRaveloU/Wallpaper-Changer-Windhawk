# Changelog

All notable changes to **Wallpaper Changer** are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-11-21

First release.

### Added

- **A wallpaper selector opened with a hotkey** (`Ctrl+Alt+P` by default). The wallpaper changes only
  when you confirm with **Enter** or a click, never while you browse.
- **Several monitors.** The selector opens on the monitor with the mouse or with the focused window
  (**Open the selector on**). The wallpaper and the transition go to every monitor, or only to the
  one the selector opened on with **Only change the current monitor**.
- **Three styles**, chosen with the **Style** setting: *Card carousel* (a fan of overlapping cards),
  *Folder strip* (slanted cards, folders first) and *Showcase* (a big preview over a dimmed copy of
  itself, with a rail of thumbnails).
- **Transitions** that play over the desktop while the wallpaper changes, chosen with the
  **Transition** setting: *Card expand* (the card you picked grows until it covers the monitor, the
  default), *Blinds*, *Pixelate* and *Tile wave*, plus *Random* and *None*.
- **Collections.** Every subfolder of your wallpapers folder is a collection, plus **All**. Switch with
  **Tab**, the tabs or chips, or by opening a folder in the Folder strip. **F5** rescans the folder.
- **Keyboard, mouse and drag navigation**: arrow keys, `Home` and `End`, the mouse wheel and dragging.
  **Esc** and clicking another window close the selector without changing anything.
- **Forgiving settings.** The wallpapers folder accepts the quotes Explorer's "Copy as path" adds,
  `%VARIABLES%`, forward slashes and the `\\?\` prefix. An invalid hotkey is ignored and logged.
- Thumbnails are decoded on a low-priority background thread, and scanning, decoding and applying never
  block `explorer.exe` or let an exception escape it.
