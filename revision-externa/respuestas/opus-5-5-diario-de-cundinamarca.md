# Respuesta — Claude Opus 5.5 sobre Diario de Cundinamarca

| | |
|---|---|
| **Modelo** | Claude Opus 5.5 |
| **Versión exacta** | `claude-opus-5-5` |
| **Fecha de la consulta** | 2026-10-10 |
| **Quién la hizo** | Claude Code, a petición del responsable editorial (ciclo 2, fase 2, tanda 6; revisor de la misma casa que el autor de las fichas, ver DECISIONES.md 2026-10-07) |
| **¿Tuvo acceso a la red?** | sí |

> **Se pega LITERAL lo que devolvió el modelo, sin editar ni resumir.** Si se
> recorta, se pierde justo lo que pueda incomodar. Los comentarios nuestros van
> al final, en la sección de resolución, claramente separados.
>
> **Edición:** retirados enlaces que pueden mostrar documentos de identidad (PROTOCOLO, Datos personales, 2026-10-10).

---

## RESPUESTA LITERAL

```
DECLARACIÓN PREVIA DE CONFLICTO
Soy Claude Opus 5.5 (id de modelo: claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Mi acuerdo con ella no debe contarse como validación independiente. Por eso he trabajado casi solo con fuentes que la ficha no usa: el registro mercantil (RUES abierto), SECOP I y II, y el HTML crudo de páginas del medio que la ficha no cita (/nuestro-diario, sitemaps y una pieza). No he leído ningún otro archivo del repositorio de DobleFoco. Fecha de toda la revisión: 2026-10-10.

MÉTODO Y DÓNDE BUSQUÉ
- robots.txt de www.diariodecundinamarca.com (descargado el 2026-10-10). No excluye a ClaudeBot, Claude-Web ni anthropic-ai: "User-agent: * / Allow: /". Solo bloquea a PetalBot. Dice además "# Auto generated, go to SEO Tools > Robots.txt Editor to change this" y el sitemap trae generatedBy="WIX". La web está hecha con Wix, no con Blogger.
- Descargas en crudo con curl -sL --ssl-no-revoke y User-Agent de navegador, guardadas en t6\cundinamarca-dl: robots.txt, /blog-feed.xml, portada, /sitemap.xml, /pages-sitemap.xml, /blog-posts-sitemap.xml, /blog-categories-sitemap.xml, /nuestro-diario y la pieza /post/pavimentación-en-la-comuna-2-... Extraje el texto con perl a partir del HTML crudo, no de un resumen.
- RUES abierto (datos.gov.co, c82u-588k):
  · upper(razon_social) like '%DIARIO DE CUNDINAMARCA%'. No conocía el NIT y lo encontré así.
  · nit='901444929'.
  · upper(razon_social) like '%ANZOLA SOLANO%'.
- SECOP II (jbjy-vk9h), documento_proveedor con igualdad exacta y sin dígito de verificación, para el NIT de la sociedad y para el documento del representante legal que da el RUES. El número de ese documento no se reproduce aquí (Ley 1581).
- SECOP I (f789-7hwg), identificacion_del_contratista con igualdad exacta, para los mismos dos identificadores.
- Robots.txt de www.alcaldiasoacha.gov.co (SharePoint) para intentar cotejar los boletines. No llegué a cotejar ningún texto.
- Buscador web: una sola consulta, con la frase literal de un titular para ver si coincidía con un boletín oficial. No dio resultados útiles. El buscador estuvo disponible y lo usé con moderación.
- Lo que no hice: no leí certificados de existencia y representación de pago (el RUES abierto no da accionistas), no consulté redes sociales del medio ni de su director y no abrí los expedientes SECOP en community.secop.gov.co (solo los metadatos del conjunto de datos).

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré venta, fusión ni escisión. Sí hay un cambio de registro dentro de los 12 meses. La sociedad MCA DIARIO DE CUNDINAMARCA SAS (NIT 901444929, matrícula 3323337) aparece dos veces en el RUES abierto:
  · Cámara de BOGOTA: "estado_matricula":"CANCELADA", "fecha_cancelacion":"20260815".
  · Cámara de SOACHA: "estado_matricula":"ACTIVA", "fecha_matricula":"20210114", "fecha_renovacion":"20260414", "ultimo_ano_renovado":"2026", "fecha_actualizacion":"2026/08/21".
  Interpreto, sin haberlo comprobado, que la matrícula pasó de la Cámara de Bogotá a la de Soacha y que la sociedad no se liquidó: la matrícula es la misma y en Soacha sigue activa.
  Fuente: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (consulta del 2026-10-10).

- La persona que la ficha nombra como titular o director, ¿sigue viva y en el cargo?
  La ficha no nombra a nadie, así que no hay nadie que comprobar. Sin embargo, la web del medio sí nombra director (ver objeción 1). Sobre esa persona hay hechos de este año que indican actividad: el 2026-08-12 firmó un contrato con el Municipio de Soacha que figura "En ejecución" hasta el 2026-12-13 (SECOP II, consulta del 2026-10-10). No encontré ningún indicio de fallecimiento. Comprobación hecha el 2026-10-10.

- ¿Quién dirige hoy la redacción?
  · Según la propia web, en /nuestro-diario, HTML crudo descargado el 2026-10-10: "MICHAEL ANZOLA SOLANO / Director". Aparece también un fotógrafo, Carlos Andrés Vásquez.
  · Según el RUES, el representante legal de la sociedad es "ANZOLA SOLANO MICHEL". Ese dato sale del registro de la Cámara de Bogotá, actualizado el 2026-08-15. El registro de Soacha no trae campos de representante legal.
  · Que el «Michael» de la web y el «Michel» del RUES sean la misma persona es una inferencia fuerte, pero no está probada documentalmente: coinciden los dos apellidos, el municipio y el nombre de la sociedad, y difiere la grafía del nombre.
  · En cambio, que el representante legal del RUES y el contratista «Michel Anzola Solano» de SECOP II son la misma persona sí está probado: el número de documento es idéntico en los dos registros.

- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que la ficha cita?
  Sí. La ficha no cita ninguna fuente de propiedad. El RUES abierto tiene la sociedad renovada el 2026-04-14 y actualizada el 2026-08-21.

## OBJECIONES

OBJECIÓN 1 — «Ni sociedad, ni NIT, ni propietario, ni director, ni editor. Su web no declara equipo ni contacto identificable.»
- QUÉ: la ficha afirma que no hay nada de nivel 1 y que la web no identifica a nadie.
- POR QUÉ: las dos cosas son falsas hoy, y lo más probable es que ya lo fueran el 2026-08-09 (ver más abajo).
  a) La web sí declara equipo y contacto. En /nuestro-diario se lee, literal: "MICHAEL ANZOLA SOLANO / Director / Profesional en Comunicación social y periodismo, 100% soachuno ... lo han llevado a crear Diario de Cundinamarca". En el pie de todas las páginas figura un correo institucional del dominio: "[correo omitido]". El sitio también publica un número de teléfono que no reproduzco porque podría ser personal.
  b) Sí hay sociedad y NIT. En el RUES: "razon_social":"MCA DIARIO DE CUNDINAMARCA SAS", "nit":"901444929", "camara_comercio":"SOACHA", "estado_matricula":"ACTIVA", "organizacion_juridica":"SOCIEDADES POR ACCIONES SIMPLIFICADAS SAS", "cod_ciiu_act_econ_pri":"9001". La fecha de matrícula (14-01-2021) cuadra con el pie de la web: "©2021 para Diario de Cundinamarca".
  c) Sí hay representante legal. En el RUES (registro de Bogotá, 2026-08-15): "representante_legal":"ANZOLA SOLANO MICHEL".
  d) Lo que sigue sin conocerse son los accionistas. Una SAS no los publica en el RUES abierto y no encontré composición accionaria publicada. A qué persona natural llega la propiedad no está documentado. Que el representante legal sea también el dueño es solo una inferencia.
  Sobre si la ficha pudo verlo en su momento: la página /nuestro-diario tiene lastmod 2026-04-24 en pages-sitemap.xml, anterior a la ficha. Es una inferencia: lastmod no prueba qué contenido había ese día.
  Aviso de homonimia: en el RUES existe otra entidad, "DIARIO DE CUNDINAMARCA E U - EN LIQUIDACION" (Cámara de Bogotá, matriculada en 2004, último año renovado 2007). No le encontré ninguna relación con el medio actual y no debe confundirse con él.
- FUENTES Y FECHAS:
  https://www.diariodecundinamarca.com/nuestro-diario (descargada el 2026-10-10).
  [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (consulta del 2026-10-10; registros actualizados el 2026-08-15 y el 2026-08-21).
- NIVEL: propiedad (parcial: hay sociedad y representante legal, pero no accionistas) y declaración del propio medio.

OBJECIÓN 2 — Conflicto de interés no declarado: el director y representante legal es contratista de comunicaciones de la Alcaldía de Soacha, y el medio publica su contenido con formato de boletín
- QUÉ: la ficha no menciona ninguna dependencia económica ni institucional. Aunque no proponga número, el expediente queda incompleto en lo que más pesa para decidir si se da de alta.
- POR QUÉ: SECOP II, consulta con documento_proveedor igual al documento del representante legal que da el RUES. Proveedor: "Michel Anzola Solano". Contratos de los últimos 12 meses o vigentes:
  · MUNICIPIO DE SOACHA, contrato 3030-2026 (CO1.PCCNTR.9800321). Firmado el 2026-08-12; del 2026-08-14 al 2026-12-13; $20.600.000; estado "En ejecución". Objeto: "PRESTACION DE SERVICIOS PROFESIONALES PARA LA ORGANIZACION; EJECUCION Y SEGUIMIENTO DEL PLAN DE DIFUSION DE LA ALCALDIA DE SOACHA.SG_174". [enlace retirado: puede mostrar documentos de identidad; ver la resolución]
  · MUNICIPIO DE SOACHA, contrato 0880-2026 (CO1.PCCNTR.8825418). Firmado el 2026-01-13; del 2026-01-14 al 2026-07-13; $30.900.000; mismo objeto (SG_72). noticeUID=CO1.NTC.9455065
  · MUNICIPIO DE SOACHA, contrato 1905-2025 (CO1.PCCNTR.8082266). Del 2025-07-23 al 2025-12-31; $27.500.000; mismo objeto (SG_130). noticeUID=CO1.NTC.8433480
  · INRAVISIÓN / RTVC (sistema de medios públicos nacional), contrato RTVC-CPS-227-2026. Del 2026-01-22 al 2026-07-21; $36.829.800. Objeto: "actividades de periodista digital; en la construcción y edición de contenidos para las plataformas digitales de RTVC". noticeUID=CO1.NTC.9653942
  · Antecedentes con el mismo objeto de difusión para la Alcaldía de Soacha: 0322-2024, 2299-2024 y 0733-2025. Con RTVC: RTVC-CPS-1517-2025. Con la Secretaría General de Cundinamarca: 2022 y 2023. Son historia y solo sirven para mostrar que la relación es continua, sin interrupciones desde febrero de 2024.
  Conducta del medio en los mismos 12 meses: de las 19 piezas con lastmod igual o posterior al 2025-10-10 en blog-posts-sitemap.xml, 16, todas entre el 2025-12-09 y el 2026-04-12, son anuncios de logros de la Alcaldía de Soacha. Ninguna es crítica. Usan la marca de gobierno de la administración y la entradilla con lugar y fecha propia de un boletín de prensa. Ejemplos literales del feed:
  · "El Gobierno de la ciudad, liderado por el alcalde Julián Sánchez “Perico”, entrega resultados en infraestructura..." (12-04-2026)
  · "El Gobierno de la Ciudad, bajo el liderazgo del alcalde Julián Sánchez Perico, realizó..." (31-01-2026)
  · "¡Soacha vuelve a brillar!" (27-03-2026)
  · "Soacha supera metas de recaudo: un resultado histórico..." (09-12-2025)
  En el HTML crudo de la pieza del 12-04-2026, la firma es "Diario de Cundinamarca". No hay ninguna marca de contenido institucional, pagado ni patrocinado: busqué "prensa", "publirreportaje", "patrocinado" y "contenido pagado" sin resultados. La cabecera del sitio dice "Independencia informativa".
  Hecho frente a inferencia:
  · Es un hecho que la misma persona figura como director en la web, como representante legal en el RUES y como contratista del «plan de difusión de la Alcaldía de Soacha» en SECOP II.
  · Es un hecho que el medio publicó contenido favorable a esa alcaldía, con formato de boletín y sin marcarlo.
  · Es inferencia, no probada, que esos textos sean boletines de la Alcaldía reproducidos o que formen parte de lo que se entrega en el contrato. No pude cotejarlos con la web de la Alcaldía, que es un SharePoint sin buscador accesible, y una búsqueda web por frase literal no devolvió el original.
  · La sociedad MCA Diario de Cundinamarca SAS también tuvo contratos de pauta en SECOP I: Empresa de Licores de Cundinamarca (2021), Agencia Inmobiliaria de Cundinamarca (2021) y Personería de Soacha (2021 y 2022). Son historia. Su único valor es mostrar que el modelo de ingresos del medio pasa por la pauta pública. En SECOP II no hay contratos a nombre de la sociedad.
- NIVEL: propiedad o control (vínculo económico de quien dirige el medio) y conducta observable. Es exactamente el tipo de conflicto que el envío pide buscar, igual que el caso de Diario La Libertad.
- Advertencia sobre el eje: esto no da un valor izquierda-derecha. Es alineamiento con un gobierno municipal concreto y, según la regla del polo fijo, a favor o en contra del gobierno de turno no es una posición en el eje. Su consecuencia es otra: el medio no es una voz independiente de Soacha, y si alguna vez entra en el catálogo, la vinculación tiene que declararse en primer plano.

OBJECIÓN 3 — «El feed lleva 437 horas parado... una ruta de Blogger», y el encuadre del medio como departamental
- QUÉ:
  a) Que el feed sea de Blogger.
  b) Que la parada sea de 18 días: así se lee en la ficha, cuando el problema es un volumen casi nulo desde 2024.
  c) Que el medio sea una voz departamental y que la búsqueda de prensa municipal de Soacha esté «por hacer».
- POR QUÉ:
  a) La web y el feed son de Wix, no de Blogger. Lo muestran el sitemap (generatedBy="WIX"), el robots.txt ("SEO Tools > Robots.txt Editor") y las imágenes, servidas desde static.wixstatic.com. En el feed, el generator es "RSS for Node". Es un error menor que no cambia nada, pero muestra que la ficha no miró el HTML crudo.
  b) La parada continúa hoy. La última entrada del feed es del Wed, 22 Jul 2026 13:28:33 GMT, aunque el canal tiene <lastBuildDate>Thu, 08 Oct 2026 20:39:10 GMT</lastBuildDate>, que solo indica que el feed se regenera, no que haya contenido nuevo. Son 80 días sin publicar a 2026-10-10. La cifra de la ficha (437 h ≈ 18 días desde el 22-07) era correcta para su fecha. Pero el dato que pesa es el volumen. Recuento de lastmod en blog-posts-sitemap.xml, 5.893 URL en total: 2021: 1.897; 2022: 1.927; 2023: 1.379; 2024: 180; 2025: 50; 2026: 12. Aviso: lastmod es fecha de modificación, no de publicación, así que esto es una aproximación. Entre el 2026-04-12 y hoy hay 3 piezas: una renuncia de un concejal de Soacha y dos elogios del gerente de Canal Trece. No encontré ningún contenido sobre Soacha posterior al cambio de gobierno del 07-08-2026. La conducta medida del envío lo confirma: 0 artículos en la ventana del 2026-08-31 al 2026-10-10.
  c) El medio es de Soacha, no de Cundinamarca. El feed dice: "Independencia informativa originada en la ciudad del 'Dios Varón', con la actualidad de Soacha, Cundinamarca, Bogotá y Colombia". La sociedad está matriculada en la Cámara de Comercio de Soacha. La salida 2 de la ficha («buscar prensa municipal de Soacha») ya la tenía delante. Lo que se encontró al buscar es un medio municipal de Soacha cuyo director trabaja en la difusión de la Alcaldía.
- FUENTES: https://www.diariodecundinamarca.com/blog-feed.xml, /sitemap.xml, /blog-posts-sitemap.xml y /robots.txt, todas descargadas el 2026-10-10.
- NIVEL: conducta observable y declaración del propio medio.

OBJECIÓN 4 — La razón de «no dar de alta» está incompleta
- QUÉ: la ficha recomienda no darlo de alta porque «no hay nivel 1» y «no aporta cobertura».
- POR QUÉ: la primera razón ya no se sostiene (objeción 1). La recomendación sigue en pie, pero por motivos distintos y más fuertes:
  · El medio está prácticamente inactivo: 12 URL en 2026 y ninguna desde el 22-07-2026.
  · Su director y representante legal tiene hoy un contrato vigente de difusión con la Alcaldía de Soacha.
  · En los últimos 12 meses su contenido sobre Soacha ha sido el de esa alcaldía.
  Mi propuesta, que es de procedimiento y no una opinión sobre el número: reescribir el expediente como «descartado: inactivo y con dependencia institucional no declarada», con las fuentes de las objeciones 1 y 2. No dejarlo como «sin nivel 1». La condición de reapertura «que vuelva a publicar y diga quién lo edita» ya se cumple a medias, porque el medio sí dice quién lo edita. Si volviera a publicar, la reapertura tendría que exigir además que se aclare o termine la relación contractual con la Alcaldía.
- FUENTES: las de las objeciones 1 a 3.
- NIVEL: propiedad o control y conducta observable.

## LO QUE NO PUDE VERIFICAR

- Los accionistas de MCA Diario de Cundinamarca SAS. El RUES abierto no los da. Haría falta el certificado de existencia y representación de la Cámara de Comercio de Soacha, que es de pago, y no lo consulté.
- Si el representante legal sigue siéndolo. El dato procede del registro de Bogotá, cancelado el 2026-08-15. El registro activo de Soacha no trae campos de representante legal.
- Que el traslado de Bogotá a Soacha sea un traslado de jurisdicción y no otra cosa. Es una inferencia a partir de la misma matrícula y el mismo NIT. No consulté actos inscritos.
- Que «Michael Anzola Solano» (web) y «Michel Anzola Solano» (RUES y SECOP) sean la misma persona. No está probado documentalmente; ver Nivel 1.
- Que las 16 piezas favorables a la Alcaldía sean boletines oficiales reproducidos o entregables del contrato. Intenté cotejarlas con alcaldiasoacha.gov.co (SharePoint, solo leí su robots.txt) y con una búsqueda web por frase literal, sin resultado. Haría falta abrir los expedientes SECOP (informes de supervisión y obligaciones contractuales) en community.secop.gov.co, cosa que no hice.
- El significado exacto del código CIIU 9001 de la sociedad. Creo que corresponde a «Creación literaria» en la adaptación colombiana CIIU Rev. 4 A.C., pero no lo comprobé en una fuente primaria.
- La comparación con «Sucre Noticias» que hace la ficha. No pude verla porque no tengo acceso al repositorio.
- Si hay contratos de la sociedad o del director con Canal Trece / Teveandina, dado que las dos últimas piezas elogian a su gerente. En SECOP I y II, por los dos identificadores, no aparece ninguno. No busqué por otros conductos.

## LO QUE FALTA

- La sociedad, su NIT y su representante legal tomado del RUES, con la fecha de la consulta (objeción 1).
- La consulta de contratación pública obligatoria del protocolo (SECOP I y II), por el NIT de la sociedad y por quien la dirige. Es la que destapa el conflicto de la objeción 2.
- Una referencia a la página /nuestro-diario del medio.
- El dato de volumen histórico (sitemap) en lugar de una sola cifra de horas sin publicar.
- Situar el medio como municipal de Soacha. Esto afecta a la discusión sobre la vista departamental: la prensa «propia» de Soacha que se encontró depende de la Alcaldía.
- Si se quiere cerrar del todo la propiedad: el certificado de existencia y representación de la Cámara de Comercio de Soacha de 2026.

## EVIDENCIA QUE NO MUEVE EL NÚMERO

(Aquí no hay número que mover, porque el valor propuesto es «ninguno». Esta evidencia tampoco justifica proponer uno.)
- En los últimos 12 meses no encontré ningún endoso electoral, editorial ni pieza de opinión de la casa. La categoría /noticias/categories/opinión tiene lastmod 2024-06-24 en blog-categories-sitemap.xml (descargado el 2026-10-10). Solo inspeccioné el sitemap, no la categoría pieza por pieza.
- Las piezas nacionales más recientes del sitemap («Falleció el senador Miguel Uribe Turbay...» y «Procuraduría pide revocar condena contra Álvaro Uribe...», ambas con lastmod de 2025-08) caen fuera de la ventana de 12 meses y no las leí. No las uso.
- No encontré piezas de después del 07-08-2026, ni favorables ni críticas, sobre ningún gobierno: ni el nacional entrante, ni el saliente, ni la Alcaldía. No hay asimetría medible a través del cambio de gobierno porque el medio no publicó nada después de ese cambio.
- Que el director haya sido contratista a la vez de RTVC (medios públicos del Gobierno nacional) y de la Alcaldía de Soacha no indica nada sobre el eje izquierda-derecha. Lo registro porque es del presente (2025-2026) y es citable, no porque mueva nada.
- El robots.txt no bloquea a ningún rastreador de IA y el sitio responde 200. Que el sitio funcione técnicamente no se discute: lo que lo descarta es la falta de contenido.

## SIN OBJECIÓN

No procede: hay cuatro objeciones.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** El revisor no copió cédulas, teléfonos ni direcciones particulares de personas naturales. Se comprobó:
- el número de documento del representante legal no aparece en el texto (búsqueda literal del número, 0 apariciones);
- las cifras largas que contiene son el NIT de la sociedad, su matrícula mercantil, cuantías, fechas y referencias de contrato;
- el correo `[correo omitido]` es el contacto que el medio publica como empresa, y la regla no lo cubre;
- el teléfono del pie del sitio no se reproduce, ni en la respuesta ni aquí.

Esta resolución tampoco escribe ninguno de esos datos.

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada:
  - www.diariodecundinamarca.com: «User-agent: * / Allow: / / Disallow: *?lightbox=», bloquea solo a PetalBot y termina con «# Auto generated, go to SEO Tools > Robots.txt Editor to change this». Nada sobre ClaudeBot, Claude-Web ni anthropic-ai.
  - datos.gov.co: `Crawl-delay: 1` y exclusiones de `/browse`; no se usó ninguna ruta excluida.
  - No se tocaron eltiempo.com, cambiocolombia.com ni lasillavacia.com.
- **Sitio**, descargado en crudo el 2026-10-10 con `curl -sL --ssl-no-revoke -A "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/126.0 Safari/537.36"`:
  - `/blog-feed.xml`, `/sitemap.xml`, `/pages-sitemap.xml`, `/blog-posts-sitemap.xml`, `/blog-categories-sitemap.xml`, `/nuestro-diario` y la portada: todo 200;
  - **las 19 piezas** del feed con fecha dentro de los 12 meses (2025-10-10 → 2026-10-10), una a una: todas 200. El texto se extrajo del HTML crudo, quitando etiquetas.
- **Registros**, en datos.gov.co:
  - RUES (`c82u-588k`): `nit='901444929'`; `upper(razon_social) like '%DIARIO DE CUNDINAMARCA%'`; `upper(razon_social) like '%ANZOLA SOLANO%'`; y, para entender el doble registro, el recuento de matrículas de la Cámara de Soacha (`codigo_camara='58'`) y de las canceladas en Bogotá el 2026-08-15, con una muestra de 8 de estas buscadas en Soacha.
  - SECOP II (`jbjy-vk9h`): `documento_proveedor` con **igualdad exacta**, sin dígito de verificación, por el NIT `901444929` y por el documento del representante legal que da el RUES; y `upper(proveedor_adjudicado) like '%ANZOLA SOLANO%'` para descartar homónimos. La entidad de dos contratos se identificó por `nit_entidad`.
  - SECOP I (`f789-7hwg`): `identificacion_del_contratista` con **igualdad exacta** por los mismos dos identificadores, y `upper(nom_razon_social_contratista) like '%ANZOLA SOLANO%'`.
  - El número de documento se leyó del archivo descargado y se pasó a las consultas sin imprimirlo. No se escribe en ningún sitio.
- **Otros intentos:**
  - la Wayback Machine (para saber si `/nuestro-diario` existía el 2026-08-09) respondió «Temporarily Offline»;
  - una búsqueda web con la frase literal de la pieza del 12-04-2026 («Secretaría de Infraestructura informa la culminación de las obras de pavimentación en los tramos 13 y 14 de la comuna 2») no devolvió el original: solo boletines de otras alcaldías. Igual que al revisor.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | Sí hay nivel 1: sociedad, NIT, representante legal, director declarado y contacto | sí | sí | **Aceptada, y reforzada.** Lo que el revisor dejó abierto se cierra: «Michael» (web) y «Michel» (RUES) son la misma persona, porque SECOP I registra las dos grafías con el mismo documento que el RUES. El doble registro Bogotá-Soacha es el paso masivo a la nueva Cámara de Soacha, no un cambio de dueño. Se rechaza la inferencia por `lastmod` (es la misma fecha para las cuatro páginas del sitio) |
| 2 | Conflicto no declarado: el director y representante legal es contratista del plan de difusión de la Alcaldía de Soacha, y el medio publica contenido de esa alcaldía con formato de boletín | sí | sí | **Aceptada en los hechos, con dos correcciones.** Los 12 contratos son a título personal (cédula), no de la sociedad. Recuento: 16 de 19, exacto. Pero la relación con la Alcaldía **no es «sin interrupciones»** (hay tres huecos de 2 a 5 semanas), la «entradilla con lugar y fecha» está en 6 de las 16, no en todas, y una de las 16 cae en un hueco entre contratos. Que las piezas sean boletines reproducidos o entregables del contrato **no entra como hecho** |
| 3 | Wix y no Blogger; la parada sigue (80 días) y el problema es el volumen; el medio es municipal de Soacha | sí | sí | **Aceptada, con una corrección.** Los 0 artículos de la conducta medida **no confirman nada**: el medio no está en el catálogo y no se ingiere. Lo confirma el feed, no el corpus. Omite además los 448 URL de 2020 en el recuento por año |
| 4 | La razón de no darlo de alta está incompleta | sí | sí | **Aceptada en el fondo; parcial en la redacción.** «Dependencia institucional» del medio no consta: consta el contrato de su director y el contenido. Se propone otra fórmula (ver la propuesta) |

### Lo verificado, objeción por objeción

**1 · Nivel 1.**
- **`/nuestro-diario`** (HTML crudo, 2026-10-10), literal: «MICHAEL ANZOLA SOLANO Director Profesional en Comunicación social y periodismo, 100% soachuno […] Su deseo de contribuir al desarrollo de la ciudad del 'Dios Varón' lo han llevado a crear Diario de Cundinamarca». Aparecen también «CARLOS ANDRÉS VÁSQUEZ Fotógrafo» y un tercer miembro con el texto de relleno de la plantilla de Wix («M. LOPEZ Posición/Rol Esta es tu descripción del Miembro del equipo…»), que el revisor no menciona.
- **Pie**, en la portada y en todas las piezas: «[correo omitido]», un teléfono (no se reproduce), «Soacha, Cundinamarca» y «©2021 para Diario de Cundinamarca. Todos los derechos reservados». El menú de cabecera de **todas** las páginas enlaza «Nuestro diario».
- **RUES** (`nit=901444929`, 2026-10-10), dos filas con la misma matrícula 3323337:
  - Cámara de SOACHA: «MCA DIARIO DE CUNDINAMARCA SAS», «ACTIVA», matrícula 20210114, renovación 20260414, último año renovado 2026, CIIU 9001, `fecha_actualizacion` 2026/08/21. Sin campos de representante legal.
  - Cámara de BOGOTA: la misma sociedad, «CANCELADA», `fecha_cancelacion` 20260815, `representante_legal` «ANZOLA SOLANO MICHEL», `fecha_actualizacion` 2026/08/15.
  - Todo coincide con el revisor.
- **El doble registro, más allá de lo que dice el revisor.** La Cámara de Comercio de Soacha (código 58) tiene **29.805 matrículas** en el RUES abierto, todas actualizadas entre el 2026-04-30 y el 2026-10-02. En Bogotá se cancelaron **7.561 matrículas el mismo día, 2026-08-15**. De una muestra de 8 de esas cancelaciones, **7 aparecen activas en Soacha con la misma matrícula**. Es un traspaso masivo de expedientes de Bogotá a la nueva cámara de Soacha, no un acto de la sociedad. El acto jurídico no se consultó, así que «traslado de jurisdicción» sigue siendo la lectura, pero ya no es una conjetura sobre un caso aislado. **No hay cambio de dueño ni liquidación.**
- **La identidad Michael / Michel, que el revisor dejó como no probada, queda probada por documento:**
  - SECOP I tiene dos contratos con la Alcaldía de Soacha en 2019 con el **mismo documento** que el representante legal del RUES: el 783-2019, a nombre de «MICHEL ANZOLA SOLANO», y el **1792-2019, a nombre de «MICHAEL ANZOLA SOLANO»**.
  - Por nombre, SECOP II solo tiene un «Michel Anzola Solano» (10 filas, todas con ese documento). SECOP I tiene a «MICHEL» y «MICHAEL», ambos con ese documento. El RUES solo tiene otra persona con esos apellidos, con otro nombre de pila y otro documento.
  - Conclusión: el «Michael Anzola Solano» que el medio declara director es el representante legal de la sociedad y el contratista de SECOP. Lo que une la web con los registros es el nombre completo exacto, que en SECOP I está ligado a ese documento, más el municipio y la razón social. **Entra como hecho.**
- **Homónimo:** «DIARIO DE CUNDINAMARCA E U - EN LIQUIDACION», Cámara de Bogotá, matrícula 1406297, del 2004-08-20, último año renovado 2007, empresa unipersonal, sin NIT en la fila. Sin relación documentada con el medio. Coincide con el revisor.
- **Lo que no se rechaza pero no prueba nada:** el revisor usa el `lastmod` 2026-04-24 de `/nuestro-diario` como indicio de que la página existía al hacerse la ficha. En `pages-sitemap.xml`, **las cuatro páginas** (portada, `/nuestro-diario`, `/covid19`, `/ultimasnoticias`) tienen ese mismo `lastmod`: es una fecha del sitio entero, no de la página. El indicio más fuerte es otro: el enlace «Nuestro diario» está en el menú de todas las páginas, y el contenido (©2021, la plantilla sin rellenar) parece antiguo. **Que la ficha pudiera verlo el 2026-08-09 es probable, no está probado.** La Wayback Machine no respondía.
- **Socios:** no constan. El RUES abierto no los da. Que el representante legal sea además el dueño no entra como hecho.

**2 · El contrato del director y el contenido del medio.**
- **SECOP II por el documento del representante legal: 10 contratos, todos con `tipodocproveedor` «Cédula de Ciudadanía».** Son contratos de persona natural, no de la sociedad. Por orden de firma:

| Contrato | Entidad | Firma | Ejecución | Valor | Estado | Objeto (literal, abreviado) |
|---|---|---|---|---|---|---|
| SG-CPS-441-2022 | Secretaría General y de Cercanía al Ciudadano (Departamento de Cundinamarca, NIT de entidad 899999114) | 2022-01-28 | 2022-02-11 → 2022-12-23 | $39.646.671 | Cerrado | «…divulgación de la información para la generación de contenidos audiovisuales; informativos y periodísti[cos]» |
| SG-CPS-507-2023 | ídem | 2023-03-02 | 2023-03-06 → 2023-12-15 | $43.498.333 | Cerrado | «…contenidos informativos y periodísticos a emitir a través de la emisora institucion[al]» |
| 0322-2024 | Municipio de Soacha | 2024-02-20 | 2024-02-21 → 2024-08-20 | $30.000.000 | Cerrado | «…plan de difusión de la Alcaldía de Soacha» |
| 2299-2024 | Municipio de Soacha | 2024-09-04 | 2024-09-05 → 2024-12-30 | $19.500.000 | Cerrado | ídem |
| 0733-2025 | Municipio de Soacha | 2025-01-14 | 2025-01-15 → 2025-07-14 | $30.000.000 | Cerrado | ídem, SG_086 |
| RTVC-CPS-1517-2025 | INRAVISIÓN | 2025-05-26 | 2025-05-28 → 2025-12-29 | $41.870.000 | Modificado | «…periodista digital; en la construcción y edición de contenidos para las plataformas digitales de RTVC» |
| 1905-2025 | Municipio de Soacha | 2025-07-15 | 2025-07-23 → 2025-12-31 | $27.500.000 | Cerrado | ídem plan de difusión, SG_130 |
| 0880-2026 | Municipio de Soacha | 2026-01-13 | 2026-01-14 → 2026-07-13 | $30.900.000 | Modificado | ídem, SG_72 |
| RTVC-CPS-227-2026 | INRAVISIÓN – Sistema de Medios Públicos | 2026-01-21 | 2026-01-22 → 2026-07-21 | $36.829.800 | Modificado | periodista digital, RTVC |
| **3030-2026** | **Municipio de Soacha** | **2026-08-12** | **2026-08-14 → 2026-12-13** | **$20.600.000** | **En ejecución** | «PRESTACION DE SERVICIOS PROFESIONALES PARA LA ORGANIZACION; EJECUCION Y SEGUIMIENTO DEL PLAN DE DIFUSION DE LA ALCALDIA DE SOACHA.SG_174» |

  - Total SECOP II: **$320.344.804 contratados**. En los últimos 12 meses (firmados del 2025-10-10 al 2026-10-10): **3 por $88.329.800** (0880-2026, RTVC-CPS-227-2026 y 3030-2026). `valor_pagado` es 0 en todos los de 2024-2026, así que se dice «contratado», nunca «cobrado».
  - Las cifras, referencias, fechas y `noticeUID` del revisor coinciden al peso. El «estado» de 0880-2026 y RTVC-CPS-227-2026 es «Modificado», no «Cerrado»: puede haber prórroga o adición que el conjunto de datos no refleja en la fecha de fin.
- **SECOP I por el mismo documento:** 2 contratos con la Alcaldía de Soacha en 2019 (783-2019 y 1792-2019), $12.920.400, de apoyo a un proyecto de convivencia y salud mental. Son historia; solo sirven para la identidad (ver 1).
- **Por el NIT de la sociedad (901444929):**
  - **SECOP II: 0.**
  - **SECOP I: 4 contratos, $13.906.600, ninguno en los últimos 12 meses:** Empresa de Licores de Cundinamarca (5320210249-2021, 2021-08-05, $3.000.000, «PUBLICIDAD DE LOS PRODUCTOS […] MEDIANTE BANNER EN EL ACCESO PRINCIPAL DE LA PAGINA WWW.DIARIOCUNDINAMARCA.COM», así, sin «de»); Agencia Logística de Gestión Inmobiliaria y Servicios de Cundinamarca (CPS 405 DE 2021, 2021-10-13, $3.600.000, banners); Personería Municipal de Soacha (MC-014-2021 G3, 2021-09-03, $2.856.000, y MC-006-2022-G3, 2022-03-24, $4.450.600, «servicio de comunicaciones en radio; medios escritos y digitales»).
  - Coincide con el revisor.
- **«Sin interrupciones desde febrero de 2024»: falso.** Entre contratos con la Alcaldía hay tres huecos: 2024-08-20 → 2024-09-05, 2024-12-30 → 2025-01-15 y 2026-07-13 → 2026-08-14. La relación es **recurrente y casi continua**, que es lo que el argumento necesita, pero no ininterrumpida.
- **El recuento de las 19 piezas, rehecho:**
  - El feed tiene 20 ítems (del 05-09-2025 al 22-07-2026). Los 19 con fecha dentro de los 12 meses coinciden uno a uno con los 19 URL de `blog-posts-sitemap.xml` con `lastmod` ≥ 2025-10-10. Las fechas del feed y del `lastmod` coinciden en 18; la de vivienda tiene `pubDate` 15-01-2026 y `lastmod` 2026-03-03.
  - **16 de las 19, del 09-12-2025 al 12-04-2026, son contenido institucional favorable a la Alcaldía de Soacha. Exacto.** Las otras 3: la renuncia del concejal Juan Carlos Arias (25-06-2026) y dos piezas sobre el gerente de Canal Trece (17-07 y 22-07-2026).
  - Rasgos, contados en el texto de cada pieza:
    - nombran al alcalde («Perico» o «Víctor Julián Sánchez Acosta, alcalde de Soacha»): **13 de 16**;
    - usan «Gobierno de la Ciudad»: **11 de 16**;
    - llevan entradilla con lugar y fecha («Soacha, Cundinamarca, 12 de abril de 2026», «Soacha, 27 de febrero de 2026», etc.): **6 de 16** (12-04, 27-02, 31-01, 17-01, 15-01-2026 y 26-12-2025). **No todas, como da a entender el revisor;**
    - una habla en primera persona del organizador: «Los esperamos este 17 de diciembre en el Rincón del Lago, Comuna 4» (17-12-2025, novenas);
    - **ninguna es crítica** con la administración. Las únicas apariciones de «irregular» y «denunci-» se refieren a un establecimiento cerrado por la Alcaldía (31-01-2026) y a una invitación a denunciar delitos (15-12-2025).
  - **Firma y marcas:** las 19 van firmadas «Diario de Cundinamarca» (autor en los datos estructurados y `dc:creator` del feed). En el HTML crudo de las 19 hay 0 apariciones de «prensa», «publirreportaje», «patrocinad», «contenido pagado», «comunicado de prensa», «oficina de prensa» y «boletín». La cabecera «Independencia informativa» aparece en todas. Coincide con el revisor, y ahora sobre las 19, no sobre una.
  - Las cuatro citas del revisor son literales en el feed y en las piezas.
- **La coincidencia en el tiempo, que el revisor no mide:**
  - **15 de las 16** piezas se publicaron mientras su director tenía vigente un contrato del plan de difusión de la Alcaldía (1905-2025, hasta el 31-12-2025, o 0880-2026, desde el 14-01-2026). **La del 08-01-2026** («Soacha acelera su transformación en 2026…») cae en el hueco entre los dos contratos.
  - **El contrato vigente (3030-2026, desde el 14-08-2026) coincide con cero publicaciones.** Es un contrapeso a leer el medio como canal de entrega del contrato: hoy el contrato existe y el medio no publica.
- **Hecho y no hecho.**
  - **Hecho:** la misma persona es director declarado del medio, representante legal de su sociedad y contratista personal del plan de difusión de la Alcaldía de Soacha, con un contrato en ejecución hoy. En los 12 meses, el medio publicó 16 piezas institucionales favorables a esa Alcaldía, 15 de ellas durante un contrato de su director, sin ninguna marca de contenido institucional.
  - **No es hecho:** que las piezas sean boletines de la Alcaldía reproducidos, que formen parte de las obligaciones o informes del contrato, que se hayan pagado, o que el medio dependa económicamente de la Alcaldía. No se abrieron los expedientes de SECOP y no se encontró el original de ningún texto.
- **Regla de quien dirige: no procede aviso.** Un contrato de prestación de servicios no es un cargo público ni una candidatura. Y el medio no está en el catálogo.
- **Polo fijo.** Coincidimos con el revisor: alinearse con un gobierno municipal no es una posición en el eje, y nada de esto da número.

**3 · Plataforma, parada, volumen y ámbito.**
- **Wix, no Blogger:** `generatedBy="WIX"` en los tres sitemaps, `<generator>RSS for Node` en el feed, el robots.txt autogenerado de Wix y las imágenes en `static.wixstatic.com`. Exacto.
- **Parada:** último ítem del feed «Wed, 22 Jul 2026 13:28:33 GMT»; `<lastBuildDate>Thu, 08 Oct 2026 20:39:10 GMT`. Del 22-07 al 10-10 van **80 días**. El índice `sitemap.xml` da `lastmod` 2026-07-22 a los posts y a las categorías. **La cifra de la ficha (437 h desde el 22-07-2026 13:28 GMT) cuadra con su fecha** (2026-08-09) y el feed tenía entonces, como hoy, 20 entradas.
- **Volumen** (`blog-posts-sitemap.xml`, 5.893 URL): 2020: **448**; 2021: 1.897; 2022: 1.927; 2023: 1.379; 2024: 180; 2025: 50; 2026: 12. Las cifras del revisor de 2021 a 2026 son exactas, pero omite las 448 de 2020 (sin ellas la suma no llega a 5.893). Desde el 12-04-2026, 3 URL, como dice.
- **Corrección: la conducta medida no confirma la parada.** El revisor escribe «La conducta medida del envío lo confirma: 0 artículos en la ventana». El medio **no está en `shared/mediaRegistry.js`** y nadie lo ingiere: `data/conducta.json` le da 0 artículos porque no tiene corpus, publique o no. Lo que confirma los 0 de la ventana es el feed, cuya última entrada es del 22-07.
- **Ámbito municipal:** la descripción del canal dice literalmente «Independencia informativa originada en la ciudad del 'Dios Varón', con la actualidad de Soacha, Cundinamarca, Bogotá y Colombia». `/nuestro-diario` dice «para ser referente en el municipio». La sociedad está en la Cámara de Soacha. Exacto.
- **Lo que el revisor no podía saber:** la «salida 2» de la ficha (buscar prensa municipal de Soacha) **ya se hizo**. Periodismo Público (Soacha) entró en el catálogo como «primer medio de Cundinamarca» (`shared/mediaRegistry.js`; ficha `fichas/periodismo-publico.md`, revisada en la tanda 4). Su ficha de propiedad documenta el mismo perfil: pauta de entidades públicas de Soacha y Cundinamarca contratada a nombre del representante legal, incluido un contrato con EPUXUA E.I.C.E. (2025) para difundir los programas «que requiera la Alcaldía Municipal de Soacha». La sección «Cundinamarca es un caso aparte» y la REFUTACIÓN 1 de esta ficha están desfasadas.

**4 · La razón del descarte.**
- La conclusión del revisor (no darlo de alta, y por otras razones) se sostiene con todo lo anterior.
- La fórmula «inactivo y con dependencia institucional no declarada» afirma una dependencia **del medio** que no consta. Lo que consta es el contrato **de su director** y el contenido. La propuesta usa esa redacción.

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se rechazan como hecho, o se corrigen, estas partes:
- **Obj. 1, el `lastmod` como indicio de fecha:** es común a las cuatro páginas del sitio y no dice nada de `/nuestro-diario`.
- **Obj. 2, «sin interrupciones desde febrero de 2024»:** hay tres huecos entre contratos.
- **Obj. 2, «usan […] la entradilla con lugar y fecha propia de un boletín» como rasgo de las 16:** está en 6.
- **Obj. 2, que las piezas sean boletines o entregables del contrato:** el revisor lo marca como inferencia, y aquí tampoco entra como hecho.
- **Obj. 3, «la conducta medida del envío lo confirma»:** no lo confirma, porque el medio no se ingiere.
- **Obj. 4, «dependencia institucional»:** no consta del medio; ver la redacción propuesta.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente.** Todas las URL del sitio respondieron 200 el 2026-10-10. Las consultas de RUES y SECOP devuelven lo que dice el revisor, con cifras exactas. Deformaciones y omisiones:
- «sin interrupciones desde febrero de 2024» (ver arriba);
- la entradilla generalizada a las 16 piezas (son 6);
- la conducta medida presentada como confirmación de la parada;
- el recuento por año sin 2020;
- deja abierta la identidad Michael / Michel, que SECOP I cierra;
- no ve que el contrato vigente coincide con cero publicaciones (contrapeso), ni que una de las 16 piezas cae entre contratos.

**Errores de la propia ficha, para no repetirlos:**
- «Nivel 1 — Nada. Ni sociedad, ni NIT, ni propietario, ni director, ni editor»: falso. Hay sociedad (MCA DIARIO DE CUNDINAMARCA SAS), NIT (901444929), representante legal y director declarado. Solo el propietario sigue sin constar.
- «Su web no declara equipo ni contacto identificable»: falso hoy, y probablemente también el 2026-08-09 (el enlace está en el menú de todas las páginas).
- «una ruta de Blogger»: falso. Es Wix.
- **Departamento: Cundinamarca**, y el encuadre como voz departamental: es un medio municipal de Soacha.
- «Es el mismo caso que Sucre Noticias»: ya no. Aquí hay nivel 1 y el problema es otro.
- La sección «Cundinamarca es un caso aparte», la salida 2 y la REFUTACIÓN 1: desfasadas, porque Periodismo Público (Soacha) ya está en el catálogo.
- Falta la línea de contratación pública que exige el protocolo desde el 2026-10-07.

**Lo que la ficha sí tenía bien:**
- la parada de 437 horas, exacta para su fecha;
- las veinte entradas del feed;
- la conclusión de no darlo de alta.

---

**Propuesta para la firma**

**Estado de la candidatura: descartada, no se da de alta.** No hay número que proponer: el valor sigue siendo «ninguno», ahora con otra razón. No hay nada que firmar en la escala.

**Razón nueva, en lugar de «no hay nivel 1»:**

> Descartado por inactividad, con nivel 1 localizado y un vínculo no declarado. No publica desde el 22-07-2026 (80 días a 2026-10-10) y en 2026 lleva 12 piezas. Su director declarado, Michael (Michel) Anzola Solano, es el representante legal de MCA DIARIO DE CUNDINAMARCA SAS (NIT 901444929) y contratista personal del plan de difusión de la Alcaldía de Soacha, con un contrato en ejecución hasta el 13-12-2026 (3030-2026). En los últimos 12 meses, 16 de sus 19 piezas son contenido institucional favorable a esa Alcaldía, sin marca de contenido institucional, y 15 se publicaron durante un contrato de su director. Que sean boletines o entregables del contrato no consta.

**Correcciones de hecho en `fichas/diario-de-cundinamarca.md`:**
1. **Cabecera:**
   - «Valor propuesto»: «**ninguno** — inactivo desde el 22-07-2026, y su director es contratista de difusión de la Alcaldía que cubre».
   - «Departamento»: «Cundinamarca (municipal: Soacha)».
   - Añadir «Revisión: ciclo 2, tanda 6, 2026-10-10».
2. **«Nivel 1 — Nada»** se sustituye por:
   - **Sociedad:** MCA DIARIO DE CUNDINAMARCA SAS, NIT 901444929, SAS, matrícula 3323337, activa en la Cámara de Comercio de Soacha (renovada en 2026). Su matrícula en Bogotá figura cancelada el 2026-08-15, el mismo día que otras 7.561, por el paso de expedientes a la nueva cámara de Soacha; no es un cambio de dueño. Fuente: RUES abierto, `c82u-588k`, consultado el 2026-10-10.
   - **Representante legal:** Michel Anzola Solano (RUES, registro de Bogotá actualizado el 2026-08-15; el de Soacha no trae el campo).
   - **Director declarado:** «MICHAEL ANZOLA SOLANO, Director» en `https://www.diariodecundinamarca.com/nuestro-diario`. Es la misma persona que el representante legal: SECOP I registra las dos grafías con el mismo documento. Sin documento en la ficha.
   - **Contacto:** el correo `[correo omitido]` del pie. El teléfono no se escribe.
   - **Socios:** no constan; el RUES abierto no los da.
   - **Homónimo a no confundir:** DIARIO DE CUNDINAMARCA E U – EN LIQUIDACION (Bogotá, 2004; último año renovado 2007).
