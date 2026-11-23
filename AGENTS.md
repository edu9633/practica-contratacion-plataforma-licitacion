# AGENTS.md — Prácticas del curso INAP «La Plataforma de Contratación del Sector Público como herramienta de transparencia»

Este archivo es para el agente que ejecuta las prácticas en el entorno de formación de la Plataforma de Contratación del Sector Público (PLACSP). El agente previsto es GPT-6.2 Sol con razonamiento medio. Léelo entero antes de tocar el navegador y vuelve a él cuando dudes.

---

## 1. Tu papel y sus límites

**Qué haces tú:** realizas en el **entorno de formación** (`https://preprod-contrataciondelestado.es`) todas las prácticas obligatorias, compruebas que han quedado bien y dejas preparada la entrega de cada ejercicio en el repo.

**Qué hace el usuario:** él sube las prácticas al Campus INAP. Tú no entregas nada.

**Prohibido, sin excepción:**
- Entregar, subir o enviar nada en el Campus INAP. Tampoco escribir en los foros ni contactar con tutores. Si hace falta preguntar algo al tutor o en el foro, prepara un **borrador** en `practicas/BORRADORES.md` y avisa al usuario.
- Enviar correos o cualquier comunicación en nombre del usuario fuera del entorno de prácticas.
- Crear, modificar o publicar nada en la Plataforma **real** (`contrataciondelestado.es`). Allí solo puedes **consultar y descargar** pliegos y documentos públicos de la licitación de referencia.
- Usar correos electrónicos reales de empresas para los operadores económicos ficticios (ver §5).
- Escribir en archivos versionados el NIF/DNI del usuario, contraseñas, pasaportes o cuentas bancarias. El repo es **público**. Las credenciales van solo en `credenciales.local.md`, que git ignora.
- Anular, desistir o borrar una licitación, o cambiar los miembros del órgano de asistencia, sin confirmación del usuario.

**Sí puedes hacer sin preguntar,** porque es el contenido de las prácticas y el entorno es ficticio: crear licitaciones, publicar anuncios con envío simulado a DOUE y BOE, crear operadores económicos ficticios, presentar ofertas con ellos, hacer preguntas y responderlas, celebrar sesiones, enviar comunicaciones y requerimientos a los operadores ficticios, adjudicar y formalizar. Antes de publicar, previsualiza siempre.

---

## 2. Fuentes, por orden de prioridad

1. **Enunciados del curso.** El texto está en `enunciados/*.txt` y los PDF originales en `enunciados/pdf/`. Mandan sobre todo lo demás en **qué** hay que hacer.
2. **Material didáctico y guías de ayuda de la PLACSP** en `material-didactico/`. Mandan en **cómo** se hace cada paso en pantalla. Consulta la guía que corresponda **antes** de cada ejercicio; el índice está en `material-didactico/README.md`. Si una guía contradice lo que digo aquí sobre la navegación, sigue la guía.
3. **Pliegos de la licitación de referencia,** descargados de la Plataforma real y guardados en `practicas/<práctica>/documentos/`. De ellos salen los datos que se cargan en la licitación: objeto, CPV, presupuesto, lotes, plazos, solvencia, criterios, sobres, etc.
4. **Instrucciones de acceso al entorno:** `instrucciones/acceso-entorno-practicas.md`.
5. Este archivo.

No inventes datos que deban salir del pliego. Si un dato no aparece en el pliego y la Plataforma lo exige, usa un valor razonable y anótalo como **supuesto** en la entrega.

Si falta el material didáctico (la carpeta solo tiene el README), avisa al usuario y sigue con los enunciados y lo que ves en pantalla, con más verificación.

---

## 3. Acceso al entorno

