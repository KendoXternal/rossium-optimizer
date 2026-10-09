# ROSSIUM Optimizer

**Optimizador para Windows 10 y 11**: más rendimiento en juegos, menos procesos en segundo plano, mejor red y todo reversible con un clic.

[![Última versión](https://img.shields.io/github/v/release/KendoXternal/rossium-optimizer?label=versi%C3%B3n&color=6d5dfc)](https://github.com/KendoXternal/rossium-optimizer/releases/latest)
[![Descargas](https://img.shields.io/github/downloads/KendoXternal/rossium-optimizer/total?label=descargas&color=4f8cff)](https://github.com/KendoXternal/rossium-optimizer/releases)
[![Discord](https://img.shields.io/badge/Discord-ROSSIUM-5865F2?logo=discord&logoColor=white)](https://discord.gg/uREQ5PmgBr)
[![Web](https://img.shields.io/badge/web-rossium.xyz-0b0e14)](https://rossium.xyz)

> Este repositorio es **solo para descargar** el programa y ver sus novedades. El código fuente no es público.

---

## ⬇️ Descargar

1. Entra en **[Releases → última versión](https://github.com/KendoXternal/rossium-optimizer/releases/latest)**.
2. Descarga **`RossiumOptimizer.exe`**.
3. Ábrelo y activa tu licencia. **Key gratis de 24 horas** con `/key` en el **[Discord](https://discord.gg/uREQ5PmgBr)** (guía en **[rossium.xyz/key-gratis](https://rossium.xyz/key-gratis)**). Cuando vence, la renuevas desde el propio programa con «Renovar 24 h».

También puedes descargarlo desde la web oficial: **https://rossium.xyz/key-gratis**. Es el mismo archivo.

**Requisitos:** Windows 10 (1809 o superior) o Windows 11, 64 bits, conexión a Internet para activar.

---

## ✨ Qué incluye

### Novedades de la versión 14
- **Estilo «Negro neón»**: negro y blanco con líneas de luz animadas y pantalla de carga nueva (el estilo azul sigue disponible).
- **Guía de optimización**: eliges para qué usas el PC y te dice qué ya tienes, qué conviene aplicar y qué conviene desactivar, con el motivo.
- **Key gratis de 24 h renovable** desde el programa.

### Inicio
- **Porcentaje de optimización real** de tu equipo: sube a medida que optimizas y baja si reviertes.
- Tarjetas en vivo de **CPU, GPU (NVIDIA, AMD e Intel), RAM, discos e Internet**.
- Tiempo restante de tu licencia siempre visible.

### Optimizar
- **178 ajustes** por categorías (rendimiento, juegos, privacidad y telemetría, Copilot/Recall, energía, personalización, seguridad…).
- **Preajustes** Predeterminado / Óptimo / Máximo que se adaptan a tu equipo: excluyen lo que perjudica a portátiles, discos HDD o equipos con poca RAM.
- Cada ajuste explica **qué hace**, un **consejo** y **qué deja de funcionar**, si aplica.
- **Modo «probar»**: aplicas los cambios unos minutos y, si no pulsas «Mantener», **se revierten solos**.
- **Red**: propiedades avanzadas del adaptador (perfiles Óptimo y Baja latencia), DNS en un clic, prueba de **ping, jitter, pérdida** y **bufferbloat**.
- **Modo Juego**: detecta el juego, sube su prioridad, activa alto rendimiento y cierra los programas que elijas; al salir, todo vuelve como estaba.
- **Limpieza** con vista previa del espacio que se libera.

### Rendimiento
- Medición de **FPS real** con PresentMon (FPS medios, 1 % y 0,1 % bajos, tiempo de fotograma), con comparación antes / después.
- **Pruebas**: detector de pérdida de velocidad de la CPU por temperatura o energía, y pruebas de CPU, memoria y disco.
- **Diagnóstico completo** del equipo con hallazgos y acceso directo a la solución (por ejemplo, un driver de gráficos con más de 6 meses).
- Overclocking guiado: abre las herramientas oficiales del fabricante. ROSSIUM no cambia voltajes ni frecuencias.

### Windows
- **Aplicaciones**: instala, actualiza y desinstala programas con winget (navegadores, Discord, Steam, Epic, runtimes…).
- **Herramientas**: SFC, DISM, restablecer red, reparar Windows Update, quitar apps preinstaladas, TRIM.
- Programas de inicio, servicios y procesos.

### Seguridad y cuenta
- **Historial de cambios con «Deshacer»** y «Restaurar todo».
- Puntos de restauración de Windows y mantenimiento programado.
- Reportes en PDF, HTML, CSV y JSON **sin datos personales**.
- Temas, colores de acento, tipografía y alto contraste.

---

## 🛡️ Seguridad

- **Todo es reversible.** ROSSIUM guarda el valor original de cada cambio antes de aplicarlo.
- **Las funciones avanzadas vienen desactivadas.** El preajuste Máximo, los ajustes avanzados, el Modo Juego, el adaptador de red, el modo portátil y la prueba de calentamiento piden aceptar antes un aviso: se usan **bajo tu propio riesgo**.
- **Administrador solo cuando hace falta.** El programa abre como usuario normal y pide permisos solo al aplicar cambios del sistema, explicando el motivo.
- **Actualizaciones verificadas.** Cada versión lleva una firma digital **Ed25519** y su huella **SHA-256**. El programa comprueba ambas antes de aceptar una actualización y no arranca si el ejecutable fue modificado.
- **Privacidad.** Para la licencia solo se envían huellas SHA-256 de los componentes del equipo, nunca los números de serie.

### Comprobar que tu descarga es original
Cada release indica la huella SHA-256 del `.exe`. En PowerShell:

```powershell
Get-FileHash .\RossiumOptimizer.exe -Algorithm SHA256
```

El resultado debe coincidir con el de la release. Si no coincide, **no lo abras** y descárgalo de nuevo desde aquí o desde rossium.xyz.

> **Aviso de Windows SmartScreen:** el ejecutable todavía no tiene certificado de firma de código de Windows, así que SmartScreen puede mostrar «Windows protegió su PC». Comprueba la huella SHA-256 y, si coincide, pulsa **Más información → Ejecutar de todas formas**.

---

## 🔄 Actualizar

ROSSIUM avisa solo cuando hay una versión nueva, muestra sus cambios y descarga el archivo verificado. Cada versión nueva también se publica:
- aquí, en **[Releases](https://github.com/KendoXternal/rossium-optimizer/releases)**, con la lista de cambios;
- en **[CHANGELOG.md](CHANGELOG.md)**, con el historial completo;
- en el canal de anuncios del **[Discord](https://discord.gg/uREQ5PmgBr)** y en las notificaciones de **[rossium.xyz](https://rossium.xyz)**.

---

## ❓ Preguntas frecuentes

**¿Puede dañar mi PC?** Los preajustes Predeterminado y Óptimo solo incluyen cambios seguros y reversibles. Las funciones avanzadas te avisan antes de activarse. Aun así, ningún optimizador garantiza un número concreto de FPS: mide antes y después con la página de Pruebas.

**¿Cómo deshago un cambio?** En *Copias y restauración* tienes el historial con «Deshacer» por bloque y «Restaurar todo».

**¿Cuánto dura la key gratis?** 24 horas. Cuando vence, pulsa «Renovar 24 h» en el programa (o usa `/key` otra vez en Discord). Funciona en el equipo donde la activaste.

**La key no se activa.** Comprueba tu conexión y que la fecha y hora de Windows estén en automático. Si sigue sin activarse, abre un ticket en el **[Discord](https://discord.gg/uREQ5PmgBr)**.

---

© ROSSIUM · [rossium.xyz](https://rossium.xyz) · Todos los derechos reservados. Se permite descargar y usar el programa con una licencia válida; no se permite redistribuirlo modificado.
