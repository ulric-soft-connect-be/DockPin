<p align="center">
  <img src="docs/icon.png" width="128" height="128" alt="DockPin-Symbol">
</p>

<h1 align="center">DockPin</h1>

<p align="center">Halte das Dock deines Mac auf dem Bildschirm deiner Wahl.</p>

<p align="center">
  <a href="https://github.com/ulric-soft-connect-be/DockPin/releases/latest"><b>⬇︎ DockPin laden</b></a>
</p>

<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.fr.md">Français</a> ·
  <b>Deutsch</b> ·
  <a href="README.nl.md">Nederlands</a> ·
  <a href="README.es.md">Español</a> ·
  <a href="README.it.md">Italiano</a>
</p>

---

Bei mehreren Bildschirmen bewegt macOS das Dock auf den Bildschirm, an dessen unteren Rand du den Zeiger schiebst. DockPin verhindert das: Das Dock bleibt auf dem gewählten Bildschirm, und du kannst es mit einem Tastaturkurzbefehl und einem Klick auf einen anderen bewegen.

## Funktionen

- **Dock auf einem Bildschirm sperren.** Auf den anderen Bildschirmen stoppt der Zeiger kurz vor dem Dock-Rand, sodass das Dock nicht mehr springt. Ränder, die zwei Bildschirme gemeinsam haben, bleiben passierbar.
- **Bildschirm per Kurzbefehl und Klick wählen.** Drücke **⌃⌥⌘D** und klicke auf den gewünschten Bildschirm. Das Dock wandert dorthin und bleibt gesperrt.
- **Weitere Bildschirme erlauben**, wenn das Dock auf mehr als einen Bildschirm wechseln darf.
- **Dock einmalig bewegen.** Halte **⌥ Wahltaste** gedrückt und schiebe den Zeiger an den unteren Rand eines anderen Bildschirms.
- **Automatische Rückkehr.** Beim Start, nach dem Ruhezustand und wenn ein Bildschirm angeschlossen oder getrennt wird, kehrt das Dock auf seinen Bildschirm zurück.
- **Präsentationsmodus**: blendet das Dock während einer Bildschirmfreigabe oder eines Meetings auf allen Bildschirmen aus und stellt danach deine Einstellung wieder her.
- **Unauffällig.** Kein Symbol im Dock (außer solange ein DockPin-Fenster geöffnet ist), und das Menüleistensymbol lässt sich ausblenden.
- **Sechs Sprachen**: Englisch, Französisch, Deutsch, Niederländisch, Spanisch, Italienisch. DockPin folgt standardmäßig der Sprache von macOS; in den Einstellungen kannst du sie ändern.

## Voraussetzungen

- macOS 13 Ventura oder neuer, Mac mit Apple Chip oder Intel.
- Systemeinstellungen › Schreibtisch & Dock › **„Monitore verwenden verschiedene Spaces“** eingeschaltet. Ohne diese Option lässt macOS das Dock immer auf dem Hauptbildschirm.
- Das Dock am unteren, linken oder rechten Bildschirmrand.

## Installation

