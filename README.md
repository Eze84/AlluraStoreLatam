# 📊 Challenge Data Science — Análisis de Tiendas

Proyecto de análisis de datos desarrollado como parte del **Challenge 1 de Data Science** de Alura Latam. El objetivo es ayudar al Sr. Juan a decidir cuál de sus 4 tiendas debería vender, basándose en métricas de rendimiento extraídas de los datos de facturación.

---

## 🗂️ Estructura del proyecto

```
challenge1-data-science/
│
├── AluraStoreLatam.ipynb       # Notebook principal con todo el análisis
├── README.md                   # Este archivo
```

---

## 🎯 Objetivo

Analizar el desempeño de 4 tiendas a partir de sus datos de ventas e identificar cuál presenta el menor rendimiento para recomendar su venta.

---

## 📋 Análisis realizados

| #  | Análisis                                 | Descripción                                              |
|----|------------------------------------------|----------------------------------------------------------|
| 1  | **Ingresos totales**                     | Suma de la columna `Precio` por tienda                  |
| 2  | **Ventas por categoría**                 | Agrupación por `Categoría del Producto` con conteo       |
| 3  | **Calificación promedio**                | Promedio de la columna `Calificación` por tienda         |
| 4  | **Productos más y menos vendidos**       | `value_counts()` sobre la columna `Producto`             |
| 5  | **Costo de envío promedio**              | Promedio de `Costo de envío` pagado por el cliente       |

---

## 📈 Visualizaciones generadas

- **Barras** — Ingreso total por tienda
- **Línea con puntos** — Calificación promedio por tienda (con línea de promedio global)
- **Barras agrupadas** — Ventas por categoría comparando las 4 tiendas
- **Dispersión** — Relación entre ingreso total y costo de envío promedio
- **Barras horizontales** — Productos más y menos vendidos por tienda

---

## 🔍 Resultados principales

| Indicador                  | Tienda 1     | Tienda 2     | Tienda 3     | Tienda 4     |
|----------------------------|--------------|--------------|--------------|--------------|
| Ingreso total              | $1.150M 🥇   | $1.116M      | $1.098M      | $1.038M 🔴   |
| Calificación promedio      | 3.98 🔴      | 4.04         | 4.05 🥇      | 4.00         |
| Costo de envío promedio    | $26.019 🔴   | $25.216      | $24.806      | $23.459 🥇   |

---

## ✅ Conclusión

Se recomienda que el **Sr. Juan venda la Tienda 4**, ya que presenta:

- Los **menores ingresos totales** del grupo (~$1.038M)
- Una **calificación de cliente intermedia** (4.00, tercera entre las cuatro)
- Un **mix de productos con segmentos débiles** (única tienda con Instrumentos musicales como categoría menos vendida)

Su único punto positivo —el costo de envío más bajo— no se traduce en mejores resultados comerciales.

---

## 🛠️ Tecnologías utilizadas

- Python 3
- Pandas
- Matplotlib
- Google Colab

---

## 📦 Datos

Los datos provienen del repositorio oficial del challenge:

```
https://github.com/alura-es-cursos/challenge1-data-science-latam
```
