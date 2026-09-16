Análisis y predicción de rotación de personal (Employee Attrition)

Proyecto personal realizado durante el Máster en Inteligencia Artificial y Ciencias del Comportamiento, aplicando técnicas de análisis de datos y machine learning a un problema real de RRHH: entender y predecir por qué se van los empleados.

Objetivo

Identificar los factores que más influyen en la rotación de personal y construir un modelo predictivo que permita anticipar el riesgo de fuga, para orientar acciones de retención.
Dataset

IBM HR Analytics Employee Attrition & Performance — 1.470 empleados, 35 variables (demografía, salario, satisfacción, horas extra, antigüedad, etc.). Datos sintéticos publicados por IBM con fines educativos.
Metodología

Limpieza de datos: eliminación de columnas sin información y comprobación de nulos.
Análisis exploratorio (EDA): identificación de las variables más asociadas a la rotación.
Modelo predictivo: regresión logística, elegida por su interpretabilidad — permite explicar el resultado a perfiles no técnicos de RRHH.
Conclusiones de negocio: traducción de los resultados en recomendaciones accionables.
Hallazgos principales

Las horas extra triplican el riesgo de fuga (30,5% vs 10,4% de rotación). Es el factor individual más determinante.
La rotación se concentra en puestos de entrada, especialmente comerciales (~40% en Sales Representative) frente a puestos directivos (~2,5%).
La antigüedad protege: a más años trabajados y más relación con el manager actual, menor riesgo de abandono — los primeros 1-2 años son el momento crítico de retención.

Resultados del modelo

Métrica	Valor
Accuracy	75%
Recall	62%
Precision	34%
F1-score	44%

El modelo prioriza el recall (detectar el mayor número posible de casos reales de fuga) sobre la precisión, ya que para RRHH el coste de no anticipar una salida real es mayor que el de revisar algún caso de más.
Recomendaciones
Priorizar la reducción de horas extra en roles junior/comerciales, con mejor relación coste-beneficio que subidas salariales generales.
Reforzar el acompañamiento (mentoring, check-ins con el manager) durante los primeros años de un empleado.
Revisar la política de viajes frecuentes en los puestos donde más impacta.
Herramientas
Python · pandas · scikit-learn · matplotlib
Estructura del repositorio
```
├── Analisis_Rotacion_Personal.ipynb   # Notebook completo (limpieza, EDA, modelo, conclusiones)
├── hr.csv                              # Dataset original
└── README.md
```
---
Proyecto con fines de aprendizaje y portfolio.