1. Lade **DockPin-x.y.z.dmg** aus der [neuesten Version](https://github.com/ulric-soft-connect-be/DockPin/releases/latest).
2. Öffne das Image und ziehe **DockPin** auf **Programme**.
3. Öffne DockPin im Ordner „Programme“. DockPin ist noch nicht von Apple notariell beglaubigt, daher verweigert macOS beim ersten Mal das Öffnen. Gehe zu **Systemeinstellungen › Datenschutz & Sicherheit**, scrolle nach unten, klicke neben der Meldung zu DockPin auf **Dennoch öffnen** und bestätige.
4. Erteile DockPin die Berechtigung für **Bedienungshilfen**, wenn du dazu aufgefordert wirst (Systemeinstellungen › Datenschutz & Sicherheit › Bedienungshilfen). DockPin braucht sie, um den Zeiger an den Bildschirmrändern zurückzuhalten und das Dock zu bewegen. Die Sperre startet, sobald die Berechtigung erteilt ist.

## Dock-Bildschirm wählen

- **Tastatur und Maus:** Drücke **⌃⌥⌘D**. Auf jedem Bildschirm erscheint eine Abdeckung mit einer Vorschau des Docks. Klicke auf den gewünschten Bildschirm. **Esc** oder ein Rechtsklick bricht ab.
- **Einstellungsfenster:** Klicke auf einen Bildschirm im Plan oder wähle ihn in der Liste *Gesperrter Bildschirm*.
- **Menüleistensymbol:** Untermenü *Dock-Bildschirm*.

## Tastaturkurzbefehle

| Aktion | Standard |
| --- | --- |
| Dock-Bildschirm wählen (dann klicken) | ⌃⌥⌘D |
| Einstellungen öffnen | ⌃⌥⌘S |
| Sperre ein- oder ausschalten | — |
| Präsentationsmodus | — |

Ändere sie unter **Einstellungen › Tastaturkurzbefehle**: Klicke auf einen Kurzbefehl und tippe die neue Kombination (⌫ löscht, Esc bricht ab). Ein rot angezeigter Kurzbefehl wird bereits von einer anderen App verwendet.

## Einstellungen

- **Dock-Bildschirm:** Plan deiner Bildschirme, gesperrter Bildschirm, *Dock jetzt zurückholen*.
- **Sperre:** Sperre ein- und ausschalten, zusätzlich erlaubte Bildschirme, Taste zum vorübergehenden Bewegen des Docks (standardmäßig ⌥ Wahltaste), automatische Rückkehr.
- **Präsentationsmodus:** Dock auf allen Bildschirmen ausblenden.
- **Tastaturkurzbefehle:** siehe oben.
- **Allgemein:** Sprache der Oberfläche, beim Anmelden öffnen, Menüleistensymbol.

Solange ein DockPin-Fenster geöffnet ist (Einstellungen, Über), zeigt DockPin sein Menü in der macOS-Menüleiste: *Über DockPin*, *Einstellungen …*, *DockPin beenden* und das Menü *Hilfe*, das diese Seite öffnet. macOS erlaubt das nur Apps mit einem Dock-Symbol – das Symbol erscheint daher vorübergehend und verschwindet, wenn du das Fenster schließt.

## Menüleistensymbol ausgeblendet?

Öffne DockPin erneut (Spotlight, Launchpad oder Finder) oder drücke **⌃⌥⌘S**: Das Einstellungsfenster erscheint wieder.

## Automatisierung

DockPin versteht `dockpin://`-Links, nutzbar aus Kurzbefehlen, Skripten oder dem Terminal:

```bash
open "dockpin://pick"                 # Bildschirm per Klick wählen
open "dockpin://lock?screen=2"        # Dock auf Bildschirm 2 sperren (von links nach rechts nummeriert)
open "dockpin://lock?screen=LG"       # … oder per (Teil-)Name, UUID oder „main“
open "dockpin://home"                 # Dock auf den gesperrten Bildschirm zurückholen
open "dockpin://unlock"               # Sperre ausschalten (auch: lock, toggle)
open "dockpin://presentation?on=1"    # Präsentationsmodus (0 zum Beenden, ohne Wert umschalten)
open "dockpin://language?code=de"     # Sprache der Oberfläche (en, fr, de, nl, es, it, system)
open "dockpin://settings"             # auch: dockpin://about
```

## Fehlerbehebung

- **Das Dock springt weiterhin auf andere Bildschirme.** Prüfe, ob DockPin unter Systemeinstellungen › Datenschutz & Sicherheit › Bedienungshilfen eingeschaltet ist. Ist es eingeschaltet und die Sperre wirkt trotzdem nicht, entferne DockPin mit der Taste **−** aus dieser Liste und füge es dann erneut hinzu.
- **Das Dock wechselt nicht auf den gewählten Bildschirm.** Prüfe, ob „Monitore verwenden verschiedene Spaces“ eingeschaltet ist (Systemeinstellungen › Schreibtisch & Dock), und melde dich dann ab und wieder an.
- **Ein Kurzbefehl funktioniert nicht.** Er wird wahrscheinlich bereits von einer anderen App verwendet (er erscheint in den Einstellungen rot). Wähle eine andere Kombination.

## Datenschutz

DockPin sammelt keine Daten und baut keine Netzwerkverbindungen auf. Links wie *Hilfe* werden einfach in deinem Browser geöffnet.

## Deinstallation

Beende DockPin (Menüleistensymbol › *DockPin beenden*), bewege es aus „Programme“ in den Papierkorb und entferne es unter Systemeinstellungen › Datenschutz & Sicherheit › Bedienungshilfen.

---

<p align="center"><sub>© 2026 Soft-Connect</sub></p>
