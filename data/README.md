# 🗂 Datos – Caso de Estudio Abandono Laboral (UdeA)

Esta carpeta contiene los archivos originales utilizados para el análisis del proyecto académico sobre abandono laboral en empleados.  
Los datos provienen del estudio suministrado como material de trabajo para el curso de Analítica y aprendizaje supervisado – Universidad de Antioquia.

## 📁 Archivos incluidos
| Archivo | Descripción |
|--------|-------------|
| `employee_survey_data.csv` | Encuesta aplicada a empleados – mide satisfacción, conciliación vida laboral, etc. |
| `manager_survey_data.csv` | Encuesta aplicada a jefes / responsables directos – incluye evaluación del rendimiento. |
| `general_data.csv` | Información general de los empleados: edad, salario, cargo, años en la empresa, etc. |
| `time_work.csv` | Métricas de tiempo y uso de jornada laboral durante el último año. |
| `diccionario_datos.xlsx` | Diccionario que describe cada columna, su significado y niveles categóricos. (Usado como referencia para este documento) |

---

## 🧾 Diccionario de Variables

A continuación se describen las columnas más relevantes encontradas en los archivos:

| Columna | Descripción | Valores / Nivel (si aplica) |
|--------|-------------|------------------------------|
| **Age** | Edad del empleado | Numérico |
| **Attrition** | Si el empleado abandonó su empleo el año anterior | Sí / No |
| **BusinessTravel** | Frecuencia de viajes por motivos laborales | Bajo, Medio, Frecuente |
| **Department** | Departamento en la empresa | Sales, HR, R&D, etc. |
| **DistanceFromHome** | Distancia del hogar al trabajo (kms) | Numérico |
| **Education** | Nivel de estudios | 1 Por debajo de universidad / 2 Universitario / 3 Licenciado / 4 Máster / 5 Doctor |
| **EducationField** | Área de formación académica | Administrativo, Técnico, Marketing, etc. |
| **EmployeeCount** | Número de empleados registrados | (Valor constante) |
| **EmployeeNumber** | Identificador único del empleado | Numérico |
| **EnvironmentSatisfaction** | Satisfacción con entorno de trabajo | 1 Bajo / 2 Medio / 3 Alto / 4 Muy alto |
| **Gender** | Sexo del empleado | Masculino / Femenino |
| **JobInvolvement** | Nivel de implicación en el trabajo | 1 Bajo / 2 Medio / 3 Alto / 4 Muy alto |
| **JobLevel** | Nivel del puesto (jerarquía) | 1 a 5 |
| **JobRole** | Cargo dentro de la empresa | Ej: Laboratory Tech, Sales Executive |
| **JobSatisfaction** | Satisfacción laboral | 1 Bajo / 2 Medio / 3 Alto / 4 Muy alto |
| **MaritalStatus** | Estado civil | Soltero, Casado, Divorciado |
| **mean_work** | Tiempo promedio de trabajo diario en el último año | Numérico (horas) |
| **MonthlyIncome** | Ingreso mensual en USD | Numérico |
| **NumCompaniesWorked** | Número de empresas previas donde trabajó | Numérico |
| **Over18** | Si el empleado es mayor de edad | Y / N |
| **PercentSalaryHike** | % aumento salarial último año | Numérico (%) |
| **PerformanceRating** | Evaluación del rendimiento | 1 Bajo / 2 Bueno / 3 Excelente / 4 Sobresaliente |
| **RelationshipSatisfaction** | Satisfacción con relaciones laborales | 1 Bajo / 2 Medio / 3 Alto / 4 Muy alto |
| **StandardHours** | Horas estándar de trabajo | Valor fijo 40 hrs |
| **StockOptionLevel** | Opciones sobre acciones | 0 a 3 |
| **TotalWorkingYears** | Total años trabajados en la vida laboral | Numérico |
| **TrainingTimesLastYear** | Número de capacitaciones recibidas en el último año | Numérico |
| **WorkLifeBalance** | Conciliación vida laboral–personal | 1 Mala / 2 Buena / 3 Muy buena / 4 La mejor |
| **YearsAtCompany** | Años en la empresa | Numérico |
| **YearsSinceLastPromotion** | Años desde el último ascenso | Numérico |
| **YearsWithCurrManager** | Años bajo la supervisión del jefe actual | Numérico |

---

## 📝 Notas importantes
- Los datos son **originales y no deben ser modificados** en esta carpeta.
- Para el procesamiento, se recomienda copiar o exportar a la carpeta `/datos/procesados` o directamente dentro de los notebooks.
- Algunas columnas como `EmployeeCount` y `StandardHours` contienen valores constantes y pueden ser excluidas del modelado.

---

## 🧭 Recomendación de uso dentro del proyecto
Para una correcta carga de datos en los notebooks:

```python
import pandas as pd
df = pd.read_csv("datos/orig_
