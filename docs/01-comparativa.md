# 1. Comparativa completa

Consultada entre el 3 y el 5 de noviembre de 2026. Ver [fuentes](06-fuentes.md).

## Qué tiene que resolver el POS en este negocio

- **Catálogo:** 29 productos vendibles (9 empanadas sueltas, 9 en bandeja x4 horneada y congelada, 9 en bandeja x5 precocida, 2 lasañas). Cada bandeja lleva un solo sabor.
- **Producción:** rellenos y salsas por lote (subrecetas que se usan en varios productos).
- **Ventas:** precio normal y mayorista (desde 10 bandejas o lasañas, 40 empanadas sueltas), promoción 15+1, anticipo del 50% en mayoristas, pedidos con fecha de entrega, domicilio y recogida.
- **Canales:** pedidos que llegan por WhatsApp y por la web.
- **Obligaciones:** factura electrónica o documento equivalente POS (Resolución DIAN 165 de 2023), trazabilidad para INVIMA cuando se formalice.

## Las 8 opciones

| # | Opción | Por qué en este lugar | Falta confirmar / en contra | Costo publicado |
|---|---|---|---|---|
| 1 | **Alegra POS** | La más barata para vender y facturar, con precios claros y soporte permanente. Su blog de Colombia dice que registra lote y vencimiento en cada entrada, alerta de productos por vencer y usa PEPS. | No confirma recetas ni órdenes de producción. Un comentario de su equipo dice que no tiene módulo de producción (fecha poco clara). El lote sale de su blog. | POS Pyme $79.900/mes. Contabilidad Pyme $163.900/mes. 25% menos pagando el año. |
| 2 | **Siigo Nube + POS Gastrobar** | Lo más seguro en facturación, contabilidad y soporte local. Descuenta ingredientes de recetas y combos. Cumple la Resolución 165. | Sin subrecetas, lotes con vencimiento ni producción confirmados en Nube. Pensado para restaurante. API sin documentar. | Gastrobar PRO $1.049.930/año (≈$87.494/mes), lista $1.499.900. POS Esencial desde $28.750/mes pagando el año. Nube aparte. |
| 3 | **Odoo** (Manufactura + Inventario + POS + Contabilidad) | Único que junta producción por lote, trazabilidad, inventario, POS y contabilidad. Localización de Colombia y API para cargar recetas. | Subrecetas (listas de materiales de varios niveles) y FEFO solo según terceros. DIAN por la ruta de DIAN o la de Carvajal: confirmar. Necesita socio de implementación. API solo en Custom. | US$ 8,95 a 11,20 por usuario/mes (Standard); US$ 16,40 a 20,40 (Custom). Implementación por cotizar. |
| 4 | **Teenus TezlikSoftware** | El mejor en producción de alimentos: fichas técnicas, lote por materia prima, FEFO, informe INVIMA, costo real por lote, HACCP. Colombiano; 4 a 8 semanas. | Sin POS ni factura electrónica: dos sistemas, o integración. No dice si maneja subrecetas. | No publicado. |
| 5 | **Loggro** (Restobar y Pymes) | POS, inventarios, apps de domicilio y factura electrónica. Blogs dicen que Restobar maneja recetas con food cost. | Recetas no se ven en su sitio; la producción solo está en su ERP grande. | No publicado. Blogs: $98.990 a $108.990/mes. |
| 6 | **FoodFactory ERP** | Lotes, producción, recetas y caducidades para fábricas pequeñas. | No cubre Colombia ni DIAN; sin POS. Solo referencia. | € 29,90/mes más IVA. |
| 7 | **POS de restaurante** (Vendty, Fudo, WARO, Cuenti, otros) | Baratos, rápidos y facturan. Buenos para mostrador y domicilio. | Descuentan insumos al vender. Ninguno confirma subrecetas, producción ni lotes. | $25.900 a $155.000/mes según plan y fuente. |
| 8 | **Poster y World Office** | Sin información pública suficiente. Un tercero dice que World Office es fuerte en inventario y producción. | Solo si fallan las demás. | No publicado. |

## POS de restaurante en detalle

Fuentes: sitio de Vendty y tres comparativas de blogs que son publicidad de su autor (Fudo, Loggro, WARO). Precios orientativos.

| Sistema | Recetas y costo | Subrecetas, producción, lotes | Factura DIAN | Precio de referencia |
|---|---|---|---|---|
| Vendty | Nombra "Recetas" sin describirlas | No aparece | Ilimitada | $85.000 a $155.000/mes |
| Fudo | Recetas y food cost solo en plan Avanzado | No aparece | Módulo aparte, desde $9.000/mes | Base $62.900; Avanzado $118.900 |
| Loggro Restobar | Recetas con food cost | No aparece | Incluida | $98.990 a $108.990 |
| WARO | Food cost con IA | No aparece | Desde $200 por factura | Desde $30.000 |
| Cuenti | Costo por receta | No aparece | Incluida | $33.300 con pago anual |
| Siigo Gastrobar / Alegra POS | Siigo: recetas básicas y combos. Alegra: sin recetas nativas | No aparece | Incluida | Siigo $87.494; Alegra desde $25.900 |

**Por qué no alcanzan solos:** un restaurante cocina cuando le piden y el POS descuenta ingredientes al vender. Yo Amo la Empanada fabrica por lotes, congela y vende producto terminado desde un inventario: los insumos se consumen el día de la producción. Que la documentación pública no lo muestre no prueba que no exista; se puede preguntar en una demo gratuita.

## Cobertura por criterio

Sí = el proveedor lo afirma · Parcial = incompleto o solo tercero · No = no lo tiene · ? = por verificar.

| Criterio | Alegra | Siigo | Odoo | Loggro | Teenus |
|---|---|---|---|---|---|
| Recetas con subrecetas | No | Parcial | Parcial | Parcial | Parcial |
| Producción por lote con órdenes | No | ? | Sí | No | Sí |
| Vencimiento y FEFO/PEPS | Parcial (blog propio: lote y vencimiento por entrada, PEPS) | ? | Parcial | ? | Sí |
| Trazabilidad INVIMA | ? | ? | Parcial | ? | Sí |
| Costo real por lote | Parcial | Parcial | Parcial | ? | Sí |
| POS mostrador, bandejas, lasañas | Sí | Sí | Sí | Sí | No |
| Factura electrónica DIAN | Sí | Sí | Parcial | Parcial | No |
| Carga masiva o API | Parcial | ? | Parcial | Parcial | ? |
| Precios por cantidad, 15+1, anticipos | ? | ? | ? | ? | Parcial |
| Precio publicado | Sí | Sí | Parcial | No | No |
| Soporte | Sí | Sí | Parcial | ? | Sí |

## Tres cosas que cambian la decisión

1. Alegra, la más barata, no tiene producción, pero sí lote y vencimiento por entrada: alcanza para la fase 1 si cada lote se registra como entrada de producto terminado.
2. Siigo es la mejor en facturar, pero hoy no confirma lotes ni producción.
3. La DIAN permite factura electrónica o documento equivalente POS (Resolución 165 de 2023). Cuál conviene lo confirma el contador antes de configurar nada.
