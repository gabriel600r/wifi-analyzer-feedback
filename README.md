<div align="center">
  <!-- Reemplaza la URL de abajo con el enlace real a tu logo -->
  <img src="./assets/logo.png" alt="EgeaINC WiFi Analyzer Logo" width="150" style="border-radius: 20px;"/>
  <h1>EgeaINC WiFi Analyzer</h1>
  <p><b>Tu Red WiFi y Móvil, Bajo Control Absoluto</b></p>
  
  <br/>
  <a href="https://egeainc.com/wifi">
    <img src="https://play.google.com/intl/en_us/badges/static/images/badges/es_badge_web_generic.png" alt="Disponible en Google Play" height="80"/>
  </a>
</div>

<br/>

<div align="center">
  <b>🇦🇷 Español</b> | <a href="README-en.md">🇺🇸 English</a>
</div>

<br/>

Analizador profesional de WiFi, redes celulares y suite de herramientas IT. Diseñado para técnicos, administradores de red, gamers y usuarios avanzados que necesitan diagnosticar, monitorear y optimizar todas sus conexiones al máximo nivel.

Monitorea tu red en tiempo real con una interfaz moderna y fluida estilo **cyberpunk "glass"**. El Panel Principal es un centro de comando que te muestra en una sola vista:
- **Estado Global:** Gauge animado de salud de conexión en tiempo real.
- **Red WiFi:** SSID, Potencia (dBm), Link Speed, Estándar (ej. WiFi 6 / 802.11ax), Seguridad y Dirección MAC (BSSID).
- **Métricas IP:** Local IP, Máscara de Subred, y servidores DNS (1 y 2).
- **Enrutamiento:** Puertas de enlace (Router IP), Frecuencia (2.4 / 5 GHz), Canales y Gráfico histórico animado con Ping al Router constante.
- **Salida a Internet:** Tu IP Pública externa, Proveedor (ISP) y Ping persistente a servidores globales (ej. Google 8.8.8.8) medidos directamente en gráficas continuas.

---

## 🔥 NUEVO EN ESTA VERSIÓN (v0.66.2)

### Nueva herramienta: Calculadora dB Fibra Óptica
- **Cálculo de atenuación por fibra:** Soporta Monomodo (SM G.652), Multimodo 50/125 y Multimodo 62.5/125 a múltiples longitudes de onda (850, 1300, 1310, 1550 nm).
- **Modelo freemium:** El cálculo básico de atenuación por distancia es gratis. Las funciones avanzadas son Pro:
  - Empalmes (fusión/mecánico), conectores y margen de seguridad.
  - Desglose visual de pérdidas con barra de componentes.
  - Comparación PASS/FAIL contra medición real con OTDR o power meter.
  - Conversor dBm ↔ mW con conversión en tiempo real.
  - Historial de hasta 50 mediciones con detalle y swipe-to-delete.
  - Compartir resultados con branding y link de descarga.
- **Glosario integrado:** Iconos de info junto a cada campo para aprender qué es cada parámetro.
- **Persistencia:** Recuerda tu último tipo de fibra, longitud de onda, tipo de empalme y margen.
- **Guía para no expertos:** Cada tipo de fibra incluye una descripción para saber cuál elegir.

### Sidebar reorganizado
- Las herramientas ahora están ordenadas por categoría lógica: WiFi → Red/Monitoreo → Internet/Exploración → Cableado/Fibra → Utilidades.
- Las herramientas Free y Pro aparecen intercaladas según su categoría, en lugar de separadas en bloques.

### Mejoras visuales
- **Selectores con colores por categoría:** Cada selector (tipo de fibra, longitud de onda, tipo de empalme) tiene su propio color distintivo para romper la monotonía visual.

👉 **[Ver el historial completo de cambios (Changelog)](CHANGELOG.md)**

---

## 📸 INTERFAZ Y HERRAMIENTAS

<div align="center">
  <img src="./assets/1.png?v=2" width="23%" alt="Pantalla de inicio"/>
  <img src="./assets/2.png?v=2" width="23%" alt="Escáner LAN"/>
  <img src="./assets/3.png?v=2" width="23%" alt="Monitor Celular"/>
  <img src="./assets/4.png?v=2" width="23%" alt="Canales WiFi"/>
</div>

<div align="center">
  <img src="./assets/5.png?v=2" width="23%" alt="Ping Monitor"/>
  <img src="./assets/6.png?v=2" width="23%" alt="Código Colores FO"/>
  <img src="./assets/7.png?v=2" width="23%" alt="Speed Test"/>
  <img src="./assets/8.png?v=2" width="23%" alt="Utilidades"/>
</div>

<div align="center">
  <img src="./assets/9.png?v=2" width="23%" alt="Detalles de Ping"/>
  <img src="./assets/10.png?v=2" width="23%" alt="Dispositivos Conectados"/>
  <img src="./assets/11.png?v=2" width="23%" alt="Escáner LAN Offline"/>
  <img src="./assets/12.png?v=2" width="23%" alt="Servicios Locales"/>
