# Respuesta — Claude Opus 5.5 sobre Diario del Sur

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
Soy Claude Opus 5.5 (claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Mi acuerdo no debe contarse como aval independiente. Para compensarlo he buscado sobre todo en fuentes que la ficha no usa: RUES abierto (datos.gov.co c82u-588k), SECOP I y II, el historial de robots/feed/sitemap en el Internet Archive y la Wikipedia en español. Revisión hecha el 2026-10-10.

MÉTODO Y DÓNDE BUSQUÉ
- robots.txt de diariodelsur.com.co, descargado hoy (2026-10-10). Literal: "User-agent: ClaudeBot / Disallow: /", "User-agent: anthropic-ai / Disallow: /", "User-agent: Claude-Web / Disallow: /", "User-agent: Claude-User / Disallow: /", más "Content-Signal: search=yes,ai-train=no,use=reference" y "Sitemap: https://www.diariodelsur.com.co/sitemap.xml". POR ESO NO DESCARGUÉ NADA MÁS DEL SITIO: ni portada, ni feed, ni sitemap, ni sección de editoriales. Tampoco abrí copias archivadas de su contenido. Del Internet Archive solo usé metadatos CDX (URL, fecha, código HTTP y tipo) y copias archivadas del propio robots.txt.
- RUES abierto: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] , el mismo recurso con nit=901804010 y una búsqueda con razon_social LIKE '%DIARIO DEL SUR%'.
- SECOP II (jbjy-vk9h), documento_proveedor = 891222292 y = 901804010 por igualdad exacta y sin DV. Además, una consulta de control con DV (8912222921) y otra por proveedor_adjudicado LIKE '%DIARIO DEL SUR%' / '%EDICIONES PERIODISTICAS%'.
- SECOP I (f789-7hwg), identificacion_del_contratista = 891222292 y = 901804010.
- empresas.larepublica.co, la fuente que cita la ficha: robots.txt "User-agent: * Allow: /". Páginas de los NIT 891222292 y 901804010, HTML crudo.
- es.wikipedia.org/wiki/Diario_del_Sur_(Colombia), HTML crudo, solo la ruta /wiki/.
- Buscador web, 3 consultas: "Ediciones Periodísticas Diario del Sur"; "Diario del Sur Pasto liquidación nueva empresa director 2026"; "Hernando Suárez Burgos" 2026. El buscador estuvo disponible. Sus resúmenes no los cito como hecho, porque no pude abrir el crudo de las páginas del medio.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré una venta documentada. Sí encontré algo que la ficha no tiene: otra sociedad con el nombre del diario factura publicaciones "en el periódico Diario del Sur". Es EDICIONES PERIODISTICAS DIARIO DEL SUR S.A.S, NIT 901804010, matriculada en la Cámara de Comercio de Bogotá el 2024-02-22. Figura ACTIVA, con la última renovación el 2026-07-14 (RUES abierto, consultado el 2026-10-10). La sociedad nació antes de los últimos 12 meses, pero facturó dentro de ellos (ver objeción 2). No está documentado si hubo cesión de la marca o del negocio desde la sociedad en liquidación: es inferencia.
- ¿La persona que la ficha nombra como titular sigue viva y en el cargo?
  No lo pude comprobar. La búsqueda web "Hernando Suárez Burgos" 2026 no devolvió nada pertinente (2026-10-10). La Wikipedia en español, con su última edición el 2026-09-17, sigue nombrándolo "propietario" y "Director". Es fuente editable, de nivel 4 como mucho, y no prueba que siga en el cargo.
- ¿Quién dirige hoy la redacción?
  No encontré un nombre en una fuente primaria. La Wikipedia (dateModified 2026-09-17) da como "editor jefe" a Robert Atis Bernal y como director a Hernando Suárez Burgos. No pude contrastarlo con el sitio del medio, porque su robots.txt excluye a los agentes de Anthropic.
- ¿Hay un registro mercantil más reciente que la fuente que cita la ficha?
  Sí, por dos vías. (a) El RUES abierto del NIT 891222292 trae "fecha_actualizacion": "2025/03/11", "estado_matricula": "ACTIVA" y "razon_social": "GRUPO EDITORIAL DIARIO DEL SUR SAS EN LIQUIDACION", con "ultimo_ano_renovado": "2024". Contradice el "Cancelada" de la ficha (objeción 1). (b) El RUES abierto del NIT 901804010 está actualizado al 2026/07/14, con "representante_legal": "MIGUEL ANGEL ARELLANO CANTILLO" (se toma del RUES, no de SECOP).

## OBJECIONES

OBJECIÓN 1. "Matrícula RUES: Cancelada" no está probado por un primario y choca con el RUES abierto.
- QUÉ afirma la ficha: que la editora, NIT 891222292, tiene la matrícula cancelada. Su fuente es un agregador, empresas.larepublica.co.
- POR QUÉ:
  · El agregador dice literal "¿Registro RUES activo?" … "No / Cancelado" (HTML crudo, 2026-10-10). La página no fecha el dato.
  · El conjunto abierto del RUES (c82u-588k), que es más primario, dice "estado_matricula":"ACTIVA" con "razon_social":"GRUPO EDITORIAL DIARIO DEL SUR SAS EN LIQUIDACION", "fecha_renovacion":"20241030" y "fecha_actualizacion":"2025/03/11 09:51:49".
  · Hecho: las dos fuentes coinciden en que la sociedad está EN LIQUIDACIÓN y discrepan en si la matrícula está cancelada.
  · Inferencia: el conjunto abierto lleva sin actualizarse desde marzo de 2025, y la cancelación puede ser posterior. Ninguna de las dos es un certificado de existencia y representación legal.
  · La ficha debería decir "en liquidación (ambas fuentes); cancelación solo según un agregador sin fecha" y pedir el certificado de la Cámara de Comercio de Pasto (matrícula 13825).
