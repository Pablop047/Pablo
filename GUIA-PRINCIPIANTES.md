# Guía para empezar

1. Abre `index.html` o inicia el servidor indicado en el README y visita `http://127.0.0.1:8080`.
2. Pulsa **Iniciar misión**. Muévete con WASD o las flechas.
3. Llega a la consola amarilla y pulsa **E** (o el botón Interactuar).
4. Lee la explicación de BIT, prueba el reto y usa **Pista** si la necesitas. Solo una solución que pasa la comprobación concede experiencia.
5. En el mapa puedes volver a cualquier mundo para repasar. El avance se guarda en el almacenamiento local del navegador.

## Seguridad de los laboratorios

- La terminal es ficticia: sus archivos no existen en Windows.
- La red usa direcciones simuladas y nunca abre conexiones de red.
- El editor de expresiones no puede leer archivos ni ejecutar comandos del equipo.
- La vista web corre en un `iframe` aislado sin permisos de origen, formularios ni ventanas emergentes.

## Qué aprenderás

Código y lógica, HTML/CSS/JavaScript, pensamiento con Python, comandos de terminal, redes, IA responsable, hábitos de ciberseguridad y fundamentos de Git, npm y APIs.

## WSL y Ubuntu en Windows

WSL permite usar herramientas Linux desde Windows. No es necesario para jugar. Antes de instalarlo, consulta la documentación oficial de Microsoft, verifica espacio disponible y pide consentimiento al propietario del equipo. Una vez instalado por el usuario, abre Ubuntu y practica primero `pwd`, `ls`, `cd` y `mkdir` en una carpeta de prueba. No ejecutes comandos de borrado ni cambies configuraciones del sistema mientras aprendes.

## Añadir contenido

En `game.js`, cada grupo dentro de `MISSION_SEEDS` corresponde a un mundo. Añade una entrada con:

`[titulo, tipo, objetivo, resultadoEsperado, pista]`

Tipos disponibles: `code`, `web`, `terminal`, `network`, `prompt` y `choice`. Conserva seis o más misiones por mundo y elige un resultado observable, no una simple coincidencia de palabras.