3. **Contratación pública**, línea nueva en el formato del protocolo:

> Contratación pública (SECOP I y II, NIT 901444929, consultado 2026-10-10): 0 contratos en los últimos 12 meses; 4 por $13.906.600 contratados en total desde 2021, todos en SECOP I (SECOP II: 0). Contratantes: Personería de Soacha (2021 y 2022), Empresa de Licores de Cundinamarca (2021, banner en la web) y Agencia Logística de Gestión Inmobiliaria y Servicios de Cundinamarca (2021). Su representante legal y director, Michel Anzola Solano, ha contratado además como persona natural 12 contratos por $333.265.204 (SECOP II: 10 por $320.344.804, 2022-2026; SECOP I: 2 por $12.920.400, 2019). En los últimos 12 meses son 3 por $88.329.800: dos con el Municipio de Soacha para el «plan de difusión de la Alcaldía de Soacha» (0880-2026 y 3030-2026, este en ejecución hasta el 13-12-2026) y uno con RTVC como periodista digital (RTVC-CPS-227-2026). La Alcaldía de Soacha es el gobierno que el medio cubre. Identidad probada por igualdad de documento en los 12.

4. **«Nivel 2 — El feed lleva 437 horas parado»** se reescribe:
   - «Wix, no Blogger (`blog-feed.xml` de Wix, generador "RSS for Node").
   - Última pieza: 22-07-2026; 80 días sin publicar a 2026-10-10 (437 h el 2026-08-09).
   - Volumen por `lastmod` del sitemap (aproximación): 2021: 1.897; 2022: 1.927; 2023: 1.379; 2024: 180; 2025: 50; 2026: 12.
   - Sin corpus propio: el medio no se ingiere».
