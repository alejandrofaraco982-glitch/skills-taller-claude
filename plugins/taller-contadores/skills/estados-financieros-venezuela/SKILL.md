---
name: estados-financieros-venezuela
description: Prepara estados financieros de empresas venezolanas (resultados, situación financiera, flujo de efectivo y cambios en el patrimonio) bajo VEN-NIF, comparando contra el período anterior y el presupuesto, y señalando variaciones importantes. Úsala al cerrar el mes, trimestre o año, al preparar un resumen financiero para la gerencia, o al revisar ajustes de cierre con bolívares, dólares, tasa BCV e inflación.
argument-hint: "<mensual | trimestral | anual | acumulado> <período>"
---

# Estados financieros (Venezuela)

**Importante:** esta guía ayuda a preparar y revisar estados financieros; no sustituye a un contador público colegiado. Los estados que se presenten a terceros (bancos, SENIAT, accionistas) deben ser revisados y firmados por un contador público colegiado. Si una norma o boletín citado aquí no se puede confirmar con la versión vigente, dilo; nunca inventes normas, tasas ni artículos.

Responde en español. Escribe montos con formato venezolano (punto para miles, coma para decimales: Bs 1.250.000,50).

## Uso

```
/estados-financieros-venezuela <tipo de período> <período>
```

- `mensual`: compara con el mes anterior y el mismo mes del año anterior.
- `trimestral`: compara con el trimestre anterior y el mismo trimestre del año anterior.
- `anual`: compara con el año anterior.
- `acumulado`: lo que va de año contra el mismo tramo del año anterior.

Ejemplo: `/estados-financieros-venezuela mensual 2026-09`

## Paso 1: Datos y reglas de la empresa

Si hay un sistema contable conectado, extrae balance de comprobación, períodos de comparación y presupuesto. Si no, pide al usuario que pegue o suba:
- Balance de comprobación o saldos por cuenta del período y de los períodos a comparar.
- Presupuesto, si existe.
- Ajustes o reclasificaciones conocidos.

Pregunta (y anota en el informe) antes de calcular, sin suponer:
1. **Marco contable:** VEN-NIF GE (grandes entidades) o VEN-NIF PYME.
2. **Moneda de los registros:** bolívares, dólares o ambas.
3. **Tasa de cambio usada:** para los libros oficiales debe ser la tasa oficial del BCV. Si el usuario quiere ver también la tasa Binance o paralela, preséntala solo en un cuadro aparte, marcado "solo para gestión, no oficial".
4. **Ajuste por inflación:** si la empresa lo aplica (BA VEN-NIF 2 y NIC 29 / Sección 31 de NIIF para PYMES) y con qué índice (INPC del BCV).
5. **Umbrales de importancia** propios de la empresa. Si no hay, usa los de por defecto (Paso 3).

## Paso 2: Estado de resultados

```
ESTADO DE RESULTADOS
Empresa: [nombre]   RIF: [J-XXXXXXXX-X]
Período: [descripción]
Expresado en: [Bs / USD a tasa BCV / Bs constantes]

                              Actual    Anterior   Var.     Var.   Presupuesto  Var. vs
                                                   (monto)  (%)                 presup.
INGRESOS
  Ventas de bienes
  Ingresos por servicios
  Otros ingresos operativos
TOTAL INGRESOS

COSTO DE VENTAS
UTILIDAD BRUTA
  Margen bruto (%)

GASTOS OPERATIVOS
  Gastos de personal (sueldos, utilidades, vacaciones, prestaciones sociales)
  Gastos de ventas y mercadeo
  Gastos generales y de administración
  Depreciación y amortización
TOTAL GASTOS OPERATIVOS

UTILIDAD (PÉRDIDA) OPERATIVA
  Margen operativo (%)

OTROS INGRESOS (EGRESOS)
  Diferencial cambiario, neto (ganancia o pérdida en cambio)
  Resultado monetario del ejercicio (REME), si aplica ajuste por inflación
  Gastos financieros (intereses, comisiones bancarias)
  IGTF (impuesto a las grandes transacciones financieras)
  Otros, neto

UTILIDAD ANTES DE IMPUESTO
  Impuesto sobre la renta (ISLR)
UTILIDAD (PÉRDIDA) NETA
  Margen neto (%)
```

Notas de presentación:
- El diferencial cambiario y el REME van separados de la operación; en Venezuela suelen mover mucho el resultado y la gerencia debe verlos aparte.
- Los aportes parafiscales y contribuciones sobre la nómina (por ejemplo, la contribución especial para pensiones) se muestran dentro de gastos de personal o en una línea propia si son importantes.
- No mezcles en una misma columna montos a tasa BCV y a otra tasa.

## Paso 3: Variaciones

Para cada línea calcula:
- **Variación en monto:** actual − anterior (o actual − presupuesto).
- **Variación %:** (actual − anterior) / |anterior| × 100.
- **Márgenes:** cambio en puntos porcentuales.

**Ojo con la inflación y el tipo de cambio.** Comparar bolívares nominales de meses distintos casi siempre muestra "crecimiento" falso. Haz siempre una de estas dos cosas y dilo en el informe:
- Comparar en USD a tasa BCV de cierre de cada período, o
- Comparar en bolívares constantes (ajustados por INPC).

### Umbrales por defecto (ajustar a la empresa)

| Tamaño de la línea (USD a tasa BCV) | Monto | % |
|---|---|---|
| Más de 1.000.000 | 50.000 | 5% |
| 100.000 a 1.000.000 | 10.000 | 10% |
| Menos de 100.000 | 5.000 | 15% |

Una variación es importante si pasa el monto **o** el porcentaje.

### Explicar cada variación importante

