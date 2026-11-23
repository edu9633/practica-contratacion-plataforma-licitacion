# Cuadro de mando de las prácticas

Estados: ⬜ pendiente · 🔄 en curso · ✅ listo para entregar · 📤 entregado (lo marca el usuario) · ⛔ bloqueado

El usuario indica que el Campus cierra el 23/11/2026. Los plazos posteriores que figuran más abajo corresponden a la Plataforma de formación y no amplían el plazo del Campus.

| Práctica | Ej. | Descripción | Estado | ID licitación | Notas |
|---|---|---|---|---|---|
| Requisito | — | Órgano de asistencia del módulo 2 (mesa + secretario) | ⛔ | — | Mesa activa. Único miembro asignado: secretario. Presidencia y vocalías necesarias vacantes. |
| Requisito | — | ≥2 operadores económicos ficticios | ⛔ | — | El alta de Empresas exige introducir manualmente los caracteres de un CAPTCHA. No se crearon cuentas. |
| Requisito | — | Certificado de pruebas + AutoFirma + Java en el navegador del agente | ⛔ | — | Sin certificado personal vigente con clave privada ni AutoFirma en la ruta estándar. Temurin 8 e IcedTea-Web portátiles arrancan, pero el simulador queda en la carga de los recursos. |
| 00 Contrato menor | 1 | Crear, publicar y verificar (OC y vista pública) | ✅ | INAP-050-CM-2026-01 | Adjudicación visible como órgano de contratación y en el buscador público sin sesión de Organismos. Texto y evidencias en `ENTREGA.md`. |
| 01 Abierto | 1 | Configuración (M3) | 🔄 | INAP-050-AB-230278 | Verificado el guardado de los tres sobres y de los enlaces de PCAP y PPT. El lanzador portátil se inicia. La vista de sobres del simulador sigue sin abrirse. |
| 01 Abierto | 2 | Anuncio de licitación DOUE/BOE, pliegos, memoria (M4) | ⛔ | INAP-050-AB-230278 | Validación de Plataforma sin errores. El servicio DOUE falló al generar la previsualización. Tras recuperar el acceso, la Plataforma indicó «No tiene la reserva de la licitación, no es modificable» y no abrió el gestor para adjuntar la memoria. Convocatoria sin publicar. |
| 01 Abierto | 3 | Pregunta/respuesta + ofertas (M4) | ⛔ | INAP-050-AB-230278 | Pregunta, respuesta y ofertas de prueba preparadas. Falta publicar la convocatoria y disponer de operadores registrados. |
| 01 Abierto | 4 | Sesiones, apertura, subsanación, valoración, propuesta (M5) | ⛔ | INAP-050-AB-230278 | Sesión provisional `INAP-050-AB-M5-ADMIN` creada. La Plataforma exige publicar los sobres antes de incorporar el acto de apertura. Revisar la fecha tras publicar la licitación. |
| 01 Abierto | 5 | Requerimiento, adjudicación, firma, formalización (M6) | ⛔ | INAP-050-AB-230278 | Texto del requerimiento preparado. El envío exige una propuesta de adjudicación aceptada. |
| 01 Abierto | 6 | Modificación de contrato (M6) | ⛔ | INAP-050-AB-230278 | Datos del caso de prueba preparados. El anuncio necesita un contrato formalizado. |
| 02 Simplificado | 1 | Configuración (M3) | 🔄 | INAP-050-AS-2023-000277-PEA | Mesa, duración, tres criterios y sobre único con documentación cargados. El lanzador portátil se inicia. La vista del sobre en el simulador sigue sin abrirse. |
| 02 Simplificado | 2 | Anuncio de licitación y pliegos + oferta (M4) | ⛔ | INAP-050-AS-2023-000277-PEA | Convocatoria y pliegos publicados y verificados en público con el PCAP, PPT y anexos III y IV. Queda presentar la oferta con un operador registrado y certificado de pruebas. |
| 02 Simplificado | 3 | Apertura, valoración, propuesta + acto adicional (M5) | ⛔ | INAP-050-AS-2023-000277-PEA | Sesión `INAP-050-AS-M5-20261130` creada para el 30/11/2026 a las 13:00, con cuatro actos en agenda y texto de convocatoria guardado. El intento de envío falló en la conexión con AutoFirma. |
| 02 Simplificado | 4 | Resolución (M6) — **opcional** | ⬜ | | |

## Plazos de presentación de ofertas
| Licitación | Publicación | Fin de plazo | Ofertas presentadas |
|---|---|---|---|
| 01 Abierto | Pendiente | 28/11/2026, 20:00, provisional | 0 |
| 02 Simplificado | 23/11/2026, 19:17 | 28/11/2026, 20:00 | 0 |

