<p align="center">
  <img src="docs/icon.png" width="128" height="128" alt="DockPin-symbool">
</p>

<h1 align="center">DockPin</h1>

<p align="center">Houd het Dock van je Mac op het scherm van je keuze.</p>

<p align="center">
  <a href="https://github.com/ulric-soft-connect-be/DockPin/releases/latest"><b>⬇︎ DockPin downloaden</b></a>
</p>

<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.fr.md">Français</a> ·
  <a href="README.de.md">Deutsch</a> ·
  <b>Nederlands</b> ·
  <a href="README.es.md">Español</a> ·
  <a href="README.it.md">Italiano</a>
</p>

---

Met meerdere schermen verplaatst macOS het Dock naar het scherm waarvan je de onderkant met de aanwijzer aanraakt. DockPin voorkomt dat: het Dock blijft op het scherm dat je hebt gekozen, en je kunt het met een toetscombinatie en een klik naar een ander scherm verplaatsen.

## Functies

- **Het Dock op één scherm vergrendelen.** Op de andere schermen stopt de aanwijzer net voor de rand van het Dock, zodat het Dock niet meer verspringt. Randen die twee schermen delen, blijven gewoon passeerbaar.
- **Het scherm kiezen met een toetscombinatie en een klik.** Druk op **⌃⌥⌘D** en klik op het gewenste scherm. Het Dock verhuist daarheen en blijft er vergrendeld.
- **Extra schermen toestaan** als het Dock naar meer dan één scherm mag gaan.
- **Het Dock eenmalig verplaatsen.** Houd **⌥ Option** ingedrukt terwijl je de aanwijzer tegen de onderkant van een ander scherm duwt.
- **Automatisch terugzetten.** Bij het opstarten, na de sluimerstand en wanneer een scherm wordt aangesloten of losgekoppeld, keert het Dock terug naar zijn scherm.
- **Presentatiemodus**: verbergt het Dock op alle schermen tijdens het delen van je scherm of een vergadering, en herstelt daarna je instelling.
- **Onopvallend.** Geen symbool in het Dock (behalve zolang een DockPin-venster open is), en het menubalksymbool kan worden verborgen.
- **Zes talen**: Engels, Frans, Duits, Nederlands, Spaans, Italiaans. DockPin volgt standaard de taal van macOS; je kunt die wijzigen in de instellingen.

## Vereisten

- macOS 13 Ventura of nieuwer, Mac met Apple chip of Intel.
- Systeeminstellingen › Bureaublad en Dock › **‘Beeldschermen hebben aparte spaces’** ingeschakeld. Zonder deze optie houdt macOS het Dock altijd op het hoofdscherm.
- Het Dock aan de onderkant, links of rechts van het scherm.

## Installatie

