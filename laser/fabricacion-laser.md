# Fabricación láser de mi caja de MDF

## 1. ¿Qué hice?

Hice una caja de MDF **sin tapa y sin pegamento**, formada por cinco piezas que se unen con pestañas (*finger joints*). Diseñé las piezas en Fusion 360, preparé el archivo DXF y realicé el corte láser en el FabLab de la IBERO Puebla.

La primera caja la hicimos con Sofía, pero **las piezas no encajaron como necesitábamos**. Después hice un segundo intento por mi cuenta, corregí el diseño y esta vez **las piezas embonaron bien y se mantienen unidas sin salirse**.

## 2. Material y medidas

| Dato | Medida |
|---|---|
| Material | MDF |
| Espesor real (medido con vernier) | **2.90 mm** |
| Caja armada | **80 × 50 × 60 mm** (ancho × fondo × alto) |
| Piezas | 5: frente, fondo, 2 laterales y base |
| Tipo de unión | Pestañas, sin pegamento |
| Kerf medido | **0.112 mm** |
| Compensación en el DXF | **0.056 mm por lado** |


## 3. Máquina y parámetros de corte

Usé la **CAMFive CFL-CMA1390T**, una cortadora láser de CO₂ del FabLab de la IBERO Puebla. El archivo se preparó como **corte vectorial**, a escala **1:1 en milímetros**.

| Parámetro | Valor de referencia |
|---|---|
| Potencia máxima | **50 %** |
| Potencia mínima | **45 %** |
| Velocidad | **15 mm/s** |
| Pasadas | **1** |
| Tipo de trabajo | Corte vectorial |
| Compensación adicional en el programa | **Ninguna**; el DXF ya estaba compensado |

Estos ajustes son una referencia documentada para cortar MDF de 3 mm en el FabLab.

## 4. Problemas y ajustes

**Primer intento (con Sofía).** Cortamos una primera versión de la caja, pero el ensamble no salió como esperábamos. Las uniones no quedaron suficientemente bien ajustadas para armar una caja firme y había uniones fantasma. Esto nos hizo ver que no bastaba con dibujar las cinco caras: también importaban las medidas de las pestañas y el espacio que se pierde con el láser.

**Qué cambié.** Para el siguiente intento revisé el espesor del MDF con vernier y confirmé que era de **2.90 mm**, no de 3.00 mm como había supuesto al principio. También retomé el **kerf de 0.112 mm**, ajusté el archivo DXF y comprobé las medidas de las piezas en Fusion 360 antes de mandarlas a cortar.

**Segundo intento (individual).** Volví a cortar las cinco piezas con el diseño corregido. Al armarlas, las pestañas **sí encajaron**, la estructura se mantuvo firme y las piezas **no se salieron de sus uniones**. Ya no fue necesario usar pegamento para mantener la caja armada.

## 5. Resultado.

El segundo corte **sí funcionó**: logré armar una caja abierta, estable y sin pegamento. La principal diferencia respecto al primer intento fue revisar las dimensiones reales del material y corregir las uniones considerando el kerf.

