## AI Log - Equipo Los Outliers

## Herramientas
- Gemini (Google Colab)

## Filosofía de uso
Decidimos usar IA exclusivamente para tareas mecánicas y de exploración inicial, así como para la generación de la estructura inicial de código y markdown. La narrativa, la selección de variables, la interpretación de los datos y las decisiones editoriales fueron 100% del equipo. Nuestro criterio: si la tarea requiere conocimiento profundo del contexto de los derrames de petróleo en México y sus implicaciones socioambientales, la realizamos nosotros.

## Registro de uso

### 2026-04-13 | Gemini | Exploración de estructura para Dashboard
- **Tarea**: Le pedimos opciones de layout para un dashboard en Colab que presentara un análisis de costos y daños ambientales de derrames de petróleo.
- **Prompt**: "Dame 3 estructuras de layout para un dashboard en Google Colab con 4 secciones: contexto histórico, costos económicos, daño ambiental, y recomendaciones."
- **Resultado**: Propuestas de layouts con secciones claras y sugerencias de tipos de gráficos para cada una.
- **Modificación**: Adaptamos una de las estructuras para nuestro notebook, enfocándonos en una progresión lógica de la información, de la contextualización a las métricas de daño y costo.

### 2026-04-13 | Gemini  | Código para visualizaciones
- **Tarea**: Generar código base para visualizar datos con Plotly, incluyendo gráficas de barras y de pastel.
- **Resultado**: Templates funcionales para gráficos de barras agrupadas y gráficos de pastel con agujero central.
- **Modificación**: Utilizamos y adaptamos estos templates. Toda la personalización visual (paletas de colores, títulos, etiquetas en español, manejo de escalas logarítmicas) fue manual, asegurando que los gráficos comunicaran efectivamente los altos costos de remediación.

### 2026-04-13 | Gemini | Refinamiento de texto explicativo
- **Tarea**: Le pedimos que revisara la redacción de la sección sobre las métricas de costo (BOSCEM - US EPA e ITOPF) para asegurar claridad y concisión.
- **Prompt**: "Revisa este texto que explica dos métricas de costo para derrames de petróleo, BOSCEM de EPA e ITOPF. Asegúrate de que la explicación sea clara, concisa y resalte la diferencia de magnitud entre ambas."
- **Resultado**: Sugerencias para simplificar oraciones, mejorar la fluidez y enfatizar la diferencia de 17x en los costos, lo cual es crucial para nuestra narrativa.
- **Modificación**: Editamos puntos concretos que la IA no abordó de forma correcta para mantener la información veraz, incluyendo la explicación de por qué los costos oficiales subestiman el daño real. El contenido técnico y la interpretación de las implicaciones permanecieron bajo nuestra autoría.

### NO usamos IA para hacer lo siguiente:
- La selección de las bases de datos (SEMARNAT, INEGI) y su procesamiento para alinear los datos.
- La formulación de las métricas de costo y daño, así como su calibración con valores específicos de Crudo Maya.
- La interpretación crítica del "Índice de Insuficiencia" (GPA/CTADA) o el significado del -999999 en los datos de SEMARNAT.
- La narrativa central del proyecto y la conclusión sobre el "verdadero costo" de los derrames de petróleo en México.