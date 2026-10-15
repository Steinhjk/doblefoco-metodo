# Respuesta — Claude Opus 5.5 sobre El Morichal

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
> **Edición:** retirados descriptores personales (DECISIONES 2026-10-10); retirados enlaces que pueden mostrar documentos de identidad (PROTOCOLO, Datos personales, 2026-10-10).

---

## RESPUESTA LITERAL

```
DECLARACIÓN PREVIA DE CONFLICTO
Soy Claude Opus 5.5 (id. claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Mi acuerdo no debe leerse como validación independiente. Para compensarlo he buscado sobre todo en fuentes que la ficha NO usa: el RUES abierto, SECOP I y II, la API pública de WordPress del medio y los PDF de rendición de cuentas que el medio tiene colgados en su biblioteca de medios. De la ficha solo usé su única fuente, la página «Nosotros», y la volví a leer en crudo. Fecha de todas las consultas: 2026-10-10.

MÉTODO Y DÓNDE BUSQUÉ
- robots.txt de elmorichal.com (solo excluye /carrito/, /cart/, /checkout/ y parámetros de carrito; no excluye a ClaudeBot, Claude-Web ni anthropic-ai) y de datos.gov.co (no excluye esos agentes; las rutas /resource/ no están bloqueadas). No toqué eltiempo.com, cambiocolombia.com ni lasillavacia.com. No usé Wikipedia.
- Citas tomadas del HTML crudo (curl -sL --ssl-no-revoke con User-Agent de navegador) y de los PDF originales (pdftotext). Copias locales en t6\morichal-dl.
- Sitio del medio: https://elmorichal.com/nosotros/ (article:modified_time 2026-08-07T17:23:20Z); API de WordPress: /wp-json/wp/v2/pages, /posts (filtrado por la categoría «editorial», id 3, y por fecha after=2025-10-10), /users, /categories, /search y /media?mime_type=application/pdf.
- RUES abierto (datos.gov.co c82u-588k): razon_social like '%MORICHAL%', '%MORICHAL COMUNICACION%', '%CORPORACION EL MORICHAL%', matrículas desde 2025, y representante_legal like '%SUAREZ NARVAEZ%'.
- SECOP II (jbjy-vk9h, documento_proveedor) y SECOP I (f789-7hwg, identificacion_del_contratista), por igualdad exacta y sin dígito de verificación, para: Corporación El Morichal (NIT 901978854), El Morichal Comunicaciones S.A.S. (NIT 900988084) y la matrícula de persona natural del fundador (consultada por su número de identificación tomado del RUES; es una cédula y no la escribo, por la Ley 1581).
- Wayback Machine: la intenté para ver versiones anteriores de «Nosotros» y respondió «Temporarily Offline». Es una laguna.
- Buscador web: NO lo usé. Todo salió de fuentes primarias, así que no puedo decir si tenía cupo.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No hay venta ni fusión, pero hubo dos movimientos de registro dentro de la ventana:
  (a) La sociedad anterior, EL MORICHAL COMUNICACIONES S A S (NIT 900988084, Cámara de Comercio de Bogotá, matrícula 2708137, CIIU 5813), figura en el RUES con estado_matricula "CANCELADA", fecha_cancelacion "20260727", fecha_renovacion "20260724" y ultimo_ano_renovado "2024" (fecha_actualizacion 2026/07/28). La ficha dice «liquidada» sin fecha. En realidad el cierre formal quedó inscrito el 27-07-2026, catorce días antes de que se escribiera la ficha.
  (b) La CORPORACIÓN EL MORICHAL (NIT 901978854, CC Villavicencio, matrícula 9000510935, «ENTIDAD SIN ANIMO DE LUCRO / CORPORACIONES», CIIU 9499) consta como "ACTIVA", con fecha_matricula "20250820", renovada el "20260216" (ultimo_ano_renovado "2026").
  Fuente: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] y ?nit=901978854 (consultadas el 2026-10-10).
- La persona que la ficha nombra como titular o director, ¿sigue viva y en el cargo?
  Edwin Ernesto Suárez Narváez figura en el RUES como representante legal de la Corporación (registro actualizado el 2026/06/05). También firma como «Representante Legal» el Informe Anual de Resultados publicado el 2026-06-20. Su última firma que encontré en el sitio es del 2026-05-23 (usuario WP id 2, «Edwin Suárez»). No encontré nada que indique fallecimiento ni salida. Comprobación: 2026-10-10.
- ¿Quién dirige hoy la redacción?
  No encontré en el sitio, hoy, a nadie nombrado expresamente «director». La página «Nosotros» anuncia el equipo («se presenta más abajo»), pero en el HTML crudo los contenedores de equipo (elementor 12a3dd6 y 3206bb6) están vacíos y la sección «Rendición de cuentas» no trae enlaces. La única pista es la ficha de autor de Edwin Suárez en la API: «Fundador del periódico EL MORICHAL». Es indicio, no prueba de que dirija hoy la redacción.
- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que la ficha cita?
  Sí. Hay tres: el registro RUES de la Corporación (2026-02-16 / 2026-06-05), la cancelación de la S.A.S. (2026-07-27) y, sobre todo, los documentos de la propia Corporación colgados el 2026-06-20 en su biblioteca de medios: Estados Financieros 2025, Informe Anual de Resultados, Acta de Asamblea 001 del 21-05-2026, Acta de Constitución, Estatutos y Libro de Fundadores.

## OBJECIONES

OBJECIÓN 1 — Composición de la Corporación: son seis fundadores, no tres
- QUÉ afirma la ficha: que tiene tres cofundadores (Suárez, Rebolledo y Guajo) y que es «una corporación pequeña de tres personas en la Orinoquía».
- POR QUÉ: el medio declara, y sus documentos lo confirman, seis fundadores con el mismo aporte cada uno.
  · «Nosotros», crudo: «En agosto de 2025 nos constituimos como organización sin ánimo de lucro: Corporación El Morichal, integrada por seis personas vinculadas directa o indirectamente con el periódico desde hace al menos siete años.» Y: «El equipo que produce el periódico día a día […] es otro y se presenta más abajo; tres personas hacen parte de ambos.»
  · Informe Anual de Resultados (PDF, periodo 20-08-2025 a 31-12-2025): seis «Aportes de constitución» de $180.000 cada uno, total «$1,080,000». Aportantes: Edwin Ernesto Suárez Narváez, Edgar Guajo Bernavé, Juliana Montoya Álvarez, Gardenia Nazareth Rebolledo Anija, Rafael Montoya Parra y Juan Miguel Chitiva.
  · Lista de asistencia del Acta de Asamblea del 21-05-2026: los mismos seis, como «Fundador 1» a «Fundador 6». La secretaria de la asamblea es Juliana Montoya Álvarez.
  Inferencia, no probada: que «tres personas» de la ficha sean las tres que están a la vez en la Corporación y en el equipo. La ficha confunde las dos figuras que el propio medio separa.
- FUENTES Y FECHAS: https://elmorichal.com/nosotros/ (modificada el 2026-08-07, leída el 2026-10-10); [PDF Informe-Anual-de-Resultados, enlace retirado: trae documentos de identidad; cuelga de https://elmorichal.com/nosotros/] y [PDF Acta-de-Asamblea-001_21_05_26, enlace retirado: trae documentos de identidad; cuelga de https://elmorichal.com/nosotros/] (subidos el 2026-06-20).
- NIVEL: propiedad (quién constituye la ESAL) y declaración del propio medio.

OBJECIÓN 2 — El NIT y el registro mercantil no faltan: están en el RUES abierto
- QUÉ afirma la ficha: «Falta el NIT y falta el certificado de Cámara de Comercio, así que sigue siendo autodeclarado.»
- POR QUÉ: el RUES abierto trae razon_social "CORPORACIÓN EL MORICHAL", nit "901978854", camara_comercio "VILLAVICENCIO", tipo_sociedad "ENTIDAD SIN ANIMO DE LUCRO", organizacion_juridica "CORPORACIONES", estado_matricula "ACTIVA", fecha_matricula "20250820", representante_legal "SUAREZ NARVAEZ EDWIN ERNESTO". Así quedan verificadas por registro externo la existencia de la ESAL, su fecha de constitución y su representante legal. Lo que el RUES abierto no da es la lista de asociados; esa sale de los PDF citados en la Objeción 1. Que el registro esté en Villavicencio y no en una cámara de Vichada coincide con la jurisdicción de esa cámara, pero eso es inferencia: no lo verifiqué.
- FUENTE: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (consultada el 2026-10-10; fecha_actualizacion del registro, 2026/06/05).
- NIVEL: registro externo / propiedad.

OBJECIÓN 3 — La laguna de financiación se cae con documentos que el medio publicó antes de la ficha
- QUÉ afirma la ficha: «no he documentado ni una sola fuente de financiación»; y entre las refutaciones, «Documentar de qué se financia la Corporación» como el nivel 1 que falta.
- POR QUÉ: el 2026-06-20, siete semanas antes de la ficha (2026-08-09), la Corporación publicó sus estados financieros y su informe anual de 2025, y «Nosotros» tiene una sección «Así nos financiamos».
  · Estados Financieros 2025: NOTA 9 – INGRESOS: «4295 Ingresos por Donaciones 0.00 / 4296 Aportes Voluntarios 0.00 / TOTAL 0.00». Total activo y patrimonio a 31-12-2025: 162,019.00.
  · Informe Anual: «La corporación no recibió donaciones ni aportes adicionales a los efectuados por los fundadores al momento de su constitución» y «La corporación no celebró contratos durante el período». El dinero de 2025 son los $1.080.000 que pusieron los seis fundadores.
  · «Nosotros», crudo: «Antes de ser Corporación El Morichal, nuestra financiación provenía principalmente de subvenciones para realizar investigaciones y de la publicidad de establecimientos de comercio privado, empresas de servicios públicos y entidades públicas del orden nacional. Ahora, con la figura jurídica de ESAL, apostamos por subvenciones internacionales, proyectos editoriales y servicios especializados.» Y: «La Corporación El Morichal se constituyó en agosto de 2025, pero no tuvo cuenta bancaria ese año: durante esos meses el medio siguió operando bajo la figura de persona natural, a nombre de Edwin Suárez.»
  · Una fuente de financiación concreta, de los últimos 12 meses, declarada en la propia pieza: «Esta pieza periodística es resultado de las Becas del Taller: ‘Periodismo y elecciones en Colombia: contar lo que importa para la democracia’, otorgadas por la Fundación Gabo en alianza con el Programa de las Naciones Unidas para el Desarrollo (PNUD).» Está en «Dos representantes elegidos por el Guainía, dos modelos de financiación» (datePublished 2026-05-23).
  · Inferencia, sin cifras: la categoría «edictos» (48 entradas en total; avisos judiciales y emplazatorios a página completa en 2026) apunta a ingresos por publicación de avisos legales. No sé si los factura la Corporación o la persona natural.
  Conclusión: la financiación de 2025 está documentada y es mínima (aportes de los fundadores). Lo que sigue sin documentar es la de 2026, porque aún no hay informe de ese año. La ficha debería decir esto y no «ni una sola fuente».
- FUENTES Y FECHAS: [PDF Estados-Financieros-2025_VF, enlace retirado: trae documentos de identidad; cuelga de https://elmorichal.com/nosotros/] (2026-06-20); .../Informe-Anual-de-Resultados.pdf (2026-06-20); https://elmorichal.com/nosotros/ (2026-08-07); https://elmorichal.com/dos-representantes-elegidos-por-el-guainia-dos-modelos-de-financiacion/ (2026-05-23, modificada el 2026-06-26). Hay además una versión «Estados-Financieros-2025-Firmados.pdf» subida el 2026-02-17 que no abrí.
- NIVEL: propiedad/financiación (documento del emisor) y declaración del propio medio.

OBJECIÓN 4 — La trayectoria societaria tiene fechas que la ficha no da, y la tercera figura sigue registrada
- QUÉ afirma la ficha: «El Morichal Comunicaciones S.A.S. (2016), liquidada; después operó como persona natural».
- POR QUÉ: hay que precisarlo con el RUES.
  (a) La cancelación de la S.A.S. es del 27-07-2026 (renovación tardía el 24-07-2026, último año renovado 2024). Es un hecho de los últimos 12 meses, no historia cerrada.
  (b) La matrícula de persona natural de Edwin Ernesto Suárez Narváez (CC Bogotá, organizacion_juridica "PERSONA NATURAL", CIIU 5813 «edición de periódicos», matriculada el 2021-02-25) sigue "ACTIVA", con último año renovado 2025.
  El propio medio dice que operó a nombre de la persona natural mientras la Corporación no tuvo cuenta. Lo que no consta hoy es si en 2026 la facturación (edictos, publicidad) ya pasó a la Corporación. Laguna: no hay informe de 2026.
- FUENTE: datos.gov.co c82u-588k (nit=900988084; consulta por razón social de la persona natural), 2026-10-10.
- NIVEL: registro externo / propiedad.

OBJECIÓN 5 — Los contratos públicos del fundador con entidades que el medio fiscaliza, y una pieza de 2026 que no los revela
- QUÉ afirma la ficha: «Esa franqueza es, por sí sola, un dato», y no menciona contratación pública.
- POR QUÉ (hecho): SECOP I y II, con el número de identificación de la persona natural tomado del RUES, devuelven 12 contratos entre 2018 y 2023, por un total de $149.897.327. Entre ellos:
  · GUAINÍA – GOBERNACIÓN, 2023-03-10, $37.800.000: «PRESTACION DE SERVICIOS PROFESIONALES PARA EL DESARROLLO DE ACTIVIDADES DE COMUNICACION QUE GARANTICEN LA DIVULGACION INTERNA; EXTERNA Y DE IMAGEN DE LA SECRETARIA DE GOBIERNO […]» ([enlace retirado: puede mostrar documentos de identidad; ver la resolución]).
  · VICHADA – GOBERNACIÓN, 2023-04-03, $29.700.000: «PRESTACION DE SERVICIOS PROFESIONALES PARA REALIZAR EL APOYO A LA SUPERVICION DEL PROYECTO […] RESGUARDOS INDIGENAS DEL DEPARTAMENTO» (numConstancia=23-12-13582425).
  · VICHADA – ASAMBLEA DEPARTAMENTAL, 2022-10-12, $3.900.000; GUAINÍA – GOBERNACIÓN, 2022-12-07 ($13.064.000) y 2022-12-09 ($6.840.000); ALCALDÍA DE INÍRIDA, 2019 y 2020; ALCALDÍA DE LA PRIMAVERA, 2019; GENSA, 2018 y 2019; CÁMARA DE REPRESENTANTES, 2019 (SECOP I) y 2020 (SECOP II, CPS_176_2020, $24.000.000).
  La identidad no es una homonimia: los contratos de GENSA con ese mismo número tienen por objeto avisos «en el periódico El Morichal».
  · SECOP para la S.A.S. (900988084): un solo contrato, CC Villavicencio, 2020-01-28, $600.000, «AVISO EN EL PERIODICO MORICHAL».
  · SECOP I y II para la Corporación (901978854): 0 contratos.
  · Últimos 12 meses: ningún contrato en ninguna de las tres identidades. El último es de abril de 2023, lo que cuadra con lo que el medio declara: «Desde finales de 2023 […] no recibimos pauta ni contratos […] de las gobernaciones, alcaldías y demás entidades del orden local de Vichada y Guainía».
- POR QUÉ (hecho editorial de los últimos 12 meses): «Nosotros» se impone esta regla: «Si una entidad con la que tenemos o hemos tenido un contrato se convierte en objeto de una investigación, la publicación se hace igual y la relación comercial se revela dentro del mismo texto.» La pieza de la Redacción del 2026-08-04, «Fiscalía compulsó copias contra el gobernador Fulberto Guevara y el exgobernador Álvaro León…», trata del gobernador de Vichada «entre 2020 y 2023». En su texto crudo no hay ninguna revelación del contrato de abril de 2023 con la Gobernación de Vichada.
- INFERENCIA, no hecho: que la regla se aplique a este caso es discutible. La investigación es contra el exgobernador, no contra la entidad, y el contrato fue un servicio profesional personal del fundador, no pauta del medio. Aun así, la ficha elogia la «franqueza» del medio sin haber mirado SECOP, y esta es justo la clase de conflicto de interés que el aviso del envío pide buscar (el caso de Diario La Libertad). Hasta abril de 2023 el fundador fue contratista de comunicaciones de las dos gobernaciones que hoy cubre.
- FUENTES: datos.gov.co f789-7hwg y jbjy-vk9h (consultadas el 2026-10-10); https://elmorichal.com/fiscalia-compulso-copias-contra-el-gobernador-fulberto-guevara-y-el-exgobernador-alvaro-leon-por-presunto-desfalco-a-dineros-de-regalias/ (2026-08-04).
- NIVEL: registro externo (SECOP) y hecho editorial de los últimos 12 meses. No mueve el número por sí sola: no hay contratos vigentes y no es evidencia de eje. Sí cambia lo que la ficha dice del perfil de conflictos.

OBJECIÓN 6 — La fuente que cita la ficha ya no sostiene los descriptores de los cofundadores
- QUÉ afirma la ficha: con «Nosotros» como fuente, «Director y cofundador», «Gardenia Nazaret Rebolledo Anija, abogada [descriptor personal retirado]» y «Edgar Guajo Bernavé, comunicador [descriptor personal retirado]».
- POR QUÉ: en el HTML crudo de «Nosotros» de hoy (modificada el 2026-08-07) no aparecen las cadenas «Gardenia», «Guajo», «Rebolledo» ni «Narváez». Tampoco están en content.rendered de /wp-json/wp/v2/pages/27228. El bloque de equipo está vacío. Los nombres sí constan como fundadores en el Informe Anual y en el Acta (Objeción 1), pero «abogada [descriptor personal retirado]», «[descriptor personal retirado]» y el cargo de «director» no se pueden comprobar hoy en la fuente citada. Gardenia Rebolledo aparece además como autora de notas del 7 y el 9 de octubre de 2026 (usuario WP id 11). No puedo saber si esos datos estaban en una versión anterior porque la Wayback Machine estaba fuera de servicio.
- FUENTE: https://elmorichal.com/nosotros/ y https://elmorichal.com/wp-json/wp/v2/pages/27228 (leídas el 2026-10-10).
- NIVEL: declaración del propio medio (comprobación de campo de la fuente).

## LO QUE NO PUDE VERIFICAR
- Profesión y nacionalidad de los cofundadores y el cargo de director: no están en el crudo de «Nosotros» hoy, y la Wayback Machine estaba fuera de servicio. Tampoco abrí el «Libro de Fundadores» (PDF escaneado de 6,3 MB sin capa de texto; pdftotext devolvió 2 bytes) ni el Acta de Constitución.
- Ingresos de 2026: no hay informe publicado y la Corporación dice que en 2025 no tenía cuenta bancaria. No sé qué parte de los ingresos actuales (edictos, becas, publicidad) entra por la Corporación y qué parte por la persona natural, cuya matrícula sigue activa.
- Posibles vínculos familiares entre fundadores (dos comparten el apellido Montoya): el medio se compromete a declararlos en «Nosotros» y no encontré esa declaración. No asumo parentesco: no está probado.
- Contratos privados o de cooperación de 2026 que no pasan por SECOP: no hay registro abierto donde buscarlos.
- La pieza «El laberinto fiscal del representante Luis Carlos Álvarez» (2026-09-29): solo vi el título en la API, no la leí.

## LO QUE FALTA
- El NIT, la matrícula y el representante legal tomados del RUES (Objeción 2), y la fecha de cancelación de la S.A.S. (Objeción 4).
- Los seis fundadores con su aporte idéntico (Objeción 1). Es la respuesta de nivel 1 a «a qué persona natural llega»: a seis personas con participación igual y un representante legal.
- Los estados financieros y el informe anual de 2025 (Objeción 3), la beca Fundación Gabo/PNUD y la línea de avisos judiciales como ingresos.
- El historial SECOP del fundador y la nota de que no hay contratos en los últimos 12 meses (Objeción 5).
- La autodeclaración editorial de hoy, que la ficha no recoge y es de nivel 4: «El Morichal concibe el periodismo como un ejercicio de contrapoder que vigila a las instituciones públicas y privadas»; «Nuestras investigaciones priorizan la empatía con las víctimas y la defensa de los derechos humanos, y dan espacio a quienes han sido silenciados por el conflicto y por los grandes medios tradicionales»; «Las directrices editoriales adoptadas por El Morichal tienen como referencia los lineamientos de Vorágine y Cuestión Pública». También: «Tampoco hacemos publicidad política de ninguna clase.» No la presento como prueba de eje (es nivel 4 y no basta para mover el número), pero la ficha debería citarla y decir por qué no la usa.
- La medición de nivel 2 del envío (38 artículos y 9 en historias en 40 días) contrasta con lo que da la API de WordPress: 45 entradas publicadas entre el 2026-08-31 y el 2026-10-09 y 293 en los últimos 12 meses. La base del 88 % de agenda propia (9 piezas) es muy pequeña. Además, una parte de esas 45 entradas son edictos judiciales, que inflan «artículos» sin ser agenda.

## EVIDENCIA QUE NO MUEVE EL NÚMERO
- Barrido de la regla del 2026-10-09 (voz de la casa, últimos 12 meses):
  · Categoría «editorial» (id 3): 25 piezas en total en la historia del sitio. La más reciente es del 2023-07-31 («Editorial: Arranca la carrera por las elecciones regionales»). Hay 0 editoriales entre el 2025-10-10 y el 2026-10-10. Consulta: https://elmorichal.com/wp-json/wp/v2/posts?categories=3&per_page=100.
  · En los 12 meses, la API da 293 entradas por autor: «Redacción» (id 5) 205; «Columnista invitado» (id 6) 25; Edwin Suárez (id 2) 15; y el resto, de autores individuales y de «Autor invitado». La cuenta de columnistas lleva esta descripción: «Los artículos de opinión no representan la posición editorial de EL MORICHAL.» Por la regla, esas 25 columnas no cuentan como voz de la casa.
  · En lo político de la Redacción, todo lo que revisé es fiscalización o información, a los dos lados del cambio de gobierno y sin postura editorial:
    – 2025-11-26, imputación a exgobernadores de Vichada por el CINER.
    – 2026-05-23, la investigación sobre la financiación de los representantes de Cambio Radical (Cuenca) y de La U (Molina), con preguntas a los dos.
    – 2026-08-04, compulsa de copias contra el gobernador en ejercicio Fulberto Guevara, de quien la pieza dice que llegó «con el aval de la Alianza Verde y el respaldo del Partido Liberal, ASI, MAIS y Colombia Humana», y contra el exgobernador León Flórez.
    – 2026-09-23, el PGN 2027 del «gobierno de Abelardo De La Espriella». La pieza recoge las críticas de los congresistas regionales y añade el contexto de que la inversión regionalizada «desde entonces ha bajado cada año» desde 2024, es decir, también con el gobierno anterior.
  · Resultado: no hay ≥10 piezas con postura en la voz de la casa, ni ≥3 a cada lado. La regla no se puede aplicar y no veo asimetría. Fiscalizar al gobernador de una coalición de izquierda local y al gobierno nacional de derecha entrante es oficio, y deja el 0,00 donde está.
  URLs: https://elmorichal.com/fiscalia-imputa-a-exgobernadores-de-vichada-por-presunta-corrupcion-en-el-ciner/ ; https://elmorichal.com/dos-representantes-elegidos-por-el-guainia-dos-modelos-de-financiacion/ ; https://elmorichal.com/fiscalia-compulso-copias-contra-el-gobernador-fulberto-guevara-y-el-exgobernador-alvaro-leon-por-presunto-desfalco-a-dineros-de-regalias/ ; https://elmorichal.com/presupuesto-general-de-la-nacion-2027-vichada-perderia-102-434-millones-y-guainia-11-995-millones/
- No encontré ningún endoso electoral en las elecciones legislativas del 08-03-2026. Su cobertura (tarjetón, candidatos, financiación de campañas) es informativa o de fiscalización. A esto se suma su declaración de que no hace «publicidad política de ninguna clase». Es conducta de la casa.
- Cero contratos públicos en los últimos 12 meses en las tres identidades (Corporación, S.A.S. y persona natural). Coincide con lo que el medio declara desde finales de 2023.
- Dejó de imprimir en diciembre de 2025, como dice la ficha. Lo confirma «Nosotros» («Hasta diciembre de 2025 mantuvimos una edición impresa mensual…») y la última edición en PDF de la biblioteca es la «No. 98», de diciembre de 2025 (subida el 2025-12-31).
- La cobertura declarada de Guainía se confirma: la categoría «guainia» tiene 1.177 entradas y «puerto-inirida», 764 (API de categorías, 2026-10-10).

## SIN OBJECIÓN
No aplica: hay seis objeciones. Ninguna mueve el valor 0,00. Todas corrigen o completan el nivel 1 (propiedad, registro y financiación) y el perfil de conflictos de interés que la ficha presenta como franqueza sin haber mirado SECOP. No encontré evidencia que sitúe al medio fuera de la banda mixta, y eso no es un aval.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** El revisor no copió cédulas, teléfonos ni direcciones particulares de personas naturales. Se comprobó por programa: el número de identificación de la persona natural del fundador no aparece en el texto, y las cifras largas que contiene son NIT de personas jurídicas, matrículas mercantiles, fechas del RUES, cuantías y números de constancia de SECOP. Los PDF del medio que cita (Informe Anual, Acta de Asamblea) sí traen cédulas y domicilios: ni el revisor ni esta resolución los copian.

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada:
  - elmorichal.com: «User-agent: *» con exclusiones solo de `/carrito/`, `/cart/`, `/checkout/` y de los parámetros `add-to-cart` y `remove_item`. No menciona a ClaudeBot, Claude-Web ni anthropic-ai.
  - datos.gov.co: `Crawl-delay: 1` y exclusiones de `/browse`, `/page`, `/catalog` con filtros; nada sobre esos agentes. Solo se usaron rutas `/resource/`.
  - contratos.gov.co: su `robots.txt` da 404 (no hay exclusiones).
  - web.archive.org: `robots.txt` da 404; la consulta CDX de `elmorichal.com/nosotros*` devolvió `[]` (no hay capturas).
  - No se tocaron eltiempo.com, cambiocolombia.com ni lasillavacia.com. No hubo buscador web.
- **Sitio**, descargado en crudo el 2026-10-10 con `curl -sL --ssl-no-revoke -A "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/126.0 Safari/537.36"`:
  - `/nosotros/` (dos veces, la segunda con un parámetro para saltar caché) y las cuatro piezas que cita el revisor; todas dieron 200.
- **API REST de WordPress**:
  - `/wp/v2/pages/27228`, `/wp/v2/pages` (8 páginas; 2 creadas en 12 meses), `/wp/v2/users`, `/wp/v2/categories`, `/wp/v2/media?mime_type=application/pdf` (`X-WP-Total: 124`, con el campo `post` para ver de qué página cuelga cada PDF) y `/wp/v2/search`;
  - `/wp/v2/posts?categories=3` (Editorial) y **todas las entradas de los 12 meses**: `/wp/v2/posts?after=2025-10-10T00:00:00`, `X-WP-Total: 293`, del 2025-10-11 al 2026-10-09, con su contenido. El barrido de la objeción 5 y el de la voz de la casa se hicieron sobre los cuerpos.
- **PDF del medio**, descargados de `wp-content/uploads` y leídos con `pdftotext`: Informe Anual de Resultados, Estados Financieros 2025 (VF), Acta de Asamblea 001, Estatutos (reforma de 2026), Directrices editoriales (2026-02-17) y la Invitación Pública de Barrancominas. Las cifras largas se enmascararon antes de leerlas.
- **Registros**, en datos.gov.co:
  - RUES (`c82u-588k`): `nit=901978854`, `nit=900988084`, `razon_social like '%MORICHAL%'` (139 filas, ninguna otra del medio) y la matrícula de persona natural por nombre.
  - SECOP I (`f789-7hwg`, `identificacion_del_contratista`) y SECOP II (`jbjy-vk9h`, `documento_proveedor`), con **igualdad exacta**, para 901978854, 900988084, los mismos NIT con dígito de verificación (0 filas) y el número de identificación de la persona natural del fundador. Además, por nombre: «MORICHAL» en SECOP II y «MORICHAL COMUNICA» / «CORPORACION EL MORICHAL» en SECOP I.
  - La ficha de proceso de SECOP I `23-12-13582425` en contratos.gov.co (los documentos adjuntos piden reCAPTCHA y no se abrieron).
  - **El número de identificación de la persona natural se usó dentro de las consultas y no se escribe en ningún sitio.**

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | Son seis fundadores, no tres | sí | sí | **Aceptada.** Y la ficha ya estaba mal el día del alta: el Informe Anual y el Acta están colgados desde el 2026-06-20, y la versión de «Nosotros» del 07-08-2026 dice «seis personas» |
| 2 | El NIT y el registro están en el RUES | sí | sí, campo por campo | **Aceptada.** Cámara de Villavicencio, no de Vichada |
| 3 | La laguna de financiación se cae | sí | sí | **Aceptada, con dos precisiones:** los $1.080.000 son aportes al patrimonio, no ingresos (ingresos de 2025: 0); y la beca Fundación Gabo/PNUD financia una pieza, no consta que entre a la Corporación |
| 4 | La S.A.S. se canceló el 27-07-2026; la persona natural sigue activa | sí | sí | **Aceptada** |
| 5 | Contratos públicos del fundador; la pieza del 04-08-2026 no los revela | sí | sí, recalculado | **Parcial.** Las 12 filas y los $149.897.327 se reproducen al peso, pero **una no entra como hecho**: el contrato de la Gobernación de Vichada (03-04-2023, $29.700.000) lleva el mismo número de documento y **otro nombre** como contratista y representante legal. Quedan 11 contratos por $120.197.327. **Se rechaza la inferencia sobre la pieza del 04-08-2026**, que se apoyaba justo en ese contrato. Sí hay dos casos análogos con contratos atribuibles, que se declaran como tensión |
| 6 | «Nosotros» ya no sostiene los descriptores de los cofundadores | sí | sí | **Parcial.** Es cierto que el HTML que ve el lector no los trae. Pero el buscador de WordPress demuestra que el contenido guardado de esa página sí contiene esos términos: la ficha no se los inventó. Aun así, **los descriptores personales salen de la ficha** |

### Lo verificado, objeción por objeción

**1 · Seis fundadores.**
- «Nosotros», crudo (`article:modified_time` 2026-08-07T17:23:20+00:00): «En agosto de 2025 nos constituimos como organización sin ánimo de lucro: Corporación El Morichal, integrada por seis personas vinculadas directa o indirectamente con el periódico desde hace al menos siete años.» y «El equipo que produce el periódico día a día —reportería, edición y plataformas digitales— es otro y se presenta más abajo; tres personas hacen parte de ambos.» Literales.
- Informe Anual de Resultados (subido el 2026-06-20; periodo 20-08-2025 a 31-12-2025): seis aportes «de constitución» de $180.000, total «$1,080,000». Aportantes: Edwin Ernesto Suárez Narváez, Edgar Guajo Bernavé, Juliana Montoya Álvarez, Gardenia Nazareth Rebolledo Anija, Rafael Montoya Parra y Juan Miguel Chitiva. Firma el Informe «Edwin Ernesto Suarez Narváez […] Representante Legal».
- Acta de Asamblea 001 (21-05-2026), lista de asistencia: los mismos seis, de «Fundador 1» a «Fundador 6». Firman el acta Edwin Ernesto Suárez Narváez (presidente) y Juliana Montoya Álvarez (secretaria). El acta escribe «Gardenia Nazaret»; el Informe, «Nazareth».
- **Fecha.** Los dos PDF son siete semanas anteriores a la ficha (2026-08-09). La versión de «Nosotros» que dice «seis personas» es de dos días antes. El error estaba ya el día del alta.
- **Quiénes son las «tres personas» que están en la Corporación y en el equipo no consta.** Gardenia Rebolledo publica como autora (usuario WP 11: cinco entradas del 02-10 al 09-10-2026, y la firma «Por: Gardenia Rebolledo» en una nota del 03-06-2026), y Edwin Suárez como fundador. El tercero no se puede afirmar.

**2 · RUES.** Fila de `nit=901978854`, literal: `"razon_social":"CORPORACIÓN EL MORICHAL"`, `"camara_comercio":"VILLAVICENCIO"`, `"matricula":"9000510935"`, `"tipo_sociedad":"ENTIDAD SIN ANIMO DE LUCRO"`, `"organizacion_juridica":"CORPORACIONES"`, `"cod_ciiu_act_econ_pri":"9499"`, `"fecha_matricula":"20250820"`, `"fecha_renovacion":"20260216"`, `"ultimo_ano_renovado":"2026"`, `"estado_matricula":"ACTIVA"`, `"representante_legal":"SUAREZ NARVAEZ EDWIN ERNESTO"`, `"fecha_actualizacion":"2026/06/05 …"`. Todo coincide con el revisor. El RUES abierto no da los asociados; los da el Informe Anual (obj. 1).

**3 · Financiación.**
- Estados Financieros 2025 (VF): «NOTA 9- INGRESOS […] 4295 Ingresos por Donaciones 0.00 / 4296 Aportes Voluntarios 0.00 / TOTAL 0.00». «Total ACTIVO 162,019.00» y «Total PATRIMONIO 162,019.00». Literales.
- Informe Anual: «La corporación no recibió donaciones ni aportes adicionales a los efectuados por los fundadores al momento de su constitución»; «La corporación no celebró contratos durante el período»; gastos de $917.981 y saldo de $162.019. **Precisión:** el propio Informe dice que los aportes «hacen parte del patrimonio de la entidad y no constituyen ingresos». La ficha debe decir «ingresos 0; patrimonio inicial de $1.080.000 aportado a partes iguales por los seis fundadores», no «se financió con $1.080.000».
- «Así nos financiamos» y la frase sobre la cuenta bancaria («no tuvo cuenta bancaria ese año: durante esos meses el medio siguió operando bajo la figura de persona natural, a nombre de Edwin Suárez»): literales.
- Beca: «Esta pieza periodística es resultado de las Becas del Taller: ‘Periodismo y elecciones en Colombia: contar lo que importa para la democracia’, otorgadas por la Fundación Gabo en alianza con el Programa de las Naciones Unidas para el Desarrollo (PNUD).» Literal. **Precisión:** esa URL es una **página** de WordPress (id 28337), no una entrada, publicada el 2026-05-23 y modificada el 2026-06-26. Financia esa pieza; no consta a quién se pagó ni si entró por la Corporación.
- Edictos: la categoría tiene 48 entradas en total y **34 en los últimos 12 meses** (del 2025-11-08 al 2026-10-07). Sigue siendo inferencia que generen ingreso y no consta quién los factura. Además hay una entrada «[Publicidad] Tarifas SIN y ZNI enero 2026 – Empresa Siglo XXI» (04-02-2026), rotulada como publicidad.
- **Lo que el revisor no trae:** los Estatutos (reforma aprobada en el Acta 001) dicen: «Queda expresamente prohibida la aceptación de donaciones provenientes de partidos o movimientos políticos, así como de empresas o entidades que pretendan influir directa o indirectamente en la línea editorial». Es declaración del propio medio (nivel 4).
- **Los PDF no están enlazados en la página que ve el lector.** La sección «Rendición de cuentas» del HTML no trae enlaces: no hay ningún `href` a un PDF en toda la página. Pero la API de medios muestra que once documentos cuelgan de la página 27228 («Nosotros»): ESFA, Acta de constitución y Estatutos (2025-09-23), Estados Financieros firmados y Directrices (2026-02-17), y los seis del 2026-06-20.

**4 · Trayectoria registral.**
- `nit=900988084`, literal: `"razon_social":"EL MORICHAL COMUNICACIONES S A S -"`, `"camara_comercio":"BOGOTA"`, `"matricula":"2708137"`, `"fecha_matricula":"20160711"`, `"fecha_renovacion":"20260724"`, `"ultimo_ano_renovado":"2024"`, `"fecha_cancelacion":"20260727"`, `"estado_matricula":"CANCELADA"`, `"representante_legal":"EDWIN ERNESTO SUAREZ NARVAEZ"`, `"fecha_actualizacion":"2026/07/28 …"`.
- Persona natural: «EDWIN ERNESTO SUAREZ NARVAEZ», Cámara de Bogotá, `"organizacion_juridica":"PERSONA NATURAL"`, CIIU 5813, `"fecha_matricula":"20210225"`, `"ultimo_ano_renovado":"2025"`, `"estado_matricula":"ACTIVA"`.
- **Identidad, por documento y sin escribirlo:** el número de identificación de esa matrícula es **idéntico** al del representante legal de la Corporación y al del representante legal de la S.A.S. (comparado por programa). Es la misma persona en los tres registros.
- «Nosotros» dice que la S.A.S. «nunca funcionó y fue liquidada». El RUES no dice «liquidada»: dice «CANCELADA», con inscripción el 27-07-2026, dentro de la ventana de 12 meses y antes de la ficha.

**5 · Contratación pública, recalculada.**
- **Corporación El Morichal (901978854):** 0 en SECOP I y 0 en SECOP II. También 0 con el dígito de verificación.
- **El Morichal Comunicaciones S.A.S. (900988084):** 1 en SECOP I, «META - CÁMARA DE COMERCIO DE VILLAVICENCIO», 2020-01-28, $600.000, «AVISO EN EL PERIODICO MORICHAL». 0 en SECOP II. 0 con dígito.
- **Persona natural del fundador**, por su número de identificación del RUES y con igualdad exacta: 11 filas en SECOP I y 1 en SECOP II. Las 12 suman **$149.897.327, al peso con el revisor**. Pero el nombre de contratista no es el mismo en todas:
  - **10 de SECOP I** van a nombre de «EDWIN ERNESTO SUAREZ NARVAEZ» o «EDWIN SUAREZ» (Gensa, 2018), y la de **SECOP II** a nombre de «Edwin Erensto Suárez Narváez», así, con la errata (Cámara de Representantes, CPS_176_2020, $24.000.000). Dos objetos de Gensa nombran el periódico («EN EL PERIoDICO EL MORICHA!», «EN EL PERIDICO EL MORLCHAL DE INLRIDA», con los errores de OCR del registro). **Estas 11 se atribuyen al fundador:** coinciden el documento y el nombre.
  - **La fila `23-12-13582425`** (VICHADA - GOBERNACIÓN, contrato 489-2023, 03-04-2023, $29.700.000, «APOYO A LA SUPERVICION DEL PROYECTO […] RESGUARDOS INDIGENAS») lleva `"nom_razon_social_contratista":"FRANCISCO JAVIER GONZALEZ"` y `"nombre_del_represen_legal":"FRANCISCO JAVIER GONZALEZ"`. La ficha del proceso en contratos.gov.co dice lo mismo: «Nombre o Razón Social del Contratista FRANCISCO JAVIER GONZALEZ», con el número de documento del fundador. **El registro se contradice a sí mismo** (nombre de una persona, documento de otra), y el revisor no lo dice. No entra como contrato del fundador. Tampoco se atribuye a nadie más: es un registro inconsistente.
- **Total atribuible: 11 contratos por $120.197.327, de 2018 a 2023.** Por contratante:
  - Gobernación del Guainía: 3, $57.704.000 (07-12-2022, $13.064.000, perifoneo de salud; 09-12-2022, $6.840.000, perifoneo; 10-03-2023, $37.800.000, comunicación «INTERNA; EXTERNA Y DE IMAGEN DE LA SECRETARIA DE GOBIERNO»);
  - Cámara de Representantes: 2, $37.333.333 (2019 y 2020);
  - Alcaldía de Inírida: 2, $17.359.994 (15-11-2019, $4.159.994; 31-08-2020, $13.200.000, «FORTALECIMEINTO DE ESTRATEGIAS COMUNICATIVAS DE LA ALCALDIA DE INiRIDA»);
  - Asamblea Departamental de Vichada: 1, $3.900.000 (12-10-2022, «UN COMUNICADOR SOCIAL»);
  - Alcaldía de La Primavera: 1, $2.000.000 (25-06-2019, avisos de prensa);
  - Gensa: 2, $1.900.000 (2018 y 2019, avisos en el periódico).
- **Últimos 12 meses: 0 en las tres identidades.** El último atribuible es del 10-03-2023. Cuadra con «Desde finales de 2023 […] no recibimos pauta ni contratos […] de las gobernaciones, alcaldías y demás entidades del orden local de Vichada y Guainía» (literal en «Nosotros»).
- **La pieza del 04-08-2026.** Las citas son literales: «Dos de los siete son de Vichada: Fulberto Guevara, gobernador en ejercicio, y Álvaro León Flórez, quien ocupó el cargo entre 2020 y 2023», y «con el aval de la Alianza Verde y el respaldo del Partido Liberal, ASI, MAIS y Colombia Humana». No hay revelación de ningún contrato. Pero el único contrato con la Gobernación de Vichada es justo el de la fila inconsistente. Con lo atribuible, el fundador no contrató con esa Gobernación (sí con la Asamblea, en 2022, que es otra entidad). **No hay omisión que anotar en esa pieza.**
- **Lo que sí aparece al barrer los 293 cuerpos de los 12 meses**, buscando las entidades que contrataron al fundador:
  - **2026-02-28**, Redacción, «Procuraduría formuló pliego de cargos al exgobernador de Guainía Juan Carlos Iral por puentes inconclusos». Iral gobernó de 2020 a 2023 (la pieza del 27-02-2026 lo fecha: «durante casi todo el mandato de Juan Carlos Iral (2020 – 2023)»). Bajo ese mandato, la Gobernación del Guainía contrató al fundador tres veces (dic-2022 y mar-2023), una de ellas para la «imagen» de su Secretaría de Gobierno.
  - **2026-03-20**, Redacción, «Procuraduría formuló pliego de cargos contra exalcalde de Inírida Pablo Acosta…»: «quien ejerció el cargo entre 2020 y 2023». Bajo ese mandato, la Alcaldía de Inírida contrató al fundador (31-08-2020, $13.200.000) para sus «estrategias comunicativas».
  - Ninguna de las dos menciona esos contratos. En ninguna de las 293 entradas aparece «relación comercial», «hemos tenido un contrato» ni una nota de revelación de ese tipo.
- **Por qué no es incumplimiento de la regla del medio, y por qué se declara igual:**
  - La regla de «Nosotros» («Si una entidad con la que tenemos o hemos tenido un contrato se convierte en objeto de una investigación, la publicación se hace igual y la relación comercial se revela dentro del mismo texto») consta en la versión del **07-08-2026**. Las Directrices en PDF del 17-02-2026 **no la traen** (no contienen «contrato» ni «pauta»; «comercial» sale una vez, en «intereses económicos o comerciales»). Solo traen una regla general: «Cualquier integrante del equipo […] incluyendo su director, debe informar sobre algún conflicto de intereses […]. Esto incluye revelar cualquier afiliación política, financiera o personal». No hay capturas de archivo de «Nosotros», así que no consta desde cuándo existe la regla específica.
  - Los procesos son disciplinarios contra personas (exgobernador, exalcalde), no contra las entidades.
  - Los contratos eran servicios personales de comunicación del fundador. Pero el propio medio dice que operaba «bajo la figura de persona natural, a nombre de nuestro fundador», y la matrícula de esa persona natural tiene el CIIU 5813 (edición de periódicos) desde 2021. La frontera entre «contrato del fundador» y «contrato del medio» no es nítida, y eso es justo lo que el lector debería saber.
  - **Conclusión:** es un **hallazgo de conducta para declarar como tensión de transparencia (desvelamiento, no acusación)**, igual que en Proclama, Lente Regional o La Nación. No es evidencia de eje (los dos procesos son fiscalización) y no mueve el número.

**6 · Descriptores de los cofundadores.**
- **Lo que dice el revisor se confirma para el lector:** en el HTML crudo, descargado dos veces, hay 0 apariciones de «Gardenia», «Guajo», «Rebolledo», «Anija», «[descriptor personal retirado]», «[descriptor personal retirado]» y «abogad». Igual en `content.rendered` de `/wp/v2/pages/27228` (`"modified":"2026-08-07T12:23:20"`). Los contenedores de Elementor `12a3dd6` y `3206bb6` están vacíos. «director» sale dos veces, siempre genérico («incluido su director», «El director, los periodistas…»).
- **Lo que el revisor no vio:** el buscador de WordPress (`/wp/v2/search?subtype=page`) busca en el contenido **guardado** de cada página, no en el que se muestra. Sobre las 8 páginas del sitio, devuelve **solo la 27228** para «Gardenia», «Guajo», «Rebolledo», «Anija», «Bernave», «[descriptor personal retirado]», «[descriptor personal retirado]», «comunicador», «cofundador» y «cofundadora», y para las frases exactas «Gardenia Nazaret Rebolledo Anija», «Edgar Guajo», «[descriptor personal retirado]», «comunicador [descriptor personal retirado]» y «fundador y director». No la devuelve para «abogada [descriptor personal retirado]» como frase exacta, «Juliana Montoya», «Rafael Montoya» ni «Chitiva». Una palabra de control inventada devuelve `[]`.
- **Lectura:** el texto del equipo sigue guardado en la página y no se publica. Encaja con la frase «se presenta más abajo» y con los contenedores vacíos. **La ficha no se inventó los descriptores**, pero hoy **ningún lector puede comprobarlos** en la fuente citada, y no se puede leer su redacción exacta.
- **Aun así salen de la ficha.** Tres motivos:
  1. Un dato que el lector no puede comprobar en la fuente enlazada no sostiene una afirmación sobre una persona natural.
  2. El origen étnico es dato sensible (Ley 1581, art. 5). La nacionalidad y el lugar de nacimiento no lo son, pero tampoco aportan nada a la pregunta de propiedad.
  3. Nada de lo que el lector necesita saber depende de ellos: basta el nombre, el papel y el enlace (regla de DATOS PERSONALES).
- **«Director».** El sitio no nombra hoy a ningún director. El fundador consta: «a nombre de nuestro fundador, Edwin Suárez» («Nosotros») y «Fundador del periódico EL MORICHAL» (descripción del usuario WP 2). Su cargo verificable es el de **representante legal de la Corporación** (RUES).

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se rechazan como hecho, o se corrigen, estas partes:
- **Obj. 5: el contrato de abril de 2023 con la Gobernación de Vichada como contrato del fundador.** El registro de SECOP lo da a nombre de otra persona, como contratista y como representante legal, aunque con el documento del fundador. Con una contradicción interna, la identidad no está probada en ninguna dirección.
- **Obj. 5: la inferencia sobre la pieza del 04-08-2026.** Cae con lo anterior. Sin ese contrato, el fundador no contrató con la Gobernación de Vichada. Se sustituye por los dos casos del 28-02 y del 20-03-2026, que sí tienen contratos atribuibles.
- **Obj. 5: «Hasta abril de 2023 el fundador fue contratista de comunicaciones de las dos gobernaciones que hoy cubre».** Solo consta de la del Guainía (hasta el 10-03-2023). De Vichada consta la Asamblea (2022) y la Alcaldía de La Primavera (2019).
- **Obj. 6: que la fuente «ya no sostiene» los descriptores, en el sentido de que no tengan base.** El contenido guardado de la página los contiene. Lo que falla es la publicación del bloque, no la fuente. La consecuencia práctica (sacarlos de la ficha) se mantiene.
- **Obj. 3: «El dinero de 2025 son los $1.080.000».** Son aportes al patrimonio. Los ingresos de 2025 son 0, según el propio documento.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente.** Todas las URL resuelven (200), las citas son literales y las cifras del RUES y de SECOP coinciden al peso. Deformaciones y omisiones:
- **Omite que la fila de la Gobernación de Vichada lleva otro nombre.** Es la omisión que más pesa: su inferencia sobre la pieza del 04-08 descansa en ella.
- **«Su última firma que encontré en el sitio es del 2026-05-23 (usuario WP id 2, «Edwin Suárez»)».** La pieza del 23-05 es la página 28337, cuyo autor en WordPress es el usuario 8. Edwin Suárez figura en el texto («Autor: Edwin Suárez»). Las últimas entradas del usuario 2 son del 2026-05-03.
- **«Gardenia Rebolledo aparece además como autora de notas del 7 y el 9 de octubre».** Son cinco entradas del usuario 11 (02-10, 06-10, dos del 07-10 y 09-10-2026), más una firma «Por: Gardenia Rebolledo» del 03-06-2026.
- **«La Wayback Machine respondió «Temporarily Offline»».** Hoy responde, pero no tiene ninguna captura de `/nosotros/`. La laguna sigue, por otra causa.
- **Nivel 2:** las 45 entradas de la ventana del envío (31-08 → 09-10) se confirman, y 7 son edictos. 45 − 7 = 38, que es el número de artículos de la medición. Puede ser coincidencia: no se comprobó si la ingesta excluye los edictos. Además, la investigación del 23-05 es una página, y las páginas no salen en el feed `/feed/`.
- **Omite** la cláusula de los Estatutos contra donaciones de partidos, la regla general de conflicto de interés de las Directrices de febrero, y la entrada «[Edicto] Invitación pública No. 001 de 2026 de la Alcaldía de Barrancominas» (25-02-2026). Esta última es un aviso de una alcaldía del Guainía publicado en la ventana. No hay contrato en SECOP con ninguna de las tres identidades, y no consta que fuera pagado. Va como pregunta, no como hecho, frente a la declaración de que no recibe «pauta ni contratos» de las alcaldías del Guainía.

**Errores de la propia ficha, para no repetirlos:**
- «uno de los tres cofundadores», «una corporación pequeña de tres personas», «En un medio de tres personas»: falso. Son seis fundadores, y lo estaba el día del alta.
- «Falta el NIT y falta el certificado de Cámara de Comercio, así que sigue siendo autodeclarado»: el NIT y la matrícula estaban en el RUES abierto. El certificado sigue sin pedirse, pero ya no hace falta para la existencia, la fecha ni el representante legal.
- «no he documentado ni una sola fuente de financiación»: los Estados Financieros 2025 (VF) y el Informe Anual estaban colgados desde el 2026-06-20, y una versión «Firmados» de los estados, desde el 2026-02-17 (esta no se abrió).
- «El Morichal Comunicaciones S.A.S. (2016), liquidada»: sin fecha. La cancelación se inscribió el 27-07-2026, dentro de la ventana.
- «abogada [descriptor personal retirado]», «comunicador [descriptor personal retirado]», «un comunicador [descriptor personal retirado]»: no comprobables hoy para el lector, y no necesarios (ver obj. 6).
- «Director y cofundador»: el sitio no nombra director. El cargo verificable es el de representante legal.
- «REFUTACIÓN 2: El certificado de Cámara de Comercio de Vichada»: la matrícula es de la Cámara de Villavicencio.
- «Nivel 2 — Conducta medida: NO EXISTE»: superado. El envío del 2026-10-10 trae 38 artículos y 9 en historias, en 40 días.
- **Falta la línea de contratación pública** que exige el protocolo desde el 2026-10-07.
- En `shared/centinela.js`: «Es la tercera figura jurídica del medio en nueve años —dos anteriores liquidadas—». Falso: solo hubo una sociedad, cancelada el 27-07-2026. La persona natural sigue con su matrícula activa.
- En `shared/mediaOwnership.js`, `holdings[1]` repite los descriptores personales y añade «con estudios en comunicación social», que tampoco se puede comprobar hoy. `notes[1]` («No consta ninguna fuente de financiación») es falso desde junio.

---

**Propuesta para la firma**

**(a) Valor: mantener 0,00, provisional.** Los motivos:
- **No hay voz de la casa con postura en los últimos 12 meses.**
  - La categoría Editorial tiene 0 entradas en la ventana; la última es del 31-07-2023.
  - La de Opinión tiene 25: 24 del usuario «Columnista invitado», cuya descripción dice «Los artículos de opinión no representan la posición editorial de EL MORICHAL», y un «[Ficción]» del 06-03-2026.
  - Un barrido por términos sobre los 293 cuerpos («extrema derecha», «ultraderecha», «progresista», «petrismo», «fascis», «oligarqu», «uribis», «castrochav», «mamert»…) da un solo resultado: «petrismo» entre comillas, en una columna invitada del 17-03-2026.
  - Las piezas de la Redacción que nombran a Petro o a De la Espriella (06-05, 16-06, 08-09, 16-09, 17-09, 18-09 y 23-09-2026, y el tarjetón del 26-02) recogen declaraciones o informan. La más crítica, la del PGN 2027 del 23-09, contextualiza que la inversión «desde entonces ha bajado cada año» desde 2024, es decir, también con el gobierno anterior.
  - La regla de «Evidencia editorial histórica» **no se puede aplicar**: no hay piezas con postura que contar.
- **Lo que sí hace la casa es fiscalizar el poder local, a los dos lados:**
  - 26-11-2025, CINER;
  - 28-02 y 20-03-2026, Iral y Acosta;
  - 04-08-2026, el gobernador Guevara, de una coalición de Alianza Verde, Liberal, ASI, MAIS y Colombia Humana, y el exgobernador León Flórez;
  - 23-09-2026, el presupuesto del gobierno De la Espriella.
  - Por el polo fijo, nada de esto sitúa al medio en el eje.
- **La propiedad (nivel 1) ya está documentada** y no sitúa al medio en el eje: es una ESAL de seis fundadores con aportes iguales, ingresos 0 en 2025 y estatutos que prohíben donaciones de partidos.
- Razón escrita propuesta: «0,00. Corporación sin ánimo de lucro de seis fundadores con aportes iguales (RUES e Informe Anual 2025). En 12 meses no publicó editoriales y su opinión es de columnistas invitados; la Redacción fiscaliza a gobiernos locales de distinto signo y al gobierno nacional entrante sin rótulos ni postura. Nada lo sitúa en el eje. No es neutralidad: su línea declarada es el contrapoder local y la defensa de comunidades indígenas y campesinas, que no es una posición izquierda-derecha».

**(b) Correcciones de hecho, con su fuente**

En `fichas/el-morichal.md`:
1. **Nivel 1, tabla:**
   - «Razón social» → «**Corporación El Morichal**, ESAL, NIT 901978854, matrícula 9000510935 de la Cámara de Comercio de Villavicencio, inscrita el 20-08-2025, activa y renovada en 2026 ([RUES abierto](https://www.datos.gov.co/resource/c82u-588k.json?$select=razon_social,sigla,nit,camara_comercio,matricula,organizacion_juridica,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,fecha_cancelacion,cod_ciiu_act_econ_pri&nit=901978854), consultado 2026-10-10)».
   - «Figura anterior» → «El Morichal Comunicaciones S.A.S. (NIT 900988084, Cámara de Bogotá, matriculada en 2016). Según el medio, “nunca funcionó y fue liquidada”; el RUES inscribe su **cancelación el 27-07-2026**. Después, el medio operó como persona natural a nombre de su fundador, cuya matrícula mercantil (Cámara de Bogotá, edición de periódicos, desde 2021) sigue activa».
   - Las tres filas de personas se sustituyen por:
     - «Representante legal: **Edwin Ernesto Suárez Narváez** (RUES), fundador del medio (“Nosotros”)»;
     - «Fundadores de la Corporación, con el mismo aporte ($180.000 cada uno): Edwin Ernesto Suárez Narváez, Edgar Guajo Bernavé, Juliana Montoya Álvarez, Gardenia Nazaret Rebolledo Anija, Rafael Montoya Parra y Juan Miguel Chitiva ([Informe Anual de Resultados 2025]([PDF Informe-Anual-de-Resultados, enlace retirado: trae documentos de identidad; cuelga de https://elmorichal.com/nosotros/]); [Acta de Asamblea 001]([PDF Acta-de-Asamblea-001_21_05_26, enlace retirado: trae documentos de identidad; cuelga de https://elmorichal.com/nosotros/]), 21-05-2026)».
     - «Dirección de la redacción: el sitio no nombra director a 2026-10-10».
   - **Sin nacionalidad, origen, lugar de nacimiento, profesión, documentos ni domicilios.** Ver la decisión 2.
2. **Párrafo «Fuente:…»** → sustituir «Falta el NIT y falta el certificado… autodeclarado» por: «Existencia, fecha, NIT y representante legal: RUES. Fundadores y cuentas: documentos de la propia Corporación, colgados el 2026-06-20 (no enlazados desde la página visible: el bloque “Rendición de cuentas” se publica vacío). Falta el certificado de existencia y representación de la Cámara de Villavicencio». Retirar «Ninguno de los otros veintiún candidatos cuenta que tuvo una sociedad y la cerró», o fecharlo: la cancelación es de julio de 2026.
3. **«Es una corporación de once meses»** → «constituida el 20-08-2025».
4. **GUAINÍA DEJA DE ESTAR DEL TODO EN BLANCO:** retirar «Y uno de los tres cofundadores es **un comunicador [descriptor personal retirado]**, lo cual es más de lo que puede decir la cobertura que hoy le llega a ese departamento desde Bogotá». Puede quedar, con su fuente: «la categoría Guainía tiene 1.177 entradas e Inírida, 764 (API, 2026-10-10)».
5. **Financiación**, sección nueva de nivel 1: «2025: ingresos 0; patrimonio inicial de $1.080.000, aportado a partes iguales por los seis fundadores; gastos de constitución de $917.981; saldo de $162.019 (Estados Financieros 2025 e Informe Anual). La Corporación no tuvo cuenta bancaria en 2025 y el medio siguió operando como persona natural. Declara que antes vivía de subvenciones para investigaciones y de publicidad privada, de empresas de servicios públicos y de entidades nacionales, y que ahora apuesta por subvenciones internacionales, proyectos editoriales y servicios. En 2026 publica edictos judiciales (34 en 12 meses) y una pieza financiada por la beca Fundación Gabo/PNUD (23-05-2026). Sus estatutos prohíben las donaciones de partidos. 2026: sin informe todavía; no consta qué ingresos entran por la Corporación y cuáles por la persona natural».
6. **CONTRATACIÓN PÚBLICA**, línea nueva en el formato del protocolo:

> Contratación pública (SECOP I y II, consultado 2026-10-10). **Corporación El Morichal (NIT 901978854):** 0 contratos. **El Morichal Comunicaciones S.A.S. (NIT 900988084, cancelada el 27-07-2026):** 0 en los últimos 12 meses; 1 por $600.000 en total (Cámara de Comercio de Villavicencio, 28-01-2020, un aviso en el periódico). **Edwin Ernesto Suárez Narváez, fundador y representante legal, como persona natural** (figura con la que operó el medio antes de la Corporación; identificado por el documento de su matrícula en el RUES, que no se escribe): 0 contratados en los últimos 12 meses; 11 por $120.197.327 de 2018 a 2023. Principales contratantes: Gobernación del Guainía ($57.704.000, tres contratos entre diciembre de 2022 y marzo de 2023, de perifoneo y de comunicación de su Secretaría de Gobierno), Cámara de Representantes ($37.333.333, 2019-2020), Alcaldía de Inírida ($17.359.994, 2019-2020), Asamblea de Vichada ($3.900.000, 2022), Alcaldía de La Primavera ($2.000.000, 2019) y Gensa ($1.900.000, avisos en el periódico, 2018-2019). La Gobernación del Guainía, la Alcaldía de Inírida, la Asamblea de Vichada y la Alcaldía de La Primavera son entidades que el medio cubre. No se cuenta un registro de la Gobernación de Vichada (03-04-2023, $29.700.000) que lleva ese mismo documento pero otro nombre como contratista.

7. **Hallazgos del ciclo 2**, sección nueva, como en las fichas de la tanda 4, separando hecho y no hecho. Tensión de transparencia: «En 2026 la Redacción publicó los pliegos de cargos contra el exgobernador del Guainía Juan Carlos Iral (28-02) y contra el exalcalde de Inírida Pablo Willan Acosta (20-03), ambos de 2020-2023, sin mencionar que esas administraciones contrataron al fundador (Gobernación del Guainía, 2022-2023; Alcaldía de Inírida, 2020). La regla de revelación de “Nosotros” consta en su versión del 07-08-2026, y no consta que existiera antes; los procesos son contra personas, no contra las entidades. Es desvelamiento, no acusación, y no mueve la clasificación».
8. **Nivel 4, nuevo:** las citas de «Nosotros» de hoy, con fecha: contrapoder, víctimas y derechos humanos, Vorágine y Cuestión Pública como referencia, «Tampoco hacemos publicidad política de ninguna clase». Se citan y se dice por qué no mueven el número (nivel 4).
9. **Nivel 2:** sustituir «NO EXISTE» por las cifras del envío del 2026-10-10 (38 artículos, 9 en historias, 40 días, agenda propia del 88 % sobre 8 historias), con la advertencia de base pequeña y la nota de que sus investigaciones largas pueden ir como páginas, fuera del feed.
10. **ARGUMENTO:** la razón de (a). Retirar «una corporación pequeña de tres personas en la Orinoquía».
11. **CONTRA:** sustituir «no he documentado ni una sola fuente de financiación» y «En un medio de tres personas» por la financiación documentada del punto 5. Lo que sigue abierto: los ingresos de 2026 y quién los factura.
12. **REFUTACIÓN:**
    - el punto 1 queda cumplido para 2025, y se reescribe: «el informe de 2026, con ingresos por fuente»;
    - el punto 2 pasa a: «el certificado de la Cámara de Comercio de Villavicencio»;
    - se añade: «si el medio enlaza o deja de publicar los documentos de rendición de cuentas, o si declara vínculos familiares entre fundadores como promete en “Nosotros”».

En `shared/mediaOwnership.js`, entrada `el-morichal`:

13. `holdings[0]` → «Lo sostiene la Corporación El Morichal, ESAL inscrita el 20-08-2025 en la Cámara de Comercio de Villavicencio (NIT 901978854), con seis fundadores que aportaron lo mismo. Su representante legal es Edwin Ernesto Suárez Narváez, fundador del medio. Antes fue El Morichal Comunicaciones S.A.S. (NIT 900988084), cuya cancelación se inscribió el 27-07-2026, y después operó como persona natural a nombre del fundador».
14. `holdings[1]` → la lista de los seis fundadores con «fundador/a» como único papel, sin descriptores. Ver la decisión 2.
15. `notes[1]` → «Ingresos de 2025: 0; patrimonio inicial de $1.080.000 de los fundadores (Estados Financieros 2025 e Informe Anual). Sin informe de 2026. Sus estatutos prohíben donaciones de partidos».
16. `notes`, nueva: la línea de contratación pública del punto 6.
17. `notes`, nueva: la tensión del punto 7.
18. `notes[2]` («La corporación tiene menos de un año…») → «constituida el 20-08-2025».
19. `sources`:
    - añadir las consultas RUES `?nit=901978854` y `?nit=900988084`, y SECOP I y II por NIT;
    - añadir el Informe Anual, los Estados Financieros 2025 (VF) y el Acta 001;
    - añadir las piezas del 28-02-2026 (`https://elmorichal.com/procuraduria-formulo-pliego-de-cargos-al-exgobernador-de-guainia-juan-carlos-iral-por-puentes-inconclusos/`) y del 20-03-2026 (`https://elmorichal.com/procuraduria-formulo-pliego-de-cargos-contra-exalcalde-de-inirida-pablo-acosta-por-presuntas-irregularidades-en-contratacion/`);
    - **no** añadir la consulta de SECOP por el documento de la persona natural: la URL llevaría la cédula.
