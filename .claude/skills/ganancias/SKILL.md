---
name: ganancias
description: >
  Playbook completo para la presentación anual de Impuesto a las Ganancias de Guillermo Bruchmann.
  Invocar cuando el usuario quiera trabajar en la presentación de ganancias, recopilar información
  para el estudio contable, o consultar el proceso. Contiene fases, checklists, formatos requeridos
  y lecciones aprendidas.
disable-model-invocation: false
---

# Playbook — Presentación Anual de Ganancias

Este es el playbook acumulado para la presentación de Impuesto a las Ganancias de Guillermo Bruchmann. Se actualiza año a año con lo aprendido en cada presentación.

## Fases del proceso

### Fase 1: Recepción del pedido del estudio

La contadora (Josela) envía un email con un PDF adjunto que detalla la información a recopilar. Esto ocurre generalmente en **enero** del año siguiente al período fiscal.

**Pasos:**
1. Descargar el email y el PDF del pedido
2. Guardarlos en `/FY{año}/`
3. **Validar los puntos del pedido** contra el año anterior:
   - Leer el PDF nuevo y extraer los puntos solicitados
   - Comparar contra los puntos del año anterior (ver sección "Puntos del pedido" abajo)
   - Si hay puntos nuevos, eliminados o modificados → alertar al usuario
   - Actualizar la estructura de `/requirements/` si es necesario
4. Confirmar recepción del email a la contadora
5. Anotar la fecha límite de envío (suele ser ~1 mes después del pedido)

### Fase 2: Recopilación de información (punto por punto)

Se trabaja cada punto del pedido de forma individual. Para cada punto:

1. **Consultar el checklist** de este punto (ver sección "Checklist por punto" abajo)
2. **Revisar qué se envió en años anteriores** para ese punto:
   - Leer los emails transcriptos en `/FY{año-anterior}/cadena-emails-*.md`
   - Extraer lo que se dijo/envió sobre ese punto específico
   - Usar como referencia de formato y nivel de detalle esperado
3. **Recopilar documentos y datos** del año actual:
   - Pedir al usuario los docs que faltan
   - Guardar docs en `/requirements/{punto}/docs-FY{año}/`
4. **Agregar al draft de email** (`/FY{año}/draft-email-info-ganancias.md`):
   - Ir construyendo el email acumulativo punto por punto
   - Usar el mismo formato/estilo que en años anteriores
   - Marcar claramente qué documentos van adjuntos

### Fase 3: Envío al estudio

1. Revisar el draft completo con el usuario
2. Listar todos los adjuntos que deben ir con el email
3. El usuario envía el email a Josela (con CC a Juan Pablo y Cecilia)
4. Guardar copia del email enviado en `/FY{año}/`

### Fase 4: Ida y vuelta con el estudio

El estudio suele pedir documentación adicional o aclaraciones. Patrón típico:
- Josela pide docs adicionales o en otro formato
- Responder lo más rápido posible (las demoras atrasan todo el proceso)
- Registrar cada intercambio

### Fase 5: Revisión del papel de trabajo

1. Josela envía el papel de trabajo de Ganancias para revisión
2. Revisar los números y que todo esté correcto
3. Confirmar o plantear dudas
4. Josela envía versión final

### Fase 6: Presentación y pago

1. Josela presenta la DDJJ y envía acuse
2. Verificar si hay saldo a pagar
3. Pagar honorarios del estudio (pedir CBU si no se tiene)

---

## Puntos del pedido (base: 21 puntos)

Estos son los puntos estándar que pide el estudio. Validar cada año si cambiaron.

| # | Punto | Aplica a Guillermo |
|---|-------|--------------------|
| 1 | Inmuebles | No posee (verificar cada año) |
| 2 | Automotores | Sí — Ecosport AD385ZZ + Vento AD800CK |
| 3 | Depósitos bancarios | Sí — múltiples cuentas (ver checklist) |
| 4 | Acciones, FCI, títulos | Verificar cada año |
| 5 | Participación en sociedades | Sí — Filadd |
| 6 | Inversiones financieras | Verificar cada año |
| 7 | Otros bienes (moneda extranjera, etc.) | Sí — USD en efectivo |
| 8 | Préstamos obtenidos | Verificar (préstamo Filadd Corp) |
| 9 | Remuneraciones | Sí — Director Filadd + Monotributo Tech |
| 10 | Alquileres cobrados | No |
| 11 | Legados/donaciones/herencias | No |
| 12 | Otros gastos actividad | Verificar cada año |
| 13 | Seguros de vida / sepelio | No |
| 14 | Cuotas prepagas | No |
| 15 | Honorarios médicos | No |
| 16 | Cargas de familia | No |
| 17 | Personal doméstico | No |
| 18 | Alquileres pagados | Sí — casa en Villa Allende |
| 19 | Servicios educativos | No |
| 20 | Indumentaria / equipamiento | No |
| 21 | Gastos consumo personal | Sí — expensas, servicios, seguros |

