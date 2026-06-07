# Dashboard de Monitoreo de Condiciones Ambientales
## DVA Ingeniería - Power BI

## Descripción
Dashboard interactivo desarrollado en Power BI para el monitoreo 
de condiciones ambientales (temperatura y humedad) de bodegas 
durante estudios de mapeo térmico. Los datos provienen de 
Termohigrómetros Dataloggers con correcciones de calibración 
acreditadas ante ONAC.

## Características técnicas

### Modelo de datos (Star Schema)
- **FACT_MEDICIONES** — tabla de hechos con mediciones por sensor
- **DIM_SENSOR** — dimensión de sensores con nivel y cluster
- **DIM_BODEGA** — dimensión de bodegas
- **DIM_TIEMPO** — dimensión de tiempo
- **Parámetros dinámicos** — Param_TempMin, Param_TempMax, Param_HumMin, Param_HumMax

### ETL en Power Query
- Separación de datos por bodega
- Limpieza y transformación de datos
- Creación de tablas dimensionales
- Aplicación de correcciones de calibración ONAC

### DAX
- Cálculo de % Cumplimiento Ambiental con CALCULATE
- Métricas de temperatura y humedad por sensor y bodega
- Clustering de sensores por cumplimiento

## Páginas del Dashboard
1. **Tendencias** — Temperatura y humedad promedio por sensor/bodega con filtros interactivos
2. **Cumplimiento Parametrizado** — % cumplimiento con sliders dinámicos de rangos
3. **Resumen** — Tendencias con intervalos de confianza al 95%
4. **Mapa de Clusters** — Dispersión de sensores por temperatura y humedad
5. **Página de Ayuda** — Guía interactiva con anotaciones + botón reset por pestaña

## Stack
- Power BI Desktop
- Power Query (ETL)
- DAX
- Termohigrómetros Dataloggers (fuente de datos)

## Capturas del Dashboard

### Tendencias de Temperatura y Humedad
![Tendencias](imagenes/tendencias.png)

### Cumplimiento Ambiental Parametrizado
![Cumplimiento](imagenes/cumplimiento.png)

### Resumen con Intervalos de Confianza
![Resumen](imagenes/resumen.png)

### Mapa de Clusters por Sensor
![Clusters](imagenes/clusters.png)

### Página de Ayuda
![Ayuda](imagenes/ayuda.png)

## Archivo .pbix
El archivo .pbix está disponible bajo solicitud.
📩 Contáctame en: linkedin.com/in/gustavo-adolfo-davila-donoso-b713302b8

## Nota
Los datos mostrados corresponden a un monitoreo de condiciones 
ambientales de 6 días con fines de demostración.
