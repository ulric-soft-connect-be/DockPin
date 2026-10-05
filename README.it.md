<p align="center">
  <img src="docs/icon.png" width="128" height="128" alt="Icona di DockPin">
</p>

<h1 align="center">DockPin</h1>

<p align="center">Tieni il Dock del tuo Mac sullo schermo che preferisci.</p>

<p align="center">
  <a href="https://github.com/ulric-soft-connect-be/DockPin/releases/latest"><b>⬇︎ Scarica DockPin</b></a>
</p>

<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.fr.md">Français</a> ·
  <a href="README.de.md">Deutsch</a> ·
  <a href="README.nl.md">Nederlands</a> ·
  <a href="README.es.md">Español</a> ·
  <b>Italiano</b>
</p>

---

Con più schermi, macOS sposta il Dock sullo schermo di cui spingi il bordo inferiore con il puntatore. DockPin lo impedisce: il Dock resta sullo schermo che hai scelto, e puoi spostarlo su un altro con un’abbreviazione da tastiera e un clic.

## Funzioni

- **Bloccare il Dock su uno schermo.** Sugli altri schermi il puntatore si ferma appena prima del bordo del Dock, così il Dock non salta più. I bordi condivisi da due schermi restano attraversabili.
- **Scegliere lo schermo con un’abbreviazione e un clic.** Premi **⌃⌥⌘D**, poi fai clic sullo schermo desiderato. Il Dock si sposta lì e resta bloccato.
- **Consentire altri schermi** se vuoi che il Dock possa andare su più di uno schermo.
- **Spostare il Dock una tantum.** Tieni premuto **⌥ Opzione** mentre spingi il puntatore contro il bordo inferiore di un altro schermo.
- **Ritorno automatico.** All’avvio, dopo lo stop e quando uno schermo viene collegato o scollegato, il Dock torna sul suo schermo.
- **Modalità presentazione**: nasconde il Dock su tutti gli schermi durante una condivisione dello schermo o una riunione, poi ripristina la tua impostazione.
- **Discreto.** Nessuna icona nel Dock (tranne mentre è aperta una finestra di DockPin), e l’icona nella barra dei menu si può nascondere.
- **Sei lingue**: inglese, francese, tedesco, olandese, spagnolo e italiano. Per impostazione predefinita DockPin segue la lingua di macOS; puoi cambiarla nelle impostazioni.

## Requisiti

- macOS 13 Ventura o successivo, Mac con chip Apple o Intel.
- Impostazioni di Sistema › Scrivania e Dock › **«I monitor hanno spazi separati»** attivato. Senza questa opzione, macOS tiene sempre il Dock sullo schermo principale.
- Il Dock sul bordo inferiore, sinistro o destro dello schermo.

## Installazione

