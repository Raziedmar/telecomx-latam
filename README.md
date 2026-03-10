# 📊 TelecomX — Análisis de Evasión de Clientes (Churn)

## 📌 Descripción del Proyecto

Este proyecto corresponde al **Challenge de Data Science de Alura LATAM: TelecomX — Análisis de Evasión de Clientes**.

El objetivo del análisis es comprender los **factores que influyen en la cancelación de clientes (Churn)** dentro de la empresa TelecomX. A través de un proceso de **Extracción, Transformación y Análisis de datos**, se busca identificar patrones en el comportamiento de los clientes que permitan proponer estrategias para reducir la evasión.

El análisis se realizó utilizando **Python y herramientas de análisis de datos** dentro de un entorno de **Jupyter Notebook**.

---

# 🎯 Objetivos del proyecto

- Analizar el comportamiento de los clientes de TelecomX.
- Identificar factores asociados con la evasión de clientes.
- Explorar relaciones entre servicios contratados, cargos y permanencia.
- Generar visualizaciones que permitan detectar patrones relevantes.
- Proponer recomendaciones para reducir el churn.

---

# 🧰 Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

# 📂 Dataset

El dataset contiene información sobre los clientes de TelecomX, incluyendo:

| Variable | Descripción |
|--------|-------------|
| customerID | Identificador único del cliente |
| Churn | Indica si el cliente canceló el servicio |
| gender | Género del cliente |
| SeniorCitizen | Indica si el cliente es adulto mayor |
| Partner | Si el cliente tiene pareja |
| Dependents | Si el cliente tiene dependientes |
| tenure | Tiempo de permanencia del cliente en meses |
| InternetService | Tipo de servicio de internet |
| Contract | Tipo de contrato |
| PaymentMethod | Método de pago |
| Charges.Monthly | Cargo mensual |
| Charges.Total | Total pagado por el cliente |

Los datos fueron importados desde un **archivo JSON**, el cual fue normalizado para su análisis en formato tabular.

---

# 🧹 Limpieza y Preparación de Datos

Durante el proceso de preparación de datos se realizaron las siguientes tareas:

- Importación del dataset y normalización del JSON.
- Exploración inicial de la estructura del dataset.
- Identificación de valores nulos utilizando `df.isnull().sum()`.
- Se detectaron **11 valores nulos en `Charges.Total`**, asociados a clientes con `tenure = 0`.
- Estos registros fueron eliminados debido a que no aportan información relevante para el análisis de evasión.
- Conversión de variables al tipo de dato adecuado.
- Creación de nuevas variables derivadas como:
Cuentas_Diarias = Charges.Monthly / 30


También se creó una variable adicional para calcular el **número de servicios contratados por cada cliente**.

---

# 📊 Análisis Exploratorio de Datos (EDA)

Se realizaron diversos análisis exploratorios para comprender los factores asociados al churn.

Entre los principales análisis realizados se encuentran:

- Distribución de clientes que cancelan el servicio.
- Relación entre **cargos diarios y evasión de clientes**.
- Análisis de la **antigüedad del cliente (tenure)**.
- Relación entre **cantidad de servicios contratados y churn**.
- Análisis de **correlación entre variables numéricas**.

Para ello se utilizaron diferentes visualizaciones:

- Histogramas
- Boxplots
- Gráficos de dispersión
- Matrices de correlación

---

# 📈 Principales Hallazgos

El análisis permitió identificar varios patrones importantes:

- Los clientes con **menor antigüedad presentan mayor probabilidad de cancelación**.
- Los clientes con **cargos más altos muestran una ligera tendencia a cancelar el servicio**.
- Los clientes que contratan **más servicios adicionales tienden a permanecer más tiempo en la empresa**.
- La evasión de clientes es un fenómeno influenciado por **múltiples factores combinados**.

---

# 💡 Recomendaciones

A partir de los resultados obtenidos se sugieren las siguientes estrategias:

### 1️⃣ Programas de retención temprana
Los clientes con menor antigüedad presentan mayor riesgo de churn, por lo que es recomendable implementar programas de fidelización durante los primeros meses.

### 2️⃣ Estrategias de precios
Evaluar promociones o planes flexibles para clientes con cargos elevados.

### 3️⃣ Promoción de paquetes de servicios
Incentivar la contratación de múltiples servicios puede aumentar la permanencia del cliente.

### 4️⃣ Mejora en la experiencia del cliente
Fortalecer la atención al cliente y el soporte técnico para reducir la probabilidad de cancelación.

---

# 📌 Conclusión

El análisis exploratorio permitió identificar patrones relevantes en el comportamiento de los clientes de TelecomX. Comprender estos factores permite desarrollar estrategias orientadas a **reducir la evasión de clientes y mejorar la retención**, contribuyendo así a la sostenibilidad del negocio.

---

# 👨‍💻 Autor

Proyecto desarrollado como parte del **Challenge de Data Science — TelecomX (Análisis de Evasión de Clientes)**.