</div>

<div align="center">
  <img src="./assets/13.png?v=2" width="23%" alt="Estadísticas de Red"/>
  <img src="./assets/14.png?v=2" width="23%" alt="Analizador UPnP"/>
  <img src="./assets/15.png?v=2" width="23%" alt="Configuración Avanzada"/>
  <img src="./assets/16.png?v=2" width="23%" alt="Acerca de"/>
</div>

<div align="center">
  <img src="./assets/17.png?v=2" width="23%" alt="Más Funciones"/>
  <img src="./assets/18.png?v=2" width="23%" alt="Vista Repartidor Fibra"/>
  <img src="./assets/19.png?v=2" width="23%" alt="Favoritos en Home"/>
  <img src="./assets/20.png?v=2" width="23%" alt="Detalle de Puerto FO"/>
</div>

<br/>

<div align="center">
  <h3>🎥 Video Demostrativo</h3>
  <a href="https://www.youtube.com/shorts/OfS71W6PvSc" target="_blank">
    <img src="https://img.youtube.com/vi/OfS71W6PvSc/0.jpg" alt="Ver el Video Demostrativo de EgeaINC WiFi Analyzer" width="250" style="border-radius: 12px;"/>
  </a>
  <br/>
  <p><i>Haz clic en la imagen para ver el YouTube Short en acción</i></p>
</div>

---

## 🛠️ SUITE DE HERRAMIENTAS INTEGRADA

### Conectividad y Diagnóstico
- 📶 **Canales WiFi:** Analiza la congestión en 2.4GHz y 5GHz para encontrar el canal óptimo.
- 📋 **Historial WiFi:** Registra tus conexiones con datos de señal e ISP y tarjetas expandibles.
- 🔍 **Escáner LAN:** Descubre dispositivos en tu red con detección inteligente de altas/bajas.
- 🚪 **Escáner Puertos:** Detecta puertos TCP abiertos y servicios activos (HTTP, SSH, etc.).
- ⏱️ **Monitor Ping:** Mide la latencia en tiempo real con gráficas de scroll continuo.
- 🚀 **Speed Test:** Prueba de velocidad multi-conexión vía Cloudflare CDN con indicadores de cuello de botella.
- 📱 **Red Móvil:** Análisis profundo de señal celular.
- 🌍 **IP Pública:** Muestra tu IP externa y tu ISP.

### Cableado y Fibra Óptica
- 🔌 **Pinout RJ-45:** Guía visual de armado de cables UTP (T-568A/B).
- 🎨 **Código Color FO:** Visor interactivo de estándares TIA-598-C y SIECOR.
- 📉 **Calculadora dB Fibra:** Calcula la atenuación esperada de un enlace de fibra óptica según tipo de fibra, longitud de onda, distancia, empalmes, conectores y margen. Compara contra medición real (PASS/FAIL) e incluye conversor dBm↔mW.

### Utilidades y Referencias
- 🔑 **Generador Passwords:** Crea claves ultra seguras y personalizables.
- 🧮 **Calculadora IP:** Calcula subredes, rangos y máscaras CIDR.

---

## 💎 EGEAINC PRO (Premium)

Desbloquea las herramientas avanzadas y elimina todos los límites:

- 🔎 **DNS Lookup:** Consulta registros DNS (A, MX, TXT, NS, etc.).
- 🕵️ **Whois:** Obtén información detallada de registro y titularidad de dominios.
- 🛤️ **Traceroute:** Rastrea la ruta y mide los tiempos de salto de los paquetes en la red.
- ⚡ **Wake on LAN (WoL):** Enciende equipos de tu red de forma remota.
- 🔌 **Escáner UPnP:** Descubre dispositivos con Universal Plug and Play activo.
- ➕ **Funciones Pro adicionales:** Detección de celdas vecinas (Red Móvil), historial extendido (Speed Test) y filtros avanzados.

---

## 📱 CARACTERÍSTICAS DESTACADAS

- ✔️ **Diseño oscuro "glass":** Optimizado para pantallas OLED.
- ✔️ **Interfaz bilingüe:** Disponible en Español e Inglés.
- ✔️ **Glosario Educativo:** Toca cualquier métrica para aprender conceptos técnicos.
- ✔️ **Privacidad Garantizada:** Experiencia limpia, segura y sin rastreo oculto.

---

## 💬 Feedback y Soporte

Este repositorio está destinado exclusivamente a la comunidad para brindar **feedback, reportar errores y sugerir nuevas mejoras** de EgeaINC WiFi Analyzer. 

Si encontraste un bug o tienes una gran idea para la app:
👉 **[Abre un nuevo Issue aquí](https://github.com/gabriel600r/wifi-analyzer-feedback/issues)**

¡Gracias por ayudarnos a mejorar!
