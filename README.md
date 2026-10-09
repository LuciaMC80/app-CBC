# Manejo del carcinoma basocelular

Herramienta web de apoyo a la decisión clínica para clasificar el carcinoma
basocelular (CBC) y obtener las recomendaciones de manejo de las guías
**EADO 2023** (European Association of Dermato‑Oncology, con EDF, ESTRO, UEMS y EADV),
**BAD 2021** (British Association of Dermatologists), **AEDV 2019** (Academia Española
de Dermatología y Venereología) y la **guía de práctica clínica del CBC en el síndrome
de Gorlin** (*J Am Acad Dermatol* 2026), con la evidencia posterior más relevante.
Cada recomendación indica la guía de la que procede.

**Abrir la aplicación:** https://luciamc80.github.io/app-CBC/

## Qué hace

A partir de los datos del caso (edad, inmunodepresión, síndrome de Gorlin, situación
terapéutica, radioterapia previa, presentación primaria o recidivada, área H/M/L, diámetro,
bordes, dificultad técnica, multiplicidad, subtipo histológico, invasión perineural, profundidad,
invasión ósea, márgenes y extensión) la aplicación devuelve:

- **Estadio EADO** (I, IIA, IIB, IIIA, IIIB, IIIC, IV): fácil o difícil de tratar.
- **Riesgo de recidiva bajo o alto** según BAD 2021 (NCCN adaptada a UICC‑8 y RCPath),
  con los factores de alto riesgo presentes, y **pT de UICC‑8**.
- **Veredictos** de tratamiento de elección, margen quirúrgico, actitud tras la exéresis
  (márgenes libres, cercanos o afectos), radioterapia, pruebas de imagen, tratamiento
  sistémico y seguimiento.
- Recomendaciones de **clasificación, diagnóstico, cirugía, tratamientos no quirúrgicos
  (imiquimod, 5‑FU, terapia fotodinámica, criocirugía, curetaje), radioterapia, CBC avanzado
  (inhibidores de Hedgehog, cemiplimab, electroquimioterapia, cuidados de soporte),
  paciente inmunodeprimido, seguimiento y prevención**.
- **Síndrome de Gorlin**: recuento de criterios diagnósticos mayores y menores, cribado
  según el gen (PTCH1 o SUFU) y las 47 recomendaciones de la guía de 2026 aplicables
  (tópicos, terapia fotodinámica, cirugía ahorradora, contraindicación de la radioterapia,
  inhibidores de Hedgehog intermitentes, SUFU, niños, salud mental).
- **Evidencia posterior a las guías** (etiqueta «Post‑guía»): análisis final de cemiplimab
  en el CBC metastásico (*Ann Oncol* 2024), cemiplimab neoadyuvante (ASCO 2026) y estado
  del ensayo fase 3 de patidegib tópico en el síndrome de Gorlin.
- **Filtro** para ver todas las recomendaciones o sólo las de una guía.
- **Resumen imprimible** del caso.

## Uso en el móvil

Se abre desde el navegador con el enlace de arriba. Para dejarla como una app:

- **Android (Chrome):** menú ⋮ → *Añadir a pantalla de inicio*.
- **iPhone (Safari):** botón de compartir → *Añadir a pantalla de inicio*.

Instalada de este modo funciona **sin conexión**.

## Compartir un caso

El botón **Compartir caso** genera un enlace que lleva los datos del caso en la
propia dirección (después de `#`). Los datos **no salen del dispositivo**: la
aplicación no tiene servidor, no guarda nada y no registra ninguna información.

## Aviso

Herramienta de apoyo a la decisión. **No sustituye el juicio clínico ni la
valoración del comité multidisciplinar de tumores.** No es un producto sanitario
certificado y no debe usarse como única base de una decisión asistencial.

## Fuentes

- Peris K, Fargnoli MC, et al. European consensus-based interdisciplinary guideline for
  diagnosis and treatment of basal cell carcinoma — update 2023. *Eur J Cancer* 2023;192:113254.
- Nasr I, et al. British Association of Dermatologists guidelines for the management of
  adults with basal cell carcinoma 2021. *Br J Dermatol* 2021;185:899–920.
- Vílchez‑Márquez F, et al. Guía de práctica clínica de carcinoma basocelular de la
  Academia Española de Dermatología y Venereología, 2019.
- Cahn BA, et al. Clinical practice guidelines for the management of basal cell carcinoma
  in Gorlin syndrome. *J Am Acad Dermatol* 2026;94:485–94.
- Grob JJ, et al. Position statement on classification of basal cell carcinomas, partes 1 y 2.
  *J Eur Acad Dermatol Venereol* 2021;35:1949–56 y 2149–53.
- UICC TNM Classification of Malignant Tumours, 8.ª ed.
- Las posiciones de NCCN se recogen tal como las citan BAD 2021, EADO 2023 y AEDV 2019.
- Evidencia posterior: Final analysis of phase II results with cemiplimab in metastatic
  basal cell carcinoma after hedgehog pathway inhibitors. *Ann Oncol* 2024;35:221–8.
  Ensayo NCT05929664 (cemiplimab neoadyuvante), ASCO 2026. Ensayo 2023‑507528‑21‑00 (patidegib).

## Contenido del repositorio

| Archivo | Descripción |
| --- | --- |
| `index.html` | La aplicación completa (interfaz y lógica en un único archivo). |
| `manifest.webmanifest` | Datos de instalación como app (nombre, iconos, colores). |
| `sw.js` | *Service worker*: permite el uso sin conexión. |
| `fonts/` | Tipografías IBM Plex Sans y JetBrains Mono (licencia SIL Open Font License). |
| `icons/` | Iconos de la app. |
