# CODEQUEST: Academia de los Programadores

Edición autónoma, sin dependencias, para Windows. Abre `index.html` en un navegador moderno o usa el servidor local de PowerShell:

```powershell
cd "C:\Users\User\Documents\Codex\2026-11-21\files-pasted-by-the-user-operaci-2"
& "C:\Users\User\AppData\Local\Python\pythoncore-3.15-64\python.exe" -m http.server 8080
```

Si Python tampoco está instalado, abre `index.html` directamente.

## Lo que incluye

- 8 mundos, 6 misiones por mundo (48 actividades) con objetivos, pistas y recompensa.
- Editor JavaScript limitado a expresiones y pruebas de resultado, vista previa HTML/CSS en `iframe sandbox`, terminal virtual y simulador de red.
- Movimiento con teclado, colisiones, NPC BIT, cámara, mapas, guardado local, inventario, logros, accesibilidad, pausa y modo de repaso.

## Arquitectura

- `index.html`: estructura y paneles.
- `styles.css`: interfaz pixel-art y diseño adaptable.
- `game.js`: motor Canvas, contenido de misiones, evaluadores y persistencia.

Para añadir una misión, incorpora una entrada en `MISSION_SEEDS` en `game.js`. Cada misión se crea con un tipo de reto (`code`, `web`, `terminal`, `network`, `choice` o `prompt`) y se evalúa por su resultado.

## Estado de verificación

El entorno inspeccionado no expone Node.js, npm ni Git, por lo que no se ejecutaron Vitest, Playwright, Vite ni empaquetado de escritorio. El juego no requiere red ni dependencias; hay una autoprueba en el menú de ajustes para validar los evaluadores en el navegador.

## Seguridad

El código del alumno no se ejecuta en procesos del sistema. JavaScript se restringe a expresiones aritméticas o de texto; HTML/CSS se muestra en un iframe sin permisos; terminal y red usan modelos de datos completamente virtuales.