20. `ownerType`: **se queda en `'independiente'`**, ahora con fuente registral. `verifiedAt` → `'2026-10-10'` cuando se apliquen las correcciones.

En `shared/mediaRegistry.js`:

21. `biasRationale` → «Corporación sin ánimo de lucro de Puerto Carreño, de seis fundadores, que cubre Vichada y Guainía. Sin editoriales en 12 meses; su Redacción fiscaliza a gobiernos de distinto signo sin postura en el eje. Orientación mixta provisional — ver fichas/el-morichal.md».

En `shared/centinela.js`:

22. Consulta «Corporación El Morichal», `vigila`: sustituir «Es la tercera figura jurídica del medio en nueve años —dos anteriores liquidadas—» por «Es la tercera figura del medio: una S.A.S. (2016, cancelada el 27-07-2026), la persona natural del fundador (matrícula activa) y esta corporación».
23. Consulta «Edwin Suárez», `vigila`: «Que su director y cofundador siga siéndolo» → «Que siga como representante legal de la Corporación y fundador del medio, y cualquier contrato público o candidatura suya».

**(c) Tensiones a declarar**
1. **Transparencia:** los dos pliegos de cargos de 2026 contra jefes de administraciones que contrataron al fundador, sin revelarlo (punto 7).
2. **Rendición de cuentas a medias:** los documentos existen y cuelgan de «Nosotros», pero la página que ve el lector no los enlaza ni muestra el equipo. Es la sección que el propio medio presenta como su garantía de transparencia.
3. **Dos figuras activas:** la Corporación y la persona natural del fundador tienen matrícula activa, y no consta por cuál entran hoy los ingresos (edictos, becas, publicidad).

