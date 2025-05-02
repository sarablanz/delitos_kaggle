📊 Análisis de Delitos en México



Este proyecto tiene como objetivo explorar y analizar datos sobre delitos cometidos en México, utilizando una base de datos obtenida de Kaggle. El análisis busca identificar patrones, tendencias y factores asociados con la incidencia delictiva, aplicando técnicas de análisis exploratorio, visualización de datos y modelos de aprendizaje automático.

🧑‍💻 Este trabajo forma parte de mi portafolio como egresada del Máster en Ciencia de Datos & AI. Aunque mi formación base es en Criminología, actualmente me estoy enfocando en aplicar herramientas y técnicas propias de la ciencia de datos para el análisis cuantitativo de fenómenos delictivos.

🔬 El objetivo de este proyecto es mantener actualizadas las competencias adquiridas durante el máster, centrándome en la parte técnica y analítica del procesamiento y modelado de datos. Debido a la limitación de fuentes, en esta fase el proyecto no aborda interpretaciones desde la dinámica social o criminológica en profundidad.



🗂️ Descripción del Dataset
Registros: 15,680


Columnas originales: 9


Fuente: Kaggle


Variables 

🆔 Clave_Ent,       int64 :        Clave numérica de la entidad federativa

📅 Año, int64:  Año del registro del delito

📈 Marzo& Abril int64: Número de delitos en marzo

🗺️ Entidad, object: Nombre del estado

🔍 Tipo_delito, object: Clasificación general del delito

🧩 Subtipo_delito, object: Subcategoría específica del delito

🧾 Modalidad, object: Modalidad bajo la cual se cometió el delito

⚖️ Bien_juridico_afectado, object: Bien jurídico afectado



🧹 Limpieza y Preprocesamiento
Estandarización de nombres de columnas (snake_case).


Eliminación de columnas redundantes.


Generación de nuevas columnas como:


total_delitos


promedio_mensual


cambio_porcentual, entre otras.


📚 Agrupación y Clasificación

Agrupación por Tipo de Delito
Los delitos fueron agrupados en categorías como:
Violencia contra personas


Delitos contra sociedad


Delitos financieros


Delitos sexuales


Otros


Se generó un gráfico de barras para visualizar la distribución por categoría, útil para detectar desequilibrios y priorizar análisis.
Agrupación por Modalidad
Delitos con violencia


Delitos sin violencia


Delitos sexuales


Delitos de secuestro


Otros


Agrupación por Subtipo
Más de 50 subtipos fueron reducidos a 10 grandes categorías usando un diccionario de mapeo.

🔍  Análisis Exploratorio (EDA)
Análisis de distribución por tipo de delito


Tendencias anuales de crímenes


Comparación marzo vs abril


Frecuencia por entidad federativa


📈 Visualizaciones utilizadas:
Gráficos de barras


Gráficos de línea


Histogramas



🤖 Modelado Predictivo
Tipo de modelo: Supervisado


Tarea: Clasificación multiclase


Algoritmo utilizado: Random Forest Classifier


Variables utilizadas:
Independientes: Año, Clave_Ent, Entidad, Bien_juridico_afectado, Marzo, Abril


Dependiente: Tipos_delitos



🏁Resultados del Modelo
Precisión general (accuracy): 96.7%


Buen rendimiento en clases mayoritarias como Violencia contra personas


Bajo rendimiento en clases minoritarias como Delitos sexuales (por desbalance)



✅ Conclusiones


Ventajas
Proceso bien estructurado

Alta precisión del modelo

Buen uso de visualizaciones y agrupaciones


⚠️Limitaciones

Dataset limitado a dos meses (marzo y abril)

Desbalance de clases afecta la clasificación de delitos poco frecuentes



💡Recomendaciones

Incluir más meses del año

Generar datos sintéticos 


🧾 Creditos 

Autor del análisis: Saray Blanco Alzola


Herramientas: Python, pandas, scikit-learn, matplotlib, seaborn