- FUENTE: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (registro actualizado el 2025-03-11, consultado el 2026-10-10); https://empresas.larepublica.co/colombia/narino/pasto/grupo-editorial-diario-del-sur-sas-891222292 (consultado el 2026-10-10, sin fecha propia).
- NIVEL: registro externo, de propiedad.

OBJECIÓN 2. La ficha da por única editora a una sociedad en liquidación, y existe otra sociedad activa que factura el periódico.
- QUÉ afirma la ficha: que la editora es Grupo Editorial Diario del Sur S.A.S. y que reabrir el expediente exigiría "que aparezca una editora con matrícula activa tras la liquidación" (refutación 2).
- POR QUÉ:
  · RUES abierto, NIT 901804010: "razon_social":"EDICIONES PERIODISTICAS DIARIO DEL SUR S.A.S", "camara_comercio":"BOGOTA", "fecha_matricula":"20240222", "estado_matricula":"ACTIVA", "ultimo_ano_renovado":"2026", "cod_ciiu_act_econ_pri":"1811" (impresión), "cod_ciiu_act_econ_sec":"5813" (edición de periódicos), "representante_legal":"MIGUEL ANGEL ARELLANO CANTILLO". El agregador de La República lo confirma con "¿Registro RUES activo?" … "Si".
  · SECOP I, contratista 901804010, firmado el 2025-07-24 con la Alcaldía de La Florida (Nariño), 5.000.000 COP. Objeto literal: "PUBLICACIoN DE MEDIA PaGINA FULL COLOR EN EL PERIoDICO DIARIO DEL SUR SOBRE AVANCE DE GESTIoN Y PROYECTOS ADELANTADOS POR LA ADMINISTRACIoN MUNICIPAL DE LA FLORIDA NARIÑO…" (constancia 25-12-14483129).
  · SECOP I, firmado el 2026-09-11 con la Cámara de Comercio de Tumaco, 2.700.000 COP. Objeto: "PUBLICACION DE LOS TERMINOS DE REFERENCIA PARA LA ELECCION DEL REVISOR FISCAL…" (constancia 26-4-14802452, contrato OCS-025-2026).
  · Hecho: una sociedad activa vende espacio en "el periódico Diario del Sur" y sigue contratando en septiembre de 2026. Eso además indica que el diario seguía circulando.
  · Inferencia, no probada: que sea hoy la editora o explotadora del diario. No encontré quiénes son sus accionistas, si hubo cesión de la marca, ni ningún vínculo documental con Hernando Suárez Burgos. Que la sede esté en Bogotá y no en Pasto también pide explicación.
  · El bloqueo de gobernanza tal como está escrito ("su editora tiene la matrícula cancelada") deja de ser concluyente. Lo que falta ahora es probar quién controla la sociedad activa.
