[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/zsPfuN_m)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=23949999&assignment_repo_type=AssignmentRepo)
🧩 Tarea 4 – Funciones y Análisis Ambiental con Pandas  
🌿 Universidad de Cundinamarca  

---

### 🎯 Objetivo general
Desarrollar funciones en Python aplicadas al análisis de información ambiental mediante la biblioteca **pandas**, fortaleciendo la capacidad para automatizar procesos de cálculo, clasificación y síntesis de datos experimentales.

---

## 👥 Roles y Retos

### 🧩 Reto 1 – Analista de temperatura y humedad
**Objetivo:** Identificar patrones térmicos y de humedad que afectan la biomasa.

**Tareas:**
- Crear una función `resumen_termico(df)` que retorne un DataFrame con promedio, máximo y mínimo de temperatura y humedad.  
- Diseñar una función `clasificar_clima(temp, hum)` que devuelva una categoría ('húmedo templado', 'seco templado', 'húmedo frío', 'seco frío').  
- Aplicar la función a todo el DataFrame con `apply`.  
- Generar una tabla resumen del número de sitios por categoría.  

**Producto esperado:** un DataFrame limpio con una nueva columna `"clima"` y una tabla de frecuencias por tipo de clima.

---

### 🌞 Reto 2 – Analista de luz
**Objetivo:** Evaluar la relación entre la cantidad de luz y la productividad (biomasa).

**Tareas:**
- Crear una función `indice_luz(df)` que calcule la razón entre la luz de cada sitio y la máxima luz del conjunto.  
- Incorporar ese índice como nueva columna en el DataFrame.  
- Crear una función `clasificar_luz(valor)` que clasifique los sitios en "baja", "media" o "alta" luz según percentiles.  
- Generar un gráfico de barras que muestre la biomasa promedio por categoría de luz.  

**Producto esperado:** gráfico `biomasa vs categoría_luz` y DataFrame con columna `"indice_luz"`.

---

### 🌿 Reto 3 – Analista de biomasa
**Objetivo:** Clasificar los ecosistemas según su productividad y asociar variables ambientales.

**Tareas:**
- Crear una función `clasificar_biomasa(b)` que devuelva: `'alta'` si > 250, `'media'` si 150–250, `'baja'` si < 150.  
- Aplicar esa función al DataFrame para crear la columna `"nivel_biomasa"`.  
- Calcular promedios de temperatura, humedad y luz por cada nivel de biomasa usando `groupby`.  
- Crear una visualización tipo boxplot o barras comparando variables por nivel de biomasa.  

**Producto esperado:** tabla de promedios agrupados + gráfico de comparación.

---

### 🌱 Reto 4 – Integrador del grupo
**Objetivo:** Combinar los resultados de los tres compañeros y crear un resumen final.

**Tareas:**
- Crear una función `integrar_datos(df1, df2, df3)` que una las tres versiones del DataFrame (de los compañeros) en uno solo.  
- Generar una función `reporte_final(df)` que calcule promedios generales, el sitio con mayor y menor biomasa, y la variable más correlacionada con la biomasa (`df.corr()`).  
- Crear un gráfico de dispersión (biomasa vs variable más correlacionada).  
- Redactar una breve conclusión sobre los resultados del grupo.  

**Producto esperado:** notebook con tabla resumen, gráfico de dispersión y conclusiones.

---

### ⚙️ Pasos para completar la tarea
1️⃣ Cada integrante debe desarrollar el notebook que le corresponde dentro de la carpeta `/notebooks`.  
2️⃣ Todos los notebooks deben trabajar sobre el archivo `data/resultados_experimentos.csv`.  
3️⃣ En cada notebook deben incluirse explicaciones en Markdown, comentarios en el código y resultados limpios.  

---

### 📊 Evaluación

| Criterio | Descripción | Ponderación |
|-----------|--------------|--------------|
| Definición y uso de funciones | Creación y aplicación de funciones personalizadas | 20% |
| Manipulación de datos | Uso de pandas para cálculos, filtros y resúmenes | 20% |
| Análisis por variable | Desarrollo de funciones específicas según el rol | 20% |
| Integración final | Coherencia del reporte y combinación de resultados | 25% |
| Documentación y presentación | Claridad del código, comentarios y celdas Markdown | 15% |

---

### 📁 Estructura del repositorio
```
📁 6_funciones_pandas
 ┣ 📁 data
 ┃ ┗ 📄 resultados_experimentos.csv
 ┣ 📁 notebooks
 ┃ ┣ 📓 ejemplo_funciones.ipynb
 ┃ ┣ 📓 reto1_termohumedad.ipynb
 ┃ ┣ 📓 reto2_luz.ipynb
 ┃ ┣ 📓 reto3_biomasa.ipynb
 ┃ ┗ 📓 reto4_integrador.ipynb
 ┗ 📄 README.md
```

🌱 **Universidad de Cundinamarca – Ingeniería Ambiental**  
*Aprender haciendo, programando y analizando el entorno local.*
