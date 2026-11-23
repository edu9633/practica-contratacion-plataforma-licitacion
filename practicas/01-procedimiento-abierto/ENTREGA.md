# Práctica 01 — Procedimiento abierto (obligatorio en todas sus fases)

Enunciado: `enunciados/01_procedimiento-abierto_v-<versión>.txt` (versión en `../datos-comunes.md`)
Pliegos de referencia descargados en `documentos/`: PCAP, PPT y memoria justificativa.

Identificador de la licitación: `INAP-050-AB-230278`

Perfil de contratante: `OC_INAP_26_AVAN_SEPT_050`

## Ejercicio 1 — Configuración (M3)
- [ ] Datos básicos del expediente según el pliego (objeto, CPV, presupuesto, valor estimado, lotes, duración)
- [x] Presentación «Electrónica a través de la Plataforma»
- [x] Mesa asignada: órgano de asistencia del módulo 2. Pendiente completar su composición para las sesiones.
- [x] Capacidad, solvencia económica (110.443,94 €) y técnica (51.540,50 €) comprobadas al reabrir el expediente.
- [x] Cinco criterios con las ponderaciones del pliego: 8, 36 y 5 puntos de juicio de valor, y 47 y 4 automáticos. [Captura](evidencias/ej01_criterios-verificados_20261123.png).
- [x] Tres sobres guardados y comprobados desde el PCAP: administrativo (declaración y Anexo VIII), técnico (proposición técnica) y automático (Anexo II). [Captura](evidencias/ej01_sobres-verificados_20261123.png).
- [ ] Fecha de presentación futura y próxima
- [ ] Simulador de presentación revisado y coherente con el pliego (captura)

**Supuestos:**

- Se creó el expediente con CPV 72320000, 182.551,95 € sin IVA, 220.887,86 € con IVA y 304.253,25 € de valor estimado. Se cargaron 36 meses de ejecución y el plazo provisional del 28/11/2026 a las 20:00.
- Se registraron la solvencia de 110.443,94 € y 51.540,50 €, los criterios de 8, 36, 5, 47 y 4 puntos, y los tres sobres del PCAP. Se verificó el guardado de los tres sobres. Falta revisar el resultado del simulador.
**Texto para el Campus:**
```
Perfil de contratante: OC_INAP_26_AVAN_SEPT_050
Identificador de la licitación: INAP-050-AB-230278
```

## Ejercicio 2 — Convocatoria (M4)

PCAP y PPT guardados mediante sus URL oficiales. La previsualización en Plataforma validó el anuncio sin errores. La previsualización del DOUE devolvió una [incidencia de la Plataforma](evidencias/ej02_error-previsualizacion-DOUE_20261123-1916.png). El anuncio sigue pendiente de publicación.

La memoria justificativa está en `documentos/memoria-justificativa.pdf`. La acción independiente de publicación abre un selector de archivos y no ofrece un campo de URL. El navegador perdió la conexión al seleccionar el PDF. Antes de reintentar, comprobar si la memoria figura adjunta en el resumen del expediente.

- [ ] Fin de plazo ≥4 días tras la publicación y no excesivo — fecha: 
- [ ] Anuncio de licitación previsualizado
- [ ] Anuncio publicado con envío a DOUE y BOE; desbloqueo confirmado
- [ ] Pliegos y anexos en PPT, PCAP y Anexo pliegos
- [ ] Anuncio de pliegos publicado
- [ ] Memoria justificativa publicada en la pestaña Resumen
- [ ] Todo visible en la vista pública (captura)

**Texto para el Campus:**
```
Perfil de contratante: 
Identificador de la licitación: 
```

## Ejercicio 3 — Pregunta/respuesta y ofertas (M4)
- [x] Preparados los dos anexos económicos y las dos memorias técnicas en PDF, con el modelo administrativo del Anexo VIII. [Documentos y reparto por sobres](documentos/borradores-m4.md).
- [ ] Pregunta hecha por un operador económico
- [ ] Pregunta respondida y publicada
- [ ] Oferta presentada por OE1 (justificante)
- [ ] Oferta presentada por OE2 con defecto subsanable (justificante)

**Texto para el Campus:**
```
Perfil de contratante: 
Identificador de la licitación: 
```

## Ejercicio 4 — Selección de licitadores (M5)

- [x] Sesión provisional `INAP-050-AB-M5-ADMIN` creada para el 30/11/2026 a las 11:00. [Evidencia](evidencias/ej04_sesion-provisional_20261123.png).
- [ ] Incorporar el acto de apertura y calificación administrativa. La Plataforma exige publicar el sobre antes de incorporarlo. Revisar el horario una vez fijado el plazo efectivo de ofertas.
- [ ] Sesiones creadas y convocadas con el usuario secretario
- [ ] Miembros marcados como presentes
- [ ] Acto de apertura y calificación administrativa (un licitador admitido provisionalmente)
- [ ] Acto de subsanación celebrado
- [ ] Apertura y valoración de los siguientes sobres
- [ ] Propuesta de adjudicación creada
- [ ] Informes generados: lista de licitadores, apertura, propuesta (en `evidencias/`)
- [ ] Comunicación genérica (aclaración de la oferta técnica u oferta anormalmente baja)
- [ ] Acta gestionada de al menos una sesión

