<p align="center">
  <img src="docs/icon.png" width="128" height="128" alt="Icono de DockPin">
</p>

<h1 align="center">DockPin</h1>

<p align="center">Mantén el Dock de tu Mac en la pantalla que elijas.</p>

<p align="center">
  <a href="https://github.com/ulric-soft-connect-be/DockPin/releases/latest"><b>⬇︎ Descargar DockPin</b></a>
</p>

<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.fr.md">Français</a> ·
  <a href="README.de.md">Deutsch</a> ·
  <a href="README.nl.md">Nederlands</a> ·
  <b>Español</b> ·
  <a href="README.it.md">Italiano</a>
</p>

---

Con varias pantallas, macOS mueve el Dock a la pantalla cuyo borde inferior empujas con el puntero. DockPin lo impide: el Dock se queda en la pantalla que hayas elegido, y puedes moverlo a otra con un atajo de teclado y un clic.

## Funciones

- **Bloquear el Dock en una pantalla.** En las demás pantallas, el puntero se detiene justo antes del borde del Dock, así que el Dock ya no salta. Los bordes compartidos por dos pantallas se pueden seguir cruzando.
- **Elegir la pantalla con un atajo y un clic.** Pulsa **⌃⌥⌘D** y haz clic en la pantalla que quieras. El Dock se mueve allí y se queda bloqueado.
- **Permitir otras pantallas** si quieres que el Dock pueda ir a más de una pantalla.
- **Mover el Dock solo esta vez.** Mantén pulsada **⌥ Opción** mientras empujas el puntero contra la parte inferior de otra pantalla.
- **Vuelta automática.** Al arrancar, al salir del reposo y cuando se conecta o desconecta una pantalla, el Dock vuelve a su pantalla.
- **Modo presentación**: oculta el Dock en todas las pantallas mientras compartes pantalla o estás en una reunión, y después restablece tu ajuste.
- **Actualizaciones integradas.** DockPin avisa de las nuevas versiones y las instala con un clic.
- **Discreto.** Sin icono en el Dock (salvo mientras hay una ventana de DockPin abierta), y el icono de la barra de menús se puede ocultar.
- **Seis idiomas**: inglés, francés, alemán, neerlandés, español e italiano. Por omisión, DockPin usa el idioma de macOS; puedes cambiarlo en los ajustes.

## Requisitos

- macOS 13 Ventura o posterior, Mac con chip de Apple o Intel.
- Ajustes del Sistema › Escritorio y Dock › **«Las pantallas tienen espacios independientes»** activado. Sin esta opción, macOS mantiene siempre el Dock en la pantalla principal.
- El Dock en el borde inferior, izquierdo o derecho de la pantalla.

## Instalación

