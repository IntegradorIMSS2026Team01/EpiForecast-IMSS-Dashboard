# 🌐 EpiForecast-MX Dashboard

**Pronósticos epidemiológicos inteligentes para padecimientos neurológicos y de salud mental en México.**

🔗 **Sitio en vivo:** [proyectointegrador.org](https://proyectointegrador.org/)

---

## Descripción

Dashboard interactivo del proyecto **EpiForecast-MX**, desarrollado en colaboración entre el **Tecnológico de Monterrey** y el **Instituto Mexicano del Seguro Social (IMSS)**. El sitio presenta visualizaciones de datos epidemiológicos para tres padecimientos clave:

| Código CIE-10 | Padecimiento |
|:-:|---|
| F32 | Depresión |
| G20 | Enfermedad de Parkinson |
| G30 | Enfermedad de Alzheimer |

## Visualizaciones

El dashboard incluye las siguientes secciones interactivas construidas con **Tableau Public**:

- **Tabla de datos consolidada** — Datos acumulados por entidad federativa, año y semana epidemiológica, con información demográfica del INEGI.
- **Mapa de México** — Densidad poblacional, superficie territorial y casos desagregados por sexo con filtros interactivos.
- **Categorías territoriales** — Categorizaciones por región geográfica, región socio-urbana, ratio de género, extensión territorial y densidad poblacional.
- **Casos por año** — Incremento anual de casos desagregado por sexo, con filtros por año y padecimiento.
- **Casos por semana** — Dinámica temporal de corto plazo dentro de cada año epidemiológico.
- **Predicciones** — Proyecciones del modelo Prophet para cada padecimiento *(en desarrollo)*.

## Fuentes de datos

- **SINAVE** — Boletines epidemiológicos semanales (2012–2025), procesados mediante pipeline automatizado.
- **INEGI** — Datos demográficos complementarios por entidad federativa.

## Stack técnico

| Componente | Tecnología |
|---|---|
| Frontend | HTML5 estático |
| Visualización | Tableau Public (embeds interactivos) |
| Hosting | Netlify |
| Repositorio | GitHub (IntegradorIMSS2026Team01) |

## Estructura del sitio

```
EpiForecast-IMSS-Dashboard/
├── index.html                  # Página principal del proyecto
├── EpiDashboard.html           # Dashboard con visualizaciones Tableau
├── Avance1.Equipo01.html       # Reporte de avance (HTML)
├── Avance1.Equipo01.pdf        # Reporte de avance (PDF)
├── pipeline_diagramEDA.html    # Diagrama del pipeline EDA
└── README.md
```

## Desarrollo local

Para visualizar el sitio localmente:

```bash
# Clonar el repositorio
git clone https://github.com/IntegradorIMSS2026Team01/EpiForecast-IMSS-Dashboard.git
cd EpiForecast-IMSS-Dashboard

# Servir con Python
python3 -m http.server 8080

# Abrir en navegador: http://localhost:8080
```

## Despliegue

El sitio se despliega automáticamente a través de **Netlify** al hacer push a la rama `main`. No requiere comandos de build.

## Proyecto principal

Este dashboard es el componente de visualización del proyecto [EpiForecast-MX](https://github.com/IntegradorIMSS2026Team01/EpiForecast-MX), que incluye el pipeline completo de extracción, procesamiento y modelado de datos epidemiológicos.

## Equipo

| Integrante | Rol |
|---|---|
| Javier Rebull | Sr. Asocciate Application Developer - Santander Bank US |
| Juan Carlos Pérez Nava | Profesional de TI — IMSS |
| Luis Gerardo Sánchez Salazar | Sr. Controls Engineer — Tesla |

**Asesora académica:** Dra. Grettel Barceló Alonso — Tecnológico de Monterrey

**Stakeholders IMSS:** Dra. Ruth Pérez (Líder de Proyecto) · Dra. Lina Díaz Castro (Investigadora en Psiquiatría)

---

<p align="center">
  <strong>Tecnológico de Monterrey</strong> · <strong>IMSS</strong> · Equipo 01 — 2026
</p>
