# Yo ❤ La Empanada · Decisión del sistema POS

Repositorio de trabajo para decidir **hoy** qué POS usa el negocio (Yo Amo la Empanada al Horno, Cajicá). Preparado por We Rock el 5 de noviembre de 2026.

## Decisión propuesta

> **Empezar con Alegra POS.** Dejar Odoo como fase 2 si el negocio crece o INVIMA exige producción formal. Siigo es el plan B si Alegra falla las pruebas 1 o 3.

**Por qué:** el negocio necesita vender, facturar y controlar el producto terminado de forma fácil. Alegra lo hace por unos $79.900 al mes y, según su propio blog, registra lote y vencimiento en cada entrada de mercancía. Las recetas y los costos ya viven en el Excel maestro (`BASE-MAESTRA-YoAmo.xlsx`), que es más completo que cualquier POS barato. Un sistema de producción completo (Odoo, Teenus) cuesta más tiempo y dinero del que el volumen actual justifica.

**Lo que falta verificar antes de pagar el año** (ver [pruebas](docs/03-pruebas-aceptacion.md)):
1. Registrar un lote de empanadas con fecha de vencimiento y verlo en reportes.
2. Precio mayorista (desde 10 bandejas) y promoción 15+1, aunque sea con un truco manual.
3. Cobro con Nequi, Daviplata y efectivo, con factura electrónica o documento equivalente POS.

## Tabla resumen

| Opción | A favor | En contra | Precio publicado | Administración |
|---|---|---|---|---|
| **Alegra POS** (recomendada) | La más barata; soporte permanente; lote y vencimiento por entrada (según su blog); factura electrónica y API | Sin recetas ni órdenes de producción confirmadas; cada lote se registra como entrada de producto terminado | POS Pyme $79.900/mes; Contabilidad Pyme $163.900/mes (opcional); 25% menos pagando el año | Fácil |
| **Siigo Nube + POS Gastrobar** (plan B) | La más sólida en facturación y soporte local; recetas, combos y costeo (según un tercero) | Sin producción por lote ni vencimiento confirmados; descuenta insumos al vender | Gastrobar PRO $1.049.930/año (≈$87.494/mes); POS Esencial desde $28.750/mes pagando el año | Fácil a media |
| **Odoo** (fase 2) | Producción por lote, trazabilidad, POS y contabilidad en uno; localización DIAN | Pesado de montar; necesita socio de implementación; API externa solo en plan Custom | US$ 8,95 a 11,20 por usuario/mes (Standard); implementación por cotizar | Difícil |
| **Teenus** (solo producción) | Mejor en producción de alimentos, trazabilidad INVIMA, costo real por lote | Sin POS ni facturación (dos sistemas); sin precio público | Por cotizar | Media |
| **Vendty / Fudo / Loggro** | Rápidos, facturan, buenos para mostrador y domicilios | Descuentan insumos al vender; sin subrecetas ni lotes confirmados | $62.900 a $155.000/mes según plan | Fácil |

## Contenido

| Archivo | Qué contiene |
|---|---|
| [docs/01-comparativa.md](docs/01-comparativa.md) | Comparativa completa: 8 opciones y los POS de restaurante, con cobertura por criterio |
| [docs/02-precios.md](docs/02-precios.md) | Precios publicados y costo estimado a 12 meses |
| [docs/03-pruebas-aceptacion.md](docs/03-pruebas-aceptacion.md) | Las 12 pruebas para la demo o el piloto, con las 3 prioritarias y formato de resultado |
| [docs/04-matriz-decision.md](docs/04-matriz-decision.md) | Matriz con pesos (original y propuesta de fase 1), puntajes por llenar |
| [docs/05-registro-de-decisiones.md](docs/05-registro-de-decisiones.md) | Qué se decidió, cuándo y por qué |
| [docs/06-fuentes.md](docs/06-fuentes.md) | Fuentes consultadas |

## Qué se necesita del negocio

1. Un **sí** a Alegra como arranque.
2. Cuántas personas usan la caja y la administración, y si el local atiende en mostrador.
3. Abrir la cuenta de prueba de Alegra (We Rock no puede crear cuentas).
4. El contador confirma si conviene factura electrónica o documento equivalente POS, y si el negocio paga impuesto al consumo.

## Cómo leer los datos

- **Verificado:** lo que el proveedor publica en su sitio oficial.
- **Tercero:** lo que dice un blog o comparativa. Muchos son publicidad de su autor. Se confirma en demo.
- **Por verificar:** no se encontró públicamente. No se llenó con suposiciones.
- Los precios cambian: se confirman con cada proveedor antes de contratar.