**Cálculo de prueba para contrastar la valoración**

Los siguientes resultados corresponden a los [borradores A y B](documentos/borradores-m4.md). Se supone que ambas ofertas se presentan y se admiten, que B subsana el Anexo VIII y que ambas obtienen al menos 29,40 puntos en la valoración técnica. El cálculo queda pendiente de comprobar contra las ofertas y puntuaciones registradas en la Plataforma.

| Oferta | Precio sin IVA | Puntos de precio (máx. 47) | Mejora de seguridad y salud sin IVA | Puntos de mejora (máx. 4) | Subtotal automático |
|---|---:|---:|---:|---:|---:|
| A | 180.000,00 € | 46,61 | 250,00 € | 3,33 | 49,94 |
| B | 178.500,00 € | 47,00 | 300,00 € | 4,00 | 51,00 |

- **Precio (§12.2.2 del PCAP).** Aplicar `47 × (1 − (precio ofertado − 178.500) / 178.500)`, con suelo de 0. La referencia es el menor precio admitido sin anormalidad.
- **Mejora social (§12.2.2).** Aplicar `4 × importe de la mejora / 300`, redondeado a dos decimales. La referencia es el mayor importe admitido para esta mejora.
- **Anormalidad (§12.5.B).** Si se admiten ambas ofertas de dos operadores independientes, la media es 179.250,00 €. Incluso el umbral más alto (75 % de la media, 134.437,50 €) queda por debajo de ambos precios. Para el acto adicional se prepara una aclaración técnica.
- **Resultado global (§12.3).** Sumar la valoración técnica al precio y a la mejora social, conservando la precisión del cálculo de precio hasta redondear el total a dos decimales. La puntuación técnica todavía debe introducirse en el acto correspondiente antes de decidir la clasificación.

**Texto para la solicitud de aclaración técnica a A**

> En el apartado 3.4 de la memoria técnica se indica que se registrarán las exclusiones, las unidades y las diferencias pendientes en la conciliación de datos. Indique qué campos del registro propuesto permiten identificar la consulta de origen y quién valida el cierre de cada diferencia. La aclaración debe referirse al método ya descrito en la oferta presentada.

**Texto para el Campus:**
```
Perfil de contratante: 
Identificador de la licitación: 
```

## Ejercicio 5 — Resolución (M6)
- [ ] Requerimiento de documentación al propuesto
- [ ] Adjudicación configurada y publicada
- [ ] Adjudicación comunicada a todas las empresas
- [ ] Contrato firmado en la Plataforma (certificado)
- [ ] Formalización publicada con DOUE y BOE; desbloqueo confirmado

**Borrador del requerimiento de formación**

> Expediente INAP-050-AB-230278. Tras la aceptación de la propuesta de la mesa, se requiere al licitador propuesto que presente la documentación justificativa del apartado 18 del PCAP. Deberá acreditar, en lo que proceda, la capacidad y representación, la solvencia y la documentación restante exigida en el pliego, incluida la garantía definitiva. El plazo previsto en el PCAP es de diez días hábiles desde el día siguiente al de recepción del requerimiento.

Seleccionar como destinatario al licitador que figure en la propuesta efectiva de la mesa. El texto está preparado para el entorno de formación y queda pendiente de envío.

**Texto para el Campus:**
```
Perfil de contratante: 
Identificador de la licitación: 
```

## Ejercicio 6 — Modificación de contrato (M6)
- [ ] Modificación publicada (DOUE opcional)
- [ ] Visible en el perfil (captura)

**Datos de prueba para el anuncio**

| Campo | Valor propuesto |
|---|---|
| Número | 1 |
| Descripción | Incorporación, durante la ejecución simulada, de una actualización adicional del diccionario de datos y de una comprobación de coherencia de los registros mensuales. |
| Duración | Sin variación. Se mantienen los 36 meses iniciales del expediente. |
| Incremento sin IVA | 1.800,00 € de prueba. |
| Importe resultante | Importe sin IVA del contrato formalizado más 1.800,00 €. Si la oferta adjudicada fuese la A del borrador, el total sería 181.800,00 € sin IVA y 219.978,00 € con IVA. |
| Fecha | Usar la fecha que corresponda al acuerdo de modificación en formación una vez formalizado el contrato. |

Estos datos describen un caso ficticio. La modificación no está registrada ni publicada.

**Texto para el Campus:**
```
Perfil de contratante: 
Identificador de la licitación: 
```