1. Abre `https://preprod-contrataciondelestado.es`. El navegador pedirá un usuario y una contraseña de **acceso al entorno** (autenticación HTTP básica). Están en `credenciales.local.md` → «Acceso al entorno». Es una protección que solo existe en el entorno de formación.
2. Entra como usuario mediante el icono **Organismos**. El identificador es el NIF del usuario; la contraseña inicial son los dígitos del NIF sin letra seguidos de `%`. Toma los datos de `credenciales.local.md`. También se puede entrar con certificado digital.
3. Si te pide cambiar la contraseña, cámbiala, **anota la nueva en `credenciales.local.md` de inmediato** y avisa al usuario. Si se pierde, solo el tutor puede restablecerla.
4. **Selecciona el contexto** en la ventana de inicio o en la esquina superior derecha:
   - **Órgano de contratación** `OC_INAP_26_AVAN_SEPT_xxx`, donde `xxx` son tres dígitos propios del usuario: configurar, publicar y resolver licitaciones.
   - **Órgano de asistencia** (mesa de contratación), con el usuario **secretario**: crear, convocar y celebrar sesiones.
   Comprueba siempre en qué contexto estás antes de actuar. La mayoría de los «no encuentro el botón» se deben a estar en el contexto equivocado.
5. Los **operadores económicos** entran por la zona de empresas, con sus propias credenciales (ver §5).

---

## 4. Cómo navegar bien por la Plataforma

La Plataforma es una aplicación web antigua basada en formularios con estado de servidor. Para no romper la sesión ni perder datos:

- **No uses el botón «Atrás» del navegador ni recargues** a mitad de un formulario. Navega con los enlaces, pestañas y botones de la propia aplicación («Volver», «Cancelar», migas de pan).
- **Guarda a menudo.** Pulsa el botón de guardar de cada pestaña antes de cambiar de pestaña y comprueba que aparece el mensaje de confirmación. Si sale un mensaje de error o de campos obligatorios, léelo entero y corrígelo antes de seguir.
- **Una sola pestaña del navegador por usuario.** No abras la misma sesión en dos pestañas. Para actuar a la vez como órgano de contratación y como operador económico, usa **perfiles o ventanas privadas distintas**, porque comparten cookies si no.
- **La sesión caduca.** Si te devuelve a la página de inicio o aparece un error genérico, vuelve a entrar, selecciona el contexto y comprueba si lo último se guardó antes de repetirlo. No dupliques licitaciones.
- **Espera las cargas.** Tras pulsar un botón, espera a que la página termine de cargar antes de la siguiente acción. Nunca hagas doble clic en «Publicar», «Enviar» o «Guardar».
- **Las licitaciones se gestionan en su Espacio Virtual de Licitación (EVL).** Se crean desde la pestaña **Licitaciones** → botón **Nuevo**. Dentro del EVL hay pestañas como **Resumen Licitación**, la de configuración de datos y sobres, **PPT**, **PCAP**, **Anexo pliegos** y documentos. Los nombres exactos y el orden están en las guías. Anota el **identificador de la licitación** en cuanto la Plataforma lo asigne.
- **Bloqueo por DOUE.** Al publicar un anuncio con envío al DOUE, la licitación queda **bloqueada hasta 30 minutos** mientras se simula la publicación. **No intentes editarla durante el bloqueo.** Espera, comprueba cada 5 minutos aproximadamente que el anuncio aparece publicado en el perfil de contratante y entonces sigue. Aprovecha la espera para avanzar en otra práctica.
- **Certificado electrónico.** Presentar ofertas como operador económico y firmar el contrato requieren certificado electrónico; algunas firmas pueden requerir también AutoFirma. Si tu navegador no tiene un certificado disponible o salta un componente de firma que no puedes manejar, **para**, deja anotado el paso exacto en `practicas/ESTADO.md` y pide al usuario que lo haga él o que instale el certificado de pruebas que facilitan los tutores. No intentes saltarte la firma.
- **Correos de aviso.** Los avisos al responsable de la licitación, como el de publicación o el de pregunta pendiente, llegan al correo del usuario, que no ves. No esperes a ese correo: comprueba el estado directamente en la Plataforma. Los avisos a los operadores ficticios sí puedes leerlos en maildrop (ver §5).
- **Capturas de pantalla** como evidencia en cada hito (§7). No hagas capturas de la pantalla de inicio de sesión ni de nada donde se vea el NIF o la contraseña. Si aparece el NIF, recorta la captura o no la guardes.

---

## 5. Datos comunes y requisitos previos

Rellena y mantén `practicas/datos-comunes.md` con lo siguiente:

