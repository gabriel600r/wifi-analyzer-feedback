# Changelog

Todos los cambios notables de este proyecto se documentarán en este archivo.

El formato está basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.0.0/), 
y este proyecto se adhiere a [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [0.73.5] - 2026-05-05

### Herramienta Código de Color de Fibra Óptica
- **Fibras por bandeja configurable** (12, 24, 36, 48 en TIA / 8, 16, 24, 32 en SIECOR). Soporta cajas tipo Centrix donde 1 bandeja física contiene 24 fibras (2 buffers).
- **Búsqueda enlazada al repartidor:** al buscar una fibra en *Código Color* y pasar a la vista *Repartidor*, el pelo queda resaltado y el rack scrollea automáticamente hasta la bandeja correspondiente.
- **Estándar y fibras/bandeja sincronizados** entre ambas pestañas, sin pisar la configuración cuando el usuario edita en cualquiera de las dos.
- Resultado de búsqueda incluye **bandeja física, posición en bandeja y buffer interno** (X/Y) en lugar de solo el buffer.
- **Índice local 1..N** visible en cada puerto del repartidor para ubicar rápido el pelo cuando estás físicamente frente al rack.
- **Pulso animado** con glow cyan sobre la fibra resaltada en la vista del repartidor para detectarla de un vistazo.

### What's New
- Panel de novedades ahora se ajusta al contenido en lugar de ocupar 70% de la pantalla siempre.

---

## [0.73.0] - 2026-04-25

### Skeletons de carga
- Placeholder con shimmer animado en Escáner de puertos, Whois, DNS Lookup e Info de celda mientras los resultados llegan. Reemplaza la pantalla en blanco por una vista con la forma del contenido final, mejorando la sensación de velocidad.
- Sección Celdas vecinas con skeleton durante los primeros polls + mensaje claro cuando no se detectan ("Por el momento no se detectaron celdas vecinas. Si aparece alguna durante el escaneo, va a aparecer acá.").

### Widgets reutilizables
- Nuevo módulo `lib/widgets/skeleton.dart` con primitivos (`SkeletonBar`, `SkeletonShimmer`, `SkeletonCard`, `SkeletonRow`) para mantener consistencia visual en todas las pantallas.

---

## [0.72.0] - 2026-04-25

### Recuperación de errores
- Tarjeta dedicada con ícono, título descriptivo y botón Reintentar cuando una consulta falla por timeout, sin internet o error del servidor. Reemplaza el mensaje rojo plano. Aplica a Whois y DNS Lookup.
- Heurística `classifyError()` que mapea excepciones a tipos (timeout, sin conexión, server error, input inválido).

### Detección de cambio de red
- Banner SnackBar cuando pasás de WiFi a datos móviles (o viceversa) durante un análisis activo. Acción "Detener" para frenar el análisis con un toque.
- Banner de recuperación cuando la red WiFi vuelve.
- Servicio `NetworkMonitor` singleton sobre `connectivity_plus`.

---

## [0.71.0] - 2026-04-24

### Pantalla de Ajustes
- Nueva pantalla dedicada con todas las opciones en un solo lugar: idioma, sonido, vibración, servidor de ping, datos y privacidad, restaurar Pro y Acerca de.
- Buscador interno para encontrar opciones al instante.
- Estética glass coherente con el resto de la app, secciones con colores accent (idioma cyan, audio violeta, ping naranja, datos verde, Pro dorado).

### Más servidores de ping
- OpenDNS (208.67.222.222), Quad9 (9.9.9.9) y opción personalizada para que elijas qué servidor mide tu latencia a internet.

### Toggle de sonido y vibración
- Activá o desactivá el sonido del análisis WiFi y la vibración táctil. Preferencias persisten entre sesiones (`SettingsProvider` + SharedPreferences).

### Datos y privacidad
- Borrar historiales de WiFi, LAN, speed test, ping, traceroute, puertos y fibra óptica desde Ajustes.
- Reproducir el tutorial de bienvenida cuando quieras.

### Restaurar Pro
- Botón dedicado para recuperar la compra Pro si reinstalaste la app o cambiaste de teléfono.

### Idioma centralizado
- El switch ES/EN se movió del sidebar a la nueva pantalla de Ajustes (única fuente de verdad).
- Ítem "Ajustes" en el menú lateral con badge "NUEVO" + glow cyan animado para que los usuarios existentes lo encuentren rápido. Auto-desaparece después del primer toque.

---

## [0.70.0] - 2026-04-22

### IP pública sobre datos móviles
- Consultá tu IP pública aunque no estés conectado a WiFi. La app detecta que estás navegando por datos móviles y muestra la IP asignada por tu operador celular.

### Detección de operador celular
- Identificación automática del operador móvil (Movistar, Claro, Personal, etc.) junto a la IP pública.

### Aviso de red móvil
- Banner amarillo en la pantalla de IP pública cuando estás sobre datos móviles, para que sepas que la IP no corresponde a una red WiFi local.

---

## [0.69.0] - 2026-04-20

### Vibración al iniciar análisis
- Vibración corta al tocar START/STOP y al iniciar escaneos. Confirma la acción de manera táctil.

### Pantallas vacías mejoradas
- Diseño más amigable cuando no hay dispositivos LAN o historial WiFi, con sugerencias y botón directo para volver a escanear.

### Pull-to-refresh en IP pública
- Deslizá hacia abajo en la pantalla de IP pública para actualizar tu IP y datos de red al instante.

---

## [0.68.0] - 2026-04-15

### Permiso de ubicación más claro
- Reescritura del mensaje del permiso de ubicación para aclarar que la app NO usa GPS, NO rastrea ubicación y NO envía datos a ningún servidor. Es solo un requisito de Android para leer datos WiFi.

### Permiso pedido al iniciar análisis
- El permiso de ubicación ya no se pide al abrir la app. Se solicita recién cuando tocás START, así podés explorar herramientas como calculadora IP o pinout RJ-45 sin dar permisos primero.

### Sin WiFi: herramientas útiles
- Si no estás conectado a una red WiFi al tocar START, la app surface todas las herramientas que funcionan offline o con datos móviles: calculadora IP, generador de contraseñas, pinout RJ-45, fibra óptica, IP pública, ping monitor, speed test, escáner de puertos, DNS lookup, traceroute, whois y más.

### Acceso directo a permisos
- Si rechazaste el permiso de ubicación, el aviso ahora trae un botón "Dar permisos" que abre directo los ajustes del sistema.

### Pantalla Pro renovada
- Cabecera de Desbloquear Pro con diseño dorado premium, halo brillante, badge "PRO" y animación sutil.

---

## [0.67.4] - 2026-04-10

### Tour de bienvenida
- Onboarding interactivo al iniciar la app por primera vez. Muestra todas las herramientas disponibles (gratuitas y Pro) organizadas por categoría.

### Panel de novedades
- Cada versión nueva muestra mejoras y cambios. Disponible en el menú lateral, sección Soporte.

---

## [0.66.2] - 2026-03-24

### Nueva herramienta
- **Calculadora dB Fibra Óptica:** cálculo de atenuación de enlace de fibra óptica con soporte para SM G.652, MM 50/125 y MM 62.5/125 a múltiples longitudes de onda (850, 1300, 1310, 1550 nm).
- Modelo freemium: cálculo básico gratis; empalmes, conectores, margen, comparación PASS/FAIL, conversor dBm↔mW, historial y compartir son funciones Pro.
- Glosario integrado con iconos de info en cada campo.
- Persistencia de configuración (tipo de fibra, longitud de onda, empalme, margen).
- Guía descriptiva de cada tipo de fibra para usuarios no expertos.

### Sidebar reorganizado
- Herramientas ordenadas por categoría lógica: WiFi → Red/Monitoreo → Internet/Exploración → Cableado/Fibra → Utilidades.
- Free y Pro intercaladas por categoría en lugar de separadas en bloques.

### Mejoras visuales
- Selectores con colores individuales por categoría (tipo de fibra, longitud de onda, tipo de empalme).
- AppBar con fondo sólido — ya no se transparenta al scrollear.

### Correcciones
- Fix de solapamiento de la barra de navegación con secciones Pro al hacer scroll.
- Texto de compartir ahora incluye branding ("Analizador WiFi EgeaINC") y link de descarga.

---

## [0.64.1] - 2026-03-18

### Nuevas herramientas
- **Calculadora IP avanzada:** subnetting, VLSM y cálculos de red organizados por tabs.
- **Traceroute visual:** compará rutas, visualizalas en mapa y guardá historial de trazados.
- **Historial Whois** integrado en la herramienta DNS.

### Mejoras en herramientas existentes
- **DNS:** consultas a múltiples servidores con comparación de resultados.
- **Escáner de puertos:** perfiles predefinidos (Web, Gaming, Mail, etc.) para escaneos rápidos.
- **IP Pública:** historial inline con cards glass en traceroute e IP pública.
- **Favoritos:** colores por categoría para distinguir herramientas rápidamente.

### Pantalla principal renovada
- **Barra de salud WiFi:** indicador visual del estado general de tu conexión.
- **Pausa y scroll en gráficas:** nuevo botón pausa en el FAB que congela las gráficas y permite hacer scroll horizontal para revisar hasta 30 minutos de datos históricos.
- **Historial agrupado por red:** los datos se organizan automáticamente por SSID.
- **Ping más fiable:** 5 paquetes mínimo con sincronización para mediciones más estables.

### Design system completo
- **Estilo visual unificado:** todas las pantallas y herramientas usan el nuevo diseño con cards gradiente navy, bordes accent y sombras consistentes.
- **Flip clock 3D** compacto para el timer de análisis.

### Correcciones
- Campanita de umbral de señal solo visible para usuarios Pro.
- Feedback visual al presionar botones en Calculadora IP.
- Mejoras estéticas en tabla de datos, pantalla de review y estado de desconexión.

---

## [0.58.1] - 2026-03-13

### Novedades
- **Favoritos en Home:** acceso rápido a tus herramientas favoritas desde la pantalla principal. Mantené presionado en el menú lateral para marcar/desmarcar. Arrastrá para reordenar.
- **Vista Repartidor de Fibra Óptica:** nueva herramienta visual que simula un repartidor/centrix configurable. Seleccioná estándar (TIA/SIECOR), puertos por bandeja (8, 12, 16, 24, 32) y cantidad de bandejas (1-48). Incluye zoom, scroll sincronizado y detalle de cada puerto.
- **Navegación por pestañas en Fibra Óptica:** accedé fácilmente entre "Código Color" y "Vista Repartidor" con tabs visibles.
- **Configuración persistente:** el repartidor recuerda tu última configuración.

### Mejoras
- Splash y barra de estado unificados con el diseño de la app.
- Corrección en el botón "Ver Pro" de Red Móvil.
- Texto de compartir actualizado (17 herramientas).
- Fix de bottom sheet Pro cortado por la barra de navegación.
- Banner GPS desactivado en Red Móvil con explicación de restricción Android.