Recalcular el plazo del abierto a partir de la fecha efectiva de publicación.

## Pasos que necesitan al usuario
- **Campus INAP.** Entregar el [contrato menor](00-contrato-menor/ENTREGA.md) con el texto y las evidencias que ya están preparados.
- **Operadores económicos.** En la zona Empresas de preproducción, completar el CAPTCHA de alta de una cuenta de formación para el simplificado. Para las dos ofertas del abierto se necesitan dos cuentas de formación. También sirven cuentas ya activas. El plazo de oferta del simplificado termina el 28/11/2026 a las 20:00 en la Plataforma de formación.
- Mesa del módulo 2: la incorporación está autorizada. El alta de presidencia y vocalías exige los identificadores de los usuarios de formación que ocuparán esos cargos.
- **Firma en preproducción.** Facilitar el certificado de pruebas de los tutores por un canal privado o realizar la firma desde un equipo con las utilidades del curso. La primera firma pendiente es la oferta del simplificado. Los [modelos y el detalle del sobre](02-abierto-simplificado/documentos/borrador-oferta.md) están en el repositorio.

## Diario
- 23/11/2026. Contrato menor `INAP-050-CM-2026-01` publicado a las 16:40. Evidencia del órgano de contratación guardada. El usuario confirmó la referencia CNMC 230278 para el abierto.
- 23/11/2026. Descargados los documentos de referencia del abierto y del simplificado. Se perdió el control de la pestaña de formación durante la preparación. Antes de seguir, recuperar la sesión de Organismos y comprobar los miembros de la mesa de contratación.
- 23/11/2026. Verificada y documentada la vista pública del contrato menor. La sesión anónima del entorno funciona. El control de la pestaña autenticada de Chrome sigue sin estar disponible.
- 23/11/2026. Recuperado el acceso de Organismos. Creados los expedientes del abierto y el simplificado. Se verificó que la mesa activa solo tiene al secretario. El control de Chrome se interrumpió en el selector de archivos al intentar adjuntar el PCAP del abierto. La carga, el simulador y la publicación de ambos expedientes siguen pendientes de confirmación.
- 23/11/2026. Recuperado el acceso en el navegador integrado. Enlazados los pliegos oficiales en ambos expedientes y los anexos III y IV del simplificado. Convocatoria y pliegos del simplificado publicados a las 19:17 y 19:18 y verificados sin iniciar sesión. El abierto superó la validación de Plataforma, pero falló la previsualización del DOUE.
- 23/11/2026. Un nuevo intento confirmó la incidencia del DOUE. El formulario de alta de operadores económicos exige CAPTCHA.
- 23/11/2026. Preparado el Anexo III del simplificado con un precio de prueba y el inventario de documentos para el sobre único. Preparados la pregunta y respuesta y los datos de dos ofertas de prueba del abierto, incluida la subsanación prevista. Los borradores quedan pendientes de firma y envío.
- 23/11/2026. Verificada la descarga del lanzador JNLP de la herramienta de simulación en Chrome. No se encontró un lanzador Java Web Start instalado. Guardada la captura del sobre único. Las configuraciones del módulo 3 figuran sin envío en el Campus.
- 23/11/2026. Creada y verificada como secretario la sesión `INAP-050-AS-M5-20261130` del simplificado. Agenda guardada con apertura, valoración, ruegos y preguntas y propuesta de adjudicación. La sesión no está convocada y los cuatro actos figuran como no celebrados.
- 23/11/2026. Se comprobó que la memoria justificativa seguía sin archivo seleccionado. Se guardó y reabrió el borrador de convocatoria del simplificado, con el lugar, el horario y el orden del día. La convocatoria no se ha enviado.
- 23/11/2026. Se intentó enviar y firmar la convocatoria del simplificado. La Plataforma mostró «No se pudo conectar con AutoFirma» y la sesión permaneció en estado «Creada».
- 23/11/2026. La planificación del abierto muestra cinco actos. Se fijó provisionalmente la apertura administrativa el 30/11/2026 y se creó la sesión `INAP-050-AB-M5-ADMIN` a las 11:00. La Plataforma impidió incorporar el acto porque el sobre aún no está publicado.
- 23/11/2026. Verificados al reabrir el abierto la presentación electrónica, la mesa asignada, la duración de 36 meses, la solvencia, los cinco criterios y los documentos de los tres sobres. Capturas de criterios y sobres archivadas. Sigue pendiente la comprobación desde el simulador.
- 23/11/2026. Descargados y comprobados los modelos oficiales de adscripción de medios (IX) y declaración responsable (X) para el sobre único del simplificado. Modelos archivados en el repositorio. La oferta sigue pendiente de cumplimentación con el operador, acreditaciones, firma y envío.