---

## Checklist de documentos por fuente

### Banco Galicia (AR)
- [ ] Reporte para impuestos ene–dic **EN EXCEL** (obligatorio, no aceptan otro formato)
- [ ] Si el homebanking falla: pedir a la asesora del banco
- [ ] Saldo al 31/12 en pesos y dólares
- [ ] Estado de cuenta CERA si aplica

### Banco Santander (AR)
- [ ] Tenencias al 31/12
- [ ] Resúmenes de cuenta (poco uso, pero Josela los pide)

### Brubank (AR)
- [ ] Tenencias al 31/12

### Mercado Pago (AR)
- [ ] Tenencias al 31/12
- [ ] Rendimientos del año

### Bull Market / S&C Inversiones (AR)
- [ ] Tenencias al 31/12
- [ ] Detalle de operaciones MEP (cuántos USD vendió, cuántos ARS recibió)
- [ ] Statement del período

### Balanz (AR)
- [ ] Cuenta corriente (mes de diciembre)
- [ ] Resultados del período (ene–dic)
- [ ] Posición consolidada
- [ ] Tenencias al 31/12 (PDF)
- [ ] Órdenes ejecutadas si hubo operaciones

### Ontop (US)
- [ ] Movimientos desde apertura de cuenta (solo dan PDF)
- [ ] Saldo al 31/12

### JPMorgan (US)
- [ ] Registro de movimientos del año
- [ ] Tenencias al 31/12 (checking + savings)

### Cuenta en Alemania (DE)
- [ ] Preparar respuesta: cuenta abierta en 2023, nunca operada, saldo cero
- [ ] Aparece en AFIP — Josela pregunta cada año

### Filadd
- [ ] Certificación de participación societaria
- [ ] Capital, resultado fiscal, cuentas particulares
- [ ] Dividendos y honorarios con retenciones
- [ ] % de participación y cargo

### Monotributo Tech
- [ ] Todas las Facturas E emitidas en el período
- [ ] Detalle de montos y fechas

### Vehículos
- [ ] Verificar si se compró/vendió algún vehículo
- [ ] Si hubo compra: boleto de compra-venta + formulario transferencia

### Alquiler
- [ ] Contrato de locación vigente
- [ ] Comprobantes de pago

### Gastos personales
- [ ] Estimación de expensas (monto mensual promedio)
- [ ] Estimación de servicios (luz, agua, gas, teléfono)
- [ ] Seguros de vehículos (monto total anual)
- [ ] Nota: dividir gastos compartidos con la novia

---

## Formato del email a la contadora

Basado en el email exitoso de FY2024 (10-feb-2025), el formato es:

- Ir **punto por punto** numerado
- Para cada punto: texto explicativo breve + mención de adjuntos
- Los adjuntos van en un ZIP o como archivos separados
- Usar **negrita** para los nombres de las cuentas/fuentes
- Mencionar saldos al 31/12 cuando se tengan
- Si hay situaciones especiales (operaciones crypto, cueveros, etc.), explicarlas con detalle
- Cerrar con "Quedo disponible para cualquier cosa"

**Destinatario**: jmorillo@estudiodelcampillo.com.ar
**CC**: jpdelcampillo@estudiodelcampillo.com.ar, cferraris@estudiodelcampillo.com.ar

---

## Lecciones aprendidas

### De FY2024
1. **Galicia siempre en Excel** — el homebanking puede fallar; tener alternativa (asesora del banco)
2. **Balanz**: bajar todo de una vez (tenencias al cierre + cuenta corriente + posición consolidada + resultados)
3. **ONTOP**: solo dan PDF, pedir con anticipación por soporte
4. **Bull Market**: tener operaciones MEP + tenencias al 31/12
5. **Brubank y Mercado Pago**: Josela los pide — tenerlos preparados
6. **Cuenta en Alemania**: aparece en AFIP cada año, preparar respuesta estándar
7. **Timing**: el proceso FY2024 tomó 5 meses por demoras en responder. Responder rápido.
8. **Monotributo Tech**: puede haber dudas sobre cobros en dólares
9. **Operaciones crypto**: crypto → cueva → dólar billete quedó como "ahorros en mano" en la DDJJ
10. **Venta MEP**: fue en Balanz (no Bull Market). Tener claros los movimientos entre cuentas.

---

## Datos de referencia

**Estudio contable**: Juan del Campillo (Córdoba Capital)
- Josela Morillo: jmorillo@estudiodelcampillo.com.ar
- Juan Pablo Del Campillo: jpdelcampillo@estudiodelcampillo.com.ar
- Cecilia Ferraris: cferraris@estudiodelcampillo.com.ar

**Honorarios FY2024**: ARS $950.000
**Resultado FY2024**: No dio saldo a pagar
