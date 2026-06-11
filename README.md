# Dashboard Interactivo CIF-IAA Honduras 2019–2025
 
<div align="center">
**Observatorio en Seguridad Alimentaria y Nutricional**  
Instituto de Investigaciones Sociales · Facultad de Ciencias Sociales  
Universidad Nacional Autónoma de Honduras (UNAH)
 
</div>
---
 
## Descripción
 
Este repositorio contiene el **dashboard interactivo** y el **boletín técnico-académico** producidos por el OBSAN-IIS-UNAH para documentar y analizar la evolución histórica de la **Clasificación Integrada de Seguridad Alimentaria en Fases (CIF)** — escala de **Inseguridad Alimentaria Aguda (IAA)** — en Honduras durante el período **2019–2025**.
 
El dashboard (`index.html`) es un archivo HTML monolítico y autocontenido que no requiere instalación, servidor web ni conexión a internet para funcionar. Incorpora ocho análisis CIF publicados por la Unidad Técnica de Seguridad Alimentaria y Nutricional (UTSAN-SAG), con cobertura de 19–20 áreas departamentales y el período noviembre 2019 – noviembre 2025.
 
---
 
## Vista rápida
 
| Indicador | Valor (CIF-2025.11, Situación Actual) |
|---|---|
| Población analizada | 10.19 millones |
| Población en Fase 3+ | ~1.39 millones (13.6 %) |
| Personas en Fase 4 | 35 449 (0.3 %) |
| Áreas en Fase 3 | 3 / 19 (Gracias a Dios, Lempira, Yoro) |
| Nivel de evidencia | *** Alto |
| Período cubierto | Nov 2025 – Mar 2026 (Situación Actual) |
| Publicación | 10 de junio de 2026 (UTSAN, oficial) |
 
> ⚠️ **Nota metodológica:** El análisis de 2019 cubre exclusivamente población rural en 13 áreas; las cifras absolutas no son directamente comparables con los años posteriores, por lo que la comparación interanual privilegia porcentajes. El análisis CIF-2025.11 es **oficial**, confirmado por el informe UTSAN *Noviembre 2025 – Octubre 2026* (publicado el 10 de junio de 2026); las cifras preliminares coincidieron exactamente con las oficiales.
 
---
 
## Contenido del repositorio
 
```
📁 /
├── index.html                          # Dashboard interactivo 
├── LICENSE                             # Licencia MIT
└── README.md                           # Este archivo
```
 
---
 
## Dashboard interactivo
 
### Características
 
- **Archivo único HTML** — sin dependencias locales; librerías cargadas por CDN (Chart.js, Leaflet)
- **Datos embebidos** como JSON — derivados de `data_historica_cif.xlsx` (393 registros)
- **Solo Situación Actual** — las dos proyecciones de cada informe se excluyen del análisis longitudinal
- **Mapa cartográfico real** — polígonos departamentales de Honduras generados con GeoJSON oficial
- **Paleta CIF oficial inviolable** para visualizaciones de fase (F1–F5)
- **Toggle de tema** claro/oscuro — la paleta CIF se mantiene inviolable en ambos modos
- **Toggle "Excluir 2019"** — para análisis de tendencia sin la asimetría de cobertura
### Paneles disponibles
 
| Panel | Descripción |
|---|---|
| **KPI** | Cifras clave del último análisis oficial (CIF-2025.11): población, % Fase 3+, áreas afectadas |
| **Serie temporal nacional** | Gráfico de línea 2019–2025 con selector de métrica (%, N absoluto, F3+, F4+) |
| **Mapa coroplético** | Honduras por departamento con selector de año y tooltip detallado |
| **Heatmap** | Matriz departamento × año de % en Fase 3+ |
| **Barras apiladas** | Distribución porcentual por fases (F1–F5) por año |
| **Tabla filtrable** | Datos detallados con filtros por año, departamento y fase; descarga CSV |
 
### Codificación cromática oficial CIF
 
