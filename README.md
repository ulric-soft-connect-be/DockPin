<p align="center">
  <img src="docs/icon.png" width="128" height="128" alt="DockPin icon">
</p>

<h1 align="center">DockPin</h1>

<p align="center">
  Keep your Mac’s Dock on the screen of your choice.<br>
  Gardez le Dock de votre Mac sur l’écran de votre choix.
</p>

<p align="center">
  <a href="https://github.com/ulric-soft-connect-be/DockPin/releases/latest"><b>⬇︎ Download / Télécharger</b></a>
  &nbsp;·&nbsp; <a href="#english">English</a>
  &nbsp;·&nbsp; <a href="#français">Français</a>
</p>

---

## English

With several displays, macOS moves the Dock to whichever screen you push the pointer against at the bottom. DockPin stops that: the Dock stays on the screen you picked, and you can move it to another one with a keyboard shortcut and a click.

### Features

- **Lock the Dock on one screen.** On the other screens, the pointer stops just before the Dock edge, so the Dock never jumps. Edges shared by two screens stay crossable.
- **Pick the screen with a shortcut and a click.** Press **⌃⌥⌘D**, then click the screen you want. The Dock moves there and stays locked.
- **Allow extra screens** if you want the Dock to be able to go to more than one screen.
- **Move the Dock just this once.** Hold **⌥ Option** while pushing the pointer against the bottom of another screen.
- **Automatic return.** At startup, after sleep and when a screen is connected or disconnected, the Dock goes back to its screen.
- **Presentation mode** hides the Dock on every screen during screen sharing or meetings, then restores your setting.
- **Discreet.** No Dock icon (except while the settings window is open), and the menu bar icon can be hidden.
- **Six languages**: English, French, German, Dutch, Spanish, Italian. DockPin follows the macOS language by default; you can change it in the settings.

### Requirements

- macOS 13 Ventura or later, Apple silicon or Intel.
- System Settings › Desktop & Dock › **“Displays have separate Spaces”** turned on. Without it, macOS always keeps the Dock on the main screen.
- The Dock on the bottom, left or right edge.

### Installation

