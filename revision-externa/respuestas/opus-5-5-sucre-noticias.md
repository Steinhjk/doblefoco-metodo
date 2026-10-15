# Respuesta — Claude Opus 5.5 sobre Sucre Noticias

| | |
|---|---|
| **Modelo** | Claude Opus 5.5 |
| **Versión exacta** | `claude-opus-5-5` |
| **Fecha de la consulta** | 2026-10-10 |
| **Quién la hizo** | Claude Code, a petición del responsable editorial (ciclo 2, fase 2, tanda 7; revisor de la misma casa que el autor de las fichas, ver DECISIONES.md 2026-10-07) |
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
Soy Claude Opus 5.5 (claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Mi acuerdo no debe leerse como validación independiente. Para compensarlo he trabajado casi solo con fuentes primarias que la ficha no usa: el HTML crudo, los feeds y los sitemaps del propio sitio, los datos abiertos del RUES y del SECOP, el RDAP del dominio y la API de mapeomedios.com. No he usado ningún juicio de modelo sobre la orientación del medio.

MÉTODO Y DÓNDE BUSQUÉ (todo el 2026-10-10)
- Dominio identificado: sucrenoticias.com (www redirige al dominio raíz). Su robots.txt es el de Yoast, con "User-agent: * / Disallow:" vacío y sin bloqueo a ClaudeBot, Claude-Web ni anthropic-ai, así que lo descargué. Todo con curl -sL y User-Agent de navegador.
- En el sitio descargué la portada, /contacto/, /feed/, sitemap_index.xml, post-sitemap6.xml, page-sitemap.xml, author-sitemap.xml y category-sitemap.xml. También los feeds de las categorías opinion/editorial, opinion/columnistas, opinion, sucre/sucreelige y especial, siete artículos de 2026 y la página de autor /author/joseiriartediaz/. Probé además /wp-json/wp/v2/users, que devuelve 401 y no lista usuarios.
- En el sitemap de entradas busqué por términos políticos en las URL de octubre de 2025 a octubre de 2026: cepeda, espriella, petro, uribe, paloma, valencia, presiden, gobierno, candidat, pacto, elecci, consulta, senado, ministr, gobernador, alcald, votac, registradur, moe.
- RUES abierto (datos.gov.co c82u-588k), por razón social: '%SUCRE NOTICIA%', '%SUCRENOTICIAS%', '%NOTICIAS SUCRE%' y '%SUCRE%NOTICI%' en todas las cámaras. En la Cámara de Sincelejo, además: '%NOTICI%', '%PERIOD%', '%MEDIO%COMUNIC%' y '%DIARIO%'.
- SECOP II (jbjy-vk9h): proveedor_adjudicado LIKE '%SUCRE NOTICIA%'; descripcion_del_proceso LIKE '%SUCRENOTICIAS%' y '%SUCRE NOTICIAS%'; objeto_del_contrato LIKE '%SUCRE NOTICIAS%'.
- SECOP I (f789-7hwg): nom_razon_social_contratista LIKE '%SUCRE NOTICIA%'; detalle_del_objeto_a_contratar LIKE '%SUCRENOTICIAS%' y '%SUCRE NOTICIAS%'.
- La consulta por NIT con igualdad exacta (documento_proveedor / identificacion_del_contratista) NO SE PUDO HACER porque no existe NIT conocido. Las búsquedas por nombre la sustituyen solo en parte.
- RDAP de Verisign para sucrenoticias.com.
- mapeomedios.com: su robots.txt lo permite. Descargué la portada, /mapa, /publicaciones y /api/municipios, el JSON de los 38 medios mapeados.
- Buscador web: estaba disponible. Hice una sola búsqueda ("Sucre Noticias" Sincelejo director periodista "sucrenoticias.com") y no devolvió nada pertinente sobre este medio. No toqué eltiempo.com, cambiocolombia.com, lasillavacia.com ni diariodelsur.com.co, aunque el buscador devolvió enlaces de dos de ellos.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré nada, pero no existe ningún dueño documentado contra el que comparar. En el RUES abierto no hay sociedad con razón social "SUCRE NOTICIAS" ni "SUCRENOTICIAS" (consulta del 2026-10-10, resultado vacío). El dominio sigue registrado y se renovó: según el RDAP de Verisign (https://rdap.verisign.com/com/v1/domain/sucrenoticias.com, consultado el 2026-10-10) el registro es de 2018-05-24, el último cambio "last changed" de 2026-05-25T08:48:17Z y el vencimiento de 2027-05-24. Es un hecho de continuidad técnica, no de propiedad. El RDAP del registro no publica titular, y no consulté el del registrador.
  Lo que sí cambió en 12 meses es el volumen. Las fechas lastmod de post-sitemap6.xml, que miden la última modificación y no la publicación (es una aproximación), dan por mes: 2025-07 = 66, 2025-08 = 67, 2025-09 = 15, 2025-11 = 3, 2025-12 = 2, 2026-01 = 11, 2026-02 = 3, 2026-03 = 12, 2026-04 = 2, 2026-05 = 21, 2026-06 = 14, 2026-07 = 5, 2026-08 = 9 y 2026-09 = 13. La caída abrupta empieza en septiembre de 2025. Fuente: https://sucrenoticias.com/post-sitemap6.xml (2026-10-10).
- La persona que la ficha nombra como titular o director, ¿sigue viva y en el cargo?
  No procede: la ficha no nombra a nadie. Comprobado el 2026-10-10.
- ¿Quién dirige hoy la redacción?
  No encontré ningún nombre de director, editor ni gerente en la portada, en /contacto/, en el pie de página ni en la página de autor. El texto del pie dice literalmente: "© Sucre Noticias. Todos los derechos reservados. [...] sin permiso expreso de esta redacción". Lo que sí hay son firmas: en el feed actual, la mayoría de las piezas de septiembre de 2026 las firma "José Iriarte Díaz", y aparecen también "Jenny Carolina González" y "Redacción". El author-sitemap lista ocho autores. Que una persona firme la mayoría de las piezas no prueba que dirija el medio: es una inferencia que no hago.
- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que la ficha cita?
  La ficha no cita ninguna fuente, y yo no encontré ningún registro (ver Objeción 6).

## OBJECIONES

OBJECIÓN 1. "El feed está parado / 332 horas sin artículo nuevo"
- QUÉ: el motivo 2 para no proponer número se apoya en un feed "quieto".
- POR QUÉ: hoy el feed no está parado. Está vivo, pero con una cadencia baja e irregular. https://sucrenoticias.com/feed/ (descargado el 2026-10-10) tiene <lastBuildDate>Wed, 30 Sep 2026 21:22:31 +0000</lastBuildDate> y diez entradas entre el 2026-09-03 y el 2026-09-30, por ejemplo "Sincelejo: lluvias y nubosidad durante los próximos días" (30-09), "Afinia denuncia la reconexión ilegal del acueducto de San Onofre" (30-09), "La Procuraduría investiga el pago de puntos salariales a docentes de la Unisucre" (22-09) y "Denuncian una «masacre laboral» en la ESE San Francisco de Asís de Sincelejo" (14-09). Son unas 2,5 piezas por semana. A la fecha de mi comprobación llevaba 10 días sin publicar, un hueco del mismo orden que el que midió la ficha.
  La conclusión de la ficha (que no aportaría cobertura comparable) se sostiene, pero hay que reformular el hecho: "publica de forma esporádica, unas 10 piezas al mes en septiembre de 2026 y en torno a 66 al mes en julio y agosto de 2025", no "parado".
  Nota sobre el bloque de conducta medida del envío: los "0 artículos" en la ventana del 2026-08-31 al 2026-10-10 reflejan, con toda probabilidad, que el medio no se ingesta porque no está en el catálogo. No significan que no publicara. Es una inferencia, no la he comprobado.
- FUENTE: https://sucrenoticias.com/feed/ y https://sucrenoticias.com/post-sitemap6.xml, ambos descargados el 2026-10-10.
- NIVEL: conducta observable.

OBJECIÓN 2. La ficha no fue a la sección editorial (premisa 5 del encargo)
- QUÉ: la ficha solo evalúa el nivel 4, lo que el medio dice de sí mismo, y no examina si existe una voz de la casa.
- POR QUÉ: el sitio tiene una sección "Editorial" (/category/opinion/editorial/) y otra de "Columnistas". Las comprobé y la ausencia se confirma, pero ahora queda auditada. El feed de la categoría editorial muestra como piezas más recientes "Un pequeño genio camina entre nosotros." (Jhony Polo Barrios, 12-08-2022) y "Editorial-25 de septiembre de 2021: Desde el desayuno se sabe cómo será el almuerzo" (Redacción, 25-09-2021). No hay ningún editorial institucional en los últimos 12 meses. La pieza más reciente de Opinión es "Monseñor Nel Beltrán: un obispo con tino y con tacto" (Redacción, 18-08-2025), y queda fuera de la ventana de 12 meses.
  Consecuencia: la excepción de la regla 3 (asimetría sostenida en la voz de la casa, con al menos 10 piezas) no es aplicable, porque no hay piezas. Esto refuerza que no se puede proponer número, pero la ficha debería haberlo dicho con esta fuente.
- FUENTE: https://sucrenoticias.com/category/opinion/editorial/feed/ y https://sucrenoticias.com/category/opinion/feed/ (2026-10-10).
- NIVEL: declaración del propio medio / conducta observable.

OBJECIÓN 3. "No dice quién lo sostiene": la ficha omite la fuente visible de ingresos
- QUÉ: la ficha dice que el medio "afirma independencia y no dice quién lo sostiene".
- POR QUÉ: no dice quién es su dueño, pero sí se ve quién paga contenido. La categoría "Especial" reúne, entre mayo y agosto de 2026, textos firmados "Redacción" que son comunicados o contenido de marca sin ninguna etiqueta de publicidad. En el HTML de las piezas revisadas busqué "patrocinad", "publirreportaje", "contenido pagado" e "informe comercial" y no hay ninguna coincidencia. Las piezas son:
  * "Superada la meta de formación en talento digital del Gobierno Petro: 1.020.181 personas capacitadas..." (21-05-2026). Empieza así: "Bogotá, mayo de 2026. (@Ministerio_TIC) – En menos de cuatro años, el Gobierno del presidente Gustavo Petro multiplicó el acceso digital a la educación...".
  * "Con cerca de 6.000 kilómetros de fibra óptica desplegados por el país, el Gobierno Petro hizo que la conectividad dejara de ser una promesa" (28-05-2026).
  * "Colombia se posiciona como referente regional en inteligencia artificial e innovación digital" (15-05 y 22-05-2026).
  * Cuatro piezas de Afinia (13, 15, 20 y 22-05-2026), por ejemplo "Afinia fortalece su clima laboral y se consolida como referente del sector eléctrico".
  * "El Grupo EPM se prepara con responsabilidad y compromiso ante la posibilidad del fenómeno de El Niño en Colombia" (19-05-2026).
  * "Conozca el proyecto Plan Sur Fase I..." (20-08-2026), escrito en primera persona por la empresa: "En Veolia, estamos convencidos de que el agua es el motor que impulsa el bienestar de las familias sincelejanas".
  Fuera de "Especial" está "El gobierno avanza en la reparación a las víctimas de Pichilín" (sección Municipios, fechada en el schema el 28-04-2026). Incrusta un vídeo cuyo nombre de archivo empieza por "[correo omitido]4".
  INFERENCIA, no probada: que sea pauta pagada por el MinTIC, Afinia/EPM y Veolia. El patrón de comunicado íntegro sin firma, en una sección aparte, lo sugiere, pero no encontré ningún contrato. Sin NIT no hay consulta exacta en el SECOP, y la pauta oficial suele contratarse a través de agencias.
  Por la regla del polo fijo, publicar comunicados del gobierno saliente no es evidencia de orientación, y no muevo el número por ello. Pero la ficha debería declarar que sus anunciantes o fuentes de contenido de marca visibles son el Gobierno nacional (MinTIC, mayo de 2026), Afinia/Grupo EPM y Veolia. Para un medio sin dueño conocido, es lo más parecido a un "de qué vive" que hay hoy.
- FUENTE: https://sucrenoticias.com/category/especial/feed/ ; https://sucrenoticias.com/superada-la-meta-de-formacion-en-talento-digital-del-gobierno-petro-1-020-181-personas-capacitadas-en-habilidades-tecnologicas/ ; https://sucrenoticias.com/conozca-el-proyecto-plan-sur-fase-i-transparencia-infraestructura-y-mejor-calidad-de-vida-para-nuestra-ciudad/ ; https://sucrenoticias.com/el-gobierno-avanza-en-la-reparacion-a-las-victimas-de-pichilin/ (todas descargadas el 2026-10-10).
- NIVEL: conducta observable (hecho editorial de los últimos 12 meses). El carácter pagado es una inferencia.

OBJECIÓN 4. "Ni director, ni editor": la ficha no registra las personas que el medio sí publica
- QUÉ: "Ni sociedad, ni NIT, ni propietario, ni director, ni editor."
- POR QUÉ: lo de director y editor es correcto, porque no hay ningún cargo publicado. Pero el sitio sí publica firmas con nombre y apellido. El author-sitemap lista ocho autores, y en el feed actual la mayoría de las piezas de septiembre de 2026 las firma José Iriarte Díaz, cuya página de autor lo presenta como "Comunicador social (UNAD) y periodista, becario de la Fundación Gabriel García Márquez para el Nuevo Periodismo Iberoamericano" (cito solo la parte profesional). Es un punto de partida para preguntar por la dirección que la ficha no recoge. No afirmo que sea director ni dueño.
- FUENTE: https://sucrenoticias.com/author-sitemap.xml ; https://sucrenoticias.com/author/joseiriartediaz/ ; https://sucrenoticias.com/feed/ (2026-10-10).
- NIVEL: declaración del propio medio.

OBJECIÓN 5. La ficha no cita ninguna fuente
- QUÉ: las citas «un medio de comunicación independiente honesto e imparcial», «alternativa informativa y periodística independiente y de calidad» y "dos correos y un teléfono" aparecen sin URL ni fecha, y la medida de "332 horas" no indica cuándo ni sobre qué feed se tomó.
- POR QUÉ: las citas existen y son literales. En https://sucrenoticias.com/contacto/ (2026-10-10), bajo "¿Quiénes somos?", se lee: "sucrenoticias.com es un medio de comunicación independiente honesto e imparcial, que brinda variedad informativa [...]". En el pie de página: "Sucre Noticias es un diario digital con sede en Sincelejo, Sucre (Colombia). Somos una alternativa informativa y periodística independiente y de calidad. Actualidad a un clic." Los dos correos son contacto@ y [correo omitido]. Pero un expediente que se va a auditar no puede apoyarse en citas sin enlace. Hay que añadir las URL y la fecha.
- FUENTE: la indicada, 2026-10-10.
- NIVEL: declaración del propio medio.

OBJECIÓN 6. La laguna registral, comprobada, y un límite de método que la ficha no declara
- QUÉ: "Ni sociedad, ni NIT".
- POR QUÉ: lo compruebo y se sostiene en lo que se puede consultar. En el RUES abierto (c82u-588k), las búsquedas por razón social "%SUCRE NOTICIA%" y "%SUCRENOTICIAS%" devuelven vacío. En la Cámara de Sincelejo, "%NOTICI%" devuelve solo "SINCELEJO NOTICIAS S.A.S" (SAS activa, matriculada en 2018-06-27, último año renovado 2024) y "TELENOTICIAS DE SUCRE SAS" (activa, matriculada en 2023-05-15, renovada en 2025). NO HAY NINGÚN VÍNCULO PROBADO entre esas sociedades y sucrenoticias.com: son homonimias parciales y no deben atribuirse.
  En SECOP I y SECOP II, las búsquedas por nombre ("SUCRE NOTICIA" como contratista u objeto, y "SUCRENOTICIAS" en el objeto) devuelven vacío. La consulta exacta por NIT, que exige el protocolo, no se pudo hacer porque no hay NIT. Contratos en los últimos 12 meses: 0 encontrados por nombre. Total histórico: 0 encontrados por nombre.
  LÍMITE que la ficha debería declarar: el dataset c82u-588k solo contiene dos categorías ("PERSONA NATURAL", 6.962.889 registros, y "SOCIEDAD ó PERSONA JURIDICA PRINCIPAL ó ESAL", 2.473.441, según un recuento por agrupación del 2026-10-10). No incluye establecimientos de comercio. Si "Sucre Noticias" estuviera matriculado como establecimiento de una persona natural, que es una figura habitual en medios pequeños, no aparecería en esa consulta. Habría que mirar el buscador web del RUES (rues.org.co) por nombre de establecimiento o pedir el certificado a la Cámara de Comercio de Sincelejo. Yo no lo hice.
- FUENTE: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] , [enlace retirado: puede mostrar documentos de identidad; ver la resolución] y [enlace retirado: puede mostrar documentos de identidad; ver la resolución] , con las consultas descritas en el método (2026-10-10).
- NIVEL: registro externo / propiedad.

OBJECIÓN 7. La vía de refutación 3 (mapeomedios.com) ya está agotada
- QUÉ: la ficha propone explorar mapeomedios.com "como el sitio evidente por donde seguir".
- POR QUÉ: lo exploré. La API pública /api/municipios devuelve 38 medios del departamento de Sucre, con nombre y descripción, y muchos con director. Sucre Noticias no está: no hay coincidencias de "Sucre Noticias" ni de "sucrenoticias". Hay medios de nombre parecido con director declarado, como "Sincelejo Noticias SN" y "Sucre Informativo", que no deben confundirse con este. La vía no aporta nivel 1 para este medio.
- FUENTE: https://www.mapeomedios.com/api/municipios (2026-10-10).
- NIVEL: registro externo.

## LO QUE NO PUDE VERIFICAR

- Si existe un establecimiento de comercio "Sucre Noticias" matriculado a nombre de una persona natural. El RUES abierto no incluye establecimientos y no consulté rues.org.co ni la Cámara de Sincelejo.
- El titular del dominio: el RDAP del registro no lo publica y no consulté el del registrador.
- Si las piezas de MinTIC, Afinia, EPM y Veolia son pauta pagada. No hay etiqueta, y sin NIT no hay consulta exacta en el SECOP.
- Quién dirige la redacción: no hay ningún cargo publicado en la portada, el contacto, el pie ni la página de autor, y la API de usuarios de WordPress está cerrada (401).
- La cifra de "332 horas" de la ficha (agosto de 2026): no puedo reconstruir el feed de esa fecha. El sitemap muestra solo unas 5 modificaciones en julio de 2026, lo que es compatible con ese hueco.
- Redes sociales (@sucrenoticiasofficial, enlazada en el pie): no las consulté.

## LO QUE FALTA

- Las URL y la fecha de cada cita que hace la ficha (Objeción 5).
- Una consulta del RUES por nombre de establecimiento y del certificado de la Cámara de Comercio de Sincelejo, o en su defecto que la ficha declare que no se hizo.
- La declaración de las fuentes de contenido de marca o pauta visibles (Objeción 3).
- La serie de volumen de publicación de los últimos 12 meses, en lugar de una medición única de horas sin publicar.
- La constancia de que la sección editorial existe y está inactiva desde 2021-2022, con su URL.

## EVIDENCIA QUE NO MUEVE EL NÚMERO

- Cobertura electoral de 2026, por los dos lados y sin endoso. "Los Nunca, la apuesta política de Abelardo de la Espriella" (Redacción, 19-05-2026, sección Sucre elige) parafrasea a la campaña ("Foto: campaña"; "Según la campaña, el movimiento está integrado por personas que trabajan, pagan impuestos..."). "Sincelejo marchará en respaldo al candidato presidencial Iván Cepeda" (Redacción, 04-06-2026) reproduce la convocatoria ("Según los organizadores, la jornada busca respaldar las propuestas de Cepeda..."). Las dos piezas son de material de campaña con atribución, tratado de forma simétrica. No encontré ningún endoso editorial. Fuentes: https://sucrenoticias.com/los-nunca-la-apuesta-politica-de-abelardo-de-la-espriella/ y https://sucrenoticias.com/sincelejo-marchara-en-respaldo-al-candidato-presidencial-ivan-cepeda/ (2026-10-10).
- Cobertura de la jornada electoral con fiscalización a ras de suelo: "Denuncian presuntas coacciones de militares sobre votantes en San Antonio de Palmito" (31-05-2026) y "Funcionarios electorales de Betulia impiden la observación ciudadana, denuncia la MOE" (21-06-2026). Fuente: https://sucrenoticias.com/category/sucre/sucreelige/feed/ (2026-10-10). Es oficio periodístico, no orientación (regla del polo fijo).
- Después del cambio de gobierno, la única pieza sobre el nuevo Ejecutivo es "Embajadora María Consuelo Araujo presenta cartas credenciales ante el presidente Donald Trump" (16-09-2026, firmada por Jenny Carolina González). Es informativa e incluye la descertificación ("tuvo que reaccionar a la decisión de éste país de mantener la descertificación"). Una sola pieza no permite medir asimetría a través del cambio de gobierno: el umbral es de 10 piezas, y no hay ninguna de voz de la casa. Fuente: https://sucrenoticias.com/embajadora-maria-consuelo-araujo-presenta-cartas-credenciales-ante-el-presidente-donald-trump/ (2026-10-10).
- Agenda propia local reciente: la Procuraduría y la Unisucre (22-09-2026), la "masacre laboral" en la ESE San Francisco de Asís (14-09-2026) y Afinia en San Onofre (30-09-2026). Es periodismo local con fiscalización de entidades del departamento, sin orientación deducible. Fuente: https://sucrenoticias.com/feed/ (2026-10-10).
- El dominio se renovó en mayo de 2026 (RDAP, arriba): el proyecto no está abandonado.

## SIN OBJECIÓN
No procede: hay objeciones. Aun así, ninguna de ellas aporta evidencia de nivel 1-3 que mueva el número.

## VALORACIÓN SOBRE LA RECOMENDACIÓN (encargo específico de esta tanda)

- ¿Sigue parado? No. Está activo pero es esporádico: 10 piezas en septiembre de 2026 y ninguna del 30-09 al 10-10. Ha pasado de unas 66 al mes a mediados de 2025 a entre 2 y 21 al mes desde septiembre de 2025.
- ¿Sociedad, NIT, dueño, director o representante legal? No aparece nada en el RUES abierto, en el SECOP por nombre, en mapeomedios ni en el propio sitio. Queda pendiente el RUES por establecimiento de comercio.
- ¿Voz editorial propia? Existe la sección, pero lleva inactiva desde 2021-2022 (editoriales) y desde agosto de 2025 (opinión). En los últimos 12 meses no tiene voz de la casa medible.
- ¿Qué cambió en 12 meses? Hubo una caída fuerte del volumen y aparece contenido de marca sin etiquetar (MinTIC, Afinia/EPM, Veolia) en mayo y agosto de 2026.
- Conclusión: LA RECOMENDACIÓN DE NO DARLO DE ALTA SIGUE EN PIE, con el motivo 2 reformulado: no "parado", sino "esporádico, unas 10 piezas al mes". No recomiendo descartarlo de forma definitiva, porque el sitio está vivo, tiene agenda local propia y el dominio se renovó. Recomiendo dejarlo "en espera" con dos condiciones verificables: (a) que aparezca un titular en el RUES por establecimiento o en un certificado de la Cámara de Comercio, o que el medio publique quién lo dirige; y (b) que sostenga una cadencia útil durante 90 días.
  Si aun así se diera de alta, el único valor provisional compatible con las reglas sería 0,00 (orientación mixta), sin firma y marcado "sin nivel 1-3". Se llega a ese valor porque la regla 3 impide moverlo y la regla 2 lleva en la duda a lo más cercano a la mixta, no porque haya evidencia de que el medio sea mixto. Habría que declarar además que la propiedad es desconocida y que los contenidos de marca visibles proceden del MinTIC, Afinia/EPM y Veolia.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** El revisor no copió cédulas, teléfonos, direcciones, nacionalidad, origen étnico ni lugar de nacimiento de personas naturales. Se comprobó:
- las únicas cifras largas son fechas, el «1.020.181» de un titular del MinTIC y recuentos del RUES;
- de la página de autor de José Iriarte Díaz cita solo la parte profesional y deja fuera, a propósito, la palabra que indica su origen. Aquí tampoco se reproduce;
- el teléfono que publica `/contacto/` no aparece en la respuesta ni en esta resolución;
- los correos `contacto@` y `[correo omitido]` son los contactos que el medio publica como medio, y la regla no los cubre;
- los nombres de personas que aparecen (José Iriarte Díaz, Jenny Carolina González, Jhony Polo Barrios) son firmas que el propio medio publica.

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada:
  - `sucrenoticias.com`: bloque de Yoast, «User-agent: * / Disallow:» vacío, más un «User-agent: Twitterbot / Disallow:». Nada sobre ClaudeBot, Claude-Web ni anthropic-ai. Exacto, como dice el revisor.
  - `datos.gov.co`: `Crawl-delay: 1` y exclusiones de `/browse`; solo se usó la API `/resource/`.
  - `mapeomedios.com`: «User-agent: * / Disallow:» vacío.
  - `korraleja.co`: «User-agent: * / Allow: /».
  - No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex.
- **Sitio**, descargado en crudo el 2026-10-10 con `curl -sL --ssl-no-revoke -A "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/126.0 Safari/537.36"`:
  - portada, `/contacto/`, `/feed/`, `sitemap_index.xml`, `post-sitemap.xml` a `post-sitemap6.xml`, `page-sitemap.xml`, `author-sitemap.xml`, `category-sitemap.xml`: todo 200. `www.sucrenoticias.com` responde 301 al dominio raíz;
  - los feeds de las categorías `opinion/editorial`, `opinion/columnistas`, `opinion`, `especial` y `sucre/sucreelige`: 200;
  - las 10 piezas de «Especial», la de Pichilín, las dos de campaña, la de la embajadora y las tres de agenda local que cita el revisor: 17 piezas, todas 200;
  - las páginas de autor `/author/joseiriartediaz/` y `/author/jiriartediaz_z36q236e/`: 200. `/wp-json/wp/v2/users`: 401;
  - rutas legales probadas: `/quienes-somos/`, `/nosotros/`, `/politica-de-privacidad/`, `/privacy-policy/`, `/aviso-legal/`, `/terminos-y-condiciones/`, `/politica-de-tratamiento-de-datos/`: las siete dan 404;
  - el texto se sacó del HTML crudo quitando etiquetas; los rótulos se buscaron en el HTML, no en el texto extraído.
- **Dominio:** RDAP del registro (`rdap.verisign.com`) y, además, el del registrador, al que el revisor no fue (`rdap.rrpproxy.net`, Key-Systems GmbH).
- **Registros**, en datos.gov.co:
  - RUES (`c82u-588k`): `upper(razon_social) like` '%SUCRE NOTICIA%', '%SUCRENOTICIA%', '%NOTICIAS SUCRE%' o '%NOTICIAS DE SUCRE%', '%SUCRE%NOTICI%' o '%NOTICI%SUCRE%', '%SINCELEJO NOTICIA%'; en la Cámara de Sincelejo, '%NOTICI%', '%PERIODI%' y '%DIGITAL%' con '%MEDIO%'; recuento por `categoria_matricula`; CIIU de las dos homonimias.
  - SECOP II contratos (`jbjy-vk9h`): `objeto_del_contrato` y `descripcion_del_proceso` con '%SUCRE NOTICIAS%' o '%SUCRENOTICIAS%'; `proveedor_adjudicado` con '%SUCRE NOTICIA%' o '%SUCRENOTICIA%'.
  - **SECOP II procesos (`p6dx-8zbt`), que el revisor no consultó:** `descripci_n_del_procedimiento`, `nombre_del_procedimiento` y `nombre_del_proveedor` con los mismos términos. Después, `jbjy-vk9h` por `proceso_de_compra` de los dos procesos encontrados y por la entidad que los publicó.
  - SECOP I (`f789-7hwg`): `detalle_del_objeto_a_contratar` con '%SUCRE NOTICIAS%' o '%SUCRENOTICIAS%'; `nom_razon_social_contratista` con '%SUCRE NOTICIA%' o '%SUCRENOTICIA%'.
- **mapeomedios.com:** `/api/municipios` (200, 34.019 bytes), con búsqueda de «sucre noticias», «sucrenoticias» e «iriarte» en todo el JSON.
- **No se visitaron** las redes sociales del medio (Facebook, Instagram, X, YouTube), ni la página pública de SECOP de los dos procesos: se trabajó con los datos abiertos, que no traen proveedor.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | El feed no está parado: 10 piezas del 03 al 30-09-2026, 10 días sin publicar; caída de ~66/mes a 2-21/mes desde septiembre de 2025 | sí | sí | **Aceptada, con tres correcciones.** Septiembre de 2026 tiene **13** URL en el sitemap (el feed solo muestra los 10 últimos ítems). El rango mensual empieza en **0**, no en 2: octubre de 2025 no tiene ninguna, y hay un hueco de **74 días** (10-09 → 23-11-2025). Y la cifra de la ficha **sí se reconstruye**: las 332 h cuadran a la hora con el `lastmod` 2026-07-26T23:01:44Z |
| 2 | La sección editorial existe y está inactiva: último editorial 25-09-2021, última opinión 18-08-2025 | sí | sí | **Aceptada.** Precisión: la pieza más reciente de la categoría Editorial (12-08-2022) la firma un columnista; el último editorial de la casa, rotulado como tal, es del 25-09-2021 |
| 3 | «Especial» publica comunicados de MinTIC, Afinia/EPM y Veolia sin rótulo; pago no probado | sí | sí | **Aceptada en los hechos; rechazado «sin ninguna etiqueta».** 8 de las 10 piezas llevan un subtítulo de procedencia: «Informe de gestión», «Informe corporativo» o «Información corporativa». Ninguna dice «publicidad» ni «pagado». La de EPM no la firma «Redacción», sino José Iriarte Díaz. Que sea pauta pagada no entra como hecho |
| 4 | Firmas: José Iriarte Díaz firma la mayoría; ocho autores en el sitemap; no se afirma que dirija | sí | sí | **Aceptada, con un dato más.** Son 8 cuentas, pero una de ellas, la que se muestra como «Redacción», tiene el identificador `jiriartediaz_z36q236e`. Es un indicio de quién maneja la firma de la casa, no la prueba de un cargo |
| 5 | La ficha cita sin URL ni fecha (`/contacto/` y pie) | sí | sí | **Aceptada.** Las dos citas son literales: «¿Quiénes somos?» está dentro de `/contacto/`, y la otra en el pie de todas las páginas |
| 6 | RUES y SECOP sin resultado por nombre; homonimias sin vínculo; c82u-588k no incluye establecimientos | sí | sí | **Aceptada en el RUES, con cifras exactas; incompleta en SECOP.** El conjunto de procesos de SECOP II tiene **2 procesos de 2024** del Sorteo Extraordinario de Colombia (Extradec) que nombran «SUCRE NOTICIAS» en el objeto. Ninguno figura adjudicado y no hay contrato en `jbjy-vk9h`. Quedan fuera de los 12 meses, y su vínculo con `sucrenoticias.com` no está probado |
| 7 | mapeomedios.com no lo lista | sí | sí | **Aceptada.** 38 medios en 28 municipios; ninguna coincidencia de «sucre noticias», «sucrenoticias» ni «iriarte» |

### Lo verificado, objeción por objeción

**Nivel 1 previo (titular del dominio y del sitio).**
- **RDAP del registro** (`https://rdap.verisign.com/com/v1/domain/sucrenoticias.com`, 2026-10-10): «registration» 2018-05-24T23:12:38Z, «last changed» 2026-05-25T08:48:17Z, «expiration» 2027-05-24T23:12:38Z, estado «client transfer prohibited», registrador Key-Systems GmbH, servidores de nombres `NS1-CPANEL-SH001.SOLUSOFTWARE.COM` y `NS2-…`. Coincide con el revisor.
- **RDAP del registrador** (`https://rdap.rrpproxy.net/domain/SUCRENOTICIAS.COM`, 2026-10-10), que el revisor no consultó: el titular está **oculto**. La entidad «registrant» trae el nombre vacío, el correo de reenvío `[correo omitido]` y el aviso «Some of the data in this object has been removed». Solo queda visible un campo de región, que no identifica a nadie y no se reproduce. **El dominio no da titular.**
- **Pie** (portada y todas las piezas), literal: «Sucre Noticias es un diario digital con sede en Sincelejo, Sucre (Colombia). Somos una alternativa informativa y periodística independiente y de calidad. Actualidad a un clic. Contáctenos: [correo omitido], [correo omitido] © Sucre Noticias. Todos los derechos reservados. Se prohíbe reproducción total o parcial de nuestros contenidos […] sin permiso expreso de esta redacción». Ningún nombre de persona ni de sociedad.
- **`/contacto/`**, literal: «sucrenoticias.com es un medio de comunicación independiente honesto e imparcial, que brinda variedad informativa a través de sus diferentes secciones. Sus noticias e informaciones están elaboradas por un equipo periodístico profesional […]». Siguen «Misión» y «Visión», «Para comentar sobre nuestro contenido, escríbanos a [correo omitido] Para pautar con nosotros, escríbanos a [correo omitido] También puede llamarnos al [teléfono, no se reproduce]», y un enlace a Instagram. Ningún cargo.
- **Datos estructurados** (JSON-LD de Yoast en la portada): `"@type":"Organization"`, `"name":"sucrenoticiasof"`, con el logo y nada más. Sin `legalName`, sin `founder`, sin dirección. La página de inicio se fecha `"datePublished":"2018-06-05T23:29:34+00:00"`.
- **Páginas legales:** no hay. `page-sitemap.xml` lista solo cinco páginas (portada, `/sample-page/`, dos de «La palabra del día» y `/contacto/`), y las siete rutas legales habituales dan 404. **No hay aviso legal, política de privacidad ni términos.**
- **Redes enlazadas en la portada:** `twitter.com/sucrenoticiasof`, `facebook.com/Sucre-Noticias-495060707578129/`, `instagram.com/sucrenoticiasofficial/` y un canal de YouTube. No se visitaron.
- **El medio sí declara que vende pauta:** «Para pautar con nosotros» y el correo `publicidad@`. Corrige en parte la frase de la ficha «no dice quién lo sostiene»: no dice quién es su dueño, pero sí que se financia con publicidad.

**1 · El feed y el volumen.**
- **`/feed/`** (2026-10-10): `<lastBuildDate>Wed, 30 Sep 2026 21:22:31 +0000`, 10 ítems del 03-09 al 30-09-2026. Por firma, 7 son de José Iriarte Díaz, 2 de Jenny Carolina González y 1 de «Redacción». Los cuatro titulares que cita el revisor están, con esas fechas. Del 30-09 a las 21:22 UTC al 10-10 a las 18:30 UTC van **9,9 días**: «10 días» es correcto.
- **Sitemap** (`post-sitemap6.xml`, recuento por `lastmod`, que mide la última modificación y no la publicación). Las cifras del revisor son exactas: 2025-07 = 66, 2025-08 = 67, 2025-09 = 15, 2025-11 = 3, 2025-12 = 2, 2026-01 = 11, 2026-02 = 3, 2026-03 = 12, 2026-04 = 2, 2026-05 = 21, 2026-06 = 14, 2026-07 = 5, 2026-08 = 9, 2026-09 = 13. Lo que omite:
  - **octubre de 2025 = 0.** El último `lastmod` de septiembre de 2025 es del 10-09 y el siguiente del 23-11-2025: **74 días sin una sola URL nueva o modificada**. El rango «de 2 a 21 al mes» empieza en realidad en 0;
  - **septiembre de 2026 tiene 13 URL**, no 10. Las del 01-09 («Una tarde de béisbol en Fenway Park») y las dos del 03-09 de madrugada ya no caben en un feed de 10 ítems. Por eso el feed da 10;
  - **en los 12 meses (2025-10-10 → 2026-10-10) hay 95 URL**, unas 8 al mes de media, con huecos de 28 días (23-11 → 21-12-2025), 25 días (04-02 → 01-03-2026) y 23 días (26-07 → 19-08-2026);
  - el `lastmod` del 2026-07-04 corresponde a la pieza de Pichilín, publicada el 28-04-2026 y modificada ese día (`"dateModified":"2026-07-04T16:22:48+00:00"`). Confirma que el `lastmod` es una aproximación.
- **Las 332 h de la ficha, que el revisor no pudo reconstruir, se reconstruyen:** el último `lastmod` antes del 2026-08-09 es 2026-07-26T23:01:44Z, y el siguiente es del 19-08. Desde esa hora, 332 h llevan al 2026-08-09 hacia las 19:00 UTC, que es el día de la ficha. **La medición de la ficha era correcta para su fecha.** Lo inexacto hoy es la palabra «parado» en la cabecera.
- **«0 artículos» en el bloque de conducta medida:** el medio no está en `shared/mediaRegistry.js` (0 coincidencias de «sucre» o «sincelejo») y nadie lo ingiere. El revisor lo marcó como inferencia; aquí queda **comprobado**. Responde a la pregunta del plan de la tanda («Sin artículos en la ventana: hay que ver por qué»): no hay artículos porque no se ingiere, no porque no publique.

**2 · La voz de la casa.**
- **`/category/opinion/editorial/feed/`** (2026-10-10), del más reciente al más antiguo: «Un pequeño genio camina entre nosotros.» (Jhony Polo Barrios, 12-08-2022); «Editorial-25 de septiembre de 2021: Desde el desayuno se sabe cómo será el almuerzo» (Redacción); «Editorial-18 de diciembre de 2020: Control al controlador»; «Editorial-10 de diciembre de 2020: ¿Quién interviene a la interventora del HUS?»; y anteriores, hasta 2019. Coincide con el revisor. La pieza de 2022 la firma una persona: **el último editorial institucional es del 25-09-2021.**
- **`/category/opinion/columnistas/feed/`** y **`/category/opinion/feed/`**: lo más reciente es «Monseñor Nel Beltrán: un obispo con tino y con tacto» (Redacción, 18-08-2025) y, antes, «“Habemus papam”: ¿qué indica el nombre de León XIV?» (Jhony Polo Barrios, 10-05-2025). Ninguna pieza de opinión dentro de los 12 meses. Exacto.
- Consecuencia, con el revisor: la regla de la evidencia editorial histórica (DECISIONES 2026-10-09) no tiene material. **No hay voz de la casa medible.**

**3 · «Especial» y el contenido institucional.**
- **`/category/especial/feed/`** (2026-10-10): 10 ítems, del 13-05 al 20-08-2026. Las fechas, los títulos y la pieza duplicada («Colombia se posiciona como referente regional…», 15-05 y 22-05-2026) coinciden con el revisor.
- **Rótulos, buscados en el HTML crudo de las 10.** El revisor buscó «patrocinad», «publirreportaje», «contenido pagado» e «informe comercial», y es cierto que no aparecen. Pero **8 de las 10 llevan, en el subtítulo (`<p class="td-post-sub-title">`), una marca de procedencia**:
  - «Informe de gestión»: las cuatro del Gobierno nacional («Superada la meta de formación en talento digital del Gobierno Petro…», 21-05; «Con cerca de 6.000 kilómetros de fibra óptica…», 28-05; y las dos «Colombia se posiciona…», 15-05 y 22-05);
  - «Informe corporativo» o «Informe corportativo» (así, con la errata): tres de Afinia («Afinia sigue impulsando el desarrollo…», 15-05; «Afinia fortalece su clima laboral…», 20-05; «En Afinia le aportan al desarrollo…», 22-05);
  - «Información corporativa»: la de Veolia («Conozca el proyecto Plan Sur Fase I…», 20-08).
  - **Sin ninguna marca:** «Afinia convierte la pasión por el fútbol…» (13-05) y «El Grupo EPM se prepara con responsabilidad…» (19-05).
  - Ninguna dice «publicidad», «pauta» ni «pagado». En el HTML de todas aparece la palabra «publicidad», pero solo por el correo `publicidad@` del pie.
- **Firmas:** 9 de las 10 van como «Redacción». **La de EPM la firma José Iriarte Díaz**, y es una de las dos sin rótulo. El revisor la mete entre los textos «firmados "Redacción"».
- **Citas comprobadas:** «Bogotá, mayo de 2026. (@Ministerio_TIC) – En menos de cuatro años, el Gobierno del presidente Gustavo Petro multiplicó el acceso digital a la educación» (pieza del 21-05, 3 apariciones en el HTML). «En Veolia, estamos convencidos de que el agua es el motor que impulsa el bienestar de las familias sincelejanas» (20-08). Ambas literales.
- **Pichilín:** «El Gobierno avanza en la reparación a las víctimas de Pichilín», sección Municipios, `datePublished` 2026-04-28. Incrusta `…/wp-content/uploads/2026/07/[correo omitido]4`. Literal. El vídeo está en la carpeta de julio y la pieza se modificó el 04-07-2026: se añadió o se cambió después de publicarse. No tiene rótulo de procedencia.
- **Fuera de «Especial»,** la pieza del 30-09-2026 «Afinia denuncia la reconexión ilegal del acueducto de San Onofre» (Judicial, José Iriarte Díaz) trae la versión de Afinia. No se le ve rótulo; no se evaluó si es comunicado.
- **Hecho y no hecho.**
  - **Hecho:** entre mayo y agosto de 2026 el medio publicó en «Especial» 10 piezas de origen institucional o corporativo (Gobierno nacional, Afinia/Grupo EPM y Veolia). 8 llevan una marca de procedencia en el subtítulo, ninguna se marca como publicidad, y 2 no llevan nada.
  - **No es hecho:** que sean pauta pagada. Encaja con el `publicidad@` y con «Para pautar con nosotros», pero no hay contrato ni factura.
  - **Polo fijo:** reproducir comunicados del gobierno saliente no es posición en el eje. Coincidimos con el revisor.

**4 · Las firmas.**
- **`author-sitemap.xml`** (2026-10-10): 8 URL de autor: `jennycarolinagonzalez`, `acelisconeobarboza`, `edithguerraalvarez`, `jiriartediaz_z36q236e`, `joseiriartediaz`, `jpolobarrios`, `marioruizsoto` y `favindiazbrieva`. Coincide con el revisor.
- **Lo que el revisor no vio:** `/author/jiriartediaz_z36q236e/` tiene por título «Redacción, autor en sucrenoticiasof». Las piezas firmadas «Redacción» enlazan a esa cuenta (comprobado en la de Veolia y en la de la ESE San Francisco de Asís). **La firma de la casa sale de una cuenta cuyo identificador lleva el nombre de José Iriarte Díaz.** Es un indicio de que él maneja la cuenta de la Redacción, no la prueba de que dirija el medio, y menos de que sea su dueño. No entra como hecho.
- **`/author/joseiriartediaz/`**, la parte profesional, literal: «Comunicador social (UNAD) y periodista, becario de la Fundación Gabriel García Márquez para el Nuevo Periodismo Iberoamericano». La palabra que sigue es un dato de origen y no se reproduce.
- **Ningún cargo** (director, editor, gerente) en la portada ni en `/contacto/`: búsqueda de «director» y «directora» en el texto de las dos, 0 resultados.

**5 · Citas de la ficha sin fuente.**
- «un medio de comunicación independiente honesto e imparcial»: literal en `https://sucrenoticias.com/contacto/` (2026-10-10), bajo «¿Quiénes somos?».
- «alternativa informativa y periodística independiente y de calidad»: literal en el pie de `https://sucrenoticias.com/`.
- «dos correos y un teléfono»: exacto (`contacto@`, `publicidad@` y un teléfono en `/contacto/`).
- La ficha no da ninguna URL ni fecha. Aceptada.

**6 · Registros.**
- **RUES** (`c82u-588k`, 2026-10-10):
  - '%SUCRE NOTICIA%' y '%SUCRENOTICIA%': 0 filas. Exacto.
  - '%NOTICIAS SUCRE%' o '%NOTICIAS DE SUCRE%', y '%SUCRE%NOTICI%' o '%NOTICI%SUCRE%': 1 fila, «TELENOTICIAS DE SUCRE SAS» (Sincelejo, activa, matrícula 2023-05-15, último año renovado 2025, **CIIU 5911**, producción audiovisual).
  - '%SINCELEJO NOTICIA%': 1 fila, «SINCELEJO NOTICIAS S.A.S» (Sincelejo, activa, matrícula 2018-06-27, último año renovado 2024, **CIIU 6010**, radiodifusión).
  - En la Cámara de Sincelejo, '%NOTICI%', '%PERIODI%' y '%DIGITAL%'+'%MEDIO%': 8 filas, entre ellas las dos anteriores, «ENFOQUE PERIODICO DIGITAL S.A.S.», asociaciones de periodistas y un periódico en liquidación. Ninguna con el nombre del medio.
  - Recuento por `categoria_matricula`: «PERSONA NATURAL» 6.962.889 y «SOCIEDAD ó PERSONA JURIDICA PRINCIPAL ó ESAL» 2.473.441. Exacto, como dice el revisor. **No hay establecimientos de comercio** en el conjunto.
- **Las homonimias, más allá del revisor.** «SINCELEJO NOTICIAS S.A.S» se matriculó el 2018-06-27, un mes después del registro del dominio (2018-05-24) y tres semanas después de la primera página del sitio (2018-06-05). **La coincidencia en el tiempo no prueba nada.** mapeomedios.com lista un «Sincelejo Noticias SN», con sus propias redes y su propio director, distinto de Sucre Noticias. La lectura más plausible es que esa sociedad sea la de ese otro medio. El CIIU de radiodifusión no encaja con un diario digital. **No se atribuye.**
- **SECOP, búsquedas del revisor:** `jbjy-vk9h` (objeto, descripción y proveedor) y `f789-7hwg` (objeto y contratista): 0 filas. Exacto.
- **SECOP II, procesos (`p6dx-8zbt`), que el revisor no consultó: 2 filas.** Las dos son del **Sorteo Extraordinario de Colombia L.T.D.A.** (Extradec, Bogotá), modalidad «Contratación régimen especial»:
  - **EXTRADEC-138-2024** (`CO1.REQ.6562799`), publicado el 2024-07-24, precio base $3.000.000, 3 meses. Objeto, literal: «PROMOCION PUBLICITARIA POR MEDIO DEL ESPACIO NOTICIOSO SUCRE NOTICIAS QUE SE TRASMITE POR LAS PLATAFORMAS DE FACEBOOK SUCRE NOTICIAS, SISTEMA DIGITAL CARIBE Y KORRALEJA.CO, TRASMITIDO A NIVEL NACIONAL E INTERNACIONAL EN EL HORARIO DE 7:00 AM A 8 AM DE LUNES A VIERNES PARA PROMOCIONAR LOS SORTEOS QUE REALICE EL SORTEO EXTRAORDINARIO DE COLOMBIA».
  - **EXTRADEC-178-2024** (`CO1.REQ.7084611`), publicado el 2024-10-28, precio base $5.000.000, 101 días. Objeto, literal: «PROMOCION PUBLICITARIA POR MEDIO DE LA EMISORA PRIMAVERA ESTEREO 88,3 FM Y POR LAS PLATAFORMAS DE STREAMING AUDIO DE KORRALEJA.COM, SUCRE NOTICIAS, PAGINAS DE DEPORTTES Y SOCIEDAD Y DANNY DEPORTES PARA PROMOCION PUBLICITARIA DE LA IMAGEN Y LOS SORTEOS DEL EXTRADEC LTDA PARA EL AÑO 2024 […] EN LA CIUDAD DE SINCELEJO».
  - En los dos: «adjudicado» «No», proveedor «No Definido», «valor_total_adjudicacion» 0, estado «Publicado».
  - Por `proceso_de_compra` (`CO1.BDOS.6437488` y `CO1.BDOS.6952620`), `jbjy-vk9h` da **0 contratos**. Esa entidad no tiene **ningún** contrato en `jbjy-vk9h` (búsqueda por `codigo_entidad` y por nombre). Que no figuren adjudicados puede ser un límite del conjunto en régimen especial, no la prueba de que no se contrataran.
  - **Lo que es hecho:** en 2024, una entidad pública publicó dos procesos de publicidad cuyo objeto nombra un «espacio noticioso SUCRE NOTICIAS» transmitido por Facebook y por plataformas de Korraleja.co.
  - **Lo que no es hecho:** que ese espacio sea `sucrenoticias.com`. El objeto no nombra el dominio. Y el sitio, en ninguno de sus seis sitemaps ni en las páginas descargadas, nombra a Korraleja, Extradec ni «Sistema Digital Caribe». El sitio enlaza una página de Facebook llamada «Sucre-Noticias», lo que hace el vínculo **verosímil, no probado**. Tampoco consta un contrato, un pago ni quién habría sido el proveedor. Los dos procesos son de 2024 y quedan **fuera de los 12 meses**.
  - **Por qué importa:** si el vínculo se confirma, Sucre Noticias y Korraleja, los dos candidatos de Sucre, aparecerían vendidos juntos a una entidad pública, y el nivel 1 de los dos tendría por dónde empezar.
- **Límite que el revisor declara bien:** sin NIT no hay consulta por igualdad exacta. Y sin establecimientos en el RUES abierto, la vía es el buscador de `rues.org.co` o un certificado de la Cámara de Comercio de Sincelejo. Tampoco se hizo aquí.

**7 · mapeomedios.com.**
- `https://www.mapeomedios.com/api/municipios` (2026-10-10): `"success":true`, 28 municipios, **38 medios** (25 en Sincelejo). En todo el JSON: «sucre noticias» no aparece, «sucrenoticias» no aparece, «iriarte» no aparece. Exacto.
- Lista, en cambio, Korraleja.co, «El Meridiano sede Sincelejo», «Sincelejo Noticias SN» y «Sucre Informativo» (dos fichas con ese nombre). La refutación 3 de la ficha queda agotada para este medio. Para el departamento, mapeomedios ofrece otros candidatos, casi todos de redes sociales y sin sitio propio.

**Evidencia que no mueve el número.** Comprobada en el HTML crudo:
- «Los Nunca, la apuesta política de Abelardo de la Espriella» (Redacción, 19-05-2026): «Foto: campaña» y «Según la campaña, el movimiento está integrado por personas que trabajan, pagan impuestos» aparecen, literales.
- «Sincelejo marchará en respaldo al candidato presidencial Iván Cepeda» (Redacción, 04-06-2026): «Según los organizadores, la jornada busca respaldar las propuestas de Cepeda», literal.
- «Embajadora María Consuelo Araujo presenta cartas credenciales ante el presidente Donald Trump» (Jenny Carolina González, 16-09-2026): «tuvo que reaccionar a la decisión de éste país de mantener la descertificación», literal.
- Las dos piezas de fiscalización electoral (31-05 y 21-06-2026) están en el feed de «Sucre elige» con esas fechas.
- Atribución simétrica y ningún endoso, como dice el revisor. Una pieza sobre el nuevo Gobierno no permite medir nada.

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se rechazan como hecho, o se corrigen, estas partes:
- **Obj. 1, «unas 10 piezas al mes en septiembre de 2026»:** el sitemap da 13; el feed da 10 porque solo muestra 10 ítems.
- **Obj. 1, «de 2 a 21 al mes desde septiembre de 2025»:** octubre de 2025 tiene 0, dentro de un hueco de 74 días.
- **«Lo que no pude verificar», la cifra de 332 h:** sí se puede reconstruir, y cuadra.
- **Obj. 3, «sin ninguna etiqueta de publicidad» y «comunicados sin rótulo»:** sin etiqueta de *publicidad*, sí; sin *rótulo*, no. 8 de 10 llevan «Informe de gestión», «Informe corporativo» o «Información corporativa». La marca es débil (dice la procedencia, no si es pagado), pero existe, y la ficha corregida tiene que decirlo.
- **Obj. 3, la pieza de EPM entre los textos «firmados "Redacción"»:** la firma José Iriarte Díaz.
- **Obj. 6, «SECOP sin resultado»:** sin resultado en contratos; con 2 procesos de 2024 en el conjunto de procesos, que no se consultó.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente.** Todas las URL del sitio que cita el revisor o que se usaron aquí respondieron 200 el 2026-10-10, salvo `/wp-json/wp/v2/users` (401, como dice). Las consultas de RUES y SECOP devuelven lo que dice, con las cifras exactas. Deformaciones y omisiones:
- el rótulo de procedencia de 8 de las 10 piezas de «Especial», que no ve;
- la firma de la pieza de EPM;
- el recuento de septiembre de 2026 (10 por 13) y el 0 de octubre de 2025;
- el conjunto de procesos de SECOP II, que no consulta;
- la cuenta «Redacción» con identificador `jiriartediaz_z36q236e`;
- el RDAP del registrador, que dice no haber consultado (no cambia nada: el titular está oculto).

**Errores de la propia ficha, para no repetirlos:**
- **Confunde «no hay número» con «no se da de alta».** La regla 3 impide *firmar* un número sin nivel 1-3. No impide el alta con 0,00 provisional y `ownerType: null`, que el catálogo admite desde el 2026-08-11 (AUSENCIA DECLARADA, en `shared/mediaOwnership.js`). Así entraron La Razón.co (Montería), EL DIARIO de Boyacá, Vive el Meta, Lente Regional, LeticiaHoy y Quindío Noticias, este con el «nivel 1 vacío del todo». El motivo 1 de la ficha no es un motivo para no dar de alta.
- **«El Meridiano… resolverlo desbloquea Córdoba y Sucre a la vez»:** desfasado. Córdoba tiene medio propio desde el 2026-08-11 (La Razón.co). `COBERTURA_DEPARTAMENTAL.md` ya lo dice: «ya no desbloquea dos departamentos, desbloquea uno».
- **«el feed está parado»** en la cabecera: era una medición de un día (exacta para el 2026-08-09) convertida en estado. Hoy el medio publica de forma esporádica.
- **«no dice quién lo sostiene»:** declara que vende pauta (`publicidad@`, «Para pautar con nosotros») y publica contenido institucional con marca de procedencia.
- **Ninguna cita con URL ni fecha.**
- **No fue a la sección editorial**, que existe y está inactiva desde 2021.
- **Falta la línea de contratación pública** que exige el protocolo desde el 2026-10-07.
- **«Es el candidato con el nivel 1 más vacío de los dieciséis»:** discutible, porque el sitio publica firmas con nombre. No es un error de hecho, pero conviene matizarlo.

**Lo que la ficha sí tenía bien:**
- las 332 h, exactas para su fecha;
- las dos citas de nivel 4 y el «dos correos y un teléfono»;
- la ausencia de sociedad, NIT, propietario, director y editor publicados;
- Korraleja sin feed: `https://www.korraleja.co/feed/` sigue dando 404 el 2026-10-10.

---

**Propuesta para la firma**

**Contexto que decide.** Sucre es el único departamento que el catálogo deja en blanco teniendo medios con sitio web. Desde el 2026-09-23 el catálogo cubre 30 de 33 departamentos, y Guainía y Vaupés están declarados sin medio propio con sitio. `shared/mediaRegistry.js` no tiene ningún medio de Sucre, y El Meridiano sigue con 403 y sin feed. Sucre Noticias es hoy el único candidato de Sucre con un feed que responde.

**Estado de la candidatura: alta con 0,00 provisional, sin firma (opción c), con `ownerType: null` y la ausencia declarada.** Es una recomendación, no una conclusión de la revisión: el revisor y la ficha recomiendan no darlo de alta. Motivo:
- los dos motivos de la ficha no se sostienen. El motivo 1 (regla 3) impide firmar, no dar de alta. El motivo 2 (feed parado) es falso hoy;
- el medio está vivo, con agenda local propia y fiscalizadora (Procuraduría y Unisucre, la ESE de Sincelejo, coacciones electorales en San Antonio de Palmito);
- su cadencia es irregular, pero no peor que la de LeticiaHoy cuando entró (7 piezas en 15 días, «antes una al mes»): 13 en septiembre de 2026 y 95 en 12 meses;
- su feed WordPress responde 200 y es ingerible;
- dejar Sucre en blanco le dice al lector «aquí no hay medios» cuando lo cierto es «no sabemos de quién es». Es la distinción que motivó AUSENCIA DECLARADA.

**Alternativa conservadora (a): en espera**, con la razón reescrita (abajo). Es lo que propone el revisor y sería coherente si el responsable editorial prefiere no sumar otro medio sin dueño. **Se desaconseja (b), descartar:** no hay inactividad prolongada (último ítem del 30-09), ni vínculo oculto probado, ni robots que lo impida.

**Texto del `biasRationale` si se da de alta:**

> Medio digital de Sincelejo (sucrenoticias.com, dominio de 2018), con agenda local propia y la mayoría de las piezas firmadas por un mismo periodista. Sin dueño ni director publicados. No tiene voz editorial desde 2021, y su sección «Especial» publica informes de gestión del Gobierno nacional y contenidos de empresas (Afinia/EPM, Veolia), marcados como tales pero no como publicidad. Orientación mixta provisional por ausencia de evidencia de nivel 1-3 — ver fichas/sucre-noticias.md.

**Ausencia declarada para `mediaOwnership.js`** (`ownerType: null`, `consultadoEl: '2026-10-10'`):
- `buscadoEn`:
  - el propio medio: portada, `/contacto/`, pie, JSON-LD («Organization: sucrenoticiasof», sin razón social), autores y siete rutas legales con 404. Resultado: no declara sociedad, propietario ni cargos; publica firmas;
  - RDAP del registro y del registrador: titular oculto;
  - RUES abierto por razón social: 0 coincidencias; homonimias sin vínculo, que no se atribuyen;
  - SECOP I y II por nombre: 0 contratos; 2 procesos de Extradec (2024) nombran un «espacio noticioso SUCRE NOTICIAS» en Facebook y Korraleja.co, sin adjudicación en los datos abiertos y sin vínculo probado con el sitio;
  - mapeomedios.com: no lo lista.
- `falta`: búsqueda por nombre de establecimiento en `rues.org.co` o certificado de la Cámara de Comercio de Sincelejo; el expediente público de SECOP de EXTRADEC-138-2024 y EXTRADEC-178-2024; que el medio publique quién lo dirige.
- `group`: `null`. `ownerType`: `null`, nunca «familiar» ni «independiente» (DECISIONES 2026-10-09).

**Condición de revisión, si entra:** se aplica la regla de los 30 días de la nota de Vorágine. Si la cadencia grabada muestra más de 30 días sin publicar, se decide la baja. En los últimos 12 meses ya hubo un hueco de 74 días (septiembre-noviembre de 2025), así que la condición tiene que estar escrita, no supuesta.

**Razón reescrita si queda en espera (a):**

> En espera, no descartado. Publica de forma esporádica: 95 URL en 12 meses, 13 en septiembre de 2026, con un hueco de 74 días entre septiembre y noviembre de 2025. No declara dueño, director ni sociedad, y el titular del dominio está oculto. No tiene voz editorial desde 2021. Se reabre si aparece su titular (RUES por establecimiento, certificado de la Cámara de Comercio de Sincelejo o el expediente de los procesos de Extradec de 2024) o si sostiene una cadencia útil 90 días.

**Correcciones de hecho en `fichas/sucre-noticias.md`** (valen para las dos opciones):
1. **Cabecera:**
   - «Valor propuesto»: «**0,00 provisional**, sin firma — sin nivel 1-3; alta con propiedad no comprobada» (opción c) o «**ninguno** — en espera: sin nivel 1 y cadencia esporádica» (opción a);
   - añadir «Revisión: ciclo 2, tanda 7, 2026-10-10».
2. **Nivel 1** se reescribe con fuentes y fecha:
   - «No publica sociedad, NIT, propietario, director ni editor (`/contacto/` y pie, 2026-10-10). Su JSON-LD declara una "Organization" llamada "sucrenoticiasof", sin razón social. No tiene aviso legal, política de privacidad ni términos.
   - Dominio registrado el 2018-05-24, renovado (último cambio 2026-05-25, vence 2027-05-24); el titular está oculto en el RDAP del registrador.
   - Publica firmas: ocho cuentas de autor. La mayoría de las piezas de septiembre de 2026 las firma José Iriarte Díaz, y la cuenta "Redacción" tiene un identificador con su nombre. Que dirija el medio no consta.
   - Declara que vende pauta (`[correo omitido]`)».
   - El teléfono no se escribe.
3. **Contratación pública**, línea nueva en el formato del protocolo:

> Contratación pública (SECOP I y II, por nombre, sin NIT conocido; consultado 2026-10-10): 0 contratos en los últimos 12 meses y 0 en total. Sin NIT no cabe la consulta exacta. En el conjunto de procesos de SECOP II, el Sorteo Extraordinario de Colombia (Extradec) publicó en 2024 dos procesos de publicidad cuyo objeto nombra un «espacio noticioso SUCRE NOTICIAS» transmitido por Facebook y por plataformas de Korraleja.co (EXTRADEC-138-2024, base $3.000.000; EXTRADEC-178-2024, base $5.000.000). Ninguno figura adjudicado y no hay contrato asociado en los datos abiertos. Que ese espacio sea este sitio no está probado.

4. **Nivel 4:** añadir las URL (`https://sucrenoticias.com/contacto/` para «independiente honesto e imparcial»; el pie de `https://sucrenoticias.com/` para «alternativa informativa…») con fecha 2026-10-10. Cambiar «no dice quién lo sostiene» por «no dice quién es su dueño; declara que vende pauta».
5. **Nivel 2:** «El feed llevaba 332 h sin artículo nuevo el 2026-08-09 (último `lastmod` del sitemap: 2026-07-26 23:01 UTC). El 2026-10-10 publica de forma esporádica: 95 URL en 12 meses por `lastmod` (aproximación), 13 en septiembre de 2026, 0 entre el 10-09 y el 23-11-2025. Último ítem: 30-09-2026. Sin corpus propio: el medio no se ingiere».
6. **Sección nueva, «Voz de la casa»:** «La categoría Editorial existe (`/category/opinion/editorial/`) y su último editorial institucional es del 25-09-2021. La última pieza de opinión es del 18-08-2025. En los 12 meses no hay voz de la casa medible».
7. **Sección nueva, «Contenido institucional»** (desvelamiento, no acusación): «En "Especial", de mayo a agosto de 2026, 10 piezas del Gobierno nacional (informes de gestión del MinTIC y del sector TIC), de Afinia/Grupo EPM y de Veolia. 8 llevan en el subtítulo "Informe de gestión", "Informe corporativo" o "Información corporativa", 2 no llevan marca y ninguna se marca como publicidad. Que sea pauta pagada no consta». Por el polo fijo, no mueve el eje.
8. **«Por qué no se propone número»** se reescribe: queda solo el motivo 1, como razón para no *firmar*. El motivo 2 se retira (opción c) o se cambia por «cadencia esporádica» (opción a).
9. **«Sucre se queda en blanco…»:** quitar «desbloquea Córdoba y Sucre a la vez». Poner: «Córdoba tiene medio propio desde el 2026-08-11 (La Razón.co); El Meridiano solo desbloquearía Sucre». Korraleja sigue sin feed (404, 2026-10-10).
10. **REFUTACIÓN:** el punto 3 (mapeomedios) se marca como hecho, sin resultado para este medio. Se añade un punto 4: «el expediente de los procesos EXTRADEC-138-2024 y EXTRADEC-178-2024 en SECOP, para saber si el "espacio noticioso SUCRE NOTICIAS" es este medio y quién lo factura».

**Fuera de la ficha:**
11. `fichas/LEEME.md`, fila de `sucre-noticias.md`: «Falta el nivel 1, y el feed está parado» → «0,00 provisional, propiedad no comprobada; publica de forma esporádica» (c), o «En espera: sin nivel 1 y cadencia esporádica» (a).
12. `MEDIOS_CANDIDATOS_DEPARTAMENTOS.md`:
    - tabla de feeds, fila de Sucre: «**332 h** ⚠» → «10 días a 2026-10-10 (13 piezas en septiembre) · ciclo 2»;
    - tabla de fichas: «**sin número**: nivel 1 vacío + feed parado 14 días» → «0,00 provisional · propiedad no comprobada · cadencia esporádica · ciclo 2, 2026-10-10» (c), o «**en espera**: nivel 1 vacío + cadencia esporádica · ciclo 2, 2026-10-10» (a);
    - «Sucre Noticias — nada, y encima el feed lleva catorce días parado»: añadir nota fechada;
    - «deja dos departamentos sin voz» (El Meridiano): nota de que Córdoba ya está cubierto;
    - «queda una pista sin explorar para Sucre: mapeomedios.com»: «explorada el 2026-10-10: 38 medios, no lista a Sucre Noticias».
13. `COBERTURA_DEPARTAMENTAL.md`: si entra (c), Sucre deja de estar en blanco y el catálogo pasa a 31 de 33. Hay que actualizar «Sucre está cerrado por vía técnica» y la nota del 2026-09-23 («Sucre sigue como estaba»). Si queda en espera (a), basta una nota fechada: el candidato publica y lo que falta es el nivel 1.
14. Si entra: entrada en `shared/mediaRegistry.js` (feed `https://sucrenoticias.com/feed/`, `departamento: 'Sucre'`, `bias: 0.0`, `reviewedAt: null`) y en `shared/mediaOwnership.js` con la ausencia declarada de arriba. No lo hace esta resolución.

**¿Aviso de quien dirige?** No procede. No hay director publicado, y nada indica candidatura ni cargo público de quien firma.

**Lo que NO entra como hecho:**
- que las piezas de «Especial» sean pauta pagada;
- que el «espacio noticioso SUCRE NOTICIAS» de los procesos de Extradec sea `sucrenoticias.com`, y que se contratara;
- que José Iriarte Díaz dirija o posea el medio, aunque la cuenta «Redacción» lleve su nombre en el identificador;
- cualquier vínculo con «SINCELEJO NOTICIAS S.A.S» o «TELENOTICIAS DE SUCRE SAS»;
- la región visible en el RDAP del registrador, que no identifica a nadie.

**Decisiones para el responsable editorial:**
1. **Estado de la candidatura.** Recomendación: **(c) alta con 0,00 provisional, `ownerType: null` y la ausencia declarada**, con la condición de los 30 días escrita. Es lo que el catálogo hizo con LeticiaHoy y Quindío Noticias, y Sucre es el único departamento con medios web que sigue en blanco. Alternativa defendible: **(a) en espera**, como piden el revisor y la ficha. No se recomienda (b).
2. **Cómo se nombra el contenido de «Especial».** Recomendación: «informes de gestión y contenidos corporativos marcados como tales, no como publicidad», y **no** «comunicados sin rótulo» (8 de 10 llevan rótulo) ni «pauta» (no consta).
3. **Los procesos de Extradec.** Recomendación: anotarlos en la línea de contratación como procesos, con «vínculo no probado». Abrir el expediente público de SECOP solo si el medio entra o si se reabre la espera. Puede traer datos de personas naturales, y habría que leerlo con la regla de datos personales.
4. **Gasto.** Recomendación: **no** pedir todavía el certificado de la Cámara de Comercio de Sincelejo ($12.100). Antes conviene la búsqueda gratuita por establecimiento en `rues.org.co`, que nadie ha hecho.
