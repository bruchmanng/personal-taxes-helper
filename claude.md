# Personal Taxes Helper — Guillermo Bruchmann

## Contexto del Proyecto
Este repositorio contiene herramientas y documentación para asistir a Guillermo en la preparación y presentación de impuestos en Argentina (Ganancias y Bienes Personales), usando Claude Code.

## Datos del Contribuyente
- **Nombre**: Guillermo Bruchmann
- **Email**: guille@filadd.com
- **Residencia fiscal**: Argentina
- **Nacionalidad**: Argentina
- **Actividad**: Co-fundador y dueño de **Filadd**
- **Historial de presentaciones**: Presenta Ganancias desde al menos 2021

## Situación Fiscal Actual
- **Blanqueo Milei**: Participó del blanqueo de capitales
- **Bienes Personales**: Adherido al **Régimen de Excepción de Bienes Personales por 4 años** → No presenta Bienes Personales durante ese período
- **FY2025** (a presentar en 2026): Se presume que solo debe presentar **Impuesto a las Ganancias** (no Bienes Personales) - A consultar con estudio contable

## Estudio Contable
- **Estudio**: Juan del Campillo (Córdoba Capital, Argentina)
- **Contacto principal**: Josela Morillo (contadora del estudio)
- **Email Josela**: jmorillo@estudiodelcampillo.com.ar
- **Email Juan Pablo**: jpdelcampillo@estudiodelcampillo.com.ar
- **Mecanismo de comunicación principal**: Email

> Nota: Este es el mismo estudio que lleva la contabilidad de la sociedad de Filadd en Argentina. 

## Estructura de Carpetas

```
/FY2024/          → Presentación del período fiscal 2024 (realizada en 2025). Referencia histórica.
/FY2025/          → Presentación del período fiscal 2025 (a realizar en 2026). Trabajo en curso.
/requirements/    → Carpeta por cada punto del pedido de información del estudio (21 puntos).
```

## Pedido de Información FY2025 (del Estudio)

Archivo fuente: [[Pedido de Información Ganancias y Bs Personales 2025.pdf]]`
Fecha del pedido: 13 de enero de 2026

### Los 21 puntos solicitados (según PDF original)

**Nota**: Guillermo solo presenta Ganancias (no Bienes Personales), por lo que algunos puntos aplican parcialmente.

1. **Inmuebles** (del país y del exterior)
2. **Automotores**, naves, aeronaves, etc.
3. **Depósitos en cuenta corriente, plazo fijo o caja de ahorro** — Galicia (Excel), Ontop, etc
4. **Acciones, cuotapartes de FCI y títulos públicos** — Balanz, S&C/Bull Market
5. **Participación en sociedades que no cotizan en bolsa** — Filadd
6. **Inversiones financieras**
7. **Otros bienes** (créditos a terceros, objetos de valor, moneda extranjera en billetes)
8. **Préstamos obtenidos**
9. **Remuneraciones percibidas** (sueldos y/o jubilaciones)
10. **Alquileres de inmuebles devengados** (cobrados)
11. **Legados, donaciones y/o herencias**
12. **Otros gastos vinculados con la actividad**
13. **Seguros de vida / gastos de sepelio**
14. **Cuotas prepagas**
15. **Honorarios por asistencia médica y sanitaria**
16. **Cargas de familia**
17. **Personal doméstico**
18. **Alquileres pagados** (casa habitación)
19. **Servicios y herramientas con fines educativos**
20. **Indumentaria / equipamiento para uso en lugar de trabajo**
21. **Estimación de gastos en consumo personal**

Cada punto tiene su carpeta en `/requirements/` con README.md detallado, historial FY2024 y subcarpetas `docs-FY2024/` y `docs-FY2025/`.

## Objetivo
1. Completar la presentación de Ganancias FY2025
2. Ir creando skills y contexto reutilizable para que las próximas presentaciones sean más fáciles y rápidas

## Obsidian
Este proyecto se gestiona como un vault de Obsidian. Al escribir o editar archivos Markdown:
- Usar `[[wikilinks]]` para referenciar otros archivos del vault (ej: `[[Pedido de Información Ganancias y Bs Personales 2025.pdf]]`)
- Se pueden usar callouts de Obsidian (`> [!note]`, `> [!warning]`, etc.)
- Las carpetas `.obsidian/` contienen configuración del vault y no deben modificarse

## Notas para Claude
- El único usuario es Guillermo. Tutear y ser directo.
- Cuando se trabaje con archivos del contador, respetar el formato que ellos pidan.
- Priorizar crear skills reutilizables para tareas repetitivas (recopilación de datos, armado de planillas, etc).
- Los archivos de FY2024 sirven como referencia de formato y estructura de presentaciones anteriores.