**¿Aviso de quien dirige?** No procede. No consta candidatura ni cargo público vigente de nadie que dirija el medio. Los contratos del fundador terminaron en 2023.

**Lo que NO entra como hecho:**
- que el contrato de la Gobernación de Vichada de abril de 2023 sea del fundador, o de cualquier otra persona;
- que la omisión en las piezas del 28-02 y del 20-03-2026 incumpla una regla vigente entonces;
- que algún edicto o la invitación de Barrancominas fueran pagados por una entidad local;
- quiénes son las «tres personas» que están a la vez en la Corporación y en el equipo;
- parentesco alguno entre fundadores (dos comparten apellido);
- la nacionalidad, el origen étnico, el lugar de nacimiento y la profesión de los fundadores;
- que Edwin Suárez dirija hoy la redacción.

**Decisiones para el responsable editorial:**
1. **Valor.** Recomendación: **0,00, provisional**, con la razón nueva de (a). No hay nada que contar con la regla de evidencia histórica. Firmable cuando se apliquen las correcciones, si el responsable editorial da por suficiente un nivel 1 documentado con un nivel 2 de 40 días. Si no, sin firmar hasta la re-medición.
2. **Si la ficha nombra a los seis fundadores.** Recomendación: **sí, nombre y papel («fundador/a de la Corporación») con enlace al Informe Anual**, porque es la respuesta de nivel 1 a «a qué persona natural llega». Sin documentos, domicilios ni descriptores. Alternativa más prudente: nombrar solo al representante legal y escribir «seis fundadores con aportes iguales», con el enlace.
3. **La tensión de transparencia (punto 7).** Recomendación: **declararla** en la ficha y en `notes`, con la salvedad de la fecha de la regla. Es el mismo criterio de la tanda 4 (Proclama, Lente Regional): desvelamiento, no acusación.
4. **El registro inconsistente de SECOP.** Recomendación: **no atribuirlo a nadie** y dejarlo escrito como excluido. Si se quiere cerrar, los documentos del proceso `23-12-13582425` (detrás de reCAPTCHA) dirían quién firmó.
5. **`alcanceDe`** (la decisión de producto que la ficha deja abierta): esta revisión no la toca.
