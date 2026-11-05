# 4. Matriz de decisión con pesos

Los pesos son una propuesta de We Rock. Los puntajes (0 a 5) quedan vacíos hasta probar los sistemas. **Puntaje ponderado = suma de (puntaje × peso) ÷ 100.**

## Pesos originales (3 de noviembre): priorizan capacidad de producción

| Criterio | Peso |
|---|---|
| Recetas con subrecetas | 15 |
| Producción por lote con vencimiento | 20 |
| Venta por unidad, bandeja y lasaña | 8 |
| Historial de precios y recálculo de costos | 7 |
| Factura electrónica y documento equivalente POS | 10 |
| Reportes: costo por lote, trazabilidad, mermas, margen | 10 |
| Carga masiva o API | 10 |
| Precios por cantidad, 15+1 y anticipos | 7 |
| Precio total a tres años | 5 |
| Soporte en español e implementación | 4 |
| Facilidad de uso para el equipo | 4 |
| **Total** | **100** |

Con estos pesos gana Odoo, porque premia la producción.

## Pesos propuestos para la fase 1 (5 de noviembre): priorizan facilidad y operación diaria

| Criterio | Peso | Alegra | Siigo | Odoo |
|---|---|---|---|---|
| Facilidad de uso para el equipo | 20 | | | |
| Factura electrónica y documento equivalente POS | 20 | | | |
| Venta por unidad, bandeja y lasaña | 15 | | | |
| Lote y vencimiento del producto terminado | 15 | | | |
| Precio total a tres años (con implementación) | 10 | | | |
| Precios por cantidad, 15+1 y anticipos | 7 | | | |
| Soporte en español e implementación | 8 | | | |
| Carga masiva o API | 5 | | | |
| **Total** | **100** | | | |
| **Puntaje ponderado** | | | | |

**Por qué cambian los pesos:** el negocio pidió que la administración sea fácil, vende unos $6 millones al mes y todavía no tiene permiso INVIMA. Producir con órdenes y trazabilidad completa se vuelve importante en la fase 2, no en el arranque.

## Cuándo pasar a la fase 2 (Odoo)

Se reabre la decisión si se cumple **cualquiera** de estas condiciones:
- El negocio supera los $17 millones al mes de ventas.
- INVIMA exige trazabilidad de lote desde las materias primas.
- Llevar los lotes y las recetas a mano en el Excel ya consume más horas de las que vale ahorrar.
