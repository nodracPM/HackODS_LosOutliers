### Información complementaria

**Artículo acerca del derrame de petróleo en 2026:**https://www.greenpeace.org/mexico/informacion-prensa/62546/

**Sitios afectados derrame de petróleo en 2026:** https://www.google.com/maps/d/u/0/viewer?mid=1Ku4wk-WcKmPcrna08enfELqsr5pp9LA&ll=22.865042981462132%2C-102.49244999494258&z=5


### Dataset 1: Fugas y derrames de hidrocarburos por organismo subsidiario de PEMEX
* **Fuente:** SEMARNAT / Sistema Nacional de Información Ambiental y de Recursos Naturales (SNIARN) - Compendio 2021.
* **Fecha de consulta/descarga:** 8 de abril de 2026.
* **Licencia:** Datos Abiertos del Gobierno de México.
* **Descripción de variables clave:** * `Año`: Año de reporte del incidente (abarca desde 1999).
  * `Organismo Subsidiario`: Entidad específica de PEMEX responsable del registro (ej. PEMEX Exploración y Producción, PEMEX Transformación Industrial).
  * `Número de derrames`: Cantidad de incidentes (fugas o derrames) reportados en ese periodo.
  * `Cantidad reportada (toneladas)`: Volumen de hidrocarburos derramados al ambiente.
