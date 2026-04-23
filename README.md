# Análisis del Desempeño Financiero de Adventure Works

## 📊 Descripción del Proyecto

Este proyecto analiza el desempeño financiero de la empresa ficticia Adventure Works, utilizando datos de órdenes, productos, territorios y campañas de marketing. El objetivo es identificar qué mercados generan mayores ingresos y rentabilidad, con el fin de optimizar la asignación de recursos y la inversión en marketing.

## 🎯 Problema de Negocio

La empresa busca determinar en qué mercados y segmentos enfocar sus esfuerzos de marketing para maximizar el retorno de inversión (ROI) y mejorar la rentabilidad general del negocio.

## 🎯 Objetivo

Realizar un análisis de datos que permita:

* Identificar los mercados más rentables
* Detectar oportunidades de optimización del presupuesto de marketing
* Priorizar territorios y productos estratégicos

## 📁 Dataset

El análisis se basa en múltiples fuentes de datos relacionales que contienen información de ventas, productos, territorios y marketing.

### 🔹 Datos de Ventas

* **Fuente:** `ventas_2017`
* **Cobertura:** Transacciones de líneas de pedido del año 2017. Cada registro corresponde a un producto dentro de un pedido.
* **Variables clave:**

  * `numero_pedido`: Identificador único del pedido
  * `fecha_pedido`: Fecha en que se realizó el pedido
  * `clave_producto`: Identificador del producto
  * `clave_territorio`: Identificador del territorio
  * `cantidad_pedido`: Cantidad de productos solicitados

---

### 🔹 Datos de Productos

* **Fuente:** `productos`
* **Cobertura:** Información detallada de productos, incluyendo características y precios.
* **Variables clave:**

  * `clave_producto`: Identificador del producto
  * `clave_subcategoria`: Identificador de la subcategoría
  * `nombre_producto`: Nombre del producto
  * `costo_producto`: Costo del producto
  * `precio_producto`: Precio de venta

---

### 🔹 Clasificación de Productos

* **Fuente:** `productos_categoricos`
* **Cobertura:** Jerarquía de categorías y subcategorías para enriquecer el análisis de productos.
* **Variables clave:**

  * `clave_subcategoria`: Identificador de subcategoría
  * `subcategoria_descripcion`: Nombre de la subcategoría
  * `clave_categoria`: Identificador de categoría
  * `categoria_descripcion`: Nombre de la categoría

---

### 🔹 Datos de Territorios

* **Fuente:** `territorios`
* **Cobertura:** Relación entre territorios, países y continentes.
* **Variables clave:**

  * `clave_territorio`: Identificador del territorio
  * `pais`: País

---

### 🔹 Datos de Marketing

* **Fuente:** `campanas`
* **Cobertura:** Información de inversión en campañas de marketing por territorio.
* **Variables clave:**

  * `clave_territorio`: Identificador del territorio
  * `costo_campana`: Costo de la campaña

---

## 🔗 Integración y Preparación de Datos

### 🧩 Proceso de Integración

* Se integraron múltiples tablas mediante consultas SQL (JOINs entre ventas, productos, categorías y territorios).
* Se utilizaron claves como `clave_producto`, `clave_subcategoria` y `clave_territorio` para relacionar la información.
* Se consolidó una tabla final para análisis que combina información de ventas, producto y ubicación geográfica.

### 🧹 Preparación de Datos

* Se validaron valores nulos y consistencia de datos
* Se calcularon métricas clave como ingresos (`precio * cantidad`) y rentabilidad (`precio - costo`)
* Se estandarizaron nombres de columnas para facilitar el análisis

## 🛠️ Herramientas y Tecnologías

* SQL (extracción, transformación y análisis de datos)
* Google Sheets (visualización y análisis complementario)

## 🔍 Proceso de Análisis

1. Extracción de datos mediante consultas SQL
2. Integración de tablas relacionales
3. Cálculo de métricas clave (ingresos, rentabilidad, desempeño por territorio)
4. Análisis comparativo entre mercados y productos
5. Generación de insights de negocio

## 📈 Principales Hallazgos

* Existen mercados que concentran la mayor parte de los ingresos y la rentabilidad
* Algunos territorios presentan alto volumen de ventas pero baja rentabilidad
* La inversión en marketing no siempre se traduce en mayor retorno

## ✅ Conclusiones

El análisis permite identificar qué mercados y productos son más estratégicos para la empresa. Una mejor asignación del presupuesto de marketing puede incrementar significativamente la rentabilidad.

## 📸 Visualizaciones

<img width="670" height="127" alt="image" src="https://github.com/user-attachments/assets/86a98264-9d52-44f8-992e-8add69a93773" />


