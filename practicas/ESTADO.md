# Cuadro de mando de las prácticas

Estados: ⬜ pendiente · 🔄 en curso · ✅ listo para entregar · 📤 entregado (lo marca el usuario) · ⛔ bloqueado

| Práctica | Ej. | Descripción | Estado | ID licitación | Notas |
|---|---|---|---|---|---|
| Requisito | — | Órgano de asistencia del módulo 2 (mesa + secretario) | ⛔ | — | Mesa activa. Único miembro asignado: secretario. Presidencia y vocalías necesarias vacantes. |
| Requisito | — | ≥2 operadores económicos ficticios | ⛔ | — | El alta de Empresas exige introducir manualmente los caracteres de un CAPTCHA. No se crearon cuentas. |
| Requisito | — | Certificado de pruebas + AutoFirma + Java en el navegador del agente | ⛔ | — | No se encontró certificado personal vigente con clave privada en el almacén del usuario, AutoFirma en la ruta estándar ni Java en PATH. |
| 00 Contrato menor | 1 | Crear, publicar y verificar (OC y vista pública) | ✅ | INAP-050-CM-2026-01 | Adjudicación visible como órgano de contratación y en el buscador público sin sesión de Organismos. Texto y evidencias en `ENTREGA.md`. |
| 01 Abierto | 1 | Configuración (M3) | 🔄 | INAP-050-AB-230278 | Verificado el guardado de los tres sobres y de los enlaces de PCAP y PPT. Falta ejecutar el simulador Java Web Start. |
| 01 Abierto | 2 | Anuncio de licitación DOUE/BOE, pliegos, memoria (M4) | ⛔ | INAP-050-AB-230278 | Validación de Plataforma sin errores. El servicio DOUE falló al generar la previsualización. La convocatoria no se ha publicado. |
| 01 Abierto | 3 | Pregunta/respuesta + ofertas (M4) | ⬜ | | |
| 01 Abierto | 4 | Sesiones, apertura, subsanación, valoración, propuesta (M5) | ⛔ | INAP-050-AB-230278 | Tras recibir ofertas y vencer el plazo, se requiere completar la mesa y disponer de certificado de pruebas. |
| 01 Abierto | 5 | Requerimiento, adjudicación, firma, formalización (M6) | ⬜ | | |
| 01 Abierto | 6 | Modificación de contrato (M6) | ⬜ | | |
| 02 Simplificado | 1 | Configuración (M3) | 🔄 | INAP-050-AS-2023-000277-PEA | Mesa, duración, tres criterios y sobre único con documentación cargados. Chrome recibió el lanzador JNLP, pero el simulador no se abrió. |
| 02 Simplificado | 2 | Anuncio de licitación y pliegos + oferta (M4) | ⛔ | INAP-050-AS-2023-000277-PEA | Convocatoria y pliegos publicados y verificados en público con el PCAP, PPT y anexos III y IV. Queda presentar la oferta con un operador registrado y certificado de pruebas. |
| 02 Simplificado | 3 | Apertura, valoración, propuesta + acto adicional (M5) | ⛔ | INAP-050-AS-2023-000277-PEA | Tras recibir ofertas y vencer el plazo, se requiere completar la mesa y disponer de certificado de pruebas. |
| 02 Simplificado | 4 | Resolución (M6) — **opcional** | ⬜ | | |

## Plazos de presentación de ofertas
| Licitación | Publicación | Fin de plazo | Ofertas presentadas |
|---|---|---|---|
| 01 Abierto | Pendiente | 28/11/2026, 20:00, provisional | 0 |
| 02 Simplificado | 23/11/2026, 19:17 | 28/11/2026, 20:00 | 0 |

Recalcular el plazo del abierto a partir de la fecha efectiva de publicación.

## Pasos que necesitan al usuario
- Operadores económicos: completar el CAPTCHA de alta de las cuentas de formación o facilitar acceso a cuentas de formación ya activas. La primera oferta debe presentarse antes del 28/11/2026 a las 20:00.
- Mesa del módulo 2: la incorporación está autorizada. El alta de presidencia y vocalías exige los identificadores de los usuarios de formación que ocuparán esos cargos.
- Ofertas, sesiones y firmas que exijan certificado: facilitar el certificado de pruebas y las utilidades requeridas, o realizar esos pasos desde un equipo preparado.

## Diario
- 23/11/2026. Contrato menor `INAP-050-CM-2026-01` publicado a las 16:40. Evidencia del órgano de contratación guardada. El usuario confirmó la referencia CNMC 230278 para el abierto.
- 23/11/2026. Descargados los documentos de referencia del abierto y del simplificado. Se perdió el control de la pestaña de formación durante la preparación. Antes de seguir, recuperar la sesión de Organismos y comprobar los miembros de la mesa de contratación.
- 23/11/2026. Verificada y documentada la vista pública del contrato menor. La sesión anónima del entorno funciona. El control de la pestaña autenticada de Chrome sigue sin estar disponible.
- 23/11/2026. Recuperado el acceso de Organismos. Creados los expedientes del abierto y el simplificado. Se verificó que la mesa activa solo tiene al secretario. El control de Chrome se interrumpió en el selector de archivos al intentar adjuntar el PCAP del abierto. La carga, el simulador y la publicación de ambos expedientes siguen pendientes de confirmación.
- 23/11/2026. Recuperado el acceso en el navegador integrado. Enlazados los pliegos oficiales en ambos expedientes y los anexos III y IV del simplificado. Convocatoria y pliegos del simplificado publicados a las 19:17 y 19:18 y verificados sin iniciar sesión. El abierto superó la validación de Plataforma, pero falló la previsualización del DOUE.
- 23/11/2026. Un nuevo intento confirmó la incidencia del DOUE. El formulario de alta de operadores económicos exige CAPTCHA.
- 23/11/2026. Preparado el Anexo III del simplificado con un precio de prueba y el inventario de documentos para el sobre único. Preparados la pregunta y respuesta y los datos de dos ofertas de prueba del abierto, incluida la subsanación prevista. Los borradores quedan pendientes de firma y envío.
- 23/11/2026. Verificada la descarga del lanzador JNLP de la herramienta de simulación en Chrome. No se encontró un lanzador Java Web Start instalado. Guardada la captura del sobre único. Las configuraciones del módulo 3 figuran sin envío en el Campus.
