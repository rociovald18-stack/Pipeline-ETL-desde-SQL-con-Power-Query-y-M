# Pipeline ETL – Power BI | TechStore

## Información del estudiante

- **Nombre:** Rocío Valdez
- **Materia:** Data Analytics
- **Módulo:** M7 – Pipeline ETL desde SQL con Power Query y M
- **Actividad:** Checkpoint – Pipeline ETL Completo

---

# Objetivo

Desarrollar un proceso ETL (Extract, Transform & Load) en Power BI utilizando Power Query y lenguaje M para limpiar, transformar y preparar los datos del sistema de ventas de TechStore, dejando un modelo listo para la etapa de modelado y análisis.

---

# Fuente de datos

El proyecto utiliza el dataset proporcionado por el curso, compuesto por las siguientes tablas:

- Dim_Clientes
- Dim_Productos
- Dim_Categorias
- Fact_Ventas

---

# Transformaciones realizadas

## Dim_Clientes

- Eliminación de registros duplicados utilizando **id_cliente** como clave primaria.
- Tratamiento de valores nulos en:
  - email
  - ciudad
- Corrección de tipos de datos.
- Renombrado de columnas utilizando nomenclatura *snake_case*.

---

## Dim_Productos

- Eliminación de registros duplicados mediante **id_producto**.
- Resolución de valores nulos en:
  - precio
  - categoría
- Corrección de tipos de datos.
- Renombrado de columnas.

---

## Fact_Ventas

- Verificación de tipos de datos.
- Conversión de fechas al formato Date.
- Incorporación mediante **Merge** de:
  - nombre_producto
  - categoría

---

## Dim_Categorias

- Verificación de tipos de datos.
- Renombrado de columnas.

---

# Calidad de datos

Se utilizaron las herramientas de perfilado de Power Query:

- Calidad de columnas
- Distribución de columnas
- Perfil de columnas

Estas herramientas permitieron identificar:

- Registros duplicados.
- Valores nulos.
- Tipos de datos incorrectos.

---

# Documentación en lenguaje M

Se documentaron las transformaciones principales mediante comentarios en el Editor Avanzado, justificando las decisiones técnicas adoptadas durante el proceso ETL.

---

# Tecnologías utilizadas

- Microsoft Power BI Desktop
- Power Query
- Lenguaje M

---

# Resultado

Se obtuvo un modelo limpio y preparado para continuar con el desarrollo del modelo analítico en los siguientes módulos del curso, garantizando la calidad e integridad de los datos.

---

# Archivo entregado

- `Pipeline_ETL_Valdez_Rocio.pbix`
