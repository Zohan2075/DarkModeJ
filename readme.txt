Pelase visit: https://www.studiospixels.com/dark-mode-j/

DarkModeJ — User Guide
======================

DarkModeJ applies a real-time dark-mode overlay to any window on your
desktop without modifying the target application.


GETTING STARTED
---------------
1. Launch DarkModeJ from the Start Menu (or run bin\DarkModeJGUI.exe).
   The app appears as an icon in the system tray and opens its Dashboard.

2. Apply dark mode to a window — two methods:

   a) Dashboard buttons:
      - Click "Light Mode" or "Hard Mode" in the Dashboard.
      - The status changes to SELECTING... (the Dashboard stays visible).
      - Click anywhere on the window you want to darken.
      - The overlay activates immediately.

   b) Keyboard hotkeys (works from any app, no need to open Dashboard):
      - Focus the window you want to darken.
      - Press Ctrl+Q for Light mode  OR  Ctrl+Shift+Q for Hard mode.
      - Press the same hotkey again on the same window to remove the overlay.

3. To disable the overlay:
   - Click "Disable" in the Dashboard,  OR
   - Right-click the tray icon and choose "Disable overlay",  OR
   - Press the active mode hotkey a second time on the same window.


OVERLAY MODES
-------------
  Light   BitBlt screen capture — client area only (no title bar).
          ~60 fps. Zero impact on the target application.
          Best for most apps.

  Hard    PrintWindow capture — full window including the title bar.
          ~30 fps. Slight impact on the target application.
          Use for GPU-accelerated apps (e.g. Windows Terminal) — Hard
          mode automatically falls back to screen-DC capture when
          PrintWindow returns blank content.


HOTKEYS
-------
  Ctrl+Q           Toggle Light mode on the focused window
  Ctrl+Shift+Q     Toggle Hard mode on the focused window
  Ctrl+Esc         Exit DarkModeJ entirely
  Esc              Hide the Dashboard (app stays running in the tray)


SYSTEM TRAY
-----------
  Left-click       Show / hide the Dashboard
  Right-click      Open tray menu:
                     Open Dashboard   — show the Dashboard window
                     Disable overlay  — turn off the current overlay
                     Exit             — quit DarkModeJ


SETTINGS
--------
  Open Settings from the Dashboard (gear icon or Settings button).
  - Launch DarkModeJ when Windows starts:
    Enable to have DarkModeJ start automatically with Windows.


NOTES
-----
  • Only one window can have an overlay active at a time.
  • DarkModeJ.exe (in bin\) is a command-line fallback for advanced users.
    Normal users should use DarkModeJGUI.exe (the tray application).
  • The translations warning during install can be safely ignored.
