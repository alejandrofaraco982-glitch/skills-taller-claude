---
name: triage-nda-venezuela
description: Revisa rápido un acuerdo de confidencialidad (NDA) bajo ley venezolana y lo clasifica en VERDE (se puede firmar), AMARILLO (que lo revise un abogado) o ROJO (no firmar sin revisión completa). Úsala cuando llegue un NDA de un cliente, proveedor o socio, o para detectar cláusulas escondidas de no competencia, exclusividad o penalidades.
argument-hint: "<NDA en archivo o texto>"
---

# Revisión rápida de NDA (Venezuela)

Revisa el NDA: @$1

Clasifica el acuerdo para saber qué hacer con él: firmarlo, pasarlo a un abogado o rechazarlo.

**Importante:** esto es un filtro inicial, no una opinión legal. Un abogado venezolano debe revisar todo antes de decidir. Si una referencia legal de esta guía no se puede confirmar con el texto vigente, dilo; nunca inventes artículos ni leyes.

Responde siempre en español, en lenguaje sencillo.

## Paso 1: Recibir el NDA

Acepta el NDA como archivo (PDF, Word), enlace o texto pegado. Si no lo dan, pídelo.

Anota de entrada:
- **Idioma.** Si está en otro idioma, avisa: para presentarlo ante un tribunal venezolano hará falta traducción de intérprete público.
- **Partes.** Persona natural o jurídica, venezolana o extranjera. Si es extranjera, el punto de ley aplicable (Paso 3, n.º 10) pesa más.

## Paso 2: Cargar las reglas de la empresa

Busca las reglas propias de la empresa (por ejemplo, un archivo `legal.local.md`): plazos aceptados, cláusulas prohibidas, quién firma.

**Si no hay reglas propias**, usa estas por defecto y dilo en el informe:
- Obligaciones mutuas (salvo que solo la empresa entregue información).
- Duración del acuerdo: 1 a 3 años. Confidencialidad después de terminar: 2 a 5 años; más tiempo solo para secretos comerciales o industriales.
- Excepciones completas (ver n.º 4).
- Sin no competencia, sin no captación de personal, sin exclusividad.
- Ley venezolana y tribunales de Caracas, o arbitraje en un centro reconocido.

## Paso 3: Revisión punto por punto

### 1. Tipo de acuerdo
- ¿Mutuo o de una sola vía? ¿Tiene sentido para la relación? (Conversaciones exploratorias: mutuo. Solo una parte entrega información: una vía, en la dirección correcta.)
- ¿Es solo un NDA, o trae escondidos términos comerciales (precios, exclusividad, compromisos de compra)? Si trae eso, es ROJO: hay que revisarlo como contrato completo.

### 2. Qué se considera confidencial
- Que no sea excesivo ("toda información de cualquier tipo, marcada o no").
- Si exige marcar la información como confidencial, que sea práctico (por ejemplo, confirmar por escrito o por correo en 30 días lo que se dijo de palabra).
- Que no declare confidencial lo que ya es público o lo que la empresa desarrolló por su cuenta.

### 3. Obligaciones de quien recibe
- Cuidado razonable, el mismo que usa con su propia información.
- Usar la información solo para el fin indicado.
- Compartirla solo con quien la necesite y esté obligado a guardar reserva.
- Sin exigencias imposibles (cifrar todo, llevar bitácoras físicas).

### 4. Excepciones obligatorias
Deben estar todas:
- Información pública sin culpa de quien la recibe.
- Información que ya se tenía antes.
- Información desarrollada por cuenta propia.
- Información recibida legítimamente de un tercero.
- **Orden de autoridad:** poder entregarla cuando lo exija la ley o una autoridad venezolana (tribunales, Ministerio Público, SENIAT, SUDEBAN u otro organismo), avisando a la otra parte cuando la ley lo permita. Sin esta excepción, la empresa queda entre incumplir el NDA o desobedecer a la autoridad.

### 5. Con quién se puede compartir
- Empleados que lo necesiten.
- Asesores externos (abogados, contadores, auditores, consultores) obligados a reserva.
- Empresas del mismo grupo, si hace falta.
- Autoridades, según el n.º 4.

### 6. Duración
- Acuerdo: 1 a 3 años es lo normal.
- Confidencialidad después de terminar: 2 a 5 años.
- Evitar "para siempre", salvo secretos comerciales o industriales.

### 7. Devolución o destrucción
- Al terminar o cuando se pida.
- Excepción para copias que la ley obliga a guardar (por ejemplo, soportes contables y fiscales que exige el SENIAT) y copias de respaldo automáticas.
- Una constancia escrita de destrucción es razonable; exigir declaración jurada o acta notariada es excesivo.

### 8. Consecuencias del incumplimiento
- **Medidas cautelares:** es normal que diga que la parte afectada puede pedir medidas cautelares a un juez. En Venezuela las prevé el Código de Procedimiento Civil.
- **Cláusula penal (monto fijo por incumplimiento):** en Venezuela es común y válida (Código Civil). No la marques ROJO solo por existir. Revisa:
  - Que el monto sea razonable frente al negocio. Si es desproporcionado: ROJO.
  - Que aplique a ambas partes en un NDA mutuo.
  - En qué moneda está. Si está en USD, que diga cómo se paga en bolívares (por ejemplo, a la tasa oficial del BCV del día de pago).
  - Que no se sume a otra indemnización por el mismo hecho sin aclararlo.