- **Órgano de contratación** (`OC_INAP_26_AVAN_SEPT_xxx`) y nombre del **perfil de contratante**, tal como aparece en la Plataforma.
- **Órgano de asistencia (mesa)** creado en el **módulo 2**: nombre, miembros y usuario secretario. **Es requisito previo** de las prácticas del abierto y del simplificado. Lo primero que haces es comprobar que existe y que tiene secretario y miembros. Si no existe, consulta la guía de órganos de asistencia del material didáctico, créalo y anótalo. Si no sabes cómo, pregunta al usuario.
- **Operadores económicos ficticios:** crea **al menos dos**, mejor tres, para preguntar, presentar ofertas y poder dejar a uno «admitido provisionalmente» para que subsane.
  - Correo: **nunca** un correo real de empresa. Usa direcciones de `maildrop.cc`, por ejemplo `inap26-oe1-<xxx>@maildrop.cc`. Para leer su correo, abre `https://maildrop.cc` y escribe la parte anterior a la arroba en la casilla. Uno de los enunciados propone mailinator.com, que funciona igual; usa uno de los dos de forma coherente.
  - Datos de empresa inventados (razón social, NIF ficticio con formato válido si lo exige el formulario, dirección).
  - Sus credenciales van en `credenciales.local.md`; en `datos-comunes.md` solo el nombre y el correo.
- **Procedimiento de referencia del abierto.** Hay tres versiones del enunciado y cada una propone una licitación real distinta para reproducir (ver §6.2). La elegida consta en `datos-comunes.md`. Si figura como «pendiente de confirmar», pregunta al usuario antes de empezar la práctica 01. Si no contesta, usa la indicada por defecto.

---

## 6. Prácticas a realizar

Plan general: deja hechas en paralelo las configuraciones y convocatorias del abierto y del simplificado, presenta las ofertas y, **cuando venza el plazo de presentación**, celebra las sesiones. Los sobres **no pueden abrirse antes de que venza el plazo**, así que el calendario manda (§6.4).

### 6.0. Contrato menor — `enunciados/00_contrato-menor.txt`
1. Crea un EVL de **contrato menor** desde Licitaciones → Nuevo.
2. Rellena los datos para publicarlo. Puedes reproducir el contrato menor 1791/2025 de la Concejalía de Contratación del Ayuntamiento de Ondara (el enlace está en el enunciado) o cualquier otro contrato menor publicado.
3. Publícalo.
4. **Verifica su visualización** de dos formas: (a) como órgano de contratación y (b) como **usuario no registrado**, en una ventana privada sin iniciar sesión en la Plataforma, buscándolo en la parte pública del entorno de formación.
5. Entrega: nombre del perfil de contratante e identificador de la licitación.

### 6.1. Procedimiento abierto — **obligatorio en todas sus fases** — `enunciados/01_procedimiento-abierto_*.txt`
Descarga primero los pliegos (PCAP, PPT y anexos) de la licitación de referencia en la Plataforma real y guárdalos en `practicas/01-procedimiento-abierto/documentos/`.