* **Enlace:** [SNIARN - Compendio de Estadísticas Ambientales 2021](https://apps1.semarnat.gob.mx:8443/dgeia/compendio_2021/dgeiawf.semarnat.gob.mx_8080/ibi_apps/WFServlet0282.html)


### Dataset 2: Cuentas Económicas y Ecológicas de México (Costos Totales por Agotamiento y Degradación Ambiental - CTADA)
* **Fuente:** Instituto Nacional de Estadística y Geografía (INEGI) / Sistema de Cuentas Económicas y Ecológicas de México (SCEEM).
* **Fecha de consulta/descarga:** 8 de abril de 2026.
* **Licencia:** Términos de Libre Uso de la Información del INEGI (Datos Abiertos).
* **Descripción de variables clave:** * `Concepto`: Indicador económico o ecológico evaluado (ej. Costos por degradación ambiental, Producción, etc.).
  * `Año`: Periodo de registro de los datos (columnas anualizadas a partir de 2003).
  * `Sector Económico`: Clasificación de la industria analizada (ej. 21 Minería, 11 Agricultura, 31-33 Industrias manufactureras).
  * `Valores Económicos`: Producción en valores básicos y a precios de mercado, representando el costo económico del impacto ambiental.
* **Enlace:** [INEGI - Tabulados SCEEM](https://www.inegi.org.mx/app/tabulados/default.aspx?pr=28&vr=3&in=23&tp=20&wr=1&cno=1&idrt=3271&opc=p)





### Dataset 3 (no estructurado) : Inventario Nacional de Sitios Contaminados y Remediados
* **Fuente:** Secretaría de Medio Ambiente y Recursos Naturales (SEMARNAT) / Portal Geomático.
* **Fecha de consulta/descarga:** 14 de abril de 2026.
* **Licencia:** Datos Abiertos del Gobierno de México (Transparencia proactiva).
* **Descripción de variables clave:** * `Estado del sitio`: Condición administrativa actual del lugar (Contaminado o Remediado).
  * `Cantidad de sitios`: Total de pasivos ambientales reconocidos oficialmente (ej. 1,114 sitios contaminados al corte de 2025).
  * `Área / Volumen`: Métrica diseñada para medir la magnitud física del daño o la limpieza. Destaca por contener masivamente el valor nulo `-999999`, lo que demuestra la falta de especificación y medición real.
* **Enlaces:** * [Página de Transparencia SEMARNAT](https://www.semarnat.gob.mx/gobmx/transparencia/tsitioscontaminados.html)
  * [Portal Geomático - Dashboard Interactivo](https://geoportal.semarnat.gob.mx/arcgisp/apps/webappviewer/index.html?id=6633959897c14220b90f1b92a6e11840)


---

##  Anexo Metodológico: Cálculo de Costos y Déficit Ecológico

Este proyecto integra modelos económicos internacionales y normativa nacional para dimensionar la brecha entre el daño ambiental reportado y la capacidad de respuesta institucional.

### Métrica 1: Escenario de Restauración Integral (Modelo BOSCEM - US EPA)
**Fuente:** *[Modeling Oil Spill Response and Damage Costs, Etkin, 2004](https://archive.epa.gov/emergencies/docs/oil/fss/fss04/web/pdf/etkin2_04.pdf)*

Para cuantificar el impacto económico real de los derrames de **Crudo Maya**, utilizamos el modelo BOSCEM de la EPA. Se seleccionó la clasificación de *Heavy Oils* por la persistencia ambiental del fluido y la complejidad de su remoción mecánica.

La fórmula integral del daño por galón se define como:
$$C_{total} = C_{respuesta} + D_{socioeconómico} + D_{ambiental}$$

* **1. Costo de Respuesta ($C_{resp}$):** $C_{resp} = \$77.00 \, \text{USD} \times 1.0 = \mathbf{\$77.00 \, \text{USD/gal}}$
* **2. Daños Socioeconómicos ($D_{soc}$):** $D_{soc} = \$175.00 \, \text{USD} \times 1.0 = \mathbf{\$175.00 \, \text{USD/gal}}$
* **3. Daños Ambientales ($D_{env}$):** $D_{env} = \$35.00 \, \text{USD} \times [0.5 \times (0.9 + 1.2)] = \mathbf{\$36.75 \, \text{USD/gal}}$

**Costo Total Integral:**
$$C_{total} = \$77.00 + \$175.00 + \$36.75 = \mathbf{\$288.75 \, \text{USD/gal}}$$

Considerando que 1 tonelada métrica de crudo pesado Maya equivale a **294 galones**, el costo real de remediación estimado es:
$$\text{Costo por Tonelada} = \$288.75 \times 294 \approx \mathbf{\$84,892.50 \, \text{USD/Ton}}$$

---

### Métrica 2: Escenario Conservador (Costo Base Histórico)
**Fuente:** *[A Taxonomy of Oil Spill Costs, Cohen, 2010](https://media.rff.org/documents/RFF-BCK-Cohen-DHCosts.pdf)*

Basado en el análisis de reclamaciones globales reales y promedios históricos de indemnización, se establece un costo base de **$16 USD por galón**. Utilizando la conversión de crudo estándar (310 galones por tonelada):
$$\text{Costo Histórico} = \$16 \, \text{USD/gal} \times 310 \approx \mathbf{\$4,960 \, \text{USD/Ton}}$$

> **Nota Crítica:** En las visualizaciones de este Dashboard, para mantener un criterio **ultraconservador**, se utiliza un piso mínimo redondeado de **$5,000 USD/Ton**. Como se observa en la Métrica 1, el costo real validado por modelos de la EPA puede ser hasta **17 veces mayor** al valor presentado en nuestras gráficas.

---

### Métrica 3: Déficit de Inversión y Daño Real (INEGI)
**Fuente:** *Sistema de Cuentas Económicas y Ecológicas de México (INEGI)*

Se contrastan los costos de los derrames con la capacidad de respuesta del Estado Mexicano mediante indicadores macroeconómicos:
* **GPA (Gastos en Protección Ambiental):** Inversión real del sector público en remediación y protección.
* **CTADA (Costos Totales por Agotamiento y Degradación):** Impacto económico reconocido por la pérdida de recursos y calidad ambiental.

El ratio **GPA/CTADA** se emplea como un *Índice de Insuficiencia*, permitiendo visualizar qué porcentaje del daño ecológico anual está siendo efectivamente cubierto por la inversión federal.

---

### Métrica 4: Tope Legal de Sanción (LFRA)
**Fuente:** *Ley Federal de Responsabilidad Ambiental (Art. 19)*

Representa el techo económico máximo de sanción aplicable. La legislación mexicana establece una multa máxima de **600,000 UMAs** para personas morales. Al valor actual, esto representa un tope duro de aproximadamente **$65.1 Millones de MXN**, evidenciando la asimetría entre el costo de remediación internacional y la capacidad punitiva del Estado.

---