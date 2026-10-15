# Respuesta — Claude Opus 5.5 sobre Volcánicas

| | |
|---|---|
| **Modelo** | Claude Opus 5.5 |
| **Versión exacta** | `claude-opus-5-5` |
| **Fecha de la consulta** | 2026-10-10 |
| **Quién la hizo** | Claude Code, a petición del responsable editorial (ciclo 2, fase 2, tanda 8; revisor de la misma casa que el autor de las fichas, ver DECISIONES.md 2026-10-07) |
| **¿Tuvo acceso a la red?** | sí |

> **Se pega LITERAL lo que devolvió el modelo, sin editar ni resumir.** Si se
> recorta, se pierde justo lo que pueda incomodar. Los comentarios nuestros van
> al final, en la sección de resolución, claramente separados.
>
> **Sin ediciones:** el revisor no copió cédulas, teléfonos ni direcciones, y
> no enlaza ninguna página que muestre un documento de identidad. Se explica al
> principio de la resolución.

---

## RESPUESTA LITERAL

```
REVISIÓN EXTERNA — Volcánicas — ciclo 2 (tanda 8)
Revisor: Claude Opus 5.5 (claude-opus-5-5), Anthropic. Fecha de la revisión: 2026-10-10.

DECLARACIÓN PREVIA DE CONFLICTO
Soy un modelo de Anthropic, de la misma casa que el modelo que escribió la ficha. Comparto con él entrenamiento y probablemente sesgos. Para compensarlo he buscado sobre todo en fuentes que la ficha NO usa: el archivo propio del medio (API pública de WordPress, secciones Editorial y Gobierno y política, piezas firmadas «Volcánicas»), la página /financiamiento/, el RUES y SECOP I/II en datos.gov.co, y las webs de dos de los donantes. No traigo juicio propio sobre dónde va el medio. Mi acuerdo, si lo hay, no debe usarse como aval.

MÉTODO Y DÓNDE BUSQUÉ
- robots.txt de volcanicas.com (consultado el 2026-10-10): «User-agent: * / Disallow:» (vacío). No excluye a ClaudeBot, Claude-Web ni anthropic-ai. Lo mismo en datos.gov.co (solo Crawl-delay y rutas /browse), fordfoundation.org y fjs.org.
- Todas las citas salen del HTML crudo, descargado con curl -sL y UA de navegador (con --ssl-no-revoke) en t89\volcanicas-dl, el 2026-10-10.
- Archivo del medio: API pública https://volcanicas.com/wp-json/wp/v2/posts con after=2025-10-10.
  · Total de piezas en los 12 meses: 267.
  · Categoría «gobierno-politica» (id 22): 126.
  · Categoría «editorial» (id 953): 5 en todo el sitio.
  · Búsquedas internas: «Petro» (37 resultados), «gobierno Petro», «Cepeda», «Pacto Histórico» y «Benedetti» (0).
  · Leí entera cada pieza de Colombia con firma «Volcánicas» (la voz de la casa) y anoté firma, categoría y fecha de cada una.
- Páginas institucionales: /nosotras/ (modificada el 2025-05-15), /nuestra-historia/ (modificada el 2026-03-16) y /financiamiento/ (modificada el 2024-11-23).
- RUES (c82u-588k): consulta upper(razon_social) like '%HOJA BLANCA%', con $select limitado a cámara, razón social, NIT, organización jurídica, estado, fechas de matrícula y renovación, y representante legal.
- SECOP II (jbjy-vk9h, documento_proveedor) y SECOP I (f789-7hwg, identificacion_del_contratista). Igualdad exacta con el NIT sin dígito de verificación (900414071) y con el DV pegado. Probé 9004140711 y 900414071-1, y también el DV calculado con el algoritmo de la DIAN, 5 (9004140715 y 900414071-5). En SECOP II además busqué por nombre del proveedor. Resultado: 0 registros en todas las consultas.
- Donantes:
  · Ford Foundation: su base de subvenciones carga por JavaScript; el HTML crudo (2,7 KB) no trae resultados.
  · fjs.org: la búsqueda «volcanicas» no devuelve resultados.
  · Hispanics in Philanthropy: no consultado.
- Buscador web: usé una sola consulta y no dio nada pertinente; el resto del trabajo se hizo con fuentes primarias. El buscador estaba disponible.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré ningún cambio. Es una ESAL sin propietarios. El RUES devuelve: «FUNDACION HOJA BLANCA-ONG SIGLA HB-ONG», NIT 900414071, Cámara de Comercio de Barranquilla, organización jurídica «FUNDACIONES», estado «ACTIVA», matrícula del 2011-02-15, «ultimo_ano_renovado»: «2024», fecha de renovación 2024-03-28 (consulta del 2026-10-10).
  El único cambio estructural documentado es de financiación: «OSF fue el principal donante de Volcánicas hasta junio de 2025» (/nuestra-historia/). Eso queda unos 16 meses atrás, así que está fuera de la ventana de 12 meses, aunque la página se modificó el 2026-03-16.

- La persona que la ficha nombra como titular o directora, ¿sigue viva y en el cargo?
  Sí, según lo comprobado el 2026-10-10. /nosotras/ dice «Catalina Ruiz Navarro … Directora», y firma una pieza en el propio medio el 2026-05-27 (https://volcanicas.com/que-es-el-centro-politico/). La gerencia administrativa y financiera, Martha Beatriz Navarro, figura además en el RUES como representante legal de la fundación. No afirmo ningún parentesco entre las personas citadas.

- ¿Quién dirige hoy la redacción?
  Ita María, «Editora General», según /nosotras/ (2026-10-10). La ficha no la nombra (ver objeción 5).

- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que la ficha cita?
  La ficha no cita ningún registro: solo dos páginas del propio medio. El RUES es un registro externo que la ficha no tiene. Ojo: su último año renovado es 2024, y no consta renovación para 2025 ni 2026 en el conjunto de datos. Puede ser un rezago del conjunto o una falta de renovación; no lo pude distinguir.

## OBJECIONES

OBJECIÓN 1 — La ficha sostiene −0,50 solo con nivel 4, y el protocolo lo prohíbe
- QUÉ afirma la ficha: «El valor se deriva de una declaración vigente de misión, que es evidencia de nivel 4». El «Nivel 1 bis» de financiación no aporta posición en el eje: no dice qué postura izquierda-derecha tienen los donantes, solo que «tienen agenda declarada».
- POR QUÉ: el contexto del proyecto dice literalmente: «Una clasificación no puede apoyarse solo en los niveles 4 y 5». Tal como está escrita, la ficha incumple esa regla. Esto no significa que el número sea falso. Significa que la ficha no tiene hoy la evidencia que lo sostendría. Esa evidencia existe y está en el archivo del medio (objeciones 3 y 4), pero la ficha no la cita.
- FUENTE: el propio envío (CONTEXTO, «Jerarquía de evidencia admisible») y la ficha («ARGUMENTO»), fecha 2026-10-10.
- NIVEL: es una objeción de procedimiento sobre la jerarquía de evidencia.

OBJECIÓN 2 — Lectura selectiva del nivel 4: la ficha omite que el medio se declara «no partidista»
- QUÉ afirma la ficha: cita de /nosotras/ la misión «avanzar los derechos de las mujeres», y nada más.
- POR QUÉ: la misma página dice, en negrita: «Volcánicas es un proyecto de Fundación Hoja Blanca ONG, una organización sin ánimo de lucro y no partidista. No apoya a ningún candidato ni partido político, y no tiene propietarios ni propietarias.» Si la ficha se apoya en la declaración propia, tiene que recoger la declaración completa.
  Las tres frases siguientes de la misma página delimitan la línea en lo temático, no en lo partidista:
  · «Nuestra línea editorial es transincluyente, antirracista, decolonial y a favor de los derechos de las trabajadoras sexuales»
  · «el periodismo que se dice sin posturas o sin apuestas políticas está a la defensa del status quo, que no es más que el patriarcado»
  · «La independencia editorial es un principio innegociable. Las decisiones sobre temas y fuentes son autónomas y no responden a intereses comerciales, políticos o de otra índole.»
- FUENTE: https://volcanicas.com/nosotras/ (HTML descargado el 2026-10-10; article:modified_time 2025-05-15).
- NIVEL: declaración del propio medio, hoy.

OBJECIÓN 3 — El «CONTRA» de la ficha («No está resuelto») se puede resolver con evidencia del presente, y la ficha no la tiene
- QUÉ afirma la ficha: que periodismo feminista no equivale a izquierda y que la cuestión «No está resuelto». Su criterio de refutación 2 es si la cobertura resulta «transversal en lo económico».
- POR QUÉ: la directora y cofundadora se sitúa explícitamente en la izquierda, y también en el eje económico (redistribución y libre mercado), en una pieza firmada en su propio medio en plena campaña:
  · «Se puede asumir una postura de izquierda sin ser partidista […] Y, frente al giro regional (al fondo) a la derecha, también considero importante pararse públicamente a la izquierda para reivindicar los feminismos y la igualdad»
  · «En sus ideales, Uprimny se identifica como de izquierda: cree en la igualdad y en el papel redistributivo del Estado. Estos son, sin duda, los dos pilares de la izquierda, y los de la derecha son la aceptación de las desigualdades como si fueran una jerarquía natural y las políticas favorables al libre mercado»
  · «las políticas económicas del libre mercado no son una fuerza de la naturaleza, sino una postura política»
  · También defiende al candidato de la izquierda frente a la etiqueta de extremo: «Cepeda no está en la "extrema izquierda", pues el Pacto Histórico no ha dado muestras de querer quedarse autoritariamente en el poder…»
  La voz de la casa liga la posición económica a la crítica: en el perfil de la candidata de la derecha escribe que sus propuestas «son afines y útiles a la defensa y el mantenimiento de las estructuras de opresión que se sostienen sobre el libre mercado» (https://volcanicas.com/paloma-valencia-la-candidata-de-derecha/, 2026-03-11, firma «Volcánicas»).
  Hecho: lo anterior no es una cobertura transversal en lo económico. Inferencia: el criterio 2 de refutación no se cumple, y el argumento «es causa sociocultural, por tanto mixta» queda contradicho por la propia directora.
  Matiz importante: es una columna de opinión, aunque la firma quien dirige. Es nivel 4 (declaración) de la persona que controla la línea, no un endoso. Ver objeción 4 sobre el tope.
- FUENTE: https://volcanicas.com/que-es-el-centro-politico/ (datePublished 2026-05-27, dateModified 2026-05-28; firma Catalina Ruiz-Navarro; categorías Gobierno y política y Opinión). HTML descargado el 2026-10-10.
- NIVEL: declaración del propio medio, por boca de su directora, y hecho editorial de los últimos 12 meses.

OBJECIÓN 4 — Hay asimetría sostenida en la voz de la casa a ambos lados del cambio de gobierno (dirección izquierda). Pero con el protocolo vigente, −0,50 supera el tope de ±0,30 salvo que se acepte que hay «nivel 1 con posición conocida»
- QUÉ afirma la ficha: «Nivel 2 — Conducta medida: No hay». Ofrece −0,50 sin barrido editorial.
- BARRIDO (reproducible): API WP, categoría 22, after=2025-10-10, más las búsquedas «Petro», «Cepeda» y «Pacto Histórico». Solo cuento piezas de Colombia con firma «Volcánicas» (no las columnas de terceros), con postura valorativa explícita. Las piezas de fiscalización neutra se listan aparte y no entran en la cuenta.

  ANTES del 07-08-2026 (gobierno Petro y campaña):
  [L1] 2025-10-27 https://volcanicas.com/ivan-cepeda-el-candidato-del-pacto-historico/
       Encuadre favorable: «una candidatura que apuesta por la continuidad del proyecto progresista de Gustavo Petro, con un estilo pragmático y más prudente y conciliador que el del actual presidente».
  [L2] 2025-11-15 https://volcanicas.com/siete-menores-muertos-en-operativo-militar-en-el-guaviare/
       Bombardeo con 7 menores muertos bajo Petro. Titular: «Siete menores muertos en operativo militar». Contrasta con Duque para atenuar: «En esa ocasión, se trató de una ofensiva militar planeada —no una acción defensiva reactiva—». Hay también una línea de fiscalización: «no es negociable bajo ningún gobierno».
  [L3] 2026-03-12 https://volcanicas.com/aida-quilcue-la-formula-vicepresidencial-de-ivan-cepeda/
       Bajada: «la elección de Aida Quilcué como fórmula vicepresidencial de Iván Cepeda ratifica la apuesta social del Pacto Histórico».
  [R1] 2026-03-11 https://volcanicas.com/paloma-valencia-la-candidata-de-derecha/
       «carga una trayectoria marcada por posturas racistas y antifeministas»; «ha dejado claras sus posturas de derechas, antifeministas y antiderechos y su fidelidad al uribismo».
  [R2] 2026-06-03 https://volcanicas.com/abelardo-de-la-espriella-para-dummies/
       «promete destripar a la izquierda y dice representar a "los nunca", pero hizo su carrera con los de siempre, entre escándalos de corrupción, parapolítica y otros delitos».
  [R3] 2026-07-06 https://volcanicas.com/el-gabinete-de-abelardo-de-la-espriella-los-nunca/
       «Entre los nombramientos más problemáticos están Viviane Morales, la exfiscal fundamentalista…».

  DESPUÉS del 07-08-2026 (gobierno De la Espriella):
  [R4] 2026-08-17 https://volcanicas.com/abelardo-de-la-espriella-debuta-como-presidente-e-improvisa-en-la-emergencia-por-el-terremoto/
       «deja, más que una sucesión de desaciertos, dudas sobre la capacidad del nuevo Gobierno».
  [R5] 2026-08-19 https://volcanicas.com/la-nueva-directora-del-icbf-pide-dejar-de-nombrar-a-las-ninas-y-estigmatiza-al-colectivo-infantil-resistencia-chiquita/
       El titular afirma que «estigmatiza».
  [R6] 2026-08-31 https://volcanicas.com/abelardo-de-la-espriella-respalda-bombardeo-que-deja-tres-menores-muertos-en-guaviare-otro-menor-de-edad-murio-en-el-bombardeo-del-10-de-agosto/
       Titular: «4 menores asesinados en los primeros 2 bombardeos del gobierno De la Espriella»; cuerpo: «Tres menores de edad fueron asesinados». En la misma pieza, para el gobierno anterior: «durante el gobierno de Gustavo Petro han muerto entre 62 y 68 menores de edad». Es el mismo tipo de hecho con distinto verbo según el gobierno: «asesinados» frente a «muertos/han muerto» (comparar con L2). Esto no es fiscalización simétrica: es encuadre asimétrico.
  [R7] 2026-09-01 https://volcanicas.com/censura-a-la-prensa-en-gobierno-de-abelardo-de-la-espriella-erosiona-la-democracia/
       Titular valorativo: «erosiona la democracia».
  [R8] 2026-09-03 https://volcanicas.com/sale-viviane-morales-y-entra-ilva-myriam-hoyos-la-exprocuradora-anti-derechos-ahora-sera-ministra-de-educacion/
       «La exprocuradora anti-derechos».
  [R9] 2026-09-07 https://volcanicas.com/primer-mes-de-gestion-de-abelardo-de-la-espriella/
       «la imagen de un presidente que se pasea entre cadáveres para mostrar resultados».

  Fiscalización o información sin postura valorativa, no contada:
  · 2026-02-12 Córdoba / emergencia (Petro): neutral, cita a Petro de forma favorable sobre Urrá.
  · 2026-06-18 Arturo Calle (constreñimiento al sufragante).
  · 2026-08-07 obispo de la posesión.
  · 2026-08-29 SALVIA.
  · 2026-08-29 tutelas al Consejo de Estado.
  · 2026-08-20 elogio a la gobernadora del Chocó: no verifiqué su filiación, así que no lo asigno a ningún lado.

  CUENTA: 12 piezas con postura.
  · 3 indulgentes o favorables a la izquierda (L1–L3) y 9 hostiles a la derecha (R1–R9). Todas apuntan en la misma dirección.
  · 6 antes y 6 después del cambio de gobierno.
  · Razón 12:0 en dirección; incluso si L2 se recalifica como fiscalización de Petro, queda 11:1.
  · Piezas de la casa que fiscalicen con dureza al gobierno saliente en 10 meses de mandato: la única es L2, y viene atenuada.
  · Para el entrante, en 2 meses: R4–R9 y además las 3 de fiscalización neutra.
  Según la REGLA DEL POLO FIJO, esto no es el patrón «fiscalizaba al saliente y sigue con el entrante». Es una casa que no fiscalizó al saliente y fiscaliza con encuadre valorativo al entrante.
  Se cumplen los umbrales: ≥10 piezas, ≥3 por lado y ≥3:1.

- POR QUÉ ES OBJECIÓN: esta evidencia apoya la dirección (izquierda) que propone la ficha. La ficha no la tiene. Además, la regla dice: «Mueve como mucho hasta ±0,30» y «Tope ±0,30 sin endoso ni nivel 1 con posición conocida».
  · Endoso: no encontré ninguno (ver más abajo), y el medio declara que no apoya candidatos.
  · Nivel 1 con posición conocida: la ficha no lo documenta.
  Por tanto, con las reglas tal como están escritas, −0,50 excede el tope, salvo que la persona que firma decida que la posición de izquierda declarada públicamente por la directora y cofundadora de una ESAL sin propietarios (objeción 3) equivale a «nivel 1 con posición conocida». Es una decisión de protocolo que no me corresponde. Lo que sí afirmo es que la ficha tiene que declarar esta tensión de forma explícita.
- FUENTE: las URL listadas, todas descargadas en HTML crudo el 2026-10-10, con las fechas de publicación indicadas; y la API https://volcanicas.com/wp-json/wp/v2/posts?categories=22&after=2025-10-10T00:00:00 (X-WP-Total: 126).
- NIVEL: hecho editorial de los últimos 12 meses (voz de la casa, barrido sistemático).

OBJECIÓN 5 — La tabla «Personas con dirección hoy» omite a quien dirige la redacción e incluye a una cofundadora sin papel actual visible
- QUÉ afirma la ficha: lista a Ruiz-Navarro, Londoño Jaramillo, Navarro y Henao como personas con dirección.
- POR QUÉ:
  · /nosotras/ lista en «Equipa» a «Ita María … Editora General». La ficha no la nombra, y es la respuesta a «¿quién dirige hoy la redacción?».
  · Matilde de los Milagros Londoño Jaramillo aparece solo bajo «Fundadoras», no en «Equipa». En la API, su único rastro en 12 meses es la mención en una pieza del 2026-01-20 sobre el documental «Silenced».
  · Inferencia (no hecho): no consta que tenga hoy funciones de dirección.
  · La ficha también omite el «Consejo Consultivo» de 5 personas, descrito como «órgano de veeduría externo».
- FUENTE: https://volcanicas.com/nosotras/ (2026-10-10); API https://volcanicas.com/wp-json/wp/v2/posts?search=Matilde+de+los+Milagros&after=2025-10-10T00:00:00 (2026-10-10).
- NIVEL: propiedad / control (quién dirige).

OBJECIÓN 6 — La composición de la financiación: «Patreon … resto» es una inferencia de la ficha, y la propia web se contradice
- QUÉ afirma la ficha: «aportes individuales (Patreon) ..... resto».
- POR QUÉ:
  · La fuente dice: «Actualmente, Volcánicas es financiada en un 40.82% por Hispanics in Philanthropy (HIP), 24.49% por Ford Foundation y 16.33% por Foundation for a Just Society (FJS). Además, recibimos aportes individuales y voluntarios de personas que apoyan nuestro trabajo a través de Patreon.» No atribuye a Patreon el 18,36 % restante.
  · Inferencia: las tres cifras son 20/49, 12/49 y 8/49, lo que deja 9/49 sin atribuir. Puede ser otro donante, servicios u otra cosa.
  · La página /financiamiento/ sigue diciendo «Gracias a un grant de Open Society Foundations» y «99% de fondos de cooperación internacional». Anuncia enlaces al «Balance General y Estado de Resultados» y al «Certificado de Representación y Existencia», pero el HTML no contiene esos enlaces.
  · /nosotras/ menciona una «rendición de cuentas anual» sin enlace.
  · Hecho: la composición es declarada, no auditada. Mientras no aparezcan los estados financieros que la propia página promete, la ficha no debería calificarla de «financiación declarada con porcentajes» sin esta salvedad.
- FUENTE: https://volcanicas.com/nuestra-historia/ (modificada el 2026-03-16) y https://volcanicas.com/financiamiento/ (modificada el 2024-11-23). Ambas descargadas el 2026-10-10.
- NIVEL: declaración del propio medio / propiedad económica.

OBJECIÓN 7 — El criterio de refutación 1 usa la compañía media, que el propio proyecto declara inválida para mover un valor
- QUÉ afirma la ficha: «si su compañía media en historias multifuente no queda por debajo de 0,00, la clasificación de izquierda no se sostiene».
- POR QUÉ: la advertencia de la conducta medida dice: «Usar la compañía media para mover un valor de sesgo es un error, y si esta ficha lo hace, es una objeción válida contra ella».
  · La medición de hoy da compañía 0,087 con solo 11 piezas en alguna historia. Con el criterio de la ficha, la clasificación ya «no se sostendría», por un artefacto de saturación.
  · Además, «Nivel 2 — No hay» ya no es cierto: hay 34 artículos y 12 historias en 40 días, aunque son insuficientes.
  · Hay que sustituir el criterio 1 por el barrido de voz de la casa de la objeción 4.
- FUENTE: el propio envío, sección «Conducta medida» (medición del 2026-10-10).
- NIVEL: conducta medida.

## LO QUE NO PUDE VERIFICAR
- Las subvenciones de HIP, Ford y FJS a Fundación Hoja Blanca.
  · Base de Ford: carga por JavaScript, sin resultados en el HTML crudo.
  · fjs.org/?s=volcanicas: sin resultados.
  · HIP: no consultado.
  · Buscador web: una consulta, nada pertinente.
  No las puedo confirmar ni refutar por terceros.
- Si la fundación renovó la matrícula en 2025 y 2026: el RUES (c82u-588k) marca 2024 como último año renovado. No sé si es un rezago del conjunto de datos.
- Los estados financieros y la «rendición de cuentas anual»: anunciados, sin enlace en el HTML.
- La filiación de la gobernadora del Chocó elogiada el 2026-08-20. No la busqué, así que esa pieza queda fuera de la cuenta.
- Contratación pública: 0 registros en SECOP I y II por NIT (con y sin DV, incluido el DV 5 calculado) y por nombre en SECOP II. Es una ausencia verificada en esos conjuntos de datos, no una prueba de que no exista financiación estatal por otras vías.

## LO QUE FALTA
- El registro RUES (NIT 900414071, Cámara de Comercio de Barranquilla, ACTIVA, representante legal la gerente administrativa) como fuente de nivel 1 en lugar de las páginas del propio medio.
- La declaración «no partidista / no apoya a ningún candidato» (objeción 2).
- La columna de la directora del 2026-05-27 (objeción 3).
- El barrido de voz de la casa con las 12 piezas (objeción 4) y la decisión explícita sobre el tope de ±0,30.
- La Editora General (objeción 5) y el Consejo Consultivo.
- La salvedad de que la composición de ingresos es declarada, no auditada, con un 18 % sin atribuir (objeción 6).

## EVIDENCIA QUE NO MUEVE EL NÚMERO
- No hay endoso. En las 37 piezas que mencionan a Petro, las 126 de Gobierno y política y las 5 de la sección Editorial (12 meses) no encontré ninguna pieza de la casa que pida el voto por un candidato. El medio declara: «No apoya a ningún candidato ni partido político» (/nosotras/, 2026-10-10).
  La carta de 2026-06-10 (https://volcanicas.com/queridas-amistades-de-colombia-panas-parces-hermanas-socias/) advierte sobre la experiencia argentina «dos semanas antes de sus elecciones», pero es de una firmante externa, no de la casa, y no nombra candidato en el texto que extraje.
- La sección Editorial (id 953) tiene 5 piezas en todo el sitio, de 2025-10-07 a 2025-11-08. Tratan sobre Israel y Gaza, Bullrich y una sentencia contra un exabogado de Uribe con eje en el «enfoque de género». Ninguna trata del gobierno Petro.
- Hay contrapesos dentro de la voz de la casa:
  · R6 da cifras del gobierno Petro («entre 62 y 68 menores») y de Duque.
  · L2 cierra con «no es negociable bajo ningún gobierno».
  · La casa critica a gobiernos de izquierda fuera de Colombia: «sentenció el dictador» (Ortega; https://volcanicas.com/daniel-ortega-entierra-las-elecciones-en-nicaragua-y-consolida-la-dictadura-familiar/, 2026-07-20, firma «Volcánicas»). La crítica a Sheinbaum del 8M (2026-03-09) la firma una autora, no la casa.
  · En la columna de la directora: «Desde la izquierda se le puede exigir a la misma izquierda, tener valores feministas, garantizar los derechos humanos, no ser corrupta y no ser autoritaria».
- La fundación no tiene contratos públicos en SECOP I ni II por NIT (2026-10-10).
- La directora sigue en el cargo y firmó en el medio el 2026-05-27. La redacción la dirige la Editora General según /nosotras/. No encontré cambio de control en 12 meses.

## SIN OBJECIÓN
No aplica: hay 7 objeciones.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** El revisor no copió cédulas, teléfonos ni direcciones, y no enlaza consultas de datos.gov.co ni constancias de SECOP: describe sus consultas sin URL. Nombra a la gerente administrativa como representante legal en el RUES, y eso es nombre y papel, que la regla permite. **Esta resolución tampoco escribe ni enlaza ningún documento:** las consultas que cita llevan `$select` con solo los campos de la fundación (comprobado: no devuelven `num_identificacion` ni otro dato de una persona natural). Tampoco copia la nacionalidad, el lugar de nacimiento ni la orientación que traen algunas biografías de /nosotras/.

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada (2026-10-10):
  - volcanicas.com: bloque de Yoast, `User-agent: *` con `Disallow:` vacío. **Literal, como dice el revisor.**
  - datos.gov.co: `Crawl-delay: 1` y exclusiones de `/browse`; se usó solo `/resource`, con un segundo entre consultas.
  - No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. **No hubo buscador web**, ni consulta a las webs de los donantes.
- **Sitio**, en crudo con `curl -sL --ssl-no-revoke -A "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/126.0 Safari/537.36"`:
  - /nosotras/, /nuestra-historia/ y /financiamiento/, y sus fechas por la API (`/wp-json/wp/v2/pages?slug=…`);
  - **las 267 piezas de la ventana, una por una**, por la API de WordPress (`posts?after=2025-10-10T00:00:00`), con la **firma visible** de cada una (`<meta name="author">`; el autor de WordPress no es la firma) y su texto completo;
  - recuentos de la API: categoría 22, categoría 953, y búsquedas «Petro», «gobierno Petro», «Cepeda», «Pacto Histórico», «Benedetti» y «Matilde de los Milagros».
- **Registros**, en datos.gov.co:
  - RUES (`c82u-588k`): `nit=900414071` y `upper(razon_social) like '%HOJA BLANCA%'`.
  - SECOP II (`jbjy-vk9h`): `documento_proveedor` = `900414071`, `9004140715` y `900414071-5` (igualdad exacta), y `upper(proveedor_adjudicado) like '%HOJA BLANCA%'`.
  - SECOP I (`f789-7hwg`): `identificacion_del_contratista` = `900414071`, `9004140715` y `900414071-5`, y `upper(nom_razon_social_contratista) like '%HOJA BLANCA%'`.
- **Repositorio:** el envío, `fichas/volcanicas.md`, las entradas de Volcánicas en `shared/mediaRegistry.js`, `shared/mediaOwnership.js` y `shared/centinela.js`, sus menciones en otras fichas (`casa-macondo.md`, `voragine.md`, `colombia-informa.md`, `las2orillas.md`), el commit del alta (`f237d52`, 2026-08-08), el protocolo, DECISIONES.md (2026-10-07 a 2026-10-10) y los barridos existentes.
- **El barrido**, reproducible, está en `revision-externa/barridos/volcanicas.md`.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | La ficha se apoya solo en nivel 4, y el §2 lo prohíbe | sí | sí | **Aceptada.** Literal en el protocolo y en el envío. **Y algo que el revisor no dice:** los tres vecinos con los que la ficha razona su −0,50 (Vorágine, RAYA, Cuestión Pública) están **sin medir** desde el 2026-09-18, por la misma razón: la materia declarada no sitúa la línea |
| 2 | Omite que la fundación se declara «no partidista» | sí | sí | **Aceptada.** Literal y en negrita (`<strong>`) en /nosotras/. Las otras tres citas, también literales. **Además, la cita de misión de la ficha no es literal:** ver «Errores de la ficha» |
| 3 | La directora se sitúa a la izquierda, también en lo económico (columna del 27-05-2026) | sí | sí | **Aceptada en los hechos.** Las cinco citas son literales. **Matiz:** la columna la firma la directora, así que cuenta como voz de la casa dentro del barrido (lo «firmado por […] su director»), no como nivel 1 |
| 4 | Asimetría sostenida en la voz de la casa (12:0, 6 y 6); −0,50 supera el tope | sí | sí, pieza por pieza | **Aceptada en la dirección y en el tope; el recuento no se sostiene.** De sus 12 piezas, 8 suman y 4 no (L2 es fiscalización de Petro y cuenta como contrapeso; R6, R7 y R9 son fiscalización del gobierno de turno). Su «6 después» se queda en 1 clara y 2 leves. Leyendo las 267: **17 piezas (12 antes, 5 después) frente a 3 contrapesos en la lectura amplia; 8 (6 y 2) en la estricta**, que no llega. Sin endoso. La posición de la directora **no** es «nivel 1 con posición conocida» (ver punto 4) |
| 5 | Falta la Editora General y el Consejo Consultivo; Londoño Jaramillo sin papel actual | sí | sí | **Aceptada.** Literal en /nosotras/. La API devuelve una sola mención de Londoño Jaramillo en 12 meses (2026-01-20) |
| 6 | «Patreon … resto» es inferencia; 18 % sin atribuir; /financiamiento/ desactualizada | sí | sí | **Aceptada, con una corrección y un dato a favor.** /financiamiento/ no es de 2024-11-23: la API da `modified` **2021-03-03**. Y la página dice «1% de microfinanciamiento a través de Paetreon», lo que contradice aún más el «resto». Los dos «aquí» no tienen enlace: son texto en negrita |
| 7 | El criterio de refutación 1 usa la compañía media, que el envío declara inválida | sí | sí | **Aceptada.** Advertencia literal en el envío; cifras exactas (34 artículos, 11 en historias, 12 historias, compañía 0,087) |

### Lo verificado, objeción por objeción

**Nivel 1 — qué cambió este año.**
- **RUES** (`c82u-588k`, `nit=900414071`, 2026-10-10), una fila, literal: «"razon_social":"FUNDACION HOJA BLANCA-ONG SIGLA HB-ONG"», «"sigla":"HB-ONG"», «"nit":"900414071"», «"digito_verificacion":"5"», «"camara_comercio":"BARRANQUILLA"», «"organizacion_juridica":"FUNDACIONES"», «"estado_matricula":"ACTIVA"», «"fecha_matricula":"20110215"», «"fecha_renovacion":"20240328"», «"ultimo_ano_renovado":"2024"», «"representante_legal":"Navarro Restrepo Martha Beatriz"», «"fecha_actualizacion":"2024/03/28 …"», «"cod_ciiu_act_econ_pri":"1812"» (actividades de servicios relacionados con la impresión). **Todo lo que cita el revisor es exacto.** Él no da el CIIU; el dígito de verificación lo confirma el propio registro (5), y su prueba con «1» sobra. Consulta sin datos personales: `https://www.datos.gov.co/resource/c82u-588k.json?nit=900414071&$select=razon_social,sigla,nit,digito_verificacion,camara_comercio,organizacion_juridica,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,representante_legal,fecha_actualizacion,cod_ciiu_act_econ_pri`.
- **Renovación:** el último año renovado es 2024. Como dice el revisor, no se puede distinguir aquí entre rezago del conjunto y falta de renovación. Queda como laguna, sin afirmar nada.
- **SECOP**, 2026-10-10: **0 filas** en SECOP II con `900414071`, `9004140715`, `900414071-5` y por razón social `like '%HOJA BLANCA%'`; **0 filas** en SECOP I con los tres NIT y por razón social. Consultas: `https://www.datos.gov.co/resource/jbjy-vk9h.json?documento_proveedor=900414071&$select=count(*)` y `https://www.datos.gov.co/resource/f789-7hwg.json?identificacion_del_contratista=900414071&$select=count(*)` (y lo mismo con `9004140715` y `900414071-5`). **Exacto.**
- **Cambio de control en 12 meses:** no consta. La salida de OSF como principal donante es de «junio de 2025» (/nuestra-historia/, `modified` 2026-03-16), fuera de la ventana. **Exacto.**
- **Directora:** «Catalina Ruiz Navarro … Directora» en /nosotras/ (`modified` 2025-05-15), y firma en el medio el 27-05-2026 y el 26-08-2026. Sigue en el cargo.