| Ej. | Módulo | Qué hacer | Comprobación mínima |
|---|---|---|---|
| 1 | 3 | Crear la licitación de procedimiento **Abierto** con los datos del pliego. Presentación de ofertas «**Electrónica a través de la Plataforma**». Mesa: el órgano de asistencia del módulo 2. Registrar como mínimo **requisitos de participación, criterios de adjudicación y sobres electrónicos** según el pliego. Fecha de presentación de ofertas **futura y próxima**, no la del pliego. | **Simulador** de la herramienta de presentación de ofertas en «Resumen Licitación»: los sobres, documentos y criterios que se piden coinciden con el pliego. Si no coinciden, corregir y volver a simular. |
| 2 | 4 | Ajustar la fecha de fin de presentación: **al menos 4 días** desde la publicación, pero no mucho más (§6.4). **Previsualizar** y publicar el **anuncio de licitación** con envío a **DOUE y BOE**. Esperar al desbloqueo (máx. 30 min). Adjuntar los pliegos y anexos en las pestañas **PPT, PCAP y Anexo pliegos** y publicar el **anuncio de pliegos**. Publicar en la pestaña **Resumen** un documento del tipo **memoria justificativa**. | El anuncio de licitación, los pliegos y la memoria aparecen publicados en el perfil de contratante, también en la vista pública sin iniciar sesión. La licitación está «en plazo». |
| 3 | 4 | Como **operador económico**, hacer una pregunta y, como órgano de contratación, **responderla** para que se publique. Presentar **ofertas** con al menos **dos** operadores propios. Prepara una de ellas con alguna deficiencia en la documentación administrativa para poder pedir subsanación en el ejercicio 4. | La pregunta y la respuesta son visibles en la licitación. Las ofertas constan como presentadas y el operador tiene el justificante. |
| 4 | 5 | Con el usuario **secretario** del órgano de asistencia: **crear y convocar sesiones** y celebrarlas marcando como **presentes** al resto de miembros. Orden de actos: **apertura y calificación administrativa**, con un licitador **admitido provisionalmente** → **subsanación** → apertura del siguiente sobre → valoración → … → **propuesta de adjudicación**. La Plataforma crea sola los actos de apertura y valoración y basta con añadirlos al orden del día; la **propuesta de adjudicación la creas tú**. Generar los **informes**: lista de licitadores, informe de apertura e informe de propuesta de adjudicación. Hacer una **comunicación genérica**: solicitud de aclaración de la oferta técnica o justificación de oferta anormalmente baja. Gestionar el **acta** de al menos una sesión. | Todas las sesiones están celebradas y cerradas, y los informes generados y guardados en `evidencias/`. Hay propuesta de adjudicación a favor de un licitador. |
| 5 | 6 | Como órgano de contratación: **requerimiento de documentación** al propuesto como adjudicatario → configurar y **publicar la adjudicación** y **comunicarla a todas las empresas** → **firma del contrato** en la Plataforma (requiere certificado, §4) → **publicar la formalización** con envío a **DOUE y BOE**, y esperar el desbloqueo (unos 30 min). | La adjudicación y la formalización están publicadas en el perfil. Las comunicaciones constan enviadas y los operadores las reciben en maildrop. |
| 6 | 6 | Publicar una **modificación de contrato**. Se puede marcar el envío al DOUE; esta vez **no bloquea** la licitación. | El anuncio de modificación es visible en el perfil de contratante. |

Cada ejercicio se entrega por separado con el **nombre del perfil de contratante** y el **identificador de la licitación**.

### 6.2. Versiones del enunciado del abierto
Las tres versiones tienen los mismos ejercicios. Solo cambian la licitación de referencia y el servicio de correo sugerido:
- `01_procedimiento-abierto_v-CNMC-230278`: expediente 230278 de la Comisión Nacional de los Mercados y la Competencia (mailinator). Es la versión repetida en los PDF de los módulos 4, 5 y 6 y la que se usa **por defecto**.
- `01_procedimiento-abierto_v-UMurcia-E-CON-2025-34`: expediente E-CON-2025-34/SE/AM de la Universidad de Murcia (maildrop). Es el PDF que venía como módulo 3.
- `01_procedimiento-abierto_v-USevilla-23-45496`: expediente 23/45496 del Rectorado de la Universidad de Sevilla.
Los enlaces a cada licitación real están en el `.txt` de cada versión.

### 6.3. Procedimiento abierto simplificado — **obligatorio hasta la selección de licitadores; la resolución es opcional** — `enunciados/02_abierto-simplificado.txt`
Referencia: expediente **2023/000277-PEA** de la Presidencia de la Diputación Provincial de Sevilla (enlace en el enunciado). Tiene **sobre único**, del tipo «documentación administrativa y criterios cuantificables automáticamente». Descarga sus pliegos en `practicas/02-abierto-simplificado/documentos/`.

| Ej. | Módulo | Qué hacer |
|---|---|---|
| 1 | 3 | Configurar la licitación **Abierto simplificado**, «Electrónica a través de la Plataforma», con la mesa del módulo 2. Sobre único como en el pliego, salvo que el usuario pida dos. Comprobar con el simulador. |
| 2 | 4 | Publicar el **anuncio de licitación** y el **de pliegos**. Presentar al menos una oferta con un operador propio; mejor dos. |
| 3 | 5 | **Sobre único:** acto de apertura de criterios cuantificables automáticamente (art. 159) → valoración → **propuesta de adjudicación**. (Con dos sobres: apertura de juicio de valor (art. 159) → valoración → apertura de cuantificables (art. 159) → valoración → propuesta.) Hacer además **algún acto distinto** de los habituales: ruegos y preguntas, comunicación genérica o aprobación del acta. |
| 4 (opcional) | 6 | Requerimiento de documentación → publicar la adjudicación y comunicarla → publicar la formalización. Hazlo solo si el usuario lo pide o si sobra tiempo una vez cerrado todo lo obligatorio. |