1. Download **DockPin-x.y.z.dmg** from the [latest release](https://github.com/ulric-soft-connect-be/DockPin/releases/latest).
2. Open the disk image and drag **DockPin** onto **Applications**.
3. Open DockPin from the Applications folder. DockPin is not yet notarized by Apple, so the first time macOS refuses to open it. Go to **System Settings › Privacy & Security**, scroll down, click **Open Anyway** next to the DockPin message, and confirm.
4. Give DockPin the **Accessibility** permission when asked (System Settings › Privacy & Security › Accessibility). DockPin needs it to hold the pointer back at the screen edges and to move the Dock. Locking starts as soon as the permission is granted.

### Choosing the Dock screen

- **Keyboard and mouse:** press **⌃⌥⌘D**. A veil appears on every screen with a preview of the Dock. Click the screen you want. **Esc** or a right-click cancels.
- **Settings window:** click a screen on the map, or choose it from the “Locked screen” list.
- **Menu bar icon:** *Dock Screen* submenu.

### Keyboard shortcuts

| Action | Default |
| --- | --- |
| Choose the Dock screen (then click) | ⌃⌥⌘D |
| Open settings | ⌃⌥⌘S |
| Turn locking on or off | — |
| Presentation mode | — |

Change them in **Settings › Keyboard Shortcuts**: click a shortcut and type the new combination (⌫ clears it, Esc cancels). A shortcut shown in red is already used by another app.

### Settings

- **Dock Screen:** map of your screens, locked screen, *Bring the Dock Back Now*.
- **Locking:** turn locking on or off, extra screens allowed, key to move the Dock temporarily (⌥ Option by default), automatic return.
- **Presentation Mode:** hide the Dock on every screen.
- **Keyboard Shortcuts:** see above.
- **General:** interface language, open at login, menu bar icon.

While the settings window is open, DockPin shows its menu in the macOS menu bar (*About DockPin*, *Settings…*, *Quit DockPin*, *Help*). macOS only allows this for apps that have a Dock icon, so the icon appears temporarily and disappears when you close the window.

### Menu bar icon hidden?

Open DockPin again (Spotlight, Launchpad or Finder) or press **⌃⌥⌘S**: the settings window reappears.

### Automation

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

### Troubleshooting

- **The Dock still jumps to other screens.** Check that DockPin is turned on in System Settings › Privacy & Security › Accessibility. After an update, remove DockPin from that list with the **−** button, then add it again.
- **The Dock doesn’t move to the screen I picked.** Check that “Displays have separate Spaces” is turned on (System Settings › Desktop & Dock), then log out and back in.
- **A shortcut doesn’t work.** It’s probably already used by another app (it appears in red in the settings). Choose another combination.

### Privacy

DockPin collects no data and makes no network connections. Links such as *Help* simply open in your browser.

### Uninstall

Quit DockPin (menu bar icon › *Quit DockPin*), move it from Applications to the Trash, then remove it from System Settings › Privacy & Security › Accessibility.

---

## Français

Avec plusieurs écrans, macOS déplace le Dock sur l’écran dont vous poussez le bas avec le curseur. DockPin l’en empêche : le Dock reste sur l’écran choisi, et vous pouvez le déplacer vers un autre écran avec un raccourci clavier et un clic.

### Fonctions

- **Verrouiller le Dock sur un écran.** Sur les autres écrans, le curseur s’arrête juste avant le bord du Dock : celui-ci ne saute plus. Les bords partagés entre deux écrans restent franchissables.
- **Choisir l’écran avec un raccourci et un clic.** Pressez **⌃⌥⌘D**, puis cliquez sur l’écran voulu. Le Dock s’y déplace et y reste verrouillé.
- **Autoriser d’autres écrans** si vous voulez que le Dock puisse aller sur plusieurs écrans.
- **Déplacer le Dock ponctuellement.** Maintenez **⌥ Option** en poussant le curseur en bas d’un autre écran.
- **Retour automatique.** Au démarrage, au réveil et au branchement ou débranchement d’un écran, le Dock revient sur son écran.
- **Mode présentation** : masque le Dock sur tous les écrans pendant un partage d’écran ou une réunion, puis rétablit votre réglage.
- **Discret.** Pas d’icône dans le Dock (sauf pendant que la fenêtre de réglages est ouverte), et l’icône de la barre des menus peut être masquée.
- **Six langues** : anglais, français, allemand, néerlandais, espagnol, italien. DockPin suit la langue de macOS par défaut ; vous pouvez la changer dans les réglages.

### Prérequis

- macOS 13 Ventura ou plus récent, Mac Apple silicon ou Intel.
- Réglages Système › Bureau et Dock › **« Les écrans disposent d’espaces distincts »** activé. Sans cela, macOS garde toujours le Dock sur l’écran principal.
- Le Dock en bas, à gauche ou à droite de l’écran.

### Installation

1. Téléchargez **DockPin-x.y.z.dmg** depuis la [dernière version](https://github.com/ulric-soft-connect-be/DockPin/releases/latest).
2. Ouvrez l’image disque et glissez **DockPin** sur **Applications**.
3. Ouvrez DockPin depuis le dossier Applications. DockPin n’est pas encore notarisé par Apple : la première fois, macOS refuse de l’ouvrir. Allez dans **Réglages Système › Confidentialité et sécurité**, faites défiler, cliquez sur **Ouvrir quand même** à côté du message concernant DockPin, puis confirmez.
4. Accordez l’autorisation **Accessibilité** quand elle est demandée (Réglages Système › Confidentialité et sécurité › Accessibilité). DockPin en a besoin pour retenir le curseur au bord des écrans et pour déplacer le Dock. Le verrouillage démarre dès que l’accès est accordé.

### Choisir l’écran du Dock

- **Clavier et souris :** pressez **⌃⌥⌘D**. Un voile apparaît sur chaque écran avec un aperçu du Dock. Cliquez sur l’écran voulu. **Échap** ou un clic droit annule.
- **Fenêtre de réglages :** cliquez sur un écran du plan, ou choisissez-le dans la liste « Écran verrouillé ».
- **Icône de la barre des menus :** sous-menu *Écran du Dock*.

### Raccourcis clavier

| Action | Par défaut |
| --- | --- |
| Choisir l’écran du Dock (puis clic) | ⌃⌥⌘D |
| Ouvrir les réglages | ⌃⌥⌘S |
| Activer / désactiver le verrouillage | — |
| Mode présentation | — |

Modifiez-les dans **Réglages › Raccourcis clavier** : cliquez sur un raccourci et tapez la nouvelle combinaison (⌫ efface, Échap annule). Un raccourci affiché en rouge est déjà utilisé par une autre app.

### Réglages

- **Écran du Dock :** plan de vos écrans, écran verrouillé, *Ramener le Dock maintenant*.
- **Verrouillage :** activation, écrans supplémentaires autorisés, touche pour déplacer le Dock ponctuellement (⌥ Option par défaut), retour automatique.
- **Mode présentation :** masquer le Dock sur tous les écrans.
- **Raccourcis clavier :** voir ci-dessus.
- **Général :** langue de l’interface, ouverture à la connexion, icône de la barre des menus.

Pendant que la fenêtre de réglages est ouverte, DockPin affiche son menu dans la barre des menus de macOS (*À propos de DockPin*, *Réglages…*, *Quitter DockPin*, *Aide*). macOS ne le permet qu’aux apps qui ont une icône dans le Dock : l’icône apparaît donc le temps que la fenêtre est ouverte, puis disparaît.

### Icône de la barre des menus masquée ?

Rouvrez DockPin (Spotlight, Launchpad ou Finder) ou pressez **⌃⌥⌘S** : la fenêtre de réglages réapparaît.

### Automatisation

DockPin comprend les liens `dockpin://`, utilisables depuis Raccourcis, des scripts ou le Terminal :

```bash
open "dockpin://pick"                 # choisir l’écran en cliquant
open "dockpin://lock?screen=2"        # caler le Dock sur l’écran n° 2 (numérotés de gauche à droite)
open "dockpin://lock?screen=LG"       # … ou par nom (partiel), UUID, ou « main »
open "dockpin://home"                 # ramener le Dock sur l’écran verrouillé
open "dockpin://unlock"               # désactiver le verrouillage (aussi : lock, toggle)
open "dockpin://presentation?on=1"    # mode présentation (0 pour en sortir, sans valeur = bascule)
open "dockpin://language?code=fr"     # langue de l’interface (en, fr, de, nl, es, it, system)
open "dockpin://settings"             # aussi : dockpin://about
```

### Dépannage

- **Le Dock saute encore sur les autres écrans.** Vérifiez que DockPin est activé dans Réglages Système › Confidentialité et sécurité › Accessibilité. Après une mise à jour, retirez DockPin de cette liste avec le bouton **−**, puis ajoutez-le de nouveau.
- **Le Dock ne va pas sur l’écran choisi.** Vérifiez que « Les écrans disposent d’espaces distincts » est activé (Réglages Système › Bureau et Dock), puis fermez et rouvrez votre session.
- **Un raccourci ne fonctionne pas.** Il est sans doute déjà utilisé par une autre app (il apparaît en rouge dans les réglages). Choisissez une autre combinaison.

### Confidentialité

DockPin ne collecte aucune donnée et n’établit aucune connexion réseau. Les liens comme *Aide* s’ouvrent simplement dans votre navigateur.

### Désinstallation

Quittez DockPin (icône de la barre des menus › *Quitter DockPin*), placez-le de Applications à la corbeille, puis retirez-le de Réglages Système › Confidentialité et sécurité › Accessibilité.

---

<p align="center"><sub>© 2026 Soft-Connect</sub></p>