**1 · Solo nivel 4.**
- §2 del protocolo, literal: «**Una ficha no puede apoyarse solo en niveles 4 y 5.**». El envío lo repite: «Una clasificación no puede apoyarse solo en los niveles 4 y 5».
- La ficha, literal: «El valor se deriva de **una declaración vigente de misión**, que es evidencia de nivel 4». El «Nivel 1 bis» de financiación no sitúa el medio en el eje: dice quién paga, no hacia dónde.
- **Cómo se llegó a −0,50** (commit `f237d52`, 2026-08-08, «Alta de CasaMacondo y Volcanicas»): «su valor se justifica solo con evidencia del presente: lo que cada uno declara HOY como mision». El número se fijó por vecindad: «en el mismo rango que otros medios de causa e investigación del catálogo (Vorágine −0,50, Revista RAYA −0,55, Cuestión Pública −0,45)».
- **Esos tres vecinos ya no tienen número.** `shared/mediaRegistry.js`: «SIN MEDIR — decisión del responsable editorial del 2026-09-16, aplicada el 2026-09-18». En `fichas/voragine.md`: «El −0,50 no viene de ninguna medición […]: es una colocación entre RAYA y Cuestión Pública». La ficha de Volcánicas sigue razonando contra ellos.

**2 · «No partidista».**
- /nosotras/ (2026-10-10), dentro de `<strong>`: «Volcánicas es un proyecto de Fundación Hoja Blanca ONG, una organización sin ánimo de lucro y no partidista. No apoya a ningún candidato ni partido político, y no tiene propietarios ni propietarias.» **Literal.**
- También literales: «Nuestra línea editorial es transincluyente, antirracista, decolonial y a favor de los derechos de las trabajadoras sexuales»; «el periodismo que se dice sin posturas o sin apuestas políticas está a la defensa del status quo, que no es más que el patriarcado»; «La independencia editorial es un principio innegociable. Las decisiones sobre temas y fuentes son autónomas y no responden a intereses comerciales, políticos o de otra índole.»
- **Y la conducta lo confirma en parte:** en las 267 piezas no hay ninguna petición de voto de la casa ni de la directora (barrido, §4).