5. **Sección nueva, «Contenido de los últimos 12 meses»** (desvelamiento, no acusación):
   - 16 de 19 piezas institucionales favorables a la Alcaldía de Soacha, del 09-12-2025 al 12-04-2026;
   - firmadas «Diario de Cundinamarca», sin marca de contenido institucional;
   - 13 nombran al alcalde, 11 dicen «Gobierno de la Ciudad», 6 llevan entradilla de comunicado;
   - 15 publicadas durante un contrato de su director;
   - ninguna crítica.
   - Lo que **no** entra como hecho: que sean boletines reproducidos, entregables del contrato o contenido pagado.
6. **«Por qué no se propone número»** → la razón nueva de arriba. Retirar «no hay nivel 1» y «Es el mismo caso que Sucre Noticias».
7. **«Cundinamarca es un caso aparte»:** añadir al principio una nota fechada. «Desde que se escribió, Periodismo Público (Soacha) entró en el catálogo como medio de Cundinamarca, y la búsqueda municipal de la salida 2 encontró dos medios de Soacha con pauta o contratos de entidades públicas que cubren». La decisión entre las tres salidas sigue siendo del responsable editorial, ahora con Periodismo Público dentro.
8. **REFUTACIÓN:**
   - el punto 1 se marca como cumplido (Periodismo Público);
   - el punto 2 pasa a ser «Que vuelva a publicar con ritmo sostenido y declare —o termine— el vínculo contractual de su director con la Alcaldía de Soacha, y marque el contenido institucional».

