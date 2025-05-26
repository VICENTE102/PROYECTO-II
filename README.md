# ⚡ Análisis Integrado de Generación Energética y Factores Climáticos en España

Este repositorio contiene el desarrollo completo del proyecto realizado en la asignatura **Proyecto II**, perteneciente al Grado en Ciencia de Datos (UPV). El objetivo general del trabajo es analizar distintos aspectos de la generación energética en España mediante la integración de datos de diferentes fuentes, principalmente **Red Eléctrica de España (REE)** y **AEMET (Agencia Estatal de Meteorología)**.

---

# Autores

- Víctor Lorenzo López
- Marc Fernández Cortina
- Pablo Alpuente Tabasco
- Vicente Ricós Caras
- José Miguel García Ríos
  
# Tutora de la Asignatura 
- 	Ramírez Quintana, María José

## 🧭 Estructura del repositorio

```text
📦 root
├── hito_1/                     # Fichas y fuentes analizadas (Hito 1)
├── hito_2/                     # Procesamiento y transformación de datos (Hito 2)
│   ├── ....pdf       # Códigos y datos relacionados con AEMET
│   └── ....html              # Códigos y datos relacionados con REE
│
├── objetivos/                 # Desarrollo de los objetivos individuales
│   ├── objetivo_1_miguel/       # Relación clima ↔ energía hidráulica
│   ├── objetivo_2_nombre/      # Objetivo 2
│   ├── objetivo_3_nombre/      # Objetivo 3
│   └── ...                     # Resto de objetivos
│
├── data/                      # Conjunto de datos finales utilizados
│   ├── aemet/
│       │── aemet_objetivo4...
│   ├── ree/   
│       ├── generacion_todas_comunidades.csv 
│       ├── generation.zip     # zip con todos los csv por comunidad       
│       ├── .....
|
├── docs/                      # Informes, memoria final y anexos HTML
│   ├── memoria_final.docx
│   ├── index_anexos.md
│   ├── hito_2.html
│   ├── objetivo_4_vicente.html
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

Durante la evaluación técnica, se podrá mostrar y explicar:

- El **flujo completo del análisis**: desde la limpieza de datos brutos hasta la obtención de los resultados.
- La **descarga y transformación** de datos desde la API de AEMET en formato JSON y su tratamiento para convertirlo en CSV limpio.
- El uso de **paquetes clave** en R como `dplyr`, `ggplot2`, `tidyr`, `corrplot`, `plotly` o `lubridate`, y su aplicación contextualizada en cada parte del análisis.
- La aplicación y justificación de técnicas como:
  - Análisis exploratorio y visualizaciones descriptivas.
  - Transformación de variables (escalado, creación de variables categóricas como estación del año…).
  - Cálculo de **correlaciones no paramétricas (Spearman)** por ser más robustas ante no linealidad y distribuciones no normales.
  - Ajuste de modelos de **regresión lineal y polinómica** para evaluar relaciones funcionales entre variables.
  - Comparación entre modelos con métricas como el **R² ajustado**.
  - Análisis estacional mediante **boxplots por estación climática**.
- La toma de decisiones fundamentadas (por ejemplo, descartar ciertas variables o cambiar de estación meteorológica en función de la disponibilidad y calidad del dato).
- Las **limitaciones identificadas** en cada objetivo y la forma en que han sido abordadas (como la inercia hídrica, gestión de embalses o comportamiento no inmediato de la lluvia sobre la generación energética).
- Las justificaciones metodológicas del **workflow seguido**, explicando por qué se ha utilizado cada técnica y qué aporta al objetivo final.

Los scripts están compilados en HTML como anexos (`docs/`) para facilitar su consulta durante la defensa. Cada estudiante deberá estar preparado para explicar su parte del código, ejecutar una parte del análisis y razonar las conclusiones obtenidas a partir de los gráficos y modelos generados.


---

## 📜 Licencia

Este proyecto es exclusivamente académico y no está destinado a uso comercial. Todas las fuentes utilizadas son públicas y oficiales.

---

## 🔄 Acceso y colaboración

Como se decia anteriormente, este repositorio es público y está pensado para que cualquier persona interesada en el análisis de datos, energías renovables o aprendizaje de R pueda consultarlo, reutilizarlo o proponer mejoras.

Se aceptan sugerencias, aportaciones o correcciones mediante Pull Requests o Issues. El código está documentado para facilitar su comprensión y reutilización.

- Clonación del repositorio:

Puedes clonar este repositorio en tu máquina local para explorar su estructura o trabajar sobre él.

#### Usando SSH (recomendado si ya tienes clave configurada):

```bash
git clone git@github.com:VICENTE102/PROYECTO-II.git
cd PROYECTO-II
```
---

### 🧪 Abrir y trabajar con los `.Rmd`

Una vez clonado el repositorio, puedes abrir cualquier archivo `.Rmd` desde **RStudio** o la terminal.

#### Opción 1: Desde RStudio

1. Abre **RStudio**.
2. Ve a **File > Open Project...** o simplemente abre la carpeta donde hayas clonado el proyecto.
3. Navega a la carpeta del objetivo que quieras consultar.
4. Abre el archivo `.Rmd` y pulsa **Knit** para compilarlo a HTML, Word o PDF.

#### Opción 2: Desde la terminal

1. Abre una terminal en la carpeta del proyecto:

```bash
cd PROYECTO-II
```
2. Inicia una sesión de R:
```bash
R
```
3. Dentro de R, compila el .Rmd que quieras: 
```bash
#ejemplo:
rmarkdown::render("objetivos/objetivo_1_pablo/analisis_objetivo_1.Rmd")
```

Esto generará automáticamente el documento de salida (por ejemplo, analisis_objetivo_1.html) en la misma carpeta.
Asegúrate de tener instalados los paquetes rmarkdown y knitr. Puedes hacerlo con:

```bash
install.packages("rmarkdown")
install.packages("knitr")
```
---

### 🛠️ Sugerencias para colaborar

- Trabaja siempre en ramas diferentes si haces cambios importantes.
- Ejecuta git pull antes de modificar nada.
- Usa nombres claros para los commits.
- Si encuentras errores o posibles mejoras, abre un Issue.
##### Las contribuciones son bienvenidas a través de Pull Requests!!!
