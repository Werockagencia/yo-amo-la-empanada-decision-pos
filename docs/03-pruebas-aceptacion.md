# 3. Pruebas de aceptación

Cada sistema debe pasarlas **en vivo y con datos reales del negocio**. Si no puede, se califica 0 en ese criterio.

## Las 3 prioritarias para decidir Alegra (fase 1)

| # | Prueba | Resultado | Notas |
|---|---|---|---|
| A | Registrar una entrada de 15 empanadas de champiñón con lote y fecha de vencimiento, y ver el vencimiento en un reporte o alerta | ☐ Pasa ☐ Falla | |
| B | Vender 10 bandejas y ver el precio mayorista aplicado; vender 16 y ver la bandeja gratis de la promoción 15+1 (aunque sea manual) | ☐ Pasa ☐ Falla | |
| C | Emitir una venta con factura electrónica o documento equivalente POS y cobrar por Nequi, Daviplata y efectivo | ☐ Pasa ☐ Falla | |

**Regla:** si falla A o C, se pasa a Siigo como plan B y se repiten estas pruebas allí.

## Las 12 pruebas completas

1. Crear la salsa criolla como subreceta (rinde 3.000 g) y usarla en la lasaña de res (30 g) sin que los ingredientes se descuenten dos veces.
2. Registrar una orden de producción de 15 empanadas de champiñón: descuenta champiñón y queso, suma producto terminado y guarda fecha de producción y de vencimiento.
3. Vender una bandeja x4 y comprobar que baja el producto terminado y no las materias primas.
4. Cambiar el precio del tomate y ver qué recetas se afectan, con el costo del lote anterior intacto.
5. Registrar una merma en un lote y ver el consumo teórico contra el real.
6. Importar las 32 materias primas y las 11 recetas desde un archivo, sin digitarlas una a una.
7. Emitir una venta con factura electrónica y pagos por Nequi, Daviplata y efectivo.
8. Sacar las ventas por producto por exportación o API, para el tablero y la asistente de WhatsApp.
9. Distinguir la empanada horneada de la congelada, con pesos y SKU distintos.
10. Vender 10 bandejas y ver el precio mayorista aplicado solo; vender 16 y ver la bandeja gratis de la promoción 15+1.
11. Registrar un pedido mayorista con anticipo del 50% y cobrar el saldo contra entrega.
12. Sacar el informe de trazabilidad de un lote: qué materias primas lo formaron y a qué clientes se vendió.

Las pruebas 1, 2, 4, 5 y 12 son de producción: **Alegra probablemente no las pase** (no se encontró recetas ni producción en su documentación; se confirma en la prueba gratuita) y se resuelven en el Excel maestro durante la fase 1. Son las que obligan a pasar a Odoo en la fase 2.

## Resultados por sistema

| Prueba | Alegra | Siigo | Odoo |
|---|---|---|---|
| 1 Subreceta | | | |
| 2 Orden de producción con lote | | | |
| 3 Venta baja producto terminado | | | |
| 4 Cambio de precio de insumo | | | |
| 5 Merma | | | |
| 6 Importación masiva | | | |
| 7 Factura y pagos | | | |
| 8 Exportación o API | | | |
| 9 Horneada vs congelada | | | |
| 10 Mayorista y 15+1 | | | |
| 11 Pedido con anticipo | | | |
| 12 Trazabilidad de lote | | | |

## Plan de arranque

| Cuándo | Qué | Quién |
|---|---|---|
| Hoy | Decisión: sí a Alegra; abrir la cuenta de prueba | Negocio |
| Esta semana | Cargar las 32 materias primas y las bandejas, correr las pruebas A, B y C | We Rock |
| Esta semana | Confirmar factura electrónica o documento equivalente POS | Contador |
| Siguiente | Si pasan A, B y C: contratar plan anual y capacitar al equipo | Negocio y We Rock |
| Siguiente | Si falla A o C: probar Siigo con las mismas pruebas | We Rock |
