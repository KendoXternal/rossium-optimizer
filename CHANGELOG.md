# Historial de cambios — ROSSIUM Optimizer

Cada versión también aparece en [Releases](../../releases) con su ejecutable y su huella SHA-256.

## v13.0.0

- Modo «probar»: aplica los cambios unos minutos; si no pulsas «Mantener» se revierten solos (también si cierras ROSSIUM).
- Historial de cambios con «Deshacer» por bloque en Copias y restauración.
- Funciones avanzadas desactivadas por defecto: Máximo, ajustes avanzados, Modo Juego, adaptador de red, modo portátil y prueba de calentamiento piden aceptar un aviso «bajo tu propio riesgo».
- Aviso de reinicio: indica qué cambios necesitan reiniciar Windows o el Explorador, con botón para hacerlo.
- Modo Juego: cierra los programas que elijas al abrir el juego y los reabre al salir.
- Nueva página Pruebas: detector de pérdida de velocidad de la CPU con carga (temperatura / energía) y comparación antes / después con tarjeta para compartir en Discord.
- Red: prueba de bufferbloat (ping con la red ocupada) con nota y consejo.
- Uso de GPU en vivo para AMD, Intel y NVIDIA, y velocidad real de la CPU (contadores de Windows).
- Aviso de controlador de gráficos con más de 6 meses, con el enlace oficial; la fecha del driver ya se muestra bien.
- Modo portátil automático: alto rendimiento enchufado, equilibrado con batería (opcional).
- Asistente de primer uso, tiempo restante de la licencia visible, botón de Ayuda al Discord.
- Diseño: tipografía Bahnschrift en títulos y cifras, más espacio, tarjetas con degradado y brillo al pasar el ratón, transiciones entre páginas, desplazamiento suave y % animado.
- Arranque más rápido: el ejecutable se descomprime una vez por versión y el inicio usa el último análisis guardado.
- Protección: código nativo con LTO, anti-depurador y autocomprobación contra la huella SHA-256 firmada de rossium.xyz (una copia modificada no arranca).

## v12.0.0

- Diseño nuevo: panel de inicio con tarjetas (optimización, licencia, CPU, GPU, discos, Internet y RAM en vivo), barra lateral con nombres y fondo azul con brillo violeta.
- Porcentaje de optimización real: la parte del preajuste «Óptimo» para tu equipo que ya está aplicada; sube al optimizar y baja al revertir.
- Optimización por categorías con preajustes Predeterminado / Óptimo / Máximo, «Consejo» desplegable y avisos de lo que deja de funcionar. Los cambios se marcan y se aplican juntos con «Aplicar».
- 36 ajustes nuevos (119 en total): telemetría de .NET, PowerShell, Visual Studio, CEIP e impacto de apps; Copilot y Recall; actualización automática de drivers, mapas y Tienda; personalización (modo oscuro, extensiones, barra de tareas, widgets); seguridad (reproducción automática, SMBv1, Asistencia remota).
- Red: propiedades avanzadas del adaptador con perfiles Óptimo y Baja latencia (guarda los valores originales), DNS en un clic y prueba de ping, jitter y pérdida de paquetes.
- Perfiles de juego con detección automática: prioridad del proceso y plan de alto rendimiento mientras juegas; al cerrar el juego todo vuelve como estaba.
- Aplicaciones: instala, desinstala y actualiza programas con winget (navegadores, Discord, Steam, Epic, herramientas de monitor y runtimes).
- Herramientas: SFC, DISM, restablecer la red, reparar Windows Update, componentes de Windows, modo de Windows Update, quitar apps preinstaladas, TRIM/desfragmentación y paneles clásicos.
- Los preajustes nunca incluyen ajustes peligrosos (hora UTC, reparación de Windows Update) ni preferencias personales, y se adaptan a portátiles y discos HDD.

## v11.2.1

- Corrige la activación en equipos con el reloj desfasado: antes bastaba con que el reloj del PC fuera unos segundos atrasado (o adelantado) para rechazar una key válida con «La firma o la vigencia del token no es válida». Ahora el vencimiento se comprueba con la hora del servidor.
- Mensajes de activación más claros: distingue una licencia vencida de un programa que no coincide con el servidor, y avisa si el reloj del PC está desfasado.

## v11.2.0

- La interfaz conserva fluidez: el muestreo de CPU, memoria, disco, red y GPU se ejecuta en segundo plano, evita trabajos superpuestos y consulta NVIDIA como máximo cada tres segundos.
- La búsqueda de juegos también se ejecuta en segundo plano; se puede ajustar la frecuencia del monitor y la duración habitual de cada captura.
- Los FPS de PresentMon se agrupan por aplicación para no mezclar juegos y escritorio; el cálculo en vivo consume menos trabajo por fotograma.
- PresentMon 2.6 de Intel (MIT) viene incluido y verificado por SHA-256; se corrigió la detección de parámetros de la consola 2.x.
- Las mediciones de un mismo juego pueden compararse con una referencia guardada: FPS medios, 1 % y 0,1 % bajos y tiempo de fotograma, con recomendaciones que abren las herramientas correspondientes.
- Las pantallas de resumen y rendimiento presentan un recorrido visual más claro y muestran solo resultados medidos.
- Ajustes visuales aplicados al instante: tema claro, oscuro o según Windows; cuatro acentos, tipografía, densidad y alto contraste.
- Cuando una versión firmada exige actualización, el programa muestra la nueva versión y la descarga verificada; el servidor bloquea activaciones y verificaciones de versiones anteriores.

