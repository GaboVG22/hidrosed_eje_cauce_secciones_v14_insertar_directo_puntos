# HidroSed · Eje Cauce y Secciones v14

Versión enfocada en edición hidráulica de secciones, conectividad longitudinal tipo HEC-RAS e inserción directa de secciones por puntos.

## Entradas principales

- Eje del cauce KMZ/KML obligatorio.
- PC hidrológico KMZ/KML obligatorio.
- PC cuenca soporte KMZ/KML obligatorio.
- DEM por OpenTopography con API Key o DEM GeoTIFF manual.
- Perfil longitudinal de respaldo opcional.
- Curvas de nivel de apoyo opcionales.
- Excel prismático opcional.

## Mejora v14

Se incorpora **secciones por puntos directo en la aplicación**, sin necesidad de subir Excel/CSV.

En la pestaña:

`Ventana sección por km → Insertar secciones por puntos: km + coordenadas + cota + station`

puedes ingresar directamente en una tabla editable:

- `km` opcional;
- `station_m` obligatorio;
- `x` opcional/recomendado;
- `y` opcional/recomendado;
- `cota_m` obligatorio.

Si no se informa `km`, la app replica la misma sección entre `km inicial` y `km final` con la separación longitudinal definida.

Si se informa `km`, la app agrupa los puntos por progresiva y genera cada sección según su km.

## Funciones mantenidas

- Vista satelital con etiquetas km de cada sección.
- Eliminar sección individual.
- Eliminar secciones por tramo km.
- Interpolación entre secciones con separación.
- Canal trapecial o rectangular entre km X y km Y.
- Conectividad longitudinal tipo HEC-RAS.
- Exportación KMZ, Excel, CSV y JSON.

## Streamlit Cloud

- Main file path: `app.py`
- Python version: `3.11`

