# Reto 03: Analizador de Ventas
Proyecto analizador y consolidado de transacciones para la materia de PCD

## Descripción
En esta practica de la semana 3 hicimos un caso de la vida real en python en el cual implementamos lo visto en la semana 3, como diccionarios, agrupar, calcular metricas, etc.

## Ejemplo: Entrada (CSV)
fecha,producto,cantidad,precio_unitario
2026-01-01,Laptop,2,15000.00
2026-01-02,Mouse,10,250.00
2026-01-03,Laptop,1,14500.00
2026-01-04,Teclado,5,800.00
2026-01-05,Mouse,8,250.00

## Ejemplo: Salida Esperada
producto,unidades_vendidas,ingreso_total,precio_promedio
Laptop,3,44500.00,14833.33
Mouse,18,4500.00,250.00
Teclado,5,4000.00,800.00

## Reglas de Procesamiento
* **Agrupación**: Consolida múltiples registros bajo el mismo nombre de producto.
* **Ordenamiento**: El reporte se genera en orden descendente por `ingreso_total`.
* **Robustez**: Ignora líneas con errores de formato o valores no numéricos (Regla 5).
* **Precisión**: Valores monetarios formateados a 2 decimales.

## Cómo ejecutar
`Get-Content tests/entrada1.txt | python main.py`

## Autor:
Huitrón Carranco José Román