Separa la causa en:
- **Precio:** cambió el precio de venta o de compra.
- **Volumen:** se vendió o compró más o menos.
- **Mezcla:** cambió la proporción de productos.
- **Tipo de cambio:** efecto de la variación de la tasa BCV.
- **Inflación:** efecto de la pérdida de valor del bolívar.
- **Partidas únicas:** no se repiten (multas, venta de un activo).
- **Fecha:** algo se registró en otro mes (no es un cambio real).

Luego: di si es favorable o desfavorable, si parece temporal o tendencia, y qué hay que hacer (investigar, corregir, ajustar el presupuesto).

## Paso 4: Indicadores clave

```
INDICADORES                    Actual   Anterior   Cambio
Crecimiento de ingresos (USD)                       X,X%
Margen bruto                   XX,X%    XX,X%       X,X pp
Margen operativo               XX,X%    XX,X%       X,X pp
Margen neto                    XX,X%    XX,X%       X,X pp
Gastos operativos / ingresos   XX,X%    XX,X%       X,X pp
Diferencial cambiario / ingresos XX,X%  XX,X%       X,X pp
Tasa BCV de cierre             Bs XX,XX Bs XX,XX    X,X%
```

## Paso 5: Lista de variaciones a investigar

| Línea | Variación (monto) | Variación % | Favorable / Desfavorable | Causa probable | Acción |
|---|---|---|---|---|---|

## Paso 6: Entrega

1. Estado de resultados con comparaciones.
2. Indicadores clave.
3. Lista de variaciones a investigar.
4. Preguntas para aclarar las variaciones sin explicación.
5. Supuestos usados: marco (GE o PYME), moneda, tasa, si hubo ajuste por inflación.
6. Aviso: "Borrador para revisión de un contador público colegiado."

## Referencia: Estado de situación financiera

```
ACTIVO
Activo corriente
  Efectivo y equivalentes (separar bolívares y divisas)
  Cuentas por cobrar comerciales, neto de estimación por incobrables
  Anticipos a proveedores
  Inventarios
  Impuestos por recuperar (IVA crédito fiscal, retenciones de IVA e ISLR)
  Gastos pagados por anticipado
Total activo corriente

Activo no corriente
  Propiedades, planta y equipo, neto
  Activos intangibles, neto
  Impuesto diferido activo
  Otros activos
Total activo no corriente

TOTAL ACTIVO

PASIVO
Pasivo corriente
  Cuentas por pagar comerciales
  Anticipos de clientes
  Préstamos bancarios, porción corriente
  Impuestos por pagar (IVA, ISLR, retenciones, IGTF)
  Gastos acumulados por pagar (utilidades, vacaciones, aportes)
Total pasivo corriente

Pasivo no corriente
  Préstamos a largo plazo
  Prestaciones sociales (garantía y retroactivo, según LOTTT)
  Impuesto diferido pasivo
Total pasivo no corriente

TOTAL PASIVO

PATRIMONIO
  Capital social
  Actualización del capital (si hay ajuste por inflación)
  Reserva legal
  Superávit por revaluación, si aplica
  Resultados acumulados
TOTAL PATRIMONIO

TOTAL PASIVO Y PATRIMONIO
```

## Referencia: Estado de flujos de efectivo (método indirecto)

```
ACTIVIDADES DE OPERACIÓN
Utilidad (pérdida) neta
Ajustes que no son efectivo:
  Depreciación y amortización
  Provisión de prestaciones sociales
  Estimación de incobrables
  Diferencial cambiario no realizado
  Resultado monetario (REME), si aplica
  Impuesto diferido
Cambios en capital de trabajo:
  Cuentas por cobrar, inventarios, anticipos
  Cuentas por pagar, impuestos y gastos acumulados
  Pago de prestaciones sociales
Efectivo neto de operación

ACTIVIDADES DE INVERSIÓN
  Compra / venta de propiedades y equipos
Efectivo neto de inversión

ACTIVIDADES DE FINANCIAMIENTO
  Préstamos recibidos / pagados
  Aportes de capital
  Dividendos pagados
Efectivo neto de financiamiento

Efecto de la variación de la tasa de cambio sobre el efectivo
Aumento (disminución) neto del efectivo
Efectivo al inicio
Efectivo al final
```

Recuerda que bajo VEN-NIF también se presenta el **estado de cambios en el patrimonio** y las notas.

## Ajustes de cierre frecuentes en Venezuela

1. **Diferencial cambiario:** revaluar saldos en divisas (efectivo, cuentas por cobrar y por pagar) a la tasa BCV de cierre.
2. **Ajuste por inflación:** si aplica, reexpresar partidas no monetarias con el INPC y registrar el REME.
3. **Nómina:** acumular utilidades, vacaciones, bono vacacional y prestaciones sociales del período.
4. **Depreciación y amortización.**
5. **Incobrables:** revisar antigüedad de saldos y estimar lo que no se cobrará.
6. **Inventarios:** bajar el valor de lo obsoleto o dañado.
7. **Impuestos:** provisión de ISLR (y diferido), cuadre de IVA débito/crédito y retenciones.
8. **Reserva legal:** al cierre anual, apartar la porción de utilidades que exige el Código de Comercio.
9. **Reconversión monetaria:** si se comparan años afectados por una reconversión, expresar todo en la misma escala de bolívares.

## Reclasificaciones frecuentes

1. Pasar a corriente la porción de préstamos que vence en 12 meses.
2. Neto de estimaciones: incobrables contra cuentas por cobrar; depreciación acumulada contra activos.
3. Separar anticipos de clientes y de proveedores de las cuentas comerciales.
4. Eliminar saldos entre empresas del mismo grupo si se consolida.