**Fuera de la ficha** (el medio no está en `mediaOwnership.js`, `mediaRegistry.js` ni `centinela.js`, y no hace falta tocarlos):
9. `fichas/LEEME.md`, fila de `diario-de-cundinamarca.md`: «Sin nivel 1 y con el feed parado» → «Inactivo desde el 22-07-2026; su director es contratista de difusión de la Alcaldía de Soacha».
10. `MEDIOS_CANDIDATOS_DEPARTAMENTOS.md`:
    - la fila de la tabla de fichas, «**sin número**: nivel 1 vacío + 18 días parado» → «**descartado**: inactivo (80 días a 10-10) + director contratista de difusión de la Alcaldía de Soacha · ciclo 2, 2026-10-10»;
    - el párrafo «Cundinamarca merece decidirse, no buscarse» lleva la misma nota que el punto 7.

**¿Aviso de quien dirige?** No procede. Un contrato de prestación de servicios no es un cargo público ni una candidatura, y el medio no está en el catálogo.

**Lo que NO entra como hecho:**
- que las 16 piezas sean boletines de la Alcaldía reproducidos, entregables del contrato o contenido pagado;
- que el medio dependa económicamente de la Alcaldía;
- que el representante legal sea también el dueño (los socios no constan);
- que `/nuestro-diario` existiera ya el 2026-08-09;
- el acto jurídico concreto del paso de Bogotá a Soacha (se infiere del patrón masivo, no se consultó).

**Decisiones para el responsable editorial:**
1. **Estado de la candidatura.** Recomendación: **descartada, con la razón nueva** (inactividad, nivel 1 localizado y vínculo no declarado), no «sin nivel 1».
2. **Cómo se nombra el vínculo.** Recomendación: «vínculo contractual de su director con la Alcaldía de Soacha, no declarado en el medio», y **no** «dependencia institucional», que afirma algo del medio que no consta.
3. **La vista departamental de Cundinamarca.** Ya no es la pregunta abierta que planteaba la ficha: Periodismo Público ocupa la plaza. Lo que queda es si basta un medio de Soacha, con su propia tensión de pauta pública, o si se busca prensa de Girardot, Zipaquirá o Fusagasugá. Sin recomendación: es una decisión de cobertura, no de evidencia.
4. **Si se pide algo más.** Recomendación: **no** gastar un certificado de Cámara de Comercio ($12.100) ni abrir los expedientes de SECOP mientras el medio no publique. Solo harían falta si se reabre la candidatura.