La entrega de cada ejercicio lleva el **nombre del órgano de contratación** y el **identificador de la licitación**.

### 6.4. Calendario y plazos
- Fija el fin de presentación de ofertas en **4 o 5 días naturales** tras la publicación prevista. No pongas mucho más, porque los sobres no se abren hasta que vence el plazo.
- Antes de que venza el plazo, deja hechas las preguntas y respuestas y todas las ofertas. Después del vencimiento ya no se pueden presentar.
- Anota en `practicas/ESTADO.md` la fecha y hora de fin de plazo de cada licitación y lo que queda pendiente para después.
- Si el plazo ya venció sin ofertas suficientes, no improvises: avisa al usuario. Puede hacer falta ampliar el plazo, si la Plataforma lo permite, o rehacer la licitación.

---

## 7. Verificación: confirmar que está bien hecho

Un ejercicio **no está terminado** hasta pasar esta comprobación. Hazla siempre y deja constancia:

1. **Contraste con el enunciado:** recorre cada punto del ejercicio y marca la casilla correspondiente en `practicas/<práctica>/ENTREGA.md`.
2. **Contraste con el pliego:** confirma que objeto, CPV, presupuesto, valor estimado, lotes, duración, solvencia, criterios con sus ponderaciones y sobres coinciden con el pliego. Anota cualquier diferencia o supuesto.
3. **Comprobación en la Plataforma:** el **estado** de la licitación es el esperado y los anuncios y documentos aparecen como **publicados**.
4. **Vista pública:** en una ventana privada, sin sesión en la Plataforma (solo con la autenticación del entorno), busca la licitación y confirma que se ve lo publicado.
5. **Evidencias:** guarda capturas en `practicas/<práctica>/evidencias/` con el nombre `ejNN_<paso>_<AAAAMMDD-HHMM>.png`, por ejemplo `ej02_anuncio-publicado_20261124-1015.png`. Descarga también los informes y actas que genere la Plataforma.
6. **Reautoevaluación:** al final, relee el ejercicio como si fueras el tutor y pregúntate si falta algo de lo que pide literalmente el enunciado. Si falta, hazlo antes de marcarlo como listo.

Si algo no ha salido bien y no puedes corregirlo, por ejemplo una firma que no puedes hacer o un error persistente de la Plataforma, márcalo como **BLOQUEADO** con la explicación. No lo des por bueno.

---

## 8. Registro y entrega

- `practicas/ESTADO.md` es el **cuadro de mando**: estado de cada ejercicio (pendiente / en curso / listo para entregar / bloqueado), identificadores, fechas de fin de plazo y próximos pasos. Actualízalo al terminar cada paso.
- `practicas/<práctica>/ENTREGA.md` recoge, por ejercicio, la lista de comprobación, los supuestos y un bloque **«Texto para el Campus»** listo para que el usuario lo copie, con el nombre del perfil de contratante o del órgano de contratación y el identificador de la licitación.
- Al terminar cada ejercicio, avisa al usuario con un resumen breve: qué está listo para entregar, con el identificador, y qué queda pendiente o bloqueado.
- Haz commit de los avances: `ENTREGA.md`, `ESTADO.md`, `datos-comunes.md`, evidencias y pliegos. Antes de cada commit comprueba con `git status` que **no** entra `credenciales.local.md` y que ningún archivo contiene el NIF ni contraseñas.

---

## 9. Mapa del repo

```
AGENTS.md                      ← este archivo
README.md                      ← descripción breve para humanos
credenciales.local.example.md  ← plantilla; cópiala a credenciales.local.md (ignorado por git)
instrucciones/                 ← acceso al entorno de prácticas (original .mhtml y versión .md)
enunciados/                    ← enunciados en .txt; los originales en pdf/
material-didactico/            ← guías de la PLACSP y temario del curso (las aporta el usuario)
practicas/
  ESTADO.md                    ← cuadro de mando
  datos-comunes.md             ← órgano de contratación, mesa, operadores ficticios, versión elegida
  BORRADORES.md                ← borradores de consultas al tutor o al foro (no se envían)
  00-contrato-menor/           ← ENTREGA.md, documentos/, evidencias/
  01-procedimiento-abierto/
  02-abierto-simplificado/
```