### 9. Cláusulas peligrosas
- **No competencia:** no pertenece a un NDA. Además puede chocar con la libertad económica y las normas de competencia. ROJO.
- **No captación de empleados:** no pertenece a un NDA. Si la otra parte insiste: limitarla a ofertas dirigidas (no avisos públicos) y a 12 meses máximo. Recuerda que no puede impedir que un trabajador renuncie y busque empleo.
- **Exclusividad:** prohibir conversar con otros. ROJO salvo que haya una razón de negocio clara.
- **Cláusula de "residuos"** (usar libremente lo que se recuerde de memoria): resistirla; si se acepta, que no cubra secretos comerciales ni invenciones.
- **Cesión o licencia de propiedad intelectual** (marcas, patentes, derechos de autor): un NDA no debe dar derechos. ROJO.
- **Auditorías** a la otra parte: inusuales en un NDA.

### 10. Ley aplicable y dónde se resuelven los conflictos
- **Entre partes venezolanas:** lo esperado es ley venezolana y tribunales venezolanos.
- **Con parte extranjera:** si pone ley extranjera y tribunales extranjeros, AMARILLO (pleitear fuera es caro y lento). Si además exige litigar en un país sin relación con el negocio, ROJO.
- **Arbitraje:** en Venezuela está reconocido (Ley de Arbitraje Comercial) y es habitual en contratos comerciales. No es malo en sí. Prefiere un centro conocido (por ejemplo, el Centro de Arbitraje de la Cámara de Caracas o CEDCA). AMARILLO si el centro, la sede o los costos son desfavorables.
- **Firma electrónica:** es válida en Venezuela (Ley sobre Mensajes de Datos y Firmas Electrónicas). No hace falta rechazar el NDA por firmarse en digital.

### 11. Datos personales
Venezuela no tiene una ley general de protección de datos; aplica la Constitución (derecho a la privacidad y habeas data). Si el NDA implica compartir datos de clientes o empleados, marca AMARILLO y sugiere agregar: uso limitado, seguridad mínima y aviso si hay filtración.

## Paso 4: Clasificar

### VERDE: se puede firmar
**Todo** esto se cumple:
- Tipo correcto (mutuo o una vía en la dirección correcta).
- Todas las excepciones del n.º 4, incluida la de orden de autoridad venezolana.
- Plazos dentro de lo normal.
- Sin no competencia, no captación ni exclusividad.
- Cláusula penal ausente, o razonable y recíproca.
- Ley y tribunales (o arbitraje) aceptables.
- Excepción para guardar copias que exige la ley.

**Qué hacer:** firmar según quién tiene autorización en la empresa. Mismo día.

### AMARILLO: que lo revise un abogado
Uno o más de estos, sin ser grave:
- Definición algo amplia.
- Plazos algo largos (por ejemplo, 5 años de acuerdo o 7 de confidencialidad).
- Falta una excepción fácil de agregar.
- Ley extranjera con parte extranjera, o arbitraje en condiciones poco favorables.
- Cláusula penal en USD sin decir cómo se paga en bolívares.
- Falta la excepción para guardar copias legales.
- Se comparten datos personales sin reglas.
- Está en otro idioma y no hay versión en español.

**Qué hacer:** enviar al abogado con los puntos señalados. 1 a 2 días hábiles.

### ROJO: no firmar
Uno o más de estos:
- Tipo equivocado (una vía cuando debe ser mutuo, o en dirección contraria).
- Falta la excepción de desarrollo propio o la de orden de autoridad.
- No competencia, no captación amplia o exclusividad.
- Duración de 10 años o más, o perpetua sin tratarse de secretos.
- Definición que atrapa información pública o propia.
- Cesión o licencia de propiedad intelectual.
- Cláusula penal desproporcionada o solo contra la empresa.
- Obliga a litigar en el extranjero sin relación con el negocio.
- No es realmente un NDA (trae términos comerciales).

**Qué hacer:** revisión completa por abogado, contrapropuesta con el modelo de NDA de la empresa, o rechazo. 3 a 5 días hábiles.

## Paso 5: Informe

```
## Revisión de NDA

**Resultado:** [VERDE / AMARILLO / ROJO]
**Partes:** [nombres]
**Tipo:** [Mutuo / Una vía (entregamos) / Una vía (recibimos)]
**Duración:** [plazo]
**Ley y conflictos:** [ley aplicable; tribunales o arbitraje]
**Idioma:** [español / otro]
**Base de revisión:** [Reglas de la empresa / Reglas por defecto]

## Revisión punto por punto

| Punto | Estado | Nota |
|---|---|---|
| Tipo de acuerdo | [OK / REVISAR / FALLA] | [detalle] |
| Qué es confidencial | ... | ... |
| Excepciones | ... | ... |
| Duración | ... | ... |
| Cláusula penal | ... | ... |
| Cláusulas peligrosas | ... | ... |
| Ley y conflictos | ... | ... |

## Problemas encontrados

### [Problema 1 – AMARILLO/ROJO]
**Qué dice:** [cita corta de la cláusula]
**Riesgo:** [qué puede pasar, en palabras simples]
**Cambio sugerido:** [texto propuesto en español]

## Recomendación
[Firmar / enviar al abogado con estas notas / rechazar o contraproponer]

## Próximos pasos
1. ...
2. ...

*Filtro inicial. No sustituye la revisión de un abogado venezolano.*
```

## Notas
- Si el documento no es realmente un NDA, márcalo ROJO de inmediato y recomienda revisión completa del contrato.
- Si la confidencialidad está dentro de un contrato mayor, avisa que el resto del contrato puede cambiar el análisis.
- Si el usuario duda de algún punto, recomiéndale consultarlo con su abogado.