**3 · La columna de la directora** (https://volcanicas.com/que-es-el-centro-politico/, `meta author` «Catalina Ruiz-Navarro», publicada el 2026-05-27).
- Las cinco citas del revisor son literales, entre ellas «Se puede asumir una postura de izquierda sin ser partidista», «también considero importante pararse públicamente a la izquierda» y «las políticas económicas del libre mercado no son una fuerza de la naturaleza, sino una postura política».
- Además: «la nueva derecha fascista encarnada en Abelardo de la Espriella» y «nada del gobierno de Petro ha mostrado que esté yendo contra la empresa privada», con una defensa del balance económico del gobierno.
- Y la cita del perfil de Valencia (11-03-2026, firma «Volcánicas»), «son afines y útiles a la defensa y el mantenimiento de las estructuras de opresión que se sostienen sobre el libre mercado», es literal.
- **El criterio 2 de refutación de la ficha** («si critica por igual políticas económicas de gobiernos de izquierda y derecha») **no se cumple:** en 12 meses no hay una pieza de la casa que critique la política económica del Gobierno Petro. La lectura «causa sociocultural, por tanto mixta» del CONTRA queda contradicha en voz de la casa.
- **Dónde va en el protocolo:** es una pieza «firmada por […] su director», así que entra en el barrido como voz de la casa (precedente: `barridos/archipielago-press.md`, §1.5). No es nivel 1 (ver punto 4).

**4 · El barrido** (completo en `revision-externa/barridos/volcanicas.md`).
- **Universo:** 267 piezas (`X-WP-Total: 267`), **196 con firma «Volcánicas»**, 4 de la directora, 4 de la editora general y 62 de terceras. Categoría 22: 126; categoría 953 (Editorial): 5 en todo el sitio, 4 en la ventana, ninguna sobre el gobierno ni los candidatos. Búsqueda «Petro»: 37. **Exacto.** Las otras búsquedas que el revisor agrupa con «(0)» no dan 0: «Cepeda» 14, «Pacto Histórico» 14, «gobierno Petro» 34; solo «Benedetti» da 0. Su frase es ambigua.
- **Las 12 del revisor:** todas existen, con su fecha, y sus citas son literales (la de R2 está en el resumen destacado de la página, no en el cuerpo). La clasificación es otra cosa:
  - **L2 (Guaviare, 15-11-2025) no es «indulgente»:** fiscaliza a Petro mientras gobierna («Este nuevo caso, ahora bajo un mandato progresista, revive la deuda»; «no es negociable bajo ningún gobierno») y recoge las críticas y la moción de censura. El atenuante (la comparación con 2019) existe. Es **contrapeso parcial**, no pieza a la izquierda.
  - **R6 (bombardeos, 31-08-2026):** la asimetría del verbo es literal («Tres menores de edad fueron asesinados» con De la Espriella; «durante el gobierno de Gustavo Petro han muerto entre 62 y 68 menores»), pero la misma pieza llama «asesinadas» a las víctimas de Duque y dedica una sección entera a los bombardeos de Petro, con su frase en X y su petición de perdón. **Es fiscalización de tres gobiernos, con una asimetría léxica dentro.** Respuesta a la pregunta del encargo: el revisor la cuenta como postura por el verbo; el resto de la pieza no lo sostiene. No suma.
  - **R7 (censura) y R9 (primer mes):** fiscalización del gobierno de turno. No suman (precisión del 2026-10-09).
  - **R4 (debut) y R5 (ICBF):** sobre todo fiscalización, pero cada una lleva una frase que sí es postura (el elogio a Petro por transmitir el empalme; la «batalla cultural» como programa para «retroceder en materia de derechos»). Suman como **leves**.
- **El recuento, leyendo las 267:**

| | Suman (I + leves) | Contrapesos | F, solo fiscaliza (no suma) |
|---|---|---|---|
| Antes del 07-08-2026 | **12** (6 + 6) | 3 parciales | — |
| Desde el 07-08-2026 | **5** (2 + 3) | 0 | 5 |
| **Total** | **17** (8 + 9) | **3** | 5 |

- **Mínimos de la regla:**
  - **Lectura amplia** (como El Informador): ≥10 → 17; ≥3 a cada lado → 12 y 5; ≥3:1 → 17:3 = 5,7:1. **Cumple.**
  - **Lectura estricta** (como Abra Noticias, sin dudosas): 8; 6 y 2; 8:3 = 2,7:1. **No cumple ninguno de los tres mínimos.**
  - Las 6 leves de antes son rótulos claros en voz propia («ultraderechista», «extrema derecha»): leves en el sentido de El Informador. **Las 3 de después se parecen a las dudosas de Abra:** dos van dentro de piezas que sobre todo fiscalizan. **El después es lo que está en el límite.**
- **Lo que el revisor no tiene:**
  - las 2 piezas de la directora (27-05 y 26-08: «un gobierno neofascista como el de Abelardo»);
  - la marcha del orgullo (16-07), las 5 leves de antes (Hay Festival, fórmulas, Mateo Pérez, Pasto, Andino) y los incendios (14-08);
  - los 3 contrapesos (L2 y las dos piezas sobre Hollman Morris, gerente de RTVC con Petro, 24-03 y 22-04-2026);
  - **el encuadre asimétrico entre candidatos** como tal: perfiles laudatorios de Cepeda (27-10-2025) y Quilcué (12-03-2026), y de escándalos de Valencia (11-03-2026) y De la Espriella (03-06-2026). La regla del polo fijo lo trata como evidencia de primer orden: «Lo mismo vale para el encuadre asimétrico entre candidatos».
- **La intensidad de la fiscalización** se declara como tensión, sin sumar: 1 pieza sobre la política de Petro y 2 sobre un funcionario suyo en 10 meses; 7 sobre el Gobierno De la Espriella en 2.
- **Endoso:** ninguno. Se buscaron peticiones de voto en las 267; el único resultado es una cita ajena. La casa no publicó nada en voz propia sobre el resultado de ninguna de las dos vueltas.
- **¿Es la posición de la directora «nivel 1 con posición conocida»?** Respuesta a la pregunta del encargo, con los textos:
  - §2, tabla: «| 1 | **Propiedad documentada** | Quién controla la empresa, con fuente citable y persona natural | `shared/mediaOwnership.js` |».
  - §1, «Cuánto mueve»: «Sin propiedad documentada con posición conocida (nivel 1) ni endoso explícito, **la magnitud no pasa de ±0,30**».
  - §5, regla 3: «mueve como mucho hasta ±0,30, **salvo endoso explícito o nivel 1 con posición conocida**».
  - §1, regla de quien dirige: «Qué NO lo dispara. Afinidad, militancia pasada, opinión publicada […]: lo del dueño ya tiene su instrumento en la ficha de propiedad, y lo demás es orientación —y la orientación se mide con corpus, no con biografía—».

  **No lo es, por cuatro razones:**
  1. El nivel 1 es «propiedad documentada», «quién controla la empresa». De la directora es nivel 1 **el cargo**. **La posición sale de una columna**, que es voz de la casa (cuenta en el barrido) o declaración (nivel 4). Contarla también como nivel 1 sería contar dos veces la misma pieza.
  2. Los precedentes son estructurales. Semanario VOZ: «control orgánico del PCC sobre la Fundación Semanario VOZ» (DECISIONES, 2026-10-07). El Nuevo Siglo: si «existe un vínculo orgánico con el Partido Conservador» (2026-09-22). Semana: el dinero del dueño y su familia en la recolección de firmas de una candidata (2026-09-22). En los tres, el dueño o controlador es o financia a un actor político, y eso consta en un registro o un documento. **Ningún precedente usa la opinión de un director.** La Libertad (directora que anunció candidatura) se trató con el aviso de quien dirige, no como nivel 1.
  3. La regla de quien dirige excluye la «opinión publicada» de quien dirige y la manda al corpus.
  4. La fundación que controla el medio se declara «no partidista» y sin propietarios.

  **Con lo que hay, el tope de ±0,30 rige.** El revisor lo dice bien: es una decisión de protocolo, y es del responsable editorial. Ver «Decisiones».
- **Su cita de la regla** «Tope ±0,30 sin endoso ni nivel 1 con posición conocida» no está en el envío, que solo dice «Mueve como mucho hasta ±0,30». El contenido coincide con el §1 y con el §5 corregido del protocolo, así que no cambia nada; pero no es literal del envío.

**5 · Quién dirige.**
- /nosotras/ (2026-10-10), «Equipa»: «Catalina Ruiz Navarro … Directora», «Martha Beatriz Navarro … Gerente administrativa y financiera», «Paula Henao Aristizábal … Coordinadora general», una asistente administrativa e «Ita María … Editora General». **Literal.**
- «Fundadoras»: «Catalina Ruiz-Navarro, Directora» y «Matilde de los Milagros Londoño Jaramillo». Londoño Jaramillo no está en «Equipa», y /nuestra-historia/ la describe como «quien fue la editora general de Volcánica en esa etapa previa».
- La API, `search=Matilde de los Milagros&after=2025-10-10`: un resultado, el 2026-01-20 (el documental «Silenced»). **Exacto.**
- «Consejo Consultivo»: «órgano de veeduría externo al funcionamiento cotidiano de la revista y está conformado por 5 personas que no son empleadas de Volcánicas ni hacen parte de la Fundación Hoja Blanca ONG». **Literal.**

**6 · Financiación.**
- /nuestra-historia/ (`modified` 2026-03-16), literal: «Actualmente, Volcánicas es financiada en un 40.82% por Hispanics in Philanthropy (HIP), 24.49% por Ford Foundation y 16.33% por Foundation for a Just Society (FJS). Además, recibimos aportes individuales y voluntarios de personas que apoyan nuestro trabajo a través de Patreon.» Suman 81,63 %: queda un **18,37 % sin atribuir**. Las fracciones 20/49, 12/49 y 8/49 son exactas, como dice el revisor (inferencia suya, aritmética correcta).
- /financiamiento/: la API da `modified` **2021-03-03**, no 2024-11-23 (esa fecha no aparece en el HTML). Literal: «Gracias a un grant de Open Society Foundations», «99% de fondos de cooperación internacional» y «**1% de microfinanciamiento a través de Paetreon**, patrocinadores para proyectos puntuales […]». Es una página de 2021: describe la etapa de OSF, y su 1 % para Patreon hace todavía menos verosímil que Patreon sea «el resto».
- Los enlaces anunciados («Balance General y Estado de Resultados», «Certificado de Representación y Existencia») son «aquí.» en `<b>`, **sin `href`**. /nosotras/ cita la «rendición de cuentas anual» sin enlace. **Exacto.**

**7 · Compañía media.** El envío, literal: «**Usar la compañía media para mover un valor de sesgo es un error**, y si esta ficha lo hace, es una objeción válida contra ella». La tabla: 34 artículos, 11 en alguna historia, 12 historias, compañía 0.087. **Exacto.** Y el criterio 1 de la ficha («si su compañía media […] no queda por debajo de 0,00, la clasificación de izquierda no se sostiene») quedaría hoy cumplido por un artefacto.

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se corrigen estas partes:
- **Obj. 4, recuento:** 12 piezas (6 y 6), 12:0 → **17 en la lectura amplia (12 y 5) frente a 3 contrapesos, y 8 en la estricta (6 y 2)**. L2 es contrapeso; R6, R7 y R9 son fiscalización del gobierno de turno; R4 y R5 son leves. El revisor no leyó lo firmado por la directora como voz de la casa ni el encuadre entre candidatos como tal.
- **Obj. 4, «Esto no es fiscalización simétrica: es encuadre asimétrico»** (R6): la asimetría del verbo es real, pero la pieza fiscaliza a Petro, Duque y De la Espriella. No suma.
- **Obj. 4, «Se cumplen los umbrales»:** solo en la lectura amplia, y el después descansa en 2 piezas claras.
- **Obj. 6, fecha de /financiamiento/:** 2021-03-03, no 2024-11-23.
- **MÉTODO, búsquedas con «(0)»:** «Cepeda», «Pacto Histórico» y «gobierno Petro» dan 14, 14 y 34.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente ni cita inventada en el material del medio.** Las 12 URL resuelven y sus citas son literales; las de /nosotras/, /nuestra-historia/ y /financiamiento/ también. RUES y SECOP coinciden con lo que él consultó. Lo que hay:
- una cita de la regla («Tope ±0,30 sin endoso ni nivel 1 con posición conocida») que no está en el envío, aunque su contenido es el del protocolo;
- una fecha de modificación de /financiamiento/ que no se encuentra (2024-11-23; la API da 2021-03-03);
- un recuento que cuenta fiscalización como postura (L2, R6, R7, R9) y deja fuera lo de la directora y 7 piezas más;
- la omisión de los 3 contrapesos al hablar de «12:0».

**Errores de la propia ficha, para no repetirlos:**
- **La cita de misión no es literal.** La ficha pone entre comillas «las herramientas del periodismo para avanzar los derechos de las mujeres y defender los derechos humanos». Esa frase no está en /nosotras/, /nuestra-historia/ ni /financiamiento/ (y /nosotras/ no ha cambiado desde el 2025-05-15, antes del alta). Lo literal es: «Usamos las múltiples herramientas de la comunicación para ayudar a deconstruir el machismo, y así avanzar en la consecución de los derechos de las mujeres y la comunidad lgbti en Latinoamérica y el Caribe. Defendemos los derechos humanos a través de la creación de un espacio seguro para las historias de mujeres en toda su diversidad». La misma paráfrasis entrecomillada está en el `biasRationale` de `mediaRegistry.js`. El revisor no lo vio.
- **Razona contra tres vecinos que ya no tienen número** (Vorágine, RAYA y Cuestión Pública, sin medir desde el 2026-09-18).
- **Omite «no partidista»** y la ausencia de endoso, que es evidencia que no mueve el número pero se escribe.
- **«aportes individuales (Patreon) ..... resto»:** inferencia, contradicha por la propia /financiamiento/ (1 % en 2021). Hay un 18,37 % sin atribuir.
- **Nivel 1 sin registro:** solo páginas del medio. El RUES da NIT, cámara, matrícula activa, forma jurídica y representante legal.
- **Sin la línea de contratación pública**, obligatoria desde el 2026-10-07. Son 0 contratos, y una ausencia comprobada también se escribe.
- **«Nivel 2 — No hay»:** ya no es cierto (34 artículos en 40 días), y el archivo propio tiene 12 meses de voz de la casa que la ficha no miró.
- **La tabla de dirección:** omite a la Editora General y al Consejo Consultivo, y da a Londoño Jaramillo como persona «con dirección hoy» sin fuente que lo sostenga.
- **«Nivel 1 bis»** no es un nivel del protocolo. La financiación es propiedad económica (nivel 1) o declaración (nivel 4), según cómo se lea; conviene decir cuál.
- **El criterio de refutación 1** usa la compañía media.
- **Error en otra ficha, de paso:** `fichas/voragine.md` (líneas 47-54 y 191-192) dice que Juan Pablo Barrientos «dirige la unidad investigativa de **Volcánicas**» y que el registro lo anota «en la ficha de propiedad de Volcánicas». **Es CasaMacondo:** así lo dicen `fichas/casa-macondo.md`, `mediaOwnership.js` y `centinela.js` en sus entradas de CasaMacondo, el commit `f237d52`, y la propia Volcánicas el 2026-08-07 («jefe de la Unidad Investigativa de Casa Macondo»). La ficha de propiedad de Volcánicas no lo menciona, y está bien que no lo haga.
- **Lo que la ficha sí tenía bien:** que es una ESAL sin propietarios, el origen de la financiación declarada y la salida de OSF, y que su CONTRA era la primera objeción que había que atacar.

---

**Propuesta para la firma**

**Valor: −0,25, izquierda moderada, provisional y sin firmar.** Cambia de −0,50.
- **La dirección es firme.** Encuadre asimétrico entre candidatos en la campaña, la directora situándose a la izquierda en su propio medio, rótulos en voz propia al candidato y luego al Gobierno De la Espriella, y ningún reconocimiento a la derecha en 12 meses.
- **La magnitud tiene tope.** No hay endoso ni nivel 1 con posición conocida, así que rige ±0,30 (§1 y regla 3 del §5).
- **Por qué −0,25 y no el tope de −0,30.** Archipiélago Press (+0,30) llegó al tope con 26 piezas y holgura a los dos lados. Aquí el barrido cumple solo en la lectura amplia, y el después se sostiene con 2 piezas claras. El Diario (Pereira, +0,25, 80 piezas con un después mezclado) y Diario La Libertad (+0,20, 27 piezas a 3,5:1) son los vecinos. La regla 2, en su espíritu: ante la duda, más cerca de la mixta.
- **Alternativas declaradas:**
  - **−0,30**, si el responsable editorial pesa más el encuadre entre candidatos y las dos piezas de la directora que la delgadez del después.
  - **−0,50 provisional, ficha incompleta**, si el responsable editorial lee el barrido en estricto (como en Abra) y aplica «un barrido que no llega a los mínimos no deshace nada». Hay que escribir entonces que la magnitud no tiene base admisible (§2).
  - **−0,50**, si el responsable editorial decide que la posición de la directora es nivel 1 con posición conocida. No se recomienda.
- El barrido no sostiene la derecha, ni un 0,00 con evidencia.

**Textos a corregir** (los aplica quien el responsable editorial decida; aquí no se toca nada):

En `fichas/volcanicas.md`:
1. **Cabecera:** «**−0,50** · Izquierda moderada» → «**−0,25** · Izquierda moderada, provisional (barrido de la voz de la casa, 2026-10-10; ver `revision-externa/barridos/volcanicas.md`)».
2. **Nivel 1:** añadir el registro: «FUNDACION HOJA BLANCA-ONG SIGLA HB-ONG, NIT 900414071-5, Cámara de Comercio de Barranquilla, fundación, ACTIVA, matriculada el 15-02-2011, último año renovado 2024 (RUES, datos.gov.co c82u-588k, consultado 2026-10-10); representante legal, Martha Beatriz Navarro Restrepo, su gerente administrativa y financiera. No consta renovación de 2025 ni de 2026 en el conjunto abierto».
3. **Tabla de personas:** añadir «Ita María | Editora General — dirige la redacción» y una línea para el «Consejo Consultivo: órgano de veeduría externo, 5 personas que no son empleadas ni de la fundación». Cambiar «Matilde de los Milagros Londoño Jaramillo | Cofundadora» → «Cofundadora; /nosotras/ la lista entre las fundadoras, no en el equipo». Paula Henao Aristizábal, «Coordinadora general».
4. **Financiación:** «aportes individuales (Patreon) ..... resto» → «sin atribuir ..... 18,4 % (la página nombra además aportes por Patreon, sin porcentaje; en 2021, /financiamiento/ los daba en el 1 %)». Añadir: «Composición declarada, no auditada: el balance y el certificado que /financiamiento/ anuncia no tienen enlace». «Nivel 1 bis» → «Nivel 1 — propiedad económica, declarada».
5. **Sección nueva «CONTRATACIÓN PÚBLICA»:** «Contratación pública (SECOP I y II, NIT 900414071, consultado 2026-10-10): 0 contratos en SECOP I y II a 2026-10-10 (con y sin dígito de verificación, y por razón social)».
6. **Nivel 4:** sustituir la cita no literal por la literal de /nosotras/ (ver «Errores de la ficha») y añadir: «Volcánicas es un proyecto de Fundación Hoja Blanca ONG, una organización sin ánimo de lucro y no partidista. No apoya a ningún candidato ni partido político, y no tiene propietarios ni propietarias» y «el periodismo que se dice sin posturas o sin apuestas políticas está a la defensa del status quo, que no es más que el patriarcado».
7. **Nivel 2:** «No hay» → el resumen del barrido (17 a 3 en la lectura amplia, 12 y 5; 8 en la estricta, que no llega; encuadre entre candidatos; dos piezas de la directora; sin endoso), con enlace al barrido, y la tabla de la conducta medida del 2026-10-10 (34 artículos, 40 días), advirtiendo que la compañía media no mueve el número.
8. **ARGUMENTO:** retirar la comparación con Vorágine, RAYA y Cuestión Pública (sin medir) y razonar contra Archipiélago (+0,30), El Diario (+0,25) y Diario La Libertad (+0,20), con el tope de ±0,30 y por qué la posición de la directora no es nivel 1.
9. **CONTRA:** «No está resuelto» → «Resuelto en la dirección por la voz de la casa: la casa no es transversal en lo económico y la directora se sitúa a la izquierda. Lo que sigue abierto es la magnitud: el barrido cumple solo contando las piezas leves y el después es delgado». Mantener lo de «periodismo feminista no equivale a izquierda» como advertencia general, y declarar que la línea declarada de la casa es temática («transincluyente, antirracista, decolonial…») y no partidista.
10. **REFUTACIÓN:** 1 → «Si en el recuento de diciembre la voz de la casa critica al Gobierno De la Espriella solo por hechos de gestión, sin rótulos, y publica fiscalización de la izquierda colombiana, el número baja hacia 0,00. Si publica un endoso en voz propia, el tope deja de aplicar». 2 se mantiene. 3 se mantiene.
11. **Sección «REVISIÓN»:** esta resolución, con modelo, versión y fecha.

En `shared/mediaRegistry.js`, entrada `volcanicas`:
- `bias: -0.50` → `bias: -0.25`.
- `biasRationale` → 'Revista de periodismo feminista latinoamericano, proyecto de la Fundación Hoja Blanca ONG (NIT 900414071, ACTIVA en el RUES), sin propietarios, que se declara «no partidista». Izquierda moderada, −0,25, por el barrido de su voz de la casa (10-10-2026): 17 piezas con postura a la izquierda frente a 3 contrapesos, 12 antes del 07-08 y 5 después. Perfiles laudatorios de Cepeda y Quilcué y de escándalos de Valencia y De la Espriella en la campaña, y rótulos al Gobierno entrante; la directora se sitúa a la izquierda en su propio medio. Sin endoso. Cumple los mínimos solo contando piezas leves. Sin firmar — ver fichas/volcanicas.md.'
- El comentario de la entrada está bien; si se toca, añadir que la composición es declarada y no auditada.

En `shared/mediaOwnership.js`:
- `'volcanicas'`: **`ownerType: 'independiente'`** se mantiene (ESAL sin propietarios, como Colombia Informa). **`verifiedAt: '2026-10-10'`.**
  - `holdings[0]` → 'Proyecto de la Fundación Hoja Blanca ONG (FUNDACION HOJA BLANCA-ONG SIGLA HB-ONG, NIT 900414071-5, Cámara de Comercio de Barranquilla, ACTIVA; último año renovado en el RUES: 2024). Sin ánimo de lucro, «no partidista» y sin propietarios, según el propio medio.'
  - `holdings[1]` → '… Hispanics in Philanthropy 40,8 %, Ford Foundation 24,5 % y Foundation for a Just Society 16,3 %; el 18,4 % restante no se atribuye (nombra aportes por Patreon, sin porcentaje). Open Society Foundations fue su principal donante hasta junio de 2025. Es composición declarada: el balance que anuncia no tiene enlace.'
  - `notes`, añadir: 'Contratación pública (SECOP I y II, NIT 900414071, consultado 2026-10-10): 0 contratos en SECOP I y II a 2026-10-10.'
  - `sources`, añadir: `https://www.datos.gov.co/resource/c82u-588k.json?nit=900414071&$select=razon_social,sigla,nit,digito_verificacion,camara_comercio,organizacion_juridica,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,representante_legal,fecha_actualizacion,cod_ciiu_act_econ_pri` y `https://volcanicas.com/financiamiento/`.
- `'volcanicas-hoja-blanca'`:
  - `label` → 'Fundación Hoja Blanca ONG — dirigida por Catalina Ruiz-Navarro'.
  - Persona nueva: Ita María, «Editora General», fuente /nosotras/.
  - Martha Beatriz Navarro: añadir «representante legal en el RUES».
  - Londoño Jaramillo: «Cofundadora; no figura en el equipo actual».

En `shared/centinela.js`, `volcanicas`: el texto «ese detalle es el que sostiene su −0,50: si la composición cambia, el número se queda sin fundamento» deja de ser cierto. Propuesta: «La fundación que lo sostiene (NIT 900414071). Declara su financiación con porcentajes; un cambio sustancial obliga a revisar la ficha (refutación 3). El número lo sostiene el barrido de su voz de la casa, no la financiación.»

En `fichas/voragine.md`, líneas 47-54 y 191-192: «Volcánicas» → «CasaMacondo» en lo de Barrientos (ver «Errores de la ficha»). No mueve ningún número.

**Lo que NO entra como hecho:**
- que la directora controle la fundación más allá de su cargo, o que su posición sea la de la fundación;
- cualquier parentesco entre personas de la fundación (el revisor tampoco lo afirma);
- que la fundación haya dejado de renovar la matrícula: el RUES abierto dice 2024 y puede ser rezago;
- las subvenciones de HIP, Ford y FJS por fuente de los donantes: no se consultaron;
- la filiación de nadie que no la declare la propia fuente (la gobernadora del Chocó consta como «candidata del Partido Liberal» en 2023 en la pieza de Volcánicas, y es local).

**¿Aviso de quien dirige?** No procede: no consta candidatura ni cargo público de la directora ni de la editora general.

**Decisiones para el responsable editorial:**
1. **Valor.** Recomendación: **−0,25**. Alternativas: −0,30 (el tope) o −0,50 provisional (lectura estricta y «no deshace nada»).
2. **¿Cuentan las leves para llegar a los mínimos?** Aquí decide el resultado. Recomendación: **sí para las de antes** (rótulos en voz propia, como en El Informador) y **declarar como dudosas las 3 de después**. Con eso el barrido cumple, en el límite, y la regla 2 justifica −0,25 en vez del tope.
3. **¿La posición declarada de quien dirige una fundación sin dueños es «nivel 1 con posición conocida»?** Recomendación: **no**, por las cuatro razones del punto 4. Si el responsable editorial decide que sí, conviene escribirlo en el protocolo, porque alcanza a cualquier medio cuyo director opine en sus páginas.
4. **La incoherencia del protocolo.** Con el barrido en estricto, la regla 3 deja −0,50 aunque solo lo sostiene el nivel 4. Con el barrido en amplio, el tope lo baja a −0,30 como mucho. **Menos evidencia deja el número más lejos de la mixta.** Recomendación: añadir a «Un barrido que no llega a los mínimos no deshace nada» la salvedad «salvo que el valor vigente se apoye solo en niveles 4 y 5, que el §2 no admite como única base». Es la misma lógica de la decisión del 2026-09-16 sobre Vorágine, RAYA y Cuestión Pública.
5. **Aplicación simultánea.** La misma pregunta está abierta en Colombia Informa (−0,55, empujado por la misión, DECISIONES 2026-09-22) y CasaMacondo (−0,35, solo nivel 4). Recomendación: decidirlos con el mismo criterio en esta tanda o en la 9, como dice «Lo que NO cambia» del §1.
6. **Recuento en diciembre.** El después tiene 2 meses. Recomendación: rehacer el barrido del después antes del 10-12-2026, como se hizo con Proclama del Pacífico.
