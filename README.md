# RUTIX Logística Global — Torre de Control Logística Multipaís BI

Este repositorio contiene la replicación completa, reactiva y *pixel-perfect* de la **Torre de Control Logística Multipaís** de **RUTIX Logística Global S.A.S.**, basada en la especificación visual y técnica del *Prompt Maestro*.

---

## 🚀 Cómo Ejecutar la Aplicación

No requiere instalación de dependencias pesadas ni compilación. La solución está desarrollada en estándares web modernos (**HTML5, Tailwind CSS 3, Chart.js**):

1. **Abrir directamente:**
   Hacer doble clic en [`index.html`](file:///Users/amauryarteagag/Desktop/Power%20bi/index.html) para abrirlo en cualquier navegador web moderno (Chrome, Safari, Edge, Firefox).

2. **O servirlo localmente mediante Python:**
   ```bash
   cd "/Users/amauryarteagag/Desktop/Power bi"
   python3 -m http.server 8080
   ```
   Luego ingresar a: [http://localhost:8080](http://localhost:8080)

---

## 📐 Estructura de Navegación (8 Vistas Interactivas)

| Vista | Identificador | Descripción y Métricas Clave |
|---|---|---|
| **1. Resumen Ejecutivo** | `resumen` | Visión holística: OTD (94.7%), Costos ($372M), Incidencias (37), CSAT (4.5/5), tendencia semanal y desglose circular de 1.240 envíos. |
| **2. Dirección General (CEO)** | `direccion` | Perspectiva ejecutiva multivariable: Evolución de costos vs Presupuesto ($380M), CSAT histórico, Pareto mensual y **Modelo Financiero ROI (29.04%, Payback 0.78 años, VPN $6.7M COP)**. |
| **3. Gerencia de País** | `gerencia` | Comparativo por Hub Urbano (Bogotá, Medellín, Cartagena, Cali, Barranquilla) con barras de cumplimiento SLA (≥95%) y participación en volumen. |
| **4. Operaciones Logísticas** | `operaciones` | Mesa de despachos por Guía de Transporte con filtrado reactivo por severidad (**Alta, Media, Baja**), modal telemático y protocolo de contingencia. |
| **5. KPI 1: Seguimiento de Envíos** | `kpi1` | Envíos monitoreados (1.240), cobertura operativa (5 ciudades), 18.4 Ton de carga movilizada, $558M COP declarados, y slicer temporal interactivo. |
| **6. KPI 2: Cumplimiento OTD** | `kpi2` | Cumplimiento OTD (92.5%), meta SLA (95%), 1.147 unidades conformes, y **Cross-Filtering dinámico por transportista** (TransLogix, Servirápido, CargaExpress, EnvíosCo, Flota Local). |
| **7. KPI 3: Costos Logísticos & ROI** | `kpi3` | Costo Total ($48.6M COP), desglose tipo cascada (Fletes $28.5M, Consolidación $12M, Sobrecostos $5.1M, Sistemas $3M), y árbol de descomposición Costo/Km por tipo de flota. |
| **8. KPI 4: Gestión de Incidencias** | `kpi4` | 38 novedades operativas, 8 casos críticos de severidad alta, SLA de cierre (4.2h vs 6h meta), diagrama de Pareto 80/20 y acción directa para aislar casos críticos. |

---

## 🎨 Sistema de Diseño y Tokens de Color

- **Canvas de fondo:** `#F8FAFC`
- **Tarjetas KPI elevadas:** `#FFFFFF` con radio `18px`, borde sutil `#F1F5F9` y sombra suave.
- **Primario Corporativo / Navy:** `#1C2D4A` / `#0F172A`
- **Acento Activo / Terracota:** `#EA580C` con badge de selección `#FEEBE7` / `#FEF3C7`
- **Meta Cumplida (Éxito):** `#16A34A` / `#DCFCE7` (SLA ≥ 95%)
- **En Alerta / Desviación Media:** `#EAB308` / `#FEF3C7`
- **Crítico / Ruptura de SLA:** `#DC2626` / `#FEE2E2`

---

## ⚡ Interacciones Implementadas

- **Simulador de Seguridad por Rol (Row-Level Security - RLS):**
  El selector superior permite alternar instantáneamente entre **Dirección General (CEO)**, **Gerencia de País** y **Jefe de Operaciones**, adaptando el alcance visual y la pantalla por defecto.
- **Cross-Filtering Interactivo:**
  Al hacer clic en cualquier barra de transportista en la vista de *Cumplimiento OTD*, se recalculan y filtran los indicadores de la flota.
- **Modo Táctil / Simulador Móvil:**
  El botón de teléfono en la cabecera activa un viewport de smartphone estilizado con esquinas redondeadas y muesca para validar la experiencia ergonómica de supervisores en terreno.
- **Expediente Telemático Modal:**
  Al hacer clic en cualquier fila de la tabla de operaciones o en "Detalles", se abre una ventana modal con el diagnóstico satelital GPS y botón para disparar WhatsApp al transportista.
- **Slicer Temporal & Buscador Global:**
  Permite filtrar por período (`Oct 2026`, `Sep 2026`, `Ago 2026`) y buscar directamente por número de guía o ciudad (`GD-20418`, etc.).

---

## 📁 Archivos en el Entorno

- [`index.html`](file:///Users/amauryarteagag/Desktop/Power%20bi/index.html): Aplicación web reactiva autónoma y completa.
- [`images/`](file:///Users/amauryarteagag/Desktop/Power%20bi/images): Capturas de referencia originales extraídas del documento maestro (`image1.png` a `image8.png`).
- [`prompt_maestro.docx`](file:///Users/amauryarteagag/Desktop/Power%20bi/prompt_maestro.docx): Documento original con las especificaciones y lineamientos.

# Power-bi