- FUENTE: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (actualizado el 2026-07-14); [enlace retirado: puede mostrar documentos de identidad; ver la resolución] ; [enlace retirado: puede mostrar documentos de identidad; ver la resolución] ; [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (todo consultado el 2026-10-10).
- NIVEL: propiedad / registro externo / hecho de los últimos 12 meses (contrato del 2026-09-11).

OBJECIÓN 3. El bloqueo técnico describe un feed que, según un tercero, ya no existe, y el medio prohíbe ahora el acceso a agentes como el que escribió la ficha.
- QUÉ afirma la ficha: que el feed trae <pubDate> vacíos, que probablemente es "un plugin mal configurado" de WordPress y que la prueba de refutación es `feed:descubrir -- diariodelsur.com.co`.
- POR QUÉ (Internet Archive, solo metadatos CDX):
  · "https://diariodelsur.com.co/feed/ … 308" y luego "https://diariodelsur.com.co/feed text/html 404", ambas capturas del 2026-10-06.
  · Entre enero y mayo de 2026, /feed/ respondía "application/rss+xml 200".
  · El sitemap también cambió. El Yoast "sitemap_index.xml" respondía 200 hasta el 2026-05-01. El 2026-10-06 aparece "https://diariodelsur.com.co/sitemap.xml application/xml 200", que en mayo era un 301.
  · La copia archivada del robots.txt del 2026-05-01 era solo el bloque Yoast ("# START YOAST BLOCK … User-agent: * Disallow:"). La de hoy es un bloque gestionado por Cloudflare que excluye ClaudeBot, anthropic-ai, Claude-Web y Claude-User. La de febrero de 2026 ya excluía ClaudeBot. No hay copia de agosto, así que no puedo saber si la descarga de la ficha del 2026-08-09 respetaba el robots vigente ese día.
  · Inferencia: el sitio migró de plataforma o de configuración entre mayo y octubre de 2026. El diagnóstico "plugin WordPress, se arregla en una tarde" y la prueba de refutación 1 ya no son aplicables tal como están escritos. El bloqueo técnico sigue en pie, pero hoy es otro: no hay feed en la ruta conocida (según un tercero) y el robots excluye a los agentes de Anthropic. No sé si el nuevo sitemap.xml trae <lastmod>, porque no lo descargué.
- FUENTE: https://web.archive.org/cdx/search/cdx?url=diariodelsur.com.co/feed*&from=2026 ; https://web.archive.org/cdx/search/cdx?url=diariodelsur.com.co/sitemap*&from=2026 ; https://web.archive.org/web/20260501013207id_/https://www.diariodelsur.com.co/robots.txt ; https://diariodelsur.com.co/robots.txt (consultado el 2026-10-10).
- NIVEL: conducta observable (técnica), registro externo.

OBJECIÓN 4. El propietario y el gerente que nombra la ficha no tienen fuente comprobable.
- QUÉ afirma la ficha: "Propietario: Hernando Suárez Burgos" y "Gerente: Ronald Tupaz Bustos", con la fuente "DataCrédito Empresas", sin enlace ni fecha.
- POR QUÉ:
  · El RUES abierto no publica accionistas. El registro del NIT 891222292 no trae representante legal. El único representante legal que da el RUES en esta órbita es el de la sociedad 901804010 (Miguel Ángel Arellano Cantillo), un nombre que la ficha no menciona.
  · Los dos nombres de la ficha coinciden literalmente con el infobox de la Wikipedia ("propietario":"Hernando Suárez Burgos", "Gerente":"Ronald Tupaz Bustos", dateModified 2026-09-17). Ese infobox es la misma fuente que la ficha usa para la circulación, y además da una "tirada" de "240.964 (lunes a sábado, 2025)" que no es creíble para un diario regional. Es una fuente débil.
  · Inferencia: el nivel 1 "persona natural identificada" descansa en una base de datos comercial sin cita y en la Wikipedia. No está "mejor cubierto que en varias fichas", como dice la ficha. La propia ficha admite en la refutación 3 que la combinación "propietario de una sociedad cancelada" pide explicación.
- FUENTE: https://es.wikipedia.org/wiki/Diario_del_Sur_(Colombia) (HTML crudo, dateModified 2026-09-17, consultado el 2026-10-10); [enlace retirado: puede mostrar documentos de identidad; ver la resolución] .
- NIVEL: propiedad.

## LO QUE NO PUDE VERIFICAR
- Si el feed o el sitemap traen fechas hoy. El robots.txt excluye ClaudeBot, anthropic-ai, Claude-Web y Claude-User, así que no descargué ni el feed, ni el sitemap.xml, ni sus copias archivadas. Solo tengo metadatos CDX (objeción 3). Esto tiene que comprobarlo una persona, o un agente al que el robots no excluya.
- Si la matrícula 891222292 está cancelada hoy o sigue en liquidación activa. El RUES abierto (actualizado el 2025-03-11) y el agregador se contradicen. No consulté el RUES web ni pedí certificado.
- Quién es accionista de Ediciones Periodísticas Diario del Sur S.A.S. y si tiene vínculo con Hernando Suárez Burgos o con el grupo Extra. No encontré fuente. El buscador no devolvió ninguna página con ese nombre exacto.
- Si Hernando Suárez Burgos vive y sigue al frente. La búsqueda web no devolvió nada pertinente.
- Si el diario sigue publicando a diario en la web. El buscador sugiere piezas de 2026, pero son resúmenes y no cito crudo. El contrato del 2026-09-11 indica actividad comercial, no frecuencia de publicación.
- La sección de editoriales del medio, la afiliación a Andiarios y que fuera "el único candidato de Nariño con feed": no los miré. Los dos primeros quedan fuera por el robots; lo tercero, por falta de tiempo y de cupo.

## LO QUE FALTA
- Contratación pública. La ficha no la trae. Por NIT exacto y sin DV:
  · NIT 891222292: SECOP II, 0 contratos. SECOP I, 23 contratos por 1.214.493.816 COP en total (con adiciones), entre el 2017-10-24 y el 2022-09-21; 0 en los últimos 12 meses. Los dos mayores son con la Alcaldía de Pasto: 480.000.000 (2018-01-25) y 501.600.000 (2019-01-22), es decir, casi el 81 % del total. El resto son entidades públicas de Nariño, entre ellas tres contratos con la editora departamental EDINAR en 2019, por 109.000.000. En SECOP II hay 1 registro cargado con DV (8912222921): SENA Regional Nariño, 2020-09-04, 356.000 COP. No aparece en la consulta exacta sin DV.
  · NIT 901804010: SECOP II, 0. SECOP I, 2 contratos por 7.700.000 COP en total; en los últimos 12 meses, 1 por 2.700.000 (Cámara de Comercio de Tumaco, 2026-09-11).
  · Es un dato de dependencia de la pauta pública local, fuerte hasta 2019. No mueve el eje, pero se declara.
- El certificado de existencia y representación de las dos sociedades, en 2026.
- El papel de Ediciones Periodísticas Diario del Sur S.A.S. y su controlante.
- La fecha y la forma de la migración del sitio, y la nueva URL del feed, si la hay.
- Una copia literal de la descarga de agosto del feed, con su cabecera. La ficha muestra solo un fragmento.

## EVIDENCIA QUE NO MUEVE EL NÚMERO
- La conducta medida da 0 artículos entre el 2026-08-31 y el 2026-10-10. Es coherente con que el medio no esté en el catálogo y con que el feed esté en 404 (CDX del 2026-10-06). No dice nada de su línea.
- La pauta pública: fuerte con la Alcaldía de Pasto en 2018-2019 y residual desde 2020 (SECOP I). Es estructura comercial, no orientación.
- El robots.txt tiene "Content-Signal: search=yes,ai-train=no,use=reference" (2026-10-10). Es una decisión técnica y de derechos del medio. No dice nada del eje.
- La recomendación de la ficha (no dar de alta todavía) sigue en pie, pero por motivos distintos de los escritos:
  · Gobernanza: ya no es "editora cancelada". Es "hay una sociedad activa, constituida en Bogotá en 2024, que factura el periódico, y no sabemos quién la controla".
  · Técnica: ya no es "<pubDate> vacío". Es "no hay feed conocido (404 según un tercero) y el robots excluye a los agentes de Anthropic".
  La ficha debería reescribir sus dos bloqueos y su apartado de refutación.

## SIN OBJECIÓN
No aplica: hay cuatro objeciones.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** El revisor no copió cédulas, teléfonos ni direcciones de personas naturales. Se comprobó: las cifras largas del texto son NIT de sociedades, cuantías, matrículas y números de constancia o de contrato. El único nombre de representante legal que da (Miguel Ángel Arellano Cantillo) sale del RUES, como pide la regla. El RUES abierto trae también el número de documento de esa persona: el revisor no lo copió y esta resolución tampoco lo escribe.

**Cómo se verificó.**
- **robots.txt de diariodelsur.com.co**, leído antes que nada (2026-10-10, HTTP 200, 3.369 bytes; idéntico en `www.` y sin `www.`). **Confirma lo que dice el revisor**: dentro del bloque «BEGIN Cloudflare Managed content» están «User-agent: ClaudeBot / Disallow: /», «User-agent: anthropic-ai / Disallow: /», «User-agent: Claude-Web / Disallow: /» y, bajo «# AI Agents», «User-agent: Claude-User / Disallow: /». También «Content-Signal: search=yes,ai-train=no,use=reference» y «Sitemap: https://www.diariodelsur.com.co/sitemap.xml». **No se descargó nada más de ese dominio**: ni portada, ni feed, ni sitemap, ni copias archivadas de su contenido.
- **Internet Archive.** La primera consulta devolvió **503 «Temporarily Offline»**; la segunda, minutos después, respondió. Solo se usaron metadatos CDX (fecha, URL, tipo y código) y las copias archivadas del propio `robots.txt`.
- **RUES abierto** (`c82u-588k`), por `nit` con **igualdad exacta** y sin dígito de verificación: 891222292 y 901804010. Además, por `razon_social like '%DIARIO DEL SUR%'` y `'%EDICIONES PERIODISTICAS%'`, y una búsqueda de control por los apellidos de los dos nombres de la ficha (ningún resultado los une a ninguna de las dos sociedades; no se reproduce porque son registros de personas ajenas).
- **SECOP I** (`f789-7hwg`, `identificacion_del_contratista`) y **SECOP II** (`jbjy-vk9h`, `documento_proveedor`), por **igualdad exacta** sin DV para los dos NIT; control con DV (8912222921 y 9018040103) y por nombre del contratista. La ficha del proceso de La Florida se abrió en `contratos.gov.co` (HTML crudo); los PDF del proceso piden un paso con reCAPTCHA y no se abrieron.
- **Agregadores**: `empresas.larepublica.co` (robots «User-agent: * / Allow: /») para los dos NIT, y `datacreditoempresas.com.co`, la fuente que cita la ficha (su `robots.txt` responde 403 «AccessDenied»; las dos páginas públicas respondieron 200 y se leyeron en crudo).
- **Wikipedia**: `https://es.wikipedia.org/wiki/Diario_del_Sur_(Colombia)`, HTML crudo, solo la ruta `/wiki/`.
- **Buscador web**, tres consultas («"Ediciones Periodísticas Diario del Sur"», «Diario del Sur Pasto periódico nueva empresa editora 2025 2026», «"Arellano Cantillo" "Diario del Sur"»), excluyendo `diariodelsur.com.co`, `eltiempo.com`, `cambiocolombia.com` y `lasillavacia.com`. Sus resúmenes no se citan como hecho. `pressreader.com` aparece en los resultados, pero su `robots.txt` excluye a ClaudeBot, Claude-Web, Claude-User y anthropic-ai, y no se abrió. `abcpublicitario.com` y `andiarios.com` no respondieron.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | «Matrícula cancelada» solo la sostiene un agregador; el RUES abierto la da ACTIVA y en liquidación | sí | sí | **Aceptada, y reforzada**: DataCrédito, la otra fuente de la ficha, dice hoy «MATRÍCULA ACTIVA». **Una deformación del revisor**: el agregador de La República **no** dice «en liquidación» (la palabra no aparece en su página), así que no es cierto que «las dos fuentes coinciden» en eso |
| 2 | Hay otra sociedad activa, Ediciones Periodísticas Diario del Sur S.A.S., que factura el periódico | sí | sí | **Aceptada como hecho**: existe, está activa y un contrato de 2025 la paga por publicar «en el periódico Diario del Sur». **No consta** que sea la editora ni quién la controla; no se encontró ningún vínculo documental |
| 3 | El feed analizado ya no existe y el robots excluye a los agentes de Anthropic | sí | sí | **Aceptada**: robots verificado hoy; CDX verificado línea a línea. Matiz: la exclusión de Claude bloquea la **revisión**, no la **ingesta** del motor (ver más abajo) |
| 4 | Propietario y gerente sin fuente comprobable | sí | sí | **Aceptada, y reforzada**: la página pública de DataCrédito **no** trae esos nombres; la Wikipedia los apoya en una página de Andiarios archivada en **2010** |
| — | «Lo que falta»: contratación pública | sí | sí | **Cifras exactas al peso. Una deformación de lectura**: el 81 % que el revisor llama «pauta pública local» son **dos contratos de arrendamiento de un inmueble** a la Alcaldía de Pasto, no publicidad |

### Lo verificado, objeción por objeción

**1 · Estado de la matrícula del NIT 891222292.**
- RUES abierto, literal: `"camara_comercio":"PASTO","matricula":"13825"`, `"razon_social":"GRUPO EDITORIAL DIARIO DEL SUR SAS EN LIQUIDACION"`, `"fecha_matricula":"19830829"`, `"fecha_renovacion":"20241030"`, `"ultimo_ano_renovado":"2024"`, `"estado_matricula":"ACTIVA"`, `"fecha_actualizacion":"2025/03/11 09:51:49.450000000"`. No trae representante legal. Coincide con el revisor.
- `empresas.larepublica.co`, HTML crudo: «GRUPO EDITORIAL DIARIO DEL SUR SAS», «¿Registro RUES activo?» «No / Cancelado», tamaño «MICRO». Sin fecha del dato. **La cadena «liquid» aparece 0 veces en la página.** La ficha atribuye a esta fuente la razón social «EN LIQUIDACIÓN», y hoy no la sostiene.
- `datacreditoempresas.com.co` (la fuente de la ficha para la constitución y los nombres), HTML crudo: «Grupo Editorial Diario Del Sur Sas En Liquidacion», «NIT: 891222292», «MATRÍCULA ACTIVA», «Fecha constitución: 26-08-1983», «Microempresa».
- **Balance:** dos fuentes (RUES abierto y DataCrédito) dicen matrícula activa en liquidación; una (La República) dice cancelada, sin fecha. Ninguna es un certificado de existencia y representación. Lo exacto es «en liquidación», y la cancelación queda como dato de un solo agregador.
- **Homónima sin relación aparente**: el RUES tiene también «DIARIO DEL SUR MORENO HERNANDEZ LTDA EN LIQUIDACION» (Bogotá, matriculada en 1999, renovada por última vez en 2001). No se usa.

**2 · Ediciones Periodísticas Diario del Sur S.A.S.**
- RUES abierto, literal: `"camara_comercio":"BOGOTA","matricula":"3786278"`, `"razon_social":"EDICIONES PERIODISTICAS DIARIO DEL SUR S.A.S"`, `"cod_ciiu_act_econ_pri":"1811"`, `"cod_ciiu_act_econ_sec":"5813"`, `"ciiu4":"9319"`, `"fecha_matricula":"20240222"`, `"fecha_renovacion":"20260714"`, `"ultimo_ano_renovado":"2026"`, `"estado_matricula":"ACTIVA"`, `"representante_legal":"MIGUEL ANGEL ARELLANO CANTILLO"`, `"fecha_actualizacion":"2026/07/14 16:10:55.333000000"`. No trae socios. Coincide con el revisor.
- La República: «¿Registro RUES activo?» «Si», «BOGOTA D.C.», tamaño «PEQUEÑA». DataCrédito: «MATRÍCULA ACTIVA», «Fecha constitución: 22-02-2024», renovación «2026-07-14».
- **SECOP I** (igualdad exacta, 2 filas, $7.700.000):
  - 2025-07-24, Alcaldía de La Florida (Nariño), $5.000.000, contratación directa, constancia 25-12-14483129. Objeto en la ficha del proceso (HTML crudo, con tildes): «PUBLICACIÓN DE MEDIA PÁGINA FULL COLOR EN EL PERIÓDICO DIARIO DEL SUR SOBRE AVANCE DE GESTIÓN Y PROYECTOS ADELANTADOS POR LA ADMINISTRACIÓN MUNICIPAL DE LA FLORIDA NARIÑO, DURANTE EL AÑO 2024 Y PRIMER SEMESTRE 2025…». La misma ficha ubica al contratista en «Colombia : Nariño», no en Bogotá.
  - 2026-09-11, Cámara de Comercio de Tumaco, $2.700.000, régimen especial, constancia 26-4-14802452, contrato OCS-025-2026. Objeto: «PUBLICACION DE LOS TERMINOS DE REFERENCIA PARA LA ELECCION DEL REVISOR FISCAL PRINCIPAL Y SUPLENTE DE LA CAMARA DE COMERCIO DE TUMACO; PERIODO 2027-2030.» **Este objeto no nombra al periódico**: que la publicación fuera en Diario del Sur es inferencia.
- **SECOP II**: 0 filas por 901804010 y por 9018040103.
- **Vínculo con el periódico: solo el objeto del contrato de La Florida.** No se encontró pie de página de terceros, prensa, contrato que la nombre «editora» ni documento que la ligue a Hernando Suárez Burgos o a la sociedad en liquidación. La búsqueda «"Arellano Cantillo" "Diario del Sur"» no devolvió ninguna página que una los dos nombres. La de «"Ediciones Periodísticas Diario del Sur"» solo devolvió directorios mercantiles.
- **Inferencia razonable, no hecho**: una sociedad con el nombre del diario, con la edición de periódicos como actividad secundaria, factura espacio en él y declara domicilio en Nariño ante SECOP. Es compatible con un traspaso del negocio, pero también con un comercializador de publicidad. Para la ficha, «no consta» quién la controla ni qué papel tiene.

**3 · El feed, el sitemap y el robots.**
- **CDX, literal** (consulta del 2026-10-10 por prefijo `diariodelsur.com.co/feed`, desde 2026):
  - `https://www.diariodelsur.com.co/feed/ application/rss+xml 200`, trece capturas entre el 20260101 y el 20260501.
  - `20261006175633 https://diariodelsur.com.co/feed/ unk 308` y `20261006180021 https://diariodelsur.com.co/feed text/html 404`.
  - `/feed.xml` y `/feeds/all.atom.xml` dan 404 en todas las capturas, antes y después.
- **Sitemap**: `sitemap_index.xml text/xml 200` del 20260101 al 20260501; `www…/sitemap.xml text/html 301` en esas mismas fechas, y `20261006181130 https://diariodelsur.com.co/sitemap.xml application/xml 200`. Coincide con el revisor.
- **robots.txt archivado** (solo esas copias):
  - 2026-01-01, 2026-04-01 y 2026-05-01: 181 bytes, solo el bloque «# START YOAST BLOCK … User-agent: * / Disallow: … # END YOAST BLOCK».
  - 2026-02-01 y 2026-03-01: 1.860 bytes, con un bloque gestionado que ya incluía «User-agent: ClaudeBot / Disallow: /» (sin anthropic-ai, Claude-Web ni Claude-User), más el bloque Yoast.
  - 2026-10-07: idéntico byte a byte al de hoy (3.369 bytes), sin bloque Yoast y con «Disallow: /admin» y «Disallow: /api/».
  - El revisor dice que la de febrero ya excluía a ClaudeBot: exacto. No menciona la de marzo, que también lo hacía, ni que en abril y mayo volvió al bloque Yoast solo. **El robots ha cambiado de un mes a otro**; no hay copia de agosto, así que no se puede saber si la descarga de la ficha (2026-08-09) lo respetaba.
- **Lectura**: el diagnóstico «plugin de WordPress mal configurado» ya no se puede comprobar, y la prueba de refutación 1 tal como está escrita apunta a una ruta que el 2026-10-06 daba 404. La desaparición del bloque Yoast y del `sitemap_index.xml` es compatible con una migración de plataforma, pero eso es inferencia.
- **Matiz que el revisor no hace, y que corrige el planteamiento del encargo.** La exclusión afecta a los agentes de Anthropic, no al motor. El motor de DobleFoco se presenta como `DobleFocoBot` (`shared/userAgent.js`), y el robots de hoy abre a «User-agent: *» con «Allow: /». Por eso **no es en sí un bloqueo de ingesta**: es un **bloqueo de revisión**, igual que con `eltiempo.com`, que excluye a ClaudeBot y sigue en el catálogo. Lo que sí impide es que una revisión hecha por Claude compruebe el feed, el sitemap o la línea del medio en su fuente primaria. Esa comprobación tiene que hacerla el responsable editorial (por ejemplo, ejecutando él mismo `npm run feed:descubrir -- diariodelsur.com.co`). El bloqueo técnico para la ingesta sigue siendo el que tenga hoy el feed: el que se vio en agosto (sin fechas) o el que sugiere el CDX (404 en la ruta conocida), sin comprobar.
- El «Content-Signal: … ai-train=no, use=reference» es una reserva de derechos del medio. Una decisión del responsable editorial: si mostrar titulares y enlaces encaja en «use=reference». Esta resolución no lo decide.

**4 · Propietario y gerente.**
- La página pública de DataCrédito del NIT 891222292 **no contiene** «Suárez», «Tupaz», «Hernando» ni «Ronald» (0 apariciones en el HTML crudo); el resto de los datos queda tras un registro. La atribución de la ficha («DataCrédito Empresas») no se puede reproducir.
- Wikipedia, HTML crudo (`"dateModified":"2026-09-17T21:39:55Z"`): infobox «"propietario":{"wt":"Hernando Suárez Burgos"}», «"Director":{"wt":"Hernando Suárez Burgos"}», «"Gerente":{"wt":"Ronald Tupaz Bustos"}», «"editor jefe":{"wt":"Robert Atis Bernal"}», «"tirada":{"wt":"240.964 (lunes a sábado, 2025)…"}»; y en el texto, «Es propiedad del Sr. Hernando Suárez Burgos. El gerente actual del diario es el Sr. Ronald Tupaz Bustos». **La única referencia de esa frase** (`cite_note-andiarios-1`) enlaza a `https://web.archive.org/web/20100210130600/http://www.andiarios.com/afiliados/Diario%20del%20Sur.html`, es decir, a una **página de Andiarios archivada en febrero de 2010**. La afiliación a Andiarios que repite la ficha sale de la misma fuente.
- RUES abierto: ninguna de las dos sociedades del diario trae a Suárez Burgos ni a Tupaz Bustos como representante. El RUES tiene una matrícula de persona natural «SUAREZ BURGOS HERNANDO» en la Cámara de Comercio de Pasto, en estado «CANCELADA»; no dice nada del periódico y no se usa.
- **Aviso cruzado con Abra Noticias**: el «editor jefe» que da la Wikipedia, «Robert Atis Bernal», coincide casi letra a letra con «Rober Atis Bernal», que firma dos columnas en Abra Noticias (`opus-5-5-abra-noticias.md`). Fuente editable y homonimia no descartada: **no entra como hecho** en ninguna de las dos fichas.

**5 · Contratación pública (lo que falta).**
- **NIT 891222292**, igualdad exacta: SECOP I, **23 contratos, $1.214.493.816** (cuantía y valor con adiciones iguales), del 2017-10-24 al 2022-09-21; **0 en los últimos 12 meses**. SECOP II, 0; con DV, 1 (SENA Regional Nariño, firmado el 2020-09-04, $356.000, CO1.PCCNTR.1814847, «Suscripción de un diario de amplia circulación…»). Todo coincide con el revisor.
- **Lo que el revisor lee mal**: los dos contratos mayores con la Alcaldía de Pasto (2018-01-25, $480.000.000, constancia 18-12-7774739; 2019-01-22, $501.600.000, constancia 19-12-8924095) son de tipo «Arrendamiento». Objeto: «EL MUNICIPIO DE PASTO; SECRETARIA DE GOBIERNO; REQUIERE ARRENDAR EL BIEN INMUEBLE UBICADO EN…». **Son el alquiler de un inmueble de la sociedad, no pauta.** Suman $981.600.000 (80,8 %). Sin ellos, la contratación de publicidad, suscripciones y avisos es de **$232.893.816 en 21 contratos**, y su mayor contratante es la Empresa Editora de Nariño (EDINAR, del departamento): 3 contratos en 2019 por $109.000.000. Llamarlo «dependencia de la pauta pública local, fuerte hasta 2019» sobrestima la pauta. Sí es dinero público de un gobierno que el medio cubre, y debe decirse así.
- Por nombre aparecen 3 contratos más en SECOP I (2018-2019, $49.020.800: Hospital de Puerto Asís, EDINAR e Ipiales) cargados con identificaciones mal escritas o con la de una persona natural. No entran en el recuento por igualdad exacta; se mencionan para que nadie los sume sin saberlo.
- **NIT 901804010**: ver la objeción 2. 2 contratos, $7.700.000; en los últimos 12 meses, 1 por $2.700.000.

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se corrigen estas partes:
- **Obj. 1, «las dos fuentes coinciden en que la sociedad está EN LIQUIDACIÓN»**: la página de La República no lo dice. Lo dicen el RUES abierto y DataCrédito.
- **Obj. 3, la consecuencia**: que el robots excluya a Claude no impide la ingesta por `DobleFocoBot`. Lo que impide es la verificación por Claude.
- **«Lo que falta», la lectura de la contratación**: el 81 % es arrendamiento, no pauta.
- **Obj. 2, el contrato de Tumaco como prueba de que el diario «seguía circulando»**: su objeto no nombra el periódico. La prueba de actividad comercial en nombre del diario es el de La Florida (2025-07-24).

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente.** Todas las URL que se pudieron abrir resolvieron, las citas del RUES, SECOP, Wikipedia, el robots y el CDX son literales, y las cifras coinciden al peso. Deformaciones u omisiones del revisor: las cuatro de arriba, más la omisión de la copia de marzo del robots.

**Errores de la propia ficha, para no repetirlos:**
- «Matrícula RUES: **Cancelada**», con La República como fuente: el RUES abierto y DataCrédito dicen activa, en liquidación.
- «Grupo Editorial Diario del Sur S.A.S. EN LIQUIDACIÓN» atribuido a La República: esa página no lo dice hoy; lo dicen el RUES abierto y DataCrédito.
- «Propietario: Hernando Suárez Burgos» y «Gerente: Ronald Tupaz Bustos», con DataCrédito como fuente: la página pública de DataCrédito no los trae; la fuente real verificable es la Wikipedia, que remite a una página de Andiarios de 2010.
- «Persona natural identificada y sociedad identificada: el nivel 1 está mejor cubierto aquí que en varias fichas»: no se sostiene.
- «Su editora tiene la matrícula cancelada» (cabecera): falso como hecho probado.
- «Diario del Sur era el único candidato de Nariño con feed»: superado; Abra Noticias está en el catálogo y Nariño Ahora quedó anotado como alternativa (`shared/mediaRegistry.js`).
- La ficha no trae la línea de contratación pública que exige el protocolo desde el 2026-10-07.
- La ficha no dice que el robots excluye a los agentes de Anthropic. Es más: no hay copia de agosto que diga si la descarga del 2026-08-09 lo respetaba.

**En `shared/mediaRegistry.js` (comentario de Abra Noticias):** «Diario del Sur tiene la editora en liquidación y entrega el feed sin fechas legibles».
- «la editora en liquidación»: exacto para la sociedad histórica, pero incompleto. Hay otra sociedad activa que factura el periódico.
- «entrega el feed sin fechas legibles»: era lo observado en agosto. Hoy no es comprobable por nosotros, y el CDX da la ruta conocida en 404 el 2026-10-06. Debe dejar de escribirse en presente.
- `shared/mediaOwnership.js` y `shared/centinela.js` no tienen entrada de Diario del Sur. Las dos menciones de `mediaOwnership.js` («Espejos del RUES que sí respondieron con El Pilón, Aguasclaras y Diario del Sur») son del método de otras fichas y no cambian.

---

**Propuesta para la firma**

**Estado de la candidatura: sigue sin alta, con los dos bloqueos reescritos.** Ninguna objeción aporta evidencia de línea editorial; no hay número que proponer.

**(a) Correcciones en `fichas/diario-del-sur.md`**
1. **Cabecera**, sustituir el recuadro por: «Dos bloqueos independientes, y cualquiera de los dos basta. Uno es de gobernanza: la sociedad editora histórica está en liquidación y una sociedad distinta, constituida en Bogotá en 2024, factura publicidad en el periódico sin que conste quién la controla. El otro es técnico: el feed de agosto venía sin fechas, el que se conocía no responde desde octubre y su robots.txt excluye a los agentes de Anthropic, de modo que ni siquiera podemos comprobarlo con la revisión habitual».
2. **Nivel 1**, tabla:
   - «Empresa editora (histórica)»: Grupo Editorial Diario del Sur S.A.S. en liquidación, NIT 891222292, matrícula 13825 de Pasto. Fuente: RUES abierto (`https://www.datos.gov.co/resource/c82u-588k.json?$select=razon_social,sigla,nit,camara_comercio,matricula,organizacion_juridica,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,fecha_cancelacion,cod_ciiu_act_econ_pri&nit=891222292`, registro actualizado el 2025-03-11, consultado el 2026-10-10).
   - «Matrícula RUES»: «Activa, en liquidación; última renovación 2024 (RUES abierto y DataCrédito, 2026-10-10). Un agregador (empresas.larepublica.co) la da por cancelada, sin fecha. Falta el certificado de la Cámara de Comercio de Pasto».
   - Fila nueva, «Otra sociedad con el nombre del diario»: Ediciones Periodísticas Diario del Sur S.A.S., NIT 901804010, matrícula 3786278 de Bogotá, constituida el 2024-02-22, activa, renovada el 2026-07-14; representante legal según el RUES: Miguel Ángel Arellano Cantillo. Factura publicidad «en el periódico Diario del Sur» (SECOP I, 2025-07-24). **No consta que sea la editora, ni quiénes son sus socios.**
   - «Propietario» y «Gerente»: cambiar la fuente a «Wikipedia (nivel 4), que remite a una página de Andiarios de 2010; no consta en un registro actual». Mantener los nombres solo con esa advertencia, o retirarlos (decisión 2).
   - «Constitución 26-08-1983 (DataCrédito)»: se mantiene, verificado. El RUES da como fecha de matrícula el 29-08-1983.
   - «Gremio: afiliado a Andiarios»: añadir «según una página de 2010».
3. **Retirar** «Persona natural identificada y sociedad identificada: el nivel 1 está mejor cubierto aquí que en varias fichas del catálogo».
4. **Nivel 2**: dejar el hallazgo de agosto en pasado y fechado («el 2026-08-09, el feed traía `<pubDate>` vacíos»). Añadir: «El Internet Archive registra `/feed/` como RSS 200 hasta mayo de 2026 y, el 2026-10-06, `/feed/` → 308 → `/feed` 404, con un `sitemap.xml` nuevo en lugar del `sitemap_index.xml` de Yoast. No se comprobó directamente: el robots.txt (2026-10-10) excluye a ClaudeBot, anthropic-ai, Claude-Web y Claude-User».
5. **Nota de método nueva**, igual que en `fichas/cambio.md`: «diariodelsur.com.co no se consulta en las revisiones: su robots.txt excluye a los agentes de Anthropic (2026-10-10; en febrero y marzo ya excluía a ClaudeBot). Lo que solo consta allí queda como "no verificable por exclusión de robots.txt". La ingesta del motor (`DobleFocoBot`) no está excluida».
6. **CONTRATACIÓN PÚBLICA**, línea nueva en el formato del protocolo:

> Contratación pública (SECOP I y II, NIT 891222292, consultado 2026-10-10): 0 contratos contratados en los últimos 12 meses; 24 por $1.214.849.816 en total desde 2017 (23 en SECOP I, 2017-2022, y 1 en SECOP II, 2020). Principales contratantes: Alcaldía de Pasto, $981.600.000 en dos contratos de **arrendamiento de un inmueble** de la sociedad (2018 y 2019), no de publicidad; Empresa Editora de Nariño (EDINAR, del departamento), $109.000.000 en divulgación institucional (2019); Terminal de Transporte de Ipiales, $40.710.000 (2022). La Alcaldía de Pasto y el departamento de Nariño son gobiernos que el medio cubre. Ediciones Periodísticas Diario del Sur S.A.S. (NIT 901804010): 1 contrato por $2.700.000 en los últimos 12 meses (Cámara de Comercio de Tumaco, 2026-09-11) y 2 por $7.700.000 desde 2025 (también Alcaldía de La Florida, 2025-07-24, publicación «en el periódico Diario del Sur»).

7. **LO QUE ESTO DEJA ABIERTO**: «Diario del Sur era el único candidato de Nariño con feed» pasa a pasado, con la nota de que Nariño ya tiene a Abra Noticias en el catálogo. El paso 1 («Escribirles… un plugin mal configurado») se cambia por: «Escribirles para preguntar por la URL del feed tras la migración y por la sociedad que lo edita hoy».
8. **REFUTACIÓN**, reescrita:
   1. Que el responsable editorial compruebe, sin pasar por un agente de Anthropic, que el sitio publica un feed con fechas (`npm run feed:descubrir -- diariodelsur.com.co`, ejecutado por él), y que el uso que haría DobleFoco encaje en su «Content-Signal».
   2. Que un certificado de existencia y representación, o un documento del propio medio, diga qué sociedad edita hoy el periódico y quién la controla.
   3. Que se documente el papel actual de Hernando Suárez Burgos con una fuente posterior a 2010.

**(b) En `shared/mediaRegistry.js`, comentario de Abra Noticias**: sustituir «Diario del Sur tiene la editora en liquidación y entrega el feed sin fechas legibles» por «Diario del Sur tiene su editora histórica en liquidación y no consta quién controla la sociedad activa que factura el periódico; su feed venía sin fechas en agosto de 2026 y desde octubre no se ha podido comprobar». Es solo un comentario: no cambia comportamiento.

**(c) En `revision-externa/ciclo-2-plan.md`**: añadir `diariodelsur.com.co` a «Bloqueados conocidos» (excluye ClaudeBot, anthropic-ai, Claude-Web y Claude-User, 2026-10-10). Y precisar que esa lista es de **revisión**, no de ingesta, como ya pasa con `eltiempo.com`.

**(d) Tensiones a declarar**
1. Una sociedad activa con el nombre del diario cobra a gobiernos locales por publicar en él, y no se sabe quién la controla.
2. Pauta y arrendamiento con la Alcaldía de Pasto (2018-2019) y con el departamento (EDINAR, 2019), gobiernos que el medio cubre. No están vigentes.

**¿Aviso de quien dirige?** No procede: el medio no está en el catálogo y no consta quién lo dirige hoy.

**Lo que NO entra como hecho:**
- que Ediciones Periodísticas Diario del Sur S.A.S. sea la editora, o que haya cesión de marca o de negocio;
- que la matrícula 891222292 esté cancelada;
- que Hernando Suárez Burgos siga siendo propietario o director, o que Ronald Tupaz Bustos sea el gerente hoy;
- que «Robert Atis Bernal» sea el editor jefe, ni que sea la misma persona que firma en Abra Noticias;
- que el sitio haya migrado de plataforma (es compatible con los metadatos, no está probado);
- la «tirada» de 240.964 de la Wikipedia.

**Decisiones para el responsable editorial:**
1. **Estado de la candidatura.** Recomendación: **sigue sin alta**, con los dos bloqueos reescritos como en (a).1.
2. **Nombres de propietario y gerente.** Recomendación: **retirarlos de la tabla** y dejarlos en una nota: «según la Wikipedia, que remite a Andiarios (2010)». Su única fuente verificable tiene 16 años.
3. **robots.txt.** Recomendación: anotar el dominio como **bloqueado para revisión** (no para ingesta) en el plan y en la ficha. Si algún día se da de alta, la comprobación del feed la hace el responsable editorial, y el responsable editorial decide si el uso de DobleFoco encaja en «use=reference».
4. **Comentario de `mediaRegistry.js`.** Recomendación: corregirlo con el texto de (b) en la PR de la tanda.