## v11.1.0

- Diagnóstico de Internet de solo lectura: revisa adaptador, puerta de enlace, DNS y HTTPS de Rossium sin bloquear la interfaz ni enviar datos del equipo.
- Incluye acceso a la configuración de red de Windows e informe copiable que omite IP e identificadores del equipo.
- La pantalla de licencia traduce las reactivaciones aprobadas por soporte a una duración clara de dos horas.
- Reactivaciones repetibles mediante un nuevo ticket de soporte cada vez; cada key dura dos horas, queda ligada a su ticket y se vincula a un equipo al activarse.

## v11.0.0

- La activación consulta los cinco componentes del equipo en un solo proceso de PowerShell (antes podía esperar hasta 40 segundos) y muestra cada etapa mientras valida y guarda la licencia.
- Interfaz nueva con PySide6, estilo «estación de control»: barra lateral de iconos, área principal e inspector plegable con el estado en vivo.
- Paleta de comandos (Ctrl+K) para ir a cualquier sección, abrir cualquier ajuste o ejecutar acciones escribiendo.
- Diagnóstico completo con datos reales: procesador, gráficos y controlador, memoria y módulos, discos y su estado, Windows, placa base y hallazgos con acceso directo a la solución.
- Planes por objetivo (Juegos, Competitivo, Trabajo, Privacidad, Portátil) que omiten lo que perjudica a tu equipo (HDD, poca RAM, portátil, Xbox/Game Pass) y lo que afecta a la seguridad.
- Programas de inicio (como el Administrador de tareas, reversible), servicios con copia del tipo de inicio original, procesos con prioridad y cierre protegido, y limpieza con vista previa del espacio.
- Medición de FPS real con PresentMon (FPS medio, 1 % y 0,1 % bajos, tiempo de fotograma y tirones), overlay flotante de FPS y modo Focus para medir sin interferencias.
- Pruebas de CPU, memoria y disco con historial y comparación antes / después.
- Overclocking guiado: detecta y abre las herramientas oficiales del fabricante, con advertencias. ROSSIUM no cambia voltajes ni frecuencias.
- Puntos de restauración de Windows, mantenimiento programado (Programador de tareas) y reportes en PDF, HTML, CSV y JSON sin datos personales.
- Un ajuste con varios pasos que Windows acepta solo en parte se informa como «parcial» en vez de como éxito.

## v10.2.0

- La aplicación ya no pide administrador al abrir: lo pide solo al aplicar, revertir o restaurar cambios del sistema, explicando el motivo.
- Antes de aplicar o revertir un ajuste se muestra qué hace, su riesgo, dónde queda registrado y cómo deshacerlo.
- Un cambio que Windows rechaza ya no se cuenta como aplicado: el interruptor vuelve a su estado y se avisa del error.
- «Restaurar todo» revierte solo los cambios que ROSSIUM registró en este equipo.
- Actualizaciones: muestra versión instalada y disponible con sus cambios, y descarga el instalador verificando tamaño, SHA-256 y firma digital cuando la versión está firmada. Nunca lo ejecuta solo.

## v10.1.0

- Se añadió un asistente de optimización con recomendaciones basadas en el hardware detectado; omite automáticamente ajustes incompatibles con HDD o menos de 16 GB de RAM.
- Se incorporaron preferencias persistentes para tema claro/oscuro/sistema, color de acento, tipografía, densidad y alto contraste.
- Presets ahora se guardan como proyectos versionados, con validación segura e importación/exportación JSON.
- Se añadió una vista de historial con búsqueda local y exportación de informe.
- La aplicación consulta el manifiesto oficial de Rossium en segundo plano y avisa cuando hay una versión nueva; la descarga siempre se hace desde rossium.xyz.
- Los perfiles muestran progreso cancelable entre cambios, registran errores individuales y guardan el estado para restaurar/deshacer.
- La versión de la pantalla de activación y del ejecutable se deriva de una única versión de aplicación.

## v10.0.0

- La licencia se solicita antes de crear la ventana principal; su cierre detiene el arranque.
- El HWID se genera a partir de hashes SHA-256 de cinco componentes y tolera un cambio de componente cuando hay suficientes lecturas disponibles.
- El token se cifra con DPAPI en `%APPDATA%\Rossium\license.dat`.
- Se incorporaron consulta online periódica y gracia offline limitada a 72 horas.