1. Download **DockPin-x.y.z.dmg** van de [nieuwste versie](https://github.com/ulric-soft-connect-be/DockPin/releases/latest).
2. Open de schijfkopie en sleep **DockPin** naar **Programma’s**.
3. Open DockPin vanuit de map ‘Programma’s’. DockPin is nog niet door Apple notarieel bekrachtigd, dus de eerste keer weigert macOS het te openen. Ga naar **Systeeminstellingen › Privacy en beveiliging**, scrol omlaag, klik naast het bericht over DockPin op **Open toch** en bevestig.
4. Geef DockPin de **Toegankelijkheid**-rechten wanneer daarom wordt gevraagd (Systeeminstellingen › Privacy en beveiliging › Toegankelijkheid). DockPin heeft die nodig om de aanwijzer aan de schermranden tegen te houden en om het Dock te verplaatsen. De vergrendeling start zodra de toegang is verleend.

## Het Dock-scherm kiezen

- **Toetsenbord en muis:** druk op **⌃⌥⌘D**. Op elk scherm verschijnt een sluier met een voorvertoning van het Dock. Klik op het gewenste scherm. **Esc** of een rechtsklik annuleert.
- **Instellingenvenster:** klik op een scherm in de plattegrond, of kies het in de lijst *Vergrendeld scherm*.
- **Menubalksymbool:** submenu *Dock-scherm*.

## Toetscombinaties

| Actie | Standaard |
| --- | --- |
| Dock-scherm kiezen (en dan klikken) | ⌃⌥⌘D |
| Instellingen openen | ⌃⌥⌘S |
| Vergrendeling aan of uit | — |
| Presentatiemodus | — |

Wijzig ze via **Instellingen › Toetscombinaties**: klik op een toetscombinatie en typ de nieuwe combinatie (⌫ wist, Esc annuleert). Een toetscombinatie in het rood wordt al door een andere app gebruikt.

## Instellingen

- **Dock-scherm:** plattegrond van je schermen, vergrendeld scherm, *Dock nu terugzetten*.
- **Vergrendeling:** vergrendeling aan of uit, extra toegestane schermen, toets om het Dock tijdelijk te verplaatsen (standaard ⌥ Option), automatisch terugzetten.
- **Presentatiemodus:** het Dock op alle schermen verbergen.
- **Toetscombinaties:** zie hierboven.
- **Algemeen:** taal van de interface, openen bij inloggen, menubalksymbool.

Zolang een DockPin-venster open is (Instellingen, Over), toont DockPin zijn menu in de menubalk van macOS: *Over DockPin*, *Instellingen…*, *Stop DockPin* en het menu *Help*, dat deze pagina opent. macOS staat dat alleen toe voor apps met een symbool in het Dock: het symbool verschijnt dus tijdelijk en verdwijnt wanneer je het venster sluit.

## Menubalksymbool verborgen?

Open DockPin opnieuw (Spotlight, Launchpad of Finder) of druk op **⌃⌥⌘S**: het instellingenvenster verschijnt weer.

## Automatisering

DockPin begrijpt `dockpin://`-links, te gebruiken vanuit Opdrachten, scripts of Terminal:

```bash
open "dockpin://pick"                 # scherm kiezen door te klikken
open "dockpin://lock?screen=2"        # Dock vergrendelen op scherm 2 (genummerd van links naar rechts)
open "dockpin://lock?screen=LG"       # … of op (gedeeltelijke) naam, UUID of "main"
open "dockpin://home"                 # Dock terugzetten op het vergrendelde scherm
open "dockpin://unlock"               # vergrendeling uitschakelen (ook: lock, toggle)
open "dockpin://presentation?on=1"    # presentatiemodus (0 om te stoppen, zonder waarde = wisselen)
open "dockpin://language?code=nl"     # taal van de interface (en, fr, de, nl, es, it, system)
open "dockpin://settings"             # ook: dockpin://about
```

## Problemen oplossen

- **Het Dock springt nog steeds naar andere schermen.** Controleer of DockPin is ingeschakeld in Systeeminstellingen › Privacy en beveiliging › Toegankelijkheid. Staat het aan maar werkt de vergrendeling nog steeds niet, verwijder DockPin dan met de knop **−** uit die lijst en voeg het daarna opnieuw toe.
- **Het Dock gaat niet naar het gekozen scherm.** Controleer of ‘Beeldschermen hebben aparte spaces’ is ingeschakeld (Systeeminstellingen › Bureaublad en Dock), en meld je daarna af en weer aan.
- **Een toetscombinatie werkt niet.** Die wordt waarschijnlijk al door een andere app gebruikt (ze verschijnt in het rood in de instellingen). Kies een andere combinatie.

## Privacy

DockPin verzamelt geen gegevens en maakt geen netwerkverbindingen. Links zoals *Help* worden gewoon in je browser geopend.

## Verwijderen

Stop DockPin (menubalksymbool › *Stop DockPin*), sleep het van ‘Programma’s’ naar de prullenmand en verwijder het daarna uit Systeeminstellingen › Privacy en beveiliging › Toegankelijkheid.

---

<p align="center"><sub>© 2026 Soft-Connect</sub></p>
