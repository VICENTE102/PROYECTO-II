# ⚡ Análisis Integrado de Generación Energética y Factores Climáticos en España

Este repositorio contiene el desarrollo completo del proyecto realizado en la asignatura **Proyecto II**, perteneciente al Grado en Ciencia de Datos (UPV). El objetivo general del trabajo es analizar distintos aspectos de la generación energética en España mediante la integración de datos de diferentes fuentes, principalmente **Red Eléctrica de España (REE)** y **AEMET (Agencia Estatal de Meteorología)**.

---

## 🧭 Estructura del repositorio

```text
📦 root
├── hito_1/                     # Fichas y fuentes analizadas (Hito 1)
├── hito_2/                     # Procesamiento y transformación de datos (Hito 2)
│   ├── clima/                  # Códigos y datos relacionados con AEMET
│   └── energia/                # Códigos y datos relacionados con REE
│
├── objetivos/                 # Desarrollo de los objetivos individuales
│   ├── objetivo_1_pablo/       # Relación clima ↔ energía hidráulica
│   ├── objetivo_2_nombre/      # Objetivo 2
│   ├── objetivo_3_nombre/      # Objetivo 3
│   └── ...                     # Resto de objetivos
│
├── data/                      # Conjunto de datos finales utilizados
│   ├── generacion_todas_comunidades.csv
│   ├── clima_coruna.csv
│   ├── clima_leon.csv
│   └── ...                     # Otros datasets limpios
│
├── docs/                      # Informes, memoria final y anexos HTML
│   ├── memoria_final.docx
│   ├── index_anexos.md
│   ├── memoria_anexo_1.html
│   ├── memoria_anexo_2.html
│   └── ...
│
└── README.md                  # Este archivo

```
---

## 🧪 Tecnologías y librerías usadas

- **Lenguaje**: R
- **Entorno**: RStudio + R Markdown
- **Librerías principales**:
  - `dplyr`, `tidyr`, `stringr`, `ggplot2`, `plotly`, `corrplot`, `scales`, `jsonlite`, `readr`, `knitr`, `naniar`, 

---

## 🎯 Objetivos del proyecto

Cada miembro del equipo se ha encargado de un **objetivo individual** dentro del marco del análisis energético. Todos los objetivos comparten las siguientes características:

- Uso de **fuentes cruzadas** (al menos dos).
- Aplicación de técnicas estadísticas y gráficas para responder una hipótesis concreta.
- Desarrollo técnico replicable y bien documentado.

### Objetivos especificos:

- **Objetivo 1**: Estudiar la relación entre precipitaciones y generación de energía hidráulica en Galicia y Castilla y León (autor: Pablo Alpuente).
- **Objetivo 2**: Analizar la evolución general de las energías renovables en invierno y verano.
- **Objetivo 3**: Evaluar el balance energético por comunidad.
- **Objetivo 4**: Estudiar la generación de energía solar fotovoltaica de las comunidades en función del tiempo meteorológico u otras variables semejantes
- **Objetivo 5**: Analizar la relación entre la precipitación mensual y la energía hidráulica generada en comunidades seleccionadas (Galicia y Castilla y León).

---

## 📥 Fuentes de datos

- **Red Eléctrica de España (REE)**: Datos de generación mensual por tecnología y comunidad autónoma --> [https://www.ree.es/es/datos/aldia]
- **AEMET (API oficial)**: Datos meteorológicos mensuales por estación (precipitaciones, temperaturas, días de lluvia…) --> [https://opendata.aemet.es/centrodedescargas/productosAEMET?]

---

## 🛠️ Ejecución del código

Todos los scripts se encuentran ordenados por carpeta. Puedes reproducir los análisis cargando cada `.Rmd` dentro de su carpeta respectiva. Los datos ya están limpios y disponibles en `data/`.

---

## 📄 Documentación y memoria

La memoria final y todos los anexos generados en RMarkdown compilado a HTML están en la carpeta `docs/`. El índice de anexos está también disponible en `docs/index_anexos.md`.

---

## 👩‍🏫 Evaluación técnica

Cada objetivo está diseñado para ser defendido individualmente por cada alumno. El código está documentado con comentarios y estructurado para facilitar su exposición en la defensa técnica final.

---

## 📜 Licencia

Este proyecto es exclusivamente académico y no está destinado a uso comercial. Todas las fuentes utilizadas son públicas y oficiales.