1. Scarica **DockPin-x.y.z.dmg** dall’[ultima versione](https://github.com/ulric-soft-connect-be/DockPin/releases/latest).
2. Apri l’immagine disco e trascina **DockPin** su **Applicazioni**.
3. Apri DockPin dalla cartella Applicazioni. DockPin non è ancora autenticato da Apple, quindi la prima volta macOS si rifiuta di aprirlo. Vai in **Impostazioni di Sistema › Privacy e sicurezza**, scorri verso il basso, fai clic su **Apri comunque** accanto al messaggio relativo a DockPin e conferma.
4. Concedi a DockPin l’autorizzazione **Accessibilità** quando viene richiesta (Impostazioni di Sistema › Privacy e sicurezza › Accessibilità). DockPin ne ha bisogno per trattenere il puntatore ai bordi degli schermi e per spostare il Dock. Il blocco parte non appena l’accesso viene concesso.

## Scegliere lo schermo del Dock

- **Tastiera e mouse:** premi **⌃⌥⌘D**. Su ogni schermo appare un velo con un’anteprima del Dock. Fai clic sullo schermo desiderato. **Esc** o un clic destro annulla.
- **Finestra delle impostazioni:** fai clic su uno schermo nella mappa, oppure sceglilo nell’elenco *Schermo bloccato*.
- **Icona nella barra dei menu:** sottomenu *Schermo del Dock*.

## Abbreviazioni da tastiera

| Azione | Predefinita |
| --- | --- |
| Scegli lo schermo del Dock (poi fai clic) | ⌃⌥⌘D |
| Apri le impostazioni | ⌃⌥⌘S |
| Attiva o disattiva il blocco | — |
| Modalità presentazione | — |

Modificale in **Impostazioni › Abbreviazioni da tastiera**: fai clic su un’abbreviazione e digita la nuova combinazione (⌫ la cancella, Esc annulla). Un’abbreviazione in rosso è già usata da un’altra app.

## Impostazioni

- **Schermo del Dock:** mappa dei tuoi schermi, schermo bloccato, *Riporta subito il Dock*.
- **Blocco:** attivazione del blocco, schermi aggiuntivi consentiti, tasto per spostare temporaneamente il Dock (⌥ Opzione per impostazione predefinita), ritorno automatico.
- **Modalità presentazione:** nascondere il Dock su tutti gli schermi.
- **Abbreviazioni da tastiera:** vedi sopra.
- **Generali:** lingua dell’interfaccia, apertura al login, icona nella barra dei menu.

Mentre è aperta una finestra di DockPin (Impostazioni, Informazioni), DockPin mostra il suo menu nella barra dei menu di macOS: *Informazioni su DockPin*, *Impostazioni…*, *Esci da DockPin* e il menu *Aiuto*, che apre questa pagina. macOS lo consente solo alle app con un’icona nel Dock: l’icona appare quindi temporaneamente e scompare quando chiudi la finestra.

## Icona nella barra dei menu nascosta?

Apri di nuovo DockPin (Spotlight, Launchpad o Finder) oppure premi **⌃⌥⌘S**: la finestra delle impostazioni ricompare.

## Automazione

DockPin comprende i link `dockpin://`, utilizzabili da Comandi Rapidi, script o dal Terminale:

```bash
open "dockpin://pick"                 # scegliere lo schermo con un clic
open "dockpin://lock?screen=2"        # bloccare il Dock sullo schermo 2 (numerati da sinistra a destra)
open "dockpin://lock?screen=LG"       # … oppure per nome (parziale), UUID o "main"
open "dockpin://home"                 # riportare il Dock sullo schermo bloccato
open "dockpin://unlock"               # disattivare il blocco (anche: lock, toggle)
open "dockpin://presentation?on=1"    # modalità presentazione (0 per uscire, senza valore = alterna)
open "dockpin://language?code=it"     # lingua dell’interfaccia (en, fr, de, nl, es, it, system)
open "dockpin://settings"             # anche: dockpin://about
```

## Risoluzione dei problemi

- **Il Dock salta ancora sugli altri schermi.** Verifica che DockPin sia attivato in Impostazioni di Sistema › Privacy e sicurezza › Accessibilità. Se è attivato ma il blocco continua a non funzionare, rimuovi DockPin da quell’elenco con il pulsante **−**, poi aggiungilo di nuovo.
- **Il Dock non va sullo schermo scelto.** Verifica che «I monitor hanno spazi separati» sia attivato (Impostazioni di Sistema › Scrivania e Dock), poi esci dalla sessione e accedi di nuovo.
- **Un’abbreviazione non funziona.** Probabilmente è già usata da un’altra app (appare in rosso nelle impostazioni). Scegli un’altra combinazione.

## Privacy

DockPin non raccoglie dati e non stabilisce connessioni di rete. I link come *Aiuto* si aprono semplicemente nel browser.

## Disinstallazione

Esci da DockPin (icona nella barra dei menu › *Esci da DockPin*), sposta l’app da Applicazioni al Cestino, poi rimuovila da Impostazioni di Sistema › Privacy e sicurezza › Accessibilità.

---

<p align="center"><sub>© 2026 Soft-Connect</sub></p>
