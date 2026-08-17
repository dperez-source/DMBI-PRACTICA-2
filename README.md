# G1DMBIPRACTICA-2
BRUNO ALEX MENDOZA
ANDRES LEONARDO ROMERO
DANNA PEREZ CORONEL
# Data Warehouse con Northwind
Módulo: MIAV1E605 - Base de Datos  
Tarea: 2.2 Diseño e Implemento un almacén de datos  
Fecha: Agosto 2026

## Descripción del Proyecto
Este repositorio contiene el diseño e implementación de un Data Warehouse (DW) basado en la base de datos transaccional Northwind.  
El objetivo es transformar el modelo OLTP normalizado en un modelo multidimensional (Star Schema) para análisis de Inteligencia de Negocios.

## Modelo Estrella
El DW se compone de una tabla de hechos y varias tablas de dimensiones:

- **Tabla de Hechos**
  - fact_ventas: almacena métricas de negocio (cantidad, monto_total) y referencias a las dimensiones.

- **Tablas de Dimensiones**
  - dim_cliente: información de clientes y segmentos.
  - dim_producto: catálogo de productos, categorías y precios base.
  - dim_empleado: datos de vendedores y cargos.
  - dim_sucursal: ubicación de sucursales.
  - dim_tiempo: jerarquía temporal (año, mes, día).

## Contenido del Repositorio
- `DW_Northwind_structure.sql`: script de creación de la base y tablas del modelo estrella.
- `DW_Northwind_inserts.sql`: script de inserción de datos de prueba en dimensiones y hechos.
- `DW_Northwind_queries.sql`: consultas analíticas de ejemplo (ventas por producto, cliente, empleado, sucursal y tiempo).
- `README.md`: documentación del proyecto.

## Instrucciones de Ejecución
1. Abrir SQL Server Management Studio (SSMS).
2. Ejecutar `DW_Northwind_structure.sql` para crear la base DW_Northwind y sus tablas.
3. Ejecutar `DW_Northwind_inserts.sql` para poblar las dimensiones y la tabla de hechos con datos de prueba.
4. Ejecutar `DW_Northwind_queries.sql` para validar las consultas analíticas.
