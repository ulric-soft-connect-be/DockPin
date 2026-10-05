<p align="center">
  <img src="docs/icon.png" width="128" height="128" alt="DockPin icon">
</p>

<h1 align="center">DockPin</h1>

<p align="center">Keep your Mac’s Dock on the screen of your choice.</p>

<p align="center">
  <a href="https://github.com/ulric-soft-connect-be/DockPin/releases/latest"><b>⬇︎ Download DockPin</b></a>
</p>

<p align="center">
  <b>English</b> ·
  <a href="README.fr.md">Français</a> ·
  <a href="README.de.md">Deutsch</a> ·
  <a href="README.nl.md">Nederlands</a> ·
  <a href="README.es.md">Español</a> ·
  <a href="README.it.md">Italiano</a>
</p>

---

With several displays, macOS moves the Dock to whichever screen you push the pointer against at the bottom. DockPin stops that: the Dock stays on the screen you picked, and you can move it to another one with a keyboard shortcut and a click.

## Features

- **Lock the Dock on one screen.** On the other screens, the pointer stops just before the Dock edge, so the Dock never jumps. Edges shared by two screens stay crossable.
- **Pick the screen with a shortcut and a click.** Press **⌃⌥⌘D**, then click the screen you want. The Dock moves there and stays locked.
- **Allow extra screens** if you want the Dock to be able to go to more than one screen.
- **Move the Dock just this once.** Hold **⌥ Option** while pushing the pointer against the bottom of another screen.
- **Automatic return.** At startup, after sleep and when a screen is connected or disconnected, the Dock goes back to its screen.
- **Presentation mode** hides the Dock on every screen during screen sharing or meetings, then restores your setting.
- **Discreet.** No Dock icon (except while a DockPin window is open), and the menu bar icon can be hidden.
- **Six languages**: English, French, German, Dutch, Spanish, Italian. DockPin follows the macOS language by default; you can change it in the settings.

## Requirements

- macOS 13 Ventura or later, Apple silicon or Intel.
- System Settings › Desktop & Dock › **“Displays have separate Spaces”** turned on. Without it, macOS always keeps the Dock on the main screen.
- The Dock on the bottom, left or right edge.

## Installation

1. Download **DockPin-x.y.z.dmg** from the [latest release](https://github.com/ulric-soft-connect-be/DockPin/releases/latest).
2. Open the disk image and drag **DockPin** onto **Applications**.
3. Open DockPin from the Applications folder. DockPin is not yet notarized by Apple, so the first time macOS refuses to open it. Go to **System Settings › Privacy & Security**, scroll down, click **Open Anyway** next to the DockPin message, and confirm.
4. Give DockPin the **Accessibility** permission when asked (System Settings › Privacy & Security › Accessibility). DockPin needs it to hold the pointer back at the screen edges and to move the Dock. Locking starts as soon as the permission is granted.

## Choosing the Dock screen

- **Keyboard and mouse:** press **⌃⌥⌘D**. A veil appears on every screen with a preview of the Dock. Click the screen you want. **Esc** or a right-click cancels.
- **Settings window:** click a screen on the map, or choose it from the *Locked screen* list.
- **Menu bar icon:** *Dock Screen* submenu.

## Keyboard shortcuts

| Action | Default |
| --- | --- |
| Choose the Dock screen (then click) | ⌃⌥⌘D |
| Open settings | ⌃⌥⌘S |
| Turn locking on or off | — |
| Presentation mode | — |

Change them in **Settings › Keyboard Shortcuts**: click a shortcut and type the new combination (⌫ clears it, Esc cancels). A shortcut shown in red is already used by another app.

## Settings

- **Dock Screen:** map of your screens, locked screen, *Bring the Dock Back Now*.
- **Locking:** turn locking on or off, extra screens allowed, key to move the Dock temporarily (⌥ Option by default), automatic return.
- **Presentation Mode:** hide the Dock on every screen.
- **Keyboard Shortcuts:** see above.
- **General:** interface language, open at login, menu bar icon.

While a DockPin window is open (Settings, About), DockPin shows its menu in the macOS menu bar: *About DockPin*, *Settings…*, *Quit DockPin* and the *Help* menu, which opens this page. macOS only allows this for apps that have a Dock icon, so the icon appears temporarily and disappears when you close the window.

## Menu bar icon hidden?

Open DockPin again (Spotlight, Launchpad or Finder) or press **⌃⌥⌘S**: the settings window reappears.

## Automation

DockPin understands `dockpin://` links, usable from Shortcuts, scripts or the Terminal:

```bash
open "dockpin://pick"                 # choose the screen by clicking
open "dockpin://lock?screen=2"        # lock the Dock on screen 2 (numbered left to right)
open "dockpin://lock?screen=LG"       # … or by (partial) name, UUID, or "main"
open "dockpin://home"                 # bring the Dock back to the locked screen
open "dockpin://unlock"               # turn locking off (also: lock, toggle)
open "dockpin://presentation?on=1"    # presentation mode (0 to leave, no value toggles)
open "dockpin://language?code=fr"     # interface language (en, fr, de, nl, es, it, system)
open "dockpin://settings"             # also: dockpin://about
```

## Troubleshooting

- **The Dock still jumps to other screens.** Check that DockPin is turned on in System Settings › Privacy & Security › Accessibility. If it is on but locking still doesn’t work, remove DockPin from that list with the **−** button, then add it again.
- **The Dock doesn’t move to the screen I picked.** Check that “Displays have separate Spaces” is turned on (System Settings › Desktop & Dock), then log out and back in.
- **A shortcut doesn’t work.** It’s probably already used by another app (it appears in red in the settings). Choose another combination.

## Privacy

DockPin collects no data and makes no network connections. Links such as *Help* simply open in your browser.

## Uninstall

Quit DockPin (menu bar icon › *Quit DockPin*), move it from Applications to the Trash, then remove it from System Settings › Privacy & Security › Accessibility.

---

<p align="center"><sub>© 2026 Soft-Connect</sub></p>
