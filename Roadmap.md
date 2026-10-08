# 🚀 Storage Manager — Roadmap & Development Cycle

Documento de ruta para el desarrollo de **Storage Manager**, siguiendo la convención de versionado `X.Y.Z-PP`.

---

## 📌 Convención de Versionado (`X.Y.Z-PP`)

* **`X` (Major):** Rediseño radical de la interfaz + adición masiva de funciones clave (ej. `2.0.0`).
* **`Y` (UI):** Cambios y mejoras enfocadas principalmente en la interfaz de usuario y navegación.
* **`Z` (Logic/Feats):** Nuevas funciones independientes, lógica del sistema o ajustes de backend.
* **`-PP` (Patch/Polish):** Parches internos de pulido, correcciones rápidas y retoques estéticos pre-release.

---

## 🗺️ Hoja de Ruta Actual

### 🟢 Versión 1.2.7 — Refinamiento Visual y Animaciones
* [x] **`1.2.7-01` (UI Polish):** Rediseño del gráfico sunburst/donut de discos, ajuste de paneles de navegación y vista de Ajustes.
* [ ] **`1.2.7-02` (Algorithm Polish):** Optimización del motor de escaneo de disco, gestión eficiente de memoria/CPU al procesar volúmenes grandes.
* [ ] **`1.2.7-03` (Animation System):** Sistema de animaciones fluidas en la interfaz con opción de personalización/ajuste en Preferencias.

---

### 🟡 Versión 1.2.8 — Modos Avanzados, Plugins y Changelog
* [ ] **Ciclo de Betas (Públicas/Testing):** Pruebas comunitarias de las funciones de la 1.2.8 antes de la integración final.
* [ ] **Escaneo Visual en Tiempo Real:**
  * Modo de escaneo interactivo ordenado de mayor a menor peso.
  * *Toggle* opcional en Ajustes (si no se activa, mantiene el spinner clásico de bajo consumo).
* [ ] **Consola CMD Integrada (Desactivada por defecto):**
  * Ventana de comandos para *power users*.
  * Ejecución de scripts que modifican la interfaz y ejecutan acciones del sistema.
  * Wiki oficial con la documentación de comandos.
* [ ] **Sistema de Plugins:** Soporte para que los usuarios creen y carguen sus propios módulos.
* [ ] **Changelog Oficial:** Panel nativo *"What's New"* dentro de la app para ver el historial de cambios y notas de versión.
* [ ] **Integración Inter-Process (IPC):** Conexión con la nueva app externa en desarrollo (fase final del ciclo 1.2.x).

---

## 🔴 Visión a Futuro — Versión 2.0.0 (Major Release)
* [ ] Salto definitivo a la versión 2.0.0 con la UI madura y lógica optimizada.
* [ ] Preparación y revisión de código fuente para el Merge Request oficial.
* [ ] Publicación en la **Droplet Store**.

---

> **Nota interna:** El desarrollo diario se mantiene en builds **Nightly privadas** utilizando el código fuente de `droppykit`. Las versiones beta y estables se compilan por separado para distribución.
