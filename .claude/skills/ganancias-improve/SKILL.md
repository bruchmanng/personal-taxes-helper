---
name: ganancias-improve
description: >
  Meta-skill: invocar PROACTIVAMENTE cuando durante el trabajo con el usuario se detecte
  conocimiento nuevo que debería incorporarse al playbook de /ganancias. Ejemplos: un formato
  que pidió la contadora, un paso no documentado, una corrección, un patrón repetitivo,
  información nueva sobre cuentas o fuentes de datos, un error que se podría prevenir.
  NO invocar si el conocimiento ya está en el playbook.
---

# Meta-skill: Mejora continua del playbook de Ganancias

## Tu rol

Sos el mecanismo de mejora continua del playbook `/ganancias`. Tu trabajo es detectar cuándo se descubre conocimiento nuevo durante el trabajo y proponerle a Guillermo incorporarlo al playbook para que el proceso sea más autónomo el año siguiente.

## Cuándo activarte

Activarte cuando detectes cualquiera de estos durante el trabajo normal:

- **Paso no documentado**: el proceso requirió un paso que no está en el playbook
- **Formato o requisito nuevo**: la contadora pidió algo en un formato específico no registrado
- **Cuenta o fuente nueva**: apareció una cuenta bancaria/financiera que no estaba en el checklist
- **Corrección del usuario**: Guillermo corrigió algo que estaba mal en el playbook
- **Patrón repetitivo**: se repite una acción que se podría sistematizar
- **Gotcha o error evitado**: algo que casi sale mal y debería documentarse como advertencia
- **Cambio en los puntos del pedido**: los 21 puntos cambiaron respecto al año anterior
- **Info de contacto actualizada**: cambió un email, nombre o mecanismo de comunicación
- **Timing útil**: se aprendió algo sobre cuándo conviene hacer algo

## Cuándo NO activarte

- El conocimiento ya está en el playbook de `/ganancias`
- Es información efímera que solo aplica a este año (ej: "el saldo de Galicia es X")
- Es un dato que pertenece al historial del año (`/FY{año}/`) y no al proceso general
- El usuario está en medio de algo urgente y la interrupción no aporta

## Cómo proponer una mejora

1. **Leer el playbook actual**: `Read .claude/skills/ganancias/SKILL.md`
2. **Identificar dónde va el cambio**: qué sección del playbook se debe actualizar
3. **Proponer al usuario** de forma concisa:

   ```
   > [!tip] Mejora para el playbook de /ganancias
   > Detecté que [descripción del conocimiento nuevo].
   > Esto no está en el playbook. Propongo agregar:
   > - [cambio concreto]
   > ¿Actualizo el playbook?
   ```

4. **Si el usuario acepta**: editar `.claude/skills/ganancias/SKILL.md` con el cambio
5. **Si el usuario rechaza**: no insistir. Si da una razón, considerar si esa razón también es una lección.

## Reglas

- **Nunca editar el playbook sin preguntar primero**
- **Ser conciso**: la propuesta debe ser de 2-3 líneas, no un ensayo
- **Un cambio a la vez**: no acumular múltiples mejoras en una sola propuesta
- **No interrumpir flujo crítico**: si el usuario está armando el draft del email o revisando un documento, esperar a un momento natural de pausa
- **Priorizar lo reutilizable**: solo proponer cosas que apliquen a años futuros, no datos puntuales de este año
