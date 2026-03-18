# Changelog

Todos los cambios notables de este proyecto se documentarán en este archivo.

El formato está basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.0.0/), 
y este proyecto se adhiere a [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

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