1. Descarga **DockPin-x.y.z.dmg** desde la [última versión](https://github.com/ulric-soft-connect-be/DockPin/releases/latest).
2. Abre la imagen de disco y arrastra **DockPin** a **Aplicaciones**.
3. Abre DockPin desde la carpeta Aplicaciones. DockPin aún no está notarizado por Apple, así que la primera vez macOS se niega a abrirlo. Ve a **Ajustes del Sistema › Privacidad y seguridad**, desplázate hacia abajo, haz clic en **Abrir igualmente** junto al mensaje sobre DockPin y confirma.
4. Concede a DockPin el permiso de **Accesibilidad** cuando te lo pida (Ajustes del Sistema › Privacidad y seguridad › Accesibilidad). DockPin lo necesita para retener el puntero en los bordes de las pantallas y para mover el Dock. El bloqueo empieza en cuanto se concede el permiso.

## Actualizaciones

DockPin busca nuevas versiones al iniciarse (se puede desactivar en **Ajustes › General**), cada vez que se abre la ventana **Acerca de** y con *Buscar actualizaciones…* (icono de la barra de menús o menú DockPin). Cuando hay una versión disponible, haz clic en **Instalar y reiniciar**: DockPin la descarga, comprueba que está firmada por Soft-Connect, sustituye la app y se reinicia. El permiso de Accesibilidad se conserva. DockPin debe estar en la carpeta Aplicaciones.

DockPin 1.0.0 todavía no puede actualizarse solo: instala la siguiente versión a mano, como se indica arriba.

## Elegir la pantalla del Dock

- **Teclado y ratón:** pulsa **⌃⌥⌘D**. Aparece un velo en cada pantalla con una vista previa del Dock. Haz clic en la pantalla que quieras. **Esc** o un clic derecho cancela.
- **Ventana de ajustes:** haz clic en una pantalla del plano, o elígela en la lista *Pantalla bloqueada*.
- **Icono de la barra de menús:** submenú *Pantalla del Dock*.

## Atajos de teclado

| Acción | Por omisión |
| --- | --- |
| Elegir la pantalla del Dock (y hacer clic) | ⌃⌥⌘D |
| Abrir los ajustes | ⌃⌥⌘S |
| Activar o desactivar el bloqueo | — |
| Modo presentación | — |

Cámbialos en **Ajustes › Atajos de teclado**: haz clic en un atajo y escribe la nueva combinación (⌫ lo borra, Esc cancela). Un atajo en rojo ya lo usa otra app.

## Ajustes

- **Pantalla del Dock:** plano de tus pantallas, pantalla bloqueada, *Devolver el Dock ahora*.
- **Bloqueo:** activar o desactivar el bloqueo, pantallas adicionales permitidas, tecla para mover el Dock temporalmente (⌥ Opción por omisión), vuelta automática.
- **Modo presentación:** ocultar el Dock en todas las pantallas.
- **Atajos de teclado:** ver más arriba.
- **General:** idioma de la interfaz, abrir al iniciar sesión, icono de la barra de menús, buscar actualizaciones al iniciar.

Mientras hay una ventana de DockPin abierta (Ajustes, Acerca de), DockPin muestra su menú en la barra de menús de macOS: *Acerca de DockPin*, *Buscar actualizaciones…*, *Ajustes…*, *Salir de DockPin* y el menú *Ayuda*, que abre esta página. macOS solo lo permite a las apps con icono en el Dock, así que el icono aparece temporalmente y desaparece al cerrar la ventana.

## ¿Icono de la barra de menús oculto?

Vuelve a abrir DockPin (Spotlight, Launchpad o Finder) o pulsa **⌃⌥⌘S**: la ventana de ajustes vuelve a aparecer.

## Automatización

DockPin entiende los enlaces `dockpin://`, que puedes usar desde Atajos, scripts o el Terminal:

```bash
open "dockpin://pick"                 # elegir la pantalla haciendo clic
open "dockpin://lock?screen=2"        # bloquear el Dock en la pantalla 2 (numeradas de izquierda a derecha)
open "dockpin://lock?screen=LG"       # … o por nombre (parcial), UUID o "main"
open "dockpin://home"                 # devolver el Dock a la pantalla bloqueada
open "dockpin://unlock"               # desactivar el bloqueo (también: lock, toggle)
open "dockpin://presentation?on=1"    # modo presentación (0 para salir, sin valor = alternar)
open "dockpin://language?code=es"     # idioma de la interfaz (en, fr, de, nl, es, it, system)
open "dockpin://settings"             # también: dockpin://about
```

## Solución de problemas

- **El Dock sigue saltando a otras pantallas.** Comprueba que DockPin está activado en Ajustes del Sistema › Privacidad y seguridad › Accesibilidad. Si está activado pero el bloqueo sigue sin funcionar, quita DockPin de esa lista con el botón **−** y vuelve a añadirlo.
- **El Dock no va a la pantalla elegida.** Comprueba que «Las pantallas tienen espacios independientes» está activado (Ajustes del Sistema › Escritorio y Dock) y, después, cierra sesión y vuelve a iniciarla.
- **Un atajo no funciona.** Probablemente ya lo usa otra app (aparece en rojo en los ajustes). Elige otra combinación.

## Privacidad

DockPin no recopila datos. Su única conexión de red busca actualizaciones en GitHub (al iniciarse, salvo que la desactives, y cuando lo pides); no se envía ninguna información personal. Los enlaces como *Ayuda* simplemente se abren en tu navegador.

## Desinstalación

Sal de DockPin (icono de la barra de menús › *Salir de DockPin*), mueve la app de Aplicaciones a la Papelera y quítala de Ajustes del Sistema › Privacidad y seguridad › Accesibilidad.

---

<p align="center"><sub>© 2026 Soft-Connect</sub></p>