| Fase | Denominación | Color |
|---|---|:---:|
| 1 | Mínima/Ninguna | ![#CDFACD](https://placehold.co/15x15/CDFACD/CDFACD.png) `#CDFACD` |
| 2 | Acentuada | ![#FAE61E](https://placehold.co/15x15/FAE61E/FAE61E.png) `#FAE61E` |
| 3 | Crisis | ![#E67800](https://placehold.co/15x15/E67800/E67800.png) `#E67800` |
| 4 | Emergencia | ![#C80000](https://placehold.co/15x15/C80000/C80000.png) `#C80000` |
| 5 | Catástrofe/Hambruna | ![#640000](https://placehold.co/15x15/640000/640000.png) `#640000` |
 
### Cómo usar
 
1. Descargar `index.html`
2. Abrir con cualquier navegador moderno (Chrome, Firefox, Edge, Safari — últimas tres versiones)
3. No se requiere instalación, servidor local ni conexión a internet
---
 
 
## Fuentes de datos
 
### Serie CIF-IAA (Situación Actual, UTSAN)
 
| Análisis | Áreas | Pob. analizada | Pob. F3+ | % F3+ |
|---|:---:|---:|---:|:---:|
| CIF-2019.12 | 13 (solo rural) | 5.12 M | 964 K | 18 % |
| CIF-2020.06 | 13 (solo rural) | 5.12 M | 1.65 M | 32 % |
| CIF-2020.12 | 18 áreas | 9.30 M | 2.91 M | 31 % |
| CIF-2021.12 | 18 áreas | 9.60 M | 2.23 M | 24 % |
| CIF-2022.12 | 20 áreas | 9.74 M | 2.30 M | 23 % |
| CIF-2023.12 | 19 áreas | 9.89 M | 1.77 M | 18 % |
| CIF-2024.12 | 19 áreas | 10.04 M | 1.78 M | 18 % |
| CIF-2025.11 | 19 áreas | 10.19 M | 1.39 M | 13.6 % |
 
> ✅ CIF-2025.11: **oficial**, confirmado por el informe UTSAN *Noviembre 2025 – Octubre 2026* (publicado el 10 de junio de 2026). Tres áreas en Fase 3 (Gracias a Dios, Lempira, Yoro); 35 449 personas en Fase 4 (0.3 %); evidencia *** Alto.
 
### Informes fuente
 
Los datos provienen de los informes oficiales UTSAN publicados por la Secretaría de Agricultura y Ganadería (SAG) de Honduras en el marco del Proceso Global CIF/IPC. Ante cualquier discrepancia entre la base `data_historica_cif.xlsx` y los informes PDF originales, **el informe PDF es la fuente canónica**.
 
- UTSAN (2020a). *Informe CIF Honduras Nov 2019 – Jun 2020*
- UTSAN (2020b). *Actualización CIF Honduras Jun – Ago 2020*
- UTSAN (2021). *Informe CIF Honduras Dic 2020 – Sep 2021*
- UTSAN (2022). *Informe CIF Honduras Dic 2021 – Ago 2022*
- UTSAN (2023). *Informe CIF Honduras Dic 2022 – Ago 2023*
- UTSAN (2024). *Informe CIF Honduras Dic 2023 – Ago 2024*
- UTSAN (2025). *Informe CIF Honduras Dic 2024 – Nov 2025*
- UTSAN (2026). *Informe CIF Honduras Nov 2025 – Oct 2026* (publicado el 10 de junio de 2026)
Metodología CIF: [https://www.ipcinfo.org](https://www.ipcinfo.org) | Manual Técnico CIF v3.1
 
---
 
## Protocolo de comparabilidad longitudinal
 
La serie 2019–2025 presenta tres fuentes de no-comparabilidad estricta:
 
1. **Asimetría 2019** — primer análisis cubre solo 13 áreas y población rural (~6 M); los posteriores incluyen 19–20 áreas y población total (~10 M). Se privilegian porcentajes sobre cifras absolutas para comparación interanual.
2. **Ventanas temporales heterogéneas** — cada informe cubre períodos distintos (Nov–Jun, Dic–Ago, Dic–Nov). Cada punto se etiqueta con su ventana exacta.
3. **Solo Situación Actual** — el análisis longitudinal excluye las proyecciones de cada informe; los 8 puntos corresponden exclusivamente a la situación observada.
---
 
## Créditos institucionales
 
**Producción y análisis:**  
Christian Alexis Manzanares Cruz  
ORCID: [0009-0004-7419-0449](https://orcid.org/0009-0004-7419-0449)  
Especialista en Sistemas de Información  
OBSAN — Instituto de Investigaciones Sociales (IIS) — Facultad de Ciencias Sociales (FCCSS) — UNAH
 
**Institución:**  
Observatorio en Seguridad Alimentaria y Nutricional (OBSAN-IIS-UNAH)  
Universidad Nacional Autónoma de Honduras  
[obsan.unah.edu.hn](https://obsan.unah.edu.hn)
 
**Datos primarios:**  
Unidad Técnica de Seguridad Alimentaria y Nutricional (UTSAN)  
Secretaría de Agricultura y Ganadería (SAG) — Honduras

---
 
## Licencia
 
Este proyecto se distribuye bajo la [Licencia MIT](./LICENSE).  
Los datos derivados de informes UTSAN deben citarse con referencia a la fuente primaria.  
La codificación cromática oficial CIF (F1–F5) es propiedad del Proceso IPC Global; su uso aquí es académico e informativo, conforme al Manual Técnico CIF v3.1.
 
---
 
<div align="center">
<sub>OBSAN-IIS-UNAH · Honduras · 2026 · v1.2 (versión final, datos oficiales CIF-2025.11) · Generado con fines académicos e institucionales</sub>
</div>
