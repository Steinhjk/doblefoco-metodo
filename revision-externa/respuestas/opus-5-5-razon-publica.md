# Respuesta — Claude Opus 5.5 sobre Razón Pública

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
> **Sin ediciones.** El revisor no copió cédulas, teléfonos ni direcciones de
> personas naturales, y no enlazó ninguna página que los muestre. Se explica al
> principio de la resolución.

---

## RESPUESTA LITERAL

```
DECLARACIÓN PREVIA DE CONFLICTO
Soy Claude Opus 5.5 (claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Para reducir el sesgo de coincidencia he buscado sobre todo en fuentes que la ficha NO usa (RUES, SECOP I y II, la API REST de WordPress del sitio, su feed RSS, la página «Nuestros Servicios», los archivos de logotipos del pie, las columnas del director) y he usado las dos páginas que sí cita la ficha solo para comprobarlas. Mi acuerdo no debe usarse como aval.

MÉTODO Y DÓNDE BUSQUÉ (todo comprobado el 2026-10-10)
- robots.txt de razonpublica.com: solo excluye rutas de WooCommerce y /wp-admin/, no excluye a ClaudeBot, Claude-Web ni anthropic-ai. Lo mismo en es.wikipedia.org, donde solo leí /wiki/.
- HTML crudo (curl -sL con UA de navegador y --ssl-no-revoke) de /quienes-somos/, /que-es-razon-publica/, /nuestros-servicios/ y /donacion(es)/. Bajé y abrí los dos logotipos del bloque «Nuestro aliados» (Group.svg, que rendericé, y LOGO-UNISANPABLO_nuevo-ES-300x86.png).
- API REST de WordPress del propio sitio: /wp-json/wp/v2/posts?after=2025-10-10T00:00:00&per_page=100&_fields=date,link,title,author,categories (9 páginas, X-WP-Total: 845 entradas) y /wp-json/wp/v2/categories. Es el barrido reproducible del periodo 2025-10-10 → 2026-10-10.
- Las páginas 1 a 4 de /author/hernandogb/ (el director) y el HTML de sus 31 piezas del periodo, con la fecha tomada de "datePublished" (JSON-LD).
- El feed /feed/ (10 ítems, con <category> y <dc:creator>).
- datos.gov.co: RUES (c82u-588k) con nit=900199696; SECOP II (jbjy-vk9h) con documento_proveedor=900199696 y =9001996965; SECOP I (f789-7hwg) con identificacion_del_contratista=900199696 y =9001996965. En todos los casos $select se limitó a los campos que cito.
- Buscador web: una sola consulta («"Razón Pública" Hernando Gómez Buendía 2026 fundación financiación»). Estuvo disponible. No trajo nada sobre financiación.
- No toqué los dominios prohibidos.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré ningún cambio. El RUES (c82u-588k, consultado el 2026-10-10) devuelve: razon_social «FUNDACION RAZON PUBLICA», nit «900199696», estado_matricula «ACTIVA», camara_comercio «BOGOTA», organizacion_juridica «LAS DEMÁS ORGANIZACIONES CIVILES,CORPORACIONES,FUNDACIONES», fecha_matricula «20071221», fecha_renovacion «20260313», ultimo_ano_renovado «2026». El NIT, 900 199 696-5, lo publica el propio sitio en el bloque de donaciones de /quienes-somos/. Al tratarse de una fundación (ESAL), no tiene dueño accionista.

- La persona que la ficha nombra como titular o director, ¿sigue viva y en el cargo?
  Sí, a 2026-10-10. Hernando Gómez Buendía firma «El Tigre y los militares» (datePublished 2026-10-05T13:23:04; en el feed, <dc:creator> «Hernando Gómez Buendía»), y /quienes-somos/ (dateModified 2026-09-02T21:22:08) lo presenta como «Director y editor general».

- ¿Quién dirige hoy la redacción?
  Según el bloque «Nuestro equipo» de /quienes-somos/ (2026-09-02): «Hernando Gómez Buendía — Director y editor general», «Adriana Camacho — Editora», «María Paula Contreras Castro — Coordinadora editorial e imágenes» y «BYB — Caricaturas».

- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que la ficha cita?
  Sí. La renovación en el RUES del 2026-03-13 (año renovado 2026) es un registro externo del presente que la ficha no cita. En SECOP no hay nada: SECOP II y SECOP I devuelven [] para 900199696 y para 9001996965. La fundación no tiene contratos públicos registrados con ese NIT.

## OBJECIONES

OBJECIÓN 1 — Los patrocinadores del pie sí se pueden identificar
- QUÉ afirma la ficha: «NO PUBLICA LA IDENTIDAD DE SUS PATROCINADORES INSTITUCIONALES: su página de aliados muestra logos sin identificarlos».
- POR QUÉ: el bloque «Nuestro aliados» de /quienes-somos/ (que se repite en el pie de todo el sitio) tiene exactamente dos imágenes: <div class="LogosAliadosFooter"> con src ".../2024/04/Group.svg" y src ".../2025/02/LOGO-UNISANPABLO_nuevo-ES-300x86.png". Al abrir el PNG se lee «UNISANPABLO — FUNDACIÓN UNIVERSITARIA SAN PABLO — mente, voluntad y corazón». Al renderizar el SVG se lee «Universidad Externado de Colombia». Los logos tienen texto legible, así que los aliados son identificables. Lo que sí falta es lo que la ficha podría llamar hueco con más precisión: el tipo de relación y los importes.
  Hecho: los dos aliados que el sitio muestra hoy son la Universidad Externado de Colombia y la Fundación Universitaria San Pablo.
  Inferencia, y no la uso: que sean donantes y no socios académicos.
- FUENTE: https://razonpublica.com/quienes-somos/ (página con dateModified 2026-09-02; el archivo del logo de San Pablo se subió en 2025-02), descargada el 2026-10-10.
- NIVEL: declaración del propio medio / propiedad y financiación.
- Efecto: cierra en parte el hueco de nivel 1 que la propia ficha lista como refutación («Si publica la identidad de sus patrocinadores institucionales: se cierra el hueco»). No mueve el número.

OBJECIÓN 2 — La ficha no recoge una fuente de ingresos declarada: servicios pagados de difusión y de contenido para fundaciones
- QUÉ afirma la ficha: que la fundación «se sostiene con donaciones directas y con aportes de miembros de su propio consejo directivo».
- POR QUÉ: la página /nuestros-servicios/ dice literalmente «Con el propósito de garantizar nuestra sostenibilidad financiera, mantener nuestra independencia y facilitar que fundaciones, centros de pensamiento y empresas comuniquen y difundan sus ideas [...] ofrecemos los siguientes servicios: Difusión de textos, vídeos y eventos de interés público / Cursos de redacción / Traducción de textos / Creación de contenido con identidad de marca». Bajo el título «Hemos trabajado con:» enumera logotipos con estos title: «Fundación Avina», «Universidad-de-Ibagué», «Universidad-del-norte», «Open-society-foundations», «Universidad-Externado-de-Colombia», «Universidad EAFIT», «Fundación-Ford» y «Fundación-Friedrich-Ebert-de-Colombia».
  Hecho: el medio declara hoy una línea de ingresos por difundir y crear contenido para terceros, y nombra a esos clientes.
  Lo que NO sé: las fechas ni la vigencia de cada relación. La página tiene dateModified 2024-04-28, sigue publicada y está enlazada desde el menú. Tampoco sé si alguna pieza del corpus es contenido difundido por encargo: en los 845 títulos del periodo, ninguno lleva una marca de «patrocinado» ni «en alianza con» que lo delate. Solo revisé títulos.
  No atribuyo orientación por la afinidad política de ningún cliente: sería una inferencia sin respaldo documental.
- FUENTE: https://razonpublica.com/nuestros-servicios/ (dateModified 2024-04-28; descargada el 2026-10-10).
- NIVEL: declaración del propio medio / financiación.

OBJECIÓN 3 — La voz de la casa existe, es medible y no apoya −0,40: el director recomienda el centro y critica a los dos polos
- QUÉ afirma la ficha: «Sin esa medida, cualquier número sería una impresión de lectura», y que el único material posible son columnas de terceros. Mantiene −0,40.
- POR QUÉ: el director y editor general firma una columna cada dos semanas aproximadamente. Es la voz de la casa más clara del sitio y la ficha no la examina. En 12 meses (2025-10-10 → 2026-10-10) hay 31 piezas suyas (lista completa al final). Estas son sus posturas sobre el eje, con cita literal:
  a) Recomienda candidatos de centro, en la izquierda y en la derecha del centro. No hay un endoso formal de la casa, pero sí una recomendación firmada por el director:
     - 2026-03-07, «¿A quién elegimos hoy?» (https://razonpublica.com/quien-elegimos-hoy/): «Si a usted le preocupa Cepeda, López es el dique más eficaz porque ofrece soluciones reales y no apenas consignas. Si le preocupa de la Espriella, Claudia es el dique más eficaz porque defiende el orden democrático sin nostalgia autoritaria.»
     - 2026-05-31, «Qué elegimos hoy» (https://razonpublica.com/que-elegimos-hoy/), día de la primera vuelta: «Sergio Fajardo representa esta apuesta: moderación, gradualismo y administración técnica. [...] Es la opción racional»; y de Claudia López: «es la candidata que mejor podría recoger las dos mitades rotas de Colombia».
     - 2026-04-06, «Entre lo malo y lo peor» (https://razonpublica.com/lo-malo-lo-peor/): «Temo que López y Fajardo, la centroizquierda y la centroderecha verdaderas, se nos están ahogando entre los polos.»
     - 2026-04-20, «El suicidio del centro» (https://razonpublica.com/suicidio-del-centro/): «Sergio Fajardo representa la centroderecha moderna [...] Y tiene razón.»
     - 2026-05-18, «En defensa del centro» (https://razonpublica.com/defensa-del-centro/): «Los extremos ofrecen identidad. El centro ofrece realidad.»
  b) En la segunda vuelta no respalda a nadie: 2026-06-15, «La otra mitad del país» (https://razonpublica.com/la-otra-mitad-del-pais/): «Esta es una elección entre dos gobiernos desastrosos.»
  c) Rechaza en lo sustantivo el programa de la izquierda, no solo la gestión del gobierno:
     - 2026-04-06: «Petro y Cepeda comparten el indudable mérito moral de hablar por los de abajo [...] Pero sucede que están completamente equivocados en materias de paz, economía, políticas sociales y política internacional.»
     - 2026-03-23, «Anatomía de las candidaturas presidenciales» (https://razonpublica.com/anatomia-las-candidaturas-presidenciales/): «Cepeda entiende todo de derechos y reclamos sociales, pero en cambio entiende nada de crecimiento económico o clima de inversión.»
  d) Rechaza con dureza a la derecha candidata:
     - 2026-04-06: «un fascismo estridente y ramplón»; «Abelardo de la Espriella es el "hijo rebelde" de Uribe, un patán exitoso».
     - 2026-03-23, «Elecciones: lo mismo de siempre» (https://razonpublica.com/elecciones-lo-siempre/): «la derecha cerril de Abelardo de la Espriella o el uribismo disfrazado de centro de Paloma Valencia».
     - 2026-02-09, «Las consultas del 8 de marzo: una equivocación» (https://razonpublica.com/las-consultas-del-8-marzo-una-equivocacion/): «Paloma Valencia es la caverna con buenos modales».
  Hecho: la voz de la casa se declara de centro, recomienda a la vez a una candidata de centroizquierda y a un candidato de centroderecha, y rechaza en lo sustantivo a los dos polos.
  Inferencia: eso describe la banda mixta, o a lo sumo una izquierda moderada muy leve, no −0,40. Hay un contrapeso que hay que registrar: el lenguaje contra la derecha es más despectivo («fascismo», «patán», «caverna», «cerril») que contra la izquierda, a la que concede «mérito moral».
  Por la regla «ante la duda, la banda más cercana a la mixta», esta evidencia empuja hacia 0.
- FUENTE: las URL citadas. Fechas tomadas de "datePublished" en su HTML, descargado el 2026-10-10.
- NIVEL: hecho editorial de los últimos 12 meses (voz de la casa). Las recomendaciones de voto son lo más parecido a un endoso, y la regla del polo fijo no las excluye.

OBJECIÓN 4 — Continuidad a través del cambio de gobierno: fiscaliza al que gobierna, antes y después. No hay asimetría 3:1
- QUÉ afirma la ficha: nada sobre los dos lados del cambio del 07-08-2026. Mantiene −0,40 sin piezas posteriores al cambio.
- POR QUÉ, en tres capas reproducibles:
  a) El director antes del cambio, contra Petro. 2026-02-23, «Los dos Petros» (https://razonpublica.com/los-dos-petros/): «el Petro agresivo, dogmático y autoritario». 2025-10-20, «Machado, Trump y Petro» (https://razonpublica.com/machado-trump-petro/): «Petro habla desde el idealismo del militante, pero olvida que su único papel es el de ser presidente de Colombia.»
     El director después del cambio, contra De la Espriella. 2026-10-05, «El Tigre y los militares» (https://razonpublica.com/el-tigre-y-los-militares/): «No, señor presidente. Usted no es un soldado. Afortunadamente.» 2026-09-20, «La insana doctrina de Abelardo» (https://razonpublica.com/la-insana-doctrina-de-abelardo/): «ser presidente no lo convierte en autoridad religiosa».
     Contrapeso: en «¿Estado laico?» (2026-08-10, https://razonpublica.com/estado-laico/) defiende al presidente en un punto concreto: «Abelardo de la Espriella no violó la Constitución. Actuó exactamente dentro del modelo que la Constitución diseñó.»
     Hay 4 piezas del director después del cambio (08-10, 08-24, 09-20, 10-05). Tres fiscalizan y una es una reflexión sobre el terremoto sin postura («Volvimos a ser colombianos», 08-24). Fiscalizar no cuenta, así que el umbral de «≥3 piezas con postura a cada lado del cambio» NO se cumple hacia la izquierda ni hacia la derecha.
  b) Las caricaturas de la casa. BYB figura en «Nuestro equipo», así que son voz propia. Según los títulos de la API, apuntan al que manda o al que lidera.
     Antes del cambio: «Caricatura Petro no Kings» (2025-10-19), «Caricatura Petro le escribe a Petro» (2025-11-18), «Caricatura Reunión Petro y Trump» (2026-02-02), «Caricatura Therian Petro y Abelardo» (2026-02-22), «Caricatura Cepeda rima con constituyente» (2026-05-04), «Caricatura Ivan Cepeda primera vuelta» (2026-05-18), «Caricatura Petro desconoce resultado» (2026-06-09).
     Después del cambio: «Caricatura Balones defensores Abelardo» (2026-08-22), «Caricatura presupuesto Abelardo austero» (2026-08-31), «Caricatura Muertos en bolsas Abelardo» (2026-09-08), «Caricatura Ecopetrol corrupción» (2026-09-21), «Caricatura Abelardo armado» (2026-09-28).
  c) La selección de temas, por títulos (barrido sobre los 845 posts de la API, separando en el 2026-08-07):
     - Antes: 691 posts, de los que 42 títulos nombran a Petro, Cepeda o el Pacto Histórico y 5 nombran a Abelardo o De la Espriella.
     - Después: 154 posts, de los que 4 títulos nombran a Petro, Cepeda o el Pacto y 15 nombran a Abelardo o De la Espriella.
     Entre los títulos de antes del cambio hay piezas críticas con el gobierno saliente, por ejemplo «Petro grita ¡CENSURA!» (2025-10-26), «La consulta inconsulta del Pacto Histórico» (2025-11-02), «El populismo del M-19, el neopopulismo de Gustavo Petro, sus contradicciones y su deriva en un eventual gobierno de Iván Cepeda» (2026-05-11), «Balance del gasto público en el gobierno Petro: altos recursos, baja ejecución» (2026-07-12) y «La salud bajo el gobierno Petro: problemas reales, diagnóstico equivocado» (2026-08-02).
  Hecho: el foco crítico sigue al gobierno de turno.
  Inferencia, con la regla del polo fijo: es el patrón de «fiscalizaba al saliente y sigue con el entrante», es decir, orientación mixta. Con este barrido no hay asimetría que justifique −0,40 por la vía del nivel 2 editorial.
  Lo que no cuento como prueba: los títulos no son posturas. Solo muestran a quién mira la casa.
- FUENTE: https://razonpublica.com/wp-json/wp/v2/posts?after=2025-10-10T00:00:00&per_page=100&page=1..9&_fields=date,link,title,author,categories (consultado el 2026-10-10) y las URL citadas.
- NIVEL: hecho editorial de los últimos 12 meses / conducta observable.

OBJECIÓN 5 — El argumento central de la ficha se apoya en cifras que la medición de hoy contradice, y su propia tabla no cuadra
- QUÉ afirma la ficha: «28 artículos», «Historias en las que entra: 15», «Historias compartidas con otro medio: 1», «Cadencia: una pieza cada 7,6 h», y de ahí: «15 de sus historias están dentro del feed como si fueran cobertura».
- POR QUÉ:
  a) La medición del 2026-10-10 que acompaña el envío dice: 67 artículos, 3 en alguna historia, 6 historias, 6 compartidas, agenda propia 0 % y coincidencias con «Infobae 3 · El Espectador 1 · La República 1». Hoy hay 3 piezas suyas dentro de historias, no 15 historias, y las 6 historias en que entra son todas compartidas. El riesgo de «opinión presentada como cobertura» existe, pero hoy es mucho menor de lo que la ficha dice.
  b) Hay una inconsistencia interna: 28 artículos en 30 días son una pieza cada 25,7 h, no cada 7,6 h. Con la medición actual (67 en 40 días) salen unas 14,3 h. La tabla de «Socios», además, mezcla filas de otros medios sin explicar qué mide.
- FUENTE: bloque «CONDUCTA MEDIDA», medición del 2026-10-10 (ventana 2026-08-31 → 2026-10-10), frente a la ficha (2026-09-08). La aritmética es mía.
- NIVEL: conducta medida (nivel 2).

OBJECIÓN 6 — La opinión y la firma sí se pueden marcar sin la URL: el feed y la API las traen
- QUÉ afirma la ficha: «Razón Pública publica en la raíz [...] así que el filtro no ve ninguna de las tres», y que medir «quién firma [...] exige una medida que hoy no existe [...] aquí no lo trae».
- POR QUÉ: el RSS del sitio trae categoría y firmante por ítem. Por ejemplo, «El Tigre y los militares» => <dc:creator> «Hernando Gómez Buendía»; «Caricatura Sergio Niño Poeta» => «B&B»; «EDICIÓN DEL 05 DE OCTUBRE AL 11 DE OCTUBRE DEL 2026» => «Equipo Razón Pública»; y la etiqueta <category> «COLUMNA DE OPINIÓN» aparece 6 veces y «Columna» 5 veces en los 10 ítems. La API REST expone las categorías: en los 845 posts de 12 meses, «COLUMNA DE OPINIÓN» tiene 180, «Voto Informado» 114, «Boletín» 43, «Detector de humo: Contra el desorden informativo» 40 y «SAZÓN PÚBLICA» 40. Y las caricaturas empiezan literalmente por «Caricatura». Es justo la vía que la ficha da como refutación («Si se marca su opinión por otra vía que la URL —el feed, la categoría del ítem RSS—»), y existe hoy.
- FUENTE: https://razonpublica.com/feed/ y https://razonpublica.com/wp-json/wp/v2/categories (consultados el 2026-10-10).
- NIVEL: conducta observable.

## LO QUE NO PUDE VERIFICAR
- Importes y peso de cada fuente de ingresos (donaciones, consejo, servicios, aliados). No encontré en el sitio estados financieros ni informe de gestión: busqué «estados financieros», «informe de gestión», «régimen tributario» y «rendición de cuentas» en /quienes-somos/, /que-es-razon-publica/, /nuestros-servicios/ y /donaciones/. No consulté el registro web de ESAL de la DIAN.
- Si siguen vigentes las relaciones con Avina, Open Society, Ford, FES, Externado, EAFIT y las demás (la página tiene dateModified 2024-04-28 y no fecha cada relación).
- Quién financia el proyecto «Voto Informado» (114 piezas). Su presentación (2025-10-13, https://razonpublica.com/voto-informado-cuando-la-verdad-importa-mas-ruido/) dice que es «una iniciativa periodística impulsada por Razón Pública» y no nombra financiador.
- Si «Detector de humo» (40 piezas) y «Boletín» (43) son producción propia de verificación o información, y no análisis. No las leí. Por eso no puedo afirmar ni negar el «100 % análisis» de la ficha.
- Si «Miembros financiadores» tiene más nombres que el que se ve en el HTML: solo aparece «Manuel Rodríguez Becerra», que también figura en el Consejo Directivo, lo que coincide con la ficha.
- La afiliación de cada columnista de terceros. No hice el barrido «quién firma, desde dónde».

## LO QUE FALTA
- El RUES de 2026 (renovación 2026-03-13) como fuente de nivel 1 del presente, y la constancia de que SECOP I y II no registran contratos con el NIT 900199696.
- La identidad de los aliados del pie (Objeción 1) y la línea de servicios pagados con sus clientes declarados (Objeción 2).
- Las columnas del director como voz de la casa (Objeciones 3 y 4). Es la evidencia que más pesa en la clasificación y la ficha no la toca.
- Miembros del Consejo Directivo que publican en el medio. En el feed actual firman Marcela Anzola («Iglesias, derecha y poder: ¿Quién usa a quién?», 2026-10-09) e Iván Jaramillo (pieza de salud, 2026-10-05); los dos figuran en el «CONSEJO DIRECTIVO FUNDACIÓN RAZÓN PÚBLICA». Sus piezas están entre la columna de terceros y la voz de la casa, y convendría tratarlas aparte.
- Un barrido por <dc:creator> sobre los 845 posts para contar firmas y su frecuencia, que es la medida que la ficha da por imposible.
- Sobre el segundo encargo (si un medio de solo análisis entra al agrupamiento): no es una cuestión de evidencia sino de catálogo. El único dato que aporto es que el medio etiqueta su opinión en el feed, así que filtrarla es técnicamente viable sin decidir nada sobre el catálogo.

## EVIDENCIA QUE NO MUEVE EL NÚMERO
- RUES (2026-10-10): matrícula ACTIVA y renovada para 2026. La fecha de matrícula (2007-12-21) no coincide del todo con el «constituida en 2008» que dice el propio sitio. No cambia nada.
- SECOP I y II: cero contratos públicos con el NIT, con o sin dígito de verificación (2026-10-10).
- El director vive y sigue en el cargo (pieza del 2026-10-05).
- El director no respaldó a nadie en la segunda vuelta: «Si gana Abelardo, la izquierda tendrá que aceptar que millones de colombianos votaron legítimamente por él. Si gana Cepeda, la derecha tendrá que aceptar exactamente lo mismo.» (2026-06-15, https://razonpublica.com/la-otra-mitad-del-pais/).
- Antes del cambio, el director defendió el mando de Petro hasta el último día frente al presidente electo: «Ese principio no protege a Gustavo Petro. Tampoco protegerá a Abelardo de la Espriella» (2026-07-27, https://razonpublica.com/la-posesion-de-abelardo/). Es fiscalización institucional en los dos sentidos.
- En política internacional, el director critica de forma constante a Trump y a la derecha estadounidense: «El imperio como víctima» (2025-12-15), «El elefante indigestado» (2025-11-04, «la "América profunda", blanca, rural, evangélica, racista») y «La paz de los mercaderes» (2026-03-09, «dictadores de extrema derecha»). Lo registro como contrapeso hacia la izquierda en el tono internacional. Son 3 piezas, que no llegan al umbral y no cruzan el cambio de gobierno colombiano.
- Wikipedia (https://es.wikipedia.org/wiki/Raz%C3%B3n_P%C3%BAblica, dateModified 2024-09-09) todavía nombra una «Subdirección Ejecutiva de María Victoria Duque». El sitio actual la lista solo entre los «MIEMBROS FUNDADORES». Wikipedia está desactualizada, pero no afecta a la orientación.
- Las presentaciones semanales sin firma («EDICIÓN DEL ...», 43 en 12 meses, firmadas como «Equipo Razón Pública») resumen las columnas y no fijan postura propia. Ejemplo del 2026-10-05: «La crisis sigue, los 10 billones no aparecen y el discurso cambió. Petro y De la Espriella acabaron en las mismas confusiones. Expone Isabel Arroyo.»

## SIN OBJECIÓN
No aplica: he presentado 6 objeciones.

ANEXO — Las 31 piezas del director en el periodo, con fecha (datePublished) y URL
2025-10-20 machado-trump-petro | 2025-11-04 el-elefante-indigestado | 2025-11-18 las-elecciones-vienen-tres-matrimonios-forzados | 2025-12-01 incendio-en-el-vecindario | 2025-12-15 el-imperio-como-victima | 2026-01-12 venezuela-nadie-manda | 2026-01-12 despues-maduro-vacio | 2026-01-26 colombia-despues-petro-lecciones-del-gobierno-del-cambio | 2026-02-09 las-consultas-del-8-marzo-una-equivocacion | 2026-02-09 problema-no-petro | 2026-02-23 los-dos-petros | 2026-03-02 colombia-despues-petro-viaje-incomodo-al-corazon-del-pais (es una crónica en tercera persona de la presentación de su libro: la excluyo como voz propia) | 2026-03-02 tres-consultas-suicidas | 2026-03-07 quien-elegimos-hoy | 2026-03-09 la-paz-los-mercaderes | 2026-03-23 anatomia-las-candidaturas-presidenciales | 2026-03-23 elecciones-lo-siempre | 2026-04-06 lo-malo-lo-peor | 2026-04-20 suicidio-del-centro | 2026-05-18 defensa-del-centro | 2026-05-31 que-elegimos-hoy | 2026-06-01 primera-vuelta-las-ocho-cosas-no-se-dijeron | 2026-06-15 la-otra-mitad-del-pais | 2026-06-29 nuestra-arma-secreta | 2026-07-13 la-verdadera-herencia-de-1991 | 2026-07-14 del-empalme-a-la-pelea | 2026-07-27 la-posesion-de-abelardo | 2026-08-10 estado-laico | 2026-08-24 volvimos-a-ser-colombianos | 2026-09-20 la-insana-doctrina-de-abelardo | 2026-10-05 el-tigre-y-los-militares
(Todas en https://razonpublica.com/<slug>/.)
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** El revisor no copió cédulas, teléfonos, direcciones, nacionalidades ni lugares de nacimiento. Sus consultas a datos.gov.co van descritas en texto, sin URL. Tampoco reprodujo los correos ni la cuenta bancaria que publica «Quiénes somos». Esta resolución tampoco los copia, y las consultas que enlaza llevan `$select` limitado a los campos de la entidad, comprobado: devuelven la fila sin datos personales.

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada (2026-10-10):
  - razonpublica.com: `User-agent: *` con `Disallow` solo en rutas de WooCommerce y `/wp-admin/`, y el bloque de Yoast con `Disallow:` vacío. No nombra a ningún agente de Anthropic. **Literal, como dice el revisor.**
  - datos.gov.co: `Crawl-delay: 1` y exclusiones de `/browse`. Se usó solo `/resource`, con pausas.
  - es.wikipedia.org: solo se leyó `/wiki/Razón_Pública`.
  - No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. **No hubo buscador web.**
- **Sitio**, en crudo, con `curl -sL --ssl-no-revoke` y User-Agent de navegador:
  - `/quienes-somos/`, `/que-es-razon-publica/`, `/nuestros-servicios/`, `/donaciones/` y `/feed/`;
  - los dos logotipos del pie: `Group.svg` se renderizó con Chrome sin interfaz y el PNG se abrió;
  - el archivo de tres autores: `/author/hernandogb/` (págs. 1-4), `/author/razonpublica/` (págs. 1-7) y `/author/b-b/` (págs. 1-7);
  - **el cuerpo completo de las 31 piezas del director y de las 50 del «Equipo Razón Pública»**;
  - `/wp-json/wp/v2/categories`.
- **Lo que no se pudo rehacer.** El cortafuegos del sitio devolvió **403** a `/wp-json/wp/v2/posts`, a `?rest_route=`, a `/feed/?paged=N`, a los sitemaps de entradas y a los feeds de categoría durante toda la sesión. A ráfagas también lo devolvió a páginas sueltas, que al reintentar despacio o con otro User-Agent dieron 200. **Las cifras que el revisor saca de la API no se pudieron recontar:** 845 entradas, 180 «COLUMNA DE OPINIÓN», 691/154 y 42/5 frente a 4/15. Quedan como suyas, sin verificar. Quien repita esto debe ir despacio: el bloqueo parece por ráfaga y por User-Agent.
- **Registros**, en datos.gov.co:
  - RUES (`c82u-588k`): por `nit=900199696` y por `razon_social like '%RAZON PUBLICA%'`.
  - SECOP II (`jbjy-vk9h`): `documento_proveedor` = `900199696` y `9001996965`, y por `proveedor_adjudicado like '%RAZON PUBLICA%'`.
  - SECOP I (`f789-7hwg`): `identificacion_del_contratista` = `900199696` y `9001996965`, y por `nom_razon_social_contratista like '%RAZON PUBLICA%'`.
- **Repositorio:**
  - el envío y `fichas/razon-publica.md`;
  - las entradas de `shared/mediaRegistry.js` y `shared/mediaOwnership.js` (en `shared/centinela.js` no tiene entrada);
  - `shared/opinion.js` y su prueba;
  - las menciones en otras fichas y documentos, el protocolo, DECISIONES.md (2026-10-07 a 2026-10-10) y el historial de git del valor.
- **El barrido**, reproducible, está en `revision-externa/barridos/razon-publica.md`.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| N1 | Nivel 1: RUES activa, renovada el 2026-03-13; 0 contratos en SECOP; director y editora | sí | sí | **Aceptada.** Todos los campos coinciden, literal. Añadido: CIIU 9499 y matrícula 90031062. Por nombre tampoco hay contratos. El RUES tiene dos homónimos activos, que no se vinculan |
| 1 | Los aliados del pie son identificables: Externado y Unisanpablo | sí | sí | **Aceptada.** Los dos logos se leen. **Y algo que el revisor deja como inferencia lo dice el propio sitio:** el bloque va precedido de «Razón Pública agradece el patrocinio de instituciones y personas…». El sitio los presenta como patrocinio, no solo como alianza |
| 2 | Línea de servicios pagados de difusión y contenido de marca, y la lista «Hemos trabajado con» | sí | sí | **Aceptada, con una precisión de fechas.** Literal. Los ocho logos de clientes se subieron en **2021-07** (ruta `/uploads/2021/07/`) y los correos de contacto son de personas que ya no están en el equipo actual. Es una declaración vigente sobre una línea de ingresos, **no prueba que esos clientes paguen hoy**. Además, un boletín rotula una pieza «del convenio con la U. Externado» (22-09-2026) |
| 3 | La voz de la casa existe (el director) y no apoya −0,40 | sí | sí, leyendo las 31 piezas enteras | **Aceptada en la dirección; el recuento la matiza.** Todas las citas son literales y las 31 fechas coinciden. La lectura completa da 2 piezas con dirección (izquierda leve), 0 a la derecha, 6 de centro, 10 mixtas, 3 que solo fiscalizan y 10 fuera del eje. **El revisor deja fuera dos rótulos que refuerzan su «contrapeso» del tono:** «el verdadero riesgo autoritario no se llama Cepeda» y «narcisista, machista y homófobo» (01-06), y «Abelardo no pertenece a esa categoría» (18-05). La regla no se activa, como él dice |
| 4 | Fiscaliza al que gobierna antes y después; no hay asimetría 3:1 | sí | **en parte** | **Aceptada en lo verificable.** Las piezas del director y las 12 caricaturas que cita existen, con esas fechas. En total hay 40 caricaturas en la ventana. **Los recuentos de títulos de la API no se pudieron rehacer** (403), y en cualquier caso los títulos no son postura. Una corrección: «¿Estado laico?» no solo fiscaliza, también exculpa en lo jurídico, y aquí se clasifica como mixta |
| 5 | Las cifras de conducta de la ficha están superadas y su aritmética no cuadra | sí | sí | **Aceptada.** 30 × 24 / 28 = 25,7 h, y 40 × 24 / 67 = 14,3 h. Para «7,6 h» harían falta unas 95 piezas en 30 días. Las cifras del envío las cita literales |
| 6 | El RSS trae categoría y firmante; la API marca las columnas | sí | sí, el feed; la API, no | **Aceptada, y va más lejos de lo que el revisor sabe:** el repositorio ya lo usa. Desde el **2026-09-09** (commit `c685969`), `shared/opinion.js` lee la categoría del ítem RSS, y «COLUMNA DE OPINIÓN» y «Caricatura» están en su lista. La prueba usa justo las etiquetas de Razón Pública. La ficha es del 08-09: lo que dice del filtro quedó viejo al día siguiente |

### Lo verificado, objeción por objeción

**N1 · Nivel 1.**
- **RUES** ([`c82u-588k`, por NIT](https://www.datos.gov.co/resource/c82u-588k.json?$select=razon_social,nit,camara_comercio,matricula,organizacion_juridica,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,fecha_cancelacion,cod_ciiu_act_econ_pri&nit=900199696), 2026-10-10), una fila, literal: «"razon_social":"FUNDACION RAZON PUBLICA"», «"nit":"900199696"», «"camara_comercio":"BOGOTA"», «"matricula":"90031062"», «"organizacion_juridica":"LAS DEMÁS ORGANIZACIONES CIVILES,CORPORACIONES,FUNDACIONES"», «"estado_matricula":"ACTIVA"», «"fecha_matricula":"20071221"», «"fecha_renovacion":"20260313"», «"ultimo_ano_renovado":"2026"», «"cod_ciiu_act_econ_pri":"9499"». **Exacto.**
- **Homónimos que no se vinculan:** por razón social salen también «CORPORACION RAZON PUBLICA» (NIT 830142705, activa) y «RAZON PUBLICA LIMITADA EN LIQUIDACION». **Nada los une a la revista**, y no entran en la ficha.
- **El NIT con su dígito, 900 199 696-5**, lo publica el propio sitio en el bloque de donaciones, como dice el revisor.
- **Contratación:**
  - SECOP II ([`jbjy-vk9h`](https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=id_contrato,nombre_entidad,proveedor_adjudicado,fecha_de_firma,valor_del_contrato&documento_proveedor=900199696)) y SECOP I ([`f789-7hwg`](https://www.datos.gov.co/resource/f789-7hwg.json?$select=numero_de_constancia,nombre_entidad,nom_razon_social_contratista,fecha_de_firma_del_contrato,cuantia_contrato&identificacion_del_contratista=900199696)) devuelven `[]` con `900199696` y con `9001996965`.
  - Por razón social (`like '%RAZON PUBLICA%'`), también `[]` en los dos.
  - **0 contratos.**
- **Director y editora:**
  - «Quiénes somos» (`dateModified` 2026-09-02) lista en «Nuestro equipo»: «Hernando Gómez Buendía — Director y editor general», «Adriana Camacho — Editora», «BYB — Caricaturas» y «María Paula Contreras Castro — Coordinadora editorial e imágenes». **Literal.**
  - Su última columna es del 2026-10-05 (`datePublished` 2026-10-05T13:23:04+00:00, y `<dc:creator>` en el feed).
  - **No consta candidatura ni cargo público** del director: el aviso de quien dirige no procede.
- **Wikipedia** (`dateModified` 2024-09-09) dice «la Subdirección Ejecutiva de María Victoria Duque». **Literal.** Hoy el sitio la lista solo entre los «MIEMBROS FUNDADORES».

**1 · Aliados del pie.**
- En el HTML, `<div class="LogosAliadosFooter">` contiene exactamente dos imágenes: `/wp-content/uploads/2024/04/Group.svg` y `/wp-content/uploads/2025/02/LOGO-UNISANPABLO_nuevo-ES-300x86.png`.
- Renderizado, el SVG dice «Universidad Externado de Colombia», y el PNG, «UNISANPABLO — FUNDACIÓN UNIVERSITARIA SAN PABLO — mente, voluntad y corazón». **Literal.**
- **El revisor dice que no usa la inferencia de que sean donantes.** Pero el sitio lo afirma: justo antes del bloque «Nuestro aliados» se lee «Razón Pública agradece el patrocinio de instituciones y personas que reconocen el valor del análisis independiente…». Lo que sigue faltando es el importe y la forma de la relación.

**2 · Servicios.**
- `/nuestros-servicios/` (`dateModified` 2024-04-28) dice, literal: «Con el propósito de garantizar nuestra sostenibilidad financiera, mantener nuestra independencia y facilitar que fundaciones, centros de pensamiento y empresas comuniquen y difundan sus ideas […] ofrecemos los siguientes servicios: Difusión de textos, vídeos y eventos de interés público / Cursos de redacción / Traducción de textos / Creación de contenido con identidad de marca».
- Los `title` de los ocho logos coinciden con los del revisor.
- **Fechas que el revisor no da:** las ocho imágenes están en `/wp-content/uploads/2021/07/`. Los dos correos de contacto de la página son de personas que figuran en el equipo de la página de 2009 y no en el «Nuestro equipo» actual. **La página sigue publicada y enlazada desde el menú**, así que la línea de servicios es una declaración vigente. **La lista de clientes, en cambio, no está fechada:** no prueba relaciones de hoy.
- **Lo que sí está fechado:** el boletín del 2026-09-22 rotula una pieza como «un artículo del convenio con la U. Externado». La misma pareja de autores aparece en 9 boletines de la ventana, y solo ese lo rotula. El mismo boletín marca otra «En convenio con Contexto Media». Es contenido de alianza **rotulado solo en el boletín**, y una vez. Desvelamiento, no acusación.
- Igual que el revisor, no se atribuye orientación por la afinidad de ningún cliente o aliado.

**3 · La voz de la casa** (completo en `revision-externa/barridos/razon-publica.md`).
- **Universo:** las 31 piezas del director (`/author/hernandogb/`, del 2025-10-20 al 2026-10-05), las mismas 31 del anexo del revisor, con las mismas fechas `datePublished`. **Se leyeron enteras.**
- **Las 50 del «Equipo Razón Pública»**, que el revisor no barrió y son la otra candidata a voz de la casa: 42 boletines y 8 síntesis. Los boletines atribuyen cada entradilla a su autor: de 523 párrafos, 452 acaban en «Analiza…/Explica…/Expone…», y el resto son títulos o avisos fijos. Las síntesis atribuyen todo a sus panelistas. **Ninguna tiene postura propia.**
- **Citas:** todas las citas del director en las objeciones 3 y 4 y en «Evidencia que no mueve» están en el HTML, con esas palabras. **Exactas.**
- **Recuento:**

| | I | D | C | M | F | X | Total |
|---|---:|---:|---:|---:|---:|---:|---:|
| Antes del 07-08-2026 | 2 (leves) | 0 | 6 | 9 | 1 | 9 | 27 |
| Desde el 07-08-2026 | 0 | 0 | 0 | 1 | 2 | 1 | 4 |

- **Mínimos de la regla:** ≥10 con postura en una dirección → 2. ≥3 a cada lado → 2 y 0. Proporción → no aplica. **No se activa.** Por rótulos, 9 piezas descalifican a la derecha y 5 rechazan de fondo a la izquierda: 9 a 5.
- **Lo que el revisor no cita y pesa en su contrapeso del tono:**
  - «el verdadero riesgo autoritario no se llama Cepeda», y del líder de la nueva derecha, «un hombre narcisista, machista y homófobo» (01-06, [primera-vuelta-las-ocho-cosas-no-se-dijeron](https://razonpublica.com/primera-vuelta-las-ocho-cosas-no-se-dijeron/));
  - «Cepeda y Paloma son personas decentes. […] Abelardo no pertenece a esa categoría» (18-05, [defensa-del-centro](https://razonpublica.com/defensa-del-centro/)).
  - **Y lo que pesa en el otro lado:** en la misma pieza del 01-06, de Cepeda: «ese también es el peligro que representa para Colombia».
- **Lectura:** el revisor tiene razón en que la voz de la casa se declara de centro, recomienda a López y a Fajardo y no endosa a nadie en la segunda vuelta. El tono es más duro con la derecha, y el fondo rechaza los dos programas. **Es nivel 5 y no mueve el número**, en ningún sentido.

**4 · Continuidad a través del cambio.**
- Del director después del 07-08 hay 4 piezas, como dice el revisor. Aquí se clasifican 2 F (20-09 y 05-10), 1 M y 1 X. «¿Estado laico?» (10-08) va a mixta y no a fiscalización: exculpa al presidente en lo jurídico («no violó la Constitución») y se burla de su gabinete («abelardadas»).
- Antes del cambio, el director fiscaliza a Petro el 23-02 y lo llama «el presidente irresponsable» el 01-06. Y defiende su mando hasta el último día frente al electo, el 27-07. **Misma conducta con los dos**: el patrón que el polo fijo llama mixta.
- **Caricaturas:** las 12 que cita existen, con esos títulos y esas fechas (`/author/b-b/`). En la ventana hay 40, y el revisor no menciona otras del mismo patrón: «Directora del ICBF» (27-08), «Tigre odia Bogotá» (28-07), «Gobierno los de siempre» (14-07) y «Paloma y Oviedo derechos» (15-03). **No se abrieron las imágenes**, así que no se clasifican.
- **Los recuentos por títulos de la API** (691 y 154; 42 y 5; 4 y 15) **no se pudieron verificar**, porque el endpoint da 403. No entran como hecho. De todos modos el revisor ya dice que «los títulos no son posturas».

**5 · Cifras de conducta.**
- La ficha (2026-09-08) da 28 artículos en 30 días y «una pieza cada 7,6 h». **Es imposible:** 720 h / 28 = 25,7 h. El envío del 2026-10-10 da 67 en 40 días, unas 14,3 h. Lo mismo se repite en la «NOTA DE CONTABILIDAD».
- **«15 historias» y «compartidas: 1»** frente a «3 en alguna historia · 6 historias · 6 compartidas» del envío: el revisor lo cita literal. **Rige la del envío**, como dice el propio envío.
- **La tabla de «Socios»** mezcla filas de otros medios sin decir qué mide: es cierto.

**6 · Opinión marcada por el feed.**
- `/feed/` (2026-10-10), 10 ítems. «COLUMNA DE OPINIÓN» aparece en 6 y «Columna» en 5. `<dc:creator>`: «Hernando Gómez Buendía», «B&amp;B» y «Equipo Razón Pública», como dice el revisor. **Literal.**
- `/wp-json/wp/v2/categories` sí responde. Totales históricos, no de 12 meses: «COLUMNA DE OPINIÓN» 645, «Voto Informado» 114, «Boletín» 568, «Detector de humo: Contra el desorden informativo» 80, «SAZÓN PÚBLICA» 517. **El 180 de 12 meses no se pudo verificar.**
- **Lo que el revisor no podía saber:** el producto ya lo hace. `shared/opinion.js` («LA SEGUNDA SEÑAL: LA ETIQUETA QUE EL MEDIO LE PONE AL ÍTEM EN SU RSS», 2026-09-09) tiene `['columna de opinion', 'columna']` y `['caricatura', 'caricatura']`. `shared/opinion.test.js` usa como caso `['COLUMNA DE OPINIÓN', 'Marta Juanita Villaveces Niño'], // Razón Pública`. Lo que **no** se marca a propósito es «análisis» («Meterlo aquí sería contestarla de tapadillo»). Y la pregunta de catálogo la cerró el responsable editorial el 2026-09-16: no noticioso, dentro del agrupamiento y fuera del mapa.

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se corrigen estas partes:
- **Obj. 2:** «el medio declara hoy una línea de ingresos [...] y nombra a esos clientes». La línea es de hoy; **los clientes, no consta**: los logos son de 2021-07. Que sean clientes actuales no entra como hecho.
- **Obj. 3:** «a lo sumo una izquierda moderada muy leve». Con el recuento completo, la regla no se activa en ninguna dirección. «Izquierda moderada muy leve» describe el tono, no un número admisible: sería nivel 5.
- **Obj. 4:** «Tres fiscalizan». Son dos; «¿Estado laico?» es mixta. Los recuentos por títulos de la API no se verifican.
- **Obj. 6:** el 180 de 12 meses no se verifica. El resto, sí.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente ni cita inventada.** Las 31 URL del director resuelven, sus fechas `datePublished` son exactas y sus citas, literales. El RUES, el SECOP, el feed, los logos y la página de servicios coinciden con lo que él consultó. Lo que hay son omisiones y una cifra que no se puede comprobar:
- omite las fechas de subida de los logos de clientes (2021-07) y el convenio rotulado con el Externado;
- omite dos rótulos que refuerzan su propio contrapeso y una frase de la otra cara (01-06);
- no barre al «Equipo Razón Pública», que es la otra voz candidata;
- sus recuentos por API no se pueden recontar hoy, por el 403 del sitio. No es culpa suya.

**Errores de la propia ficha, para no repetirlos:**
- **«su página de aliados muestra logos sin identificarlos»:** falso. Los dos logos se leen, y el sitio los presenta como patrocinio.
- **Usa como fuente de presente una página de 2009.** «Qué es Razón Pública» es una entrada con `datePublished` 2009-10-26, firmada por una persona que ya no está en el equipo y con un equipo y un «Consejo Editorial» de entonces. **De ahí sale el «Consejo editorial» de `mediaOwnership.js`** (Montenegro, Kalmanovitz, Cifuentes, Palacios, Sarmiento: «Orientan la línea sin poseerla»). Hoy «Quiénes somos» no lista ningún consejo editorial. Montenegro, Palacios y Kalmanovitz figuran como «MIEMBROS HONORARIOS»; Sarmiento y Cifuentes, como «MIEMBROS FUNDADORES». El órgano vigente es el «CONSEJO DIRECTIVO FUNDACIÓN RAZÓN PÚBLICA», con otros nombres. **Es la falta de la regla del presente.**
- **Callaba a la editora**, Adriana Camacho, y que la casa tiene caricaturista propio.
- **«el filtro no ve ninguna de las tres»:** dejó de ser cierto el 2026-09-09 (`c685969`). Las columnas y caricaturas de Razón Pública se marcan por su categoría RSS.
- **«LA PREGUNTA QUE VA ANTES DEL NÚMERO»** sigue abierta en la ficha, y el responsable editorial la cerró el 2026-09-16 (`noNoticioso`). El comentario del registro lo dice: «sí entra, y no compite en el mapa».
- **La cadencia de 7,6 h** es aritméticamente imposible con 28 piezas en 30 días, y se repite en la nota de contabilidad.
- **Faltaba la línea de contratación pública**, obligatoria desde el 2026-10-07.
- **«exige una medida que hoy no existe»:** el feed trae `<dc:creator>` por ítem.
- **Lo que la ficha sí tenía bien:** que no había evidencia para el número, que no debía firmarse y que el nivel 2 no se podía leer como agenda.

---

**Propuesta para la firma**

**Firmable: no.**

**Valor, por aplicación literal de las reglas 2 y 3: se queda en −0,40, sin firmar y con la ficha marcada como incompleta.**
- **Regla 3:** «Sin evidencia de nivel 1-3, no se mueve el número. Se deja el actual y se marca la ficha como incompleta». El nivel 1 de una fundación sin dueño no tiene posición conocida. El barrido de la voz de la casa no cumple las condiciones, así que es nivel 5. Y la conducta medida no sirve: no mide contenido y la compañía media está saturada.
- **Segunda precisión del 2026-10-09:** «Un barrido que no llega a los mínimos no deshace nada. La ficha conserva el valor que tenía.» Se aplicó igual a El Pilón (+0,20) y a Proclama (0,00).
- **Regla 2** («ante la duda entre dos bandas, la más cercana a la mixta») decide entre dos bandas cuando hay evidencia admisible con la que decidir. No es una vía para mover lo que la regla 3 congela.

**Pero la evidencia que sostenía −0,40 no existe, y la que hay apunta a otro sitio.**
- El valor viene del alta del 2026-07-27 (commit `75019ce`), con la razón «Análisis académico con énfasis en política social y crítica al modelo económico vigente». No hay fuente, ni decisión en DECISIONES.md, ni evidencia en la ficha. La propia ficha dice que cualquier número «sería una impresión de lectura, y el protocolo la excluye por escrito».
- El único barrido sistemático (31 + 50 piezas) describe una voz de centro que fiscaliza a los dos gobiernos, con el tono algo más duro hacia la derecha. **Eso es banda mixta, no el centro de la izquierda moderada.**
- El −0,40 no es inocuo. El tipo no noticioso saca al medio del mapa, pero **no del agrupamiento**. `noNoticioso` solo se filtra en `src/` (mapa, panel y transparencia), no en `shared/`, así que cada historia en la que entre Razón Pública lo sigue contando como izquierda moderada.

**Recomendación: `bias: null` («sin medir»), como decidió el responsable editorial para Vorágine, Cuestión Pública y Revista RAYA** (sesión del 16-09, código del 18-09, commit `fa77249`).
- Es el mismo tipo de medio, y el mismo defecto: un número heredado que es una colocación sin fuente. El comentario de CasaMacondo en el registro lo dice de los seis no noticiosos: «sus números eran colocaciones relativas que el expediente de Vorágine demostró insostenibles».
- **No afirma una banda**, ni la izquierda ni la mixta.
- **No es una lectura literal de la regla 3**, sino la excepción que el responsable editorial ya hizo por escrito para este tipo. Si la toma, conviene anotarla en DECISIONES.md como aplicación de la del 16-09.
- **Descartado: «0,00 con evidencia».** Sería el valor mejor apoyado, pero exige una precisión nueva del protocolo: que un barrido simétrico pueda sustituir un valor heredado sin evidencia. Además, después del cambio solo hay 3 piezas con contenido, menos que las 15 de Chocó 7 Días. Si el responsable editorial añade esa precisión, debe aplicarse a la vez a todas las fichas con valor heredado.

**Bloque propuesto para `shared/mediaRegistry.js`** (no se escribe en código; con la recomendación):

```js
        bias: null, factuality: 0.92, reviewedAt: null,
        biasRationale: 'SIN MEDIR (2026-10-10). Fundación de análisis académico; no publica editoriales sin firma. La voz de la casa —las 31 columnas y análisis del director y editor general en 12 meses— se declara de centro, recomienda a la vez a una candidata de centroizquierda y a un candidato de centroderecha, no endosa en la segunda vuelta y fiscaliza a Petro y a De la Espriella; el tono es más duro con la derecha. No llega a los mínimos de la evidencia editorial histórica (2 piezas con dirección, ninguna después del 07-08), y el −0,40 heredado no tenía fuente — ver fichas/razon-publica.md y revision-externa/barridos/razon-publica.md.',
```

Si el responsable editorial prefiere la lectura literal: `bias: -0.40` se queda, y la `biasRationale` se reescribe para decir que el valor es heredado y sin evidencia, que la ficha está incompleta y que el barrido de la voz de la casa apunta a mixta (con el mismo enlace).

**`shared/mediaOwnership.js`, entrada `razon-publica` y grupo `razon-publica-fundacion`** (los aplica quien el responsable editorial decida):
- `ownerType: 'independiente'` se queda: fundación sin ánimo de lucro y sin socios.
- `verifiedAt: '2026-10-10'` (hoy hereda `VERIFICADO`, 2026-07-29).
- `holdings`:
  - añadir el RUES: «Fundación Razón Pública, NIT 900199696, Cámara de Comercio de Bogotá, activa, renovada el 2026-03-13 (RUES)»;
  - añadir la contratación pública, con el formato del protocolo: «Contratación pública (SECOP I y II, NIT 900199696, consultado 2026-10-10): 0 contratos en SECOP I y II a 2026-10-10»;
  - **sustituir** la frase de los logos por esta: «Su pie agradece "el patrocinio de instituciones y personas" y muestra dos aliados, la Universidad Externado de Colombia y la Fundación Universitaria San Pablo; no publica importes ni la forma de la relación»;
  - añadir: «Declara una línea de servicios pagados ("Difusión de textos, vídeos y eventos de interés público", "Creación de contenido con identidad de marca") "con el propósito de garantizar nuestra sostenibilidad financiera"; la lista "Hemos trabajado con" no está fechada (logos de 2021). Al menos una pieza de 2026 se rotula como "del convenio con la U. Externado"».
- `personas` de `razon-publica-fundacion`:
  - **retirar el «Consejo editorial»**, que sale de la página de 2009;
  - poner en su lugar a **Adriana Camacho, editora**, con fuente `/quienes-somos/`;
  - y el **Consejo Directivo de la fundación como órgano**, sin papel editorial atribuido: «Gobierna la fundación; no consta que tenga autoridad editorial». Si se nombra a sus miembros, solo con nombre y papel.
- `sources`: añadir `https://razonpublica.com/nuestros-servicios/` y la consulta del RUES con `$select`. **`/que-es-razon-publica/` deja de ser fuente de presente**, porque es de 2009.

**Textos a corregir en `fichas/razon-publica.md`:**
1. Nivel 1: la frase de los logos, el RUES, la línea de contratación, la editora, los servicios y el convenio, con las fuentes de arriba.
2. Nivel 2: sustituir las tablas del 2026-09-08 por la medición del envío (2026-10-10, 67 artículos, 40 días) y **quitar la cadencia de 7,6 h**, aquí y en la nota de contabilidad.
3. «LA PREGUNTA QUE VA ANTES DEL NÚMERO»: dejarla como historia y añadir que la contestó el responsable editorial el 2026-09-16 (no noticioso) y que el filtro lee la categoría RSS desde el 2026-09-09.
4. «ARGUMENTO»: la medida «quién firma» existe (`<dc:creator>`). Añadir el barrido de la voz de la casa y su veredicto: nivel 5, mixta en conducta y tono algo inclinado a la izquierda.
5. Nueva sección de tensiones: el tono del director; el patrocinio y los servicios sin importes; el convenio rotulado solo en el boletín; y las firmas del Consejo Directivo.
6. «REFUTACIÓN»: sustituir la primera viñeta, ya cumplida. Por ejemplo: «si en el recuento de diciembre de 2026 el director acumula ≥3 piezas con postura a cada lado del 07-08 en la misma dirección, con proporción ≥3 a 1». Y: «si un documento del medio da autoridad editorial al Consejo Directivo, sus firmas pasan a contar como voz de la casa».

**Fichas y documentos que comparan o cuentan a Razón Pública:**
- `fichas/las2orillas.md` (línea 111, y la copia del envío) la cuenta entre los «SEIS» medios de raíz plana «de la banda de izquierda». Si pasa a «sin medir», **esa frase es una medición del 2026-09-08 y se deja como historia**, con una nota de que hoy son cinco con orientación medida. Ninguna ficha le pone número por comparación con ella.
- `DISENO_ALGORITMO_SESGO.md`, `ESTUDIO_PUNTOS_CIEGOS.md` y `PLAN_CONTINUIDAD.md` la citan como dato de su fecha: no se reescriben.
- El aviso de la portada cuenta la izquierda del catálogo en vivo (`AvisoDesequilibrio.jsx`): con `null`, baja uno solo.

**Lo que NO entra como hecho:**
- que los ocho clientes de «Hemos trabajado con» paguen hoy, o que alguna pieza concreta sea contenido pagado (salvo la rotulada «del convenio con la U. Externado», que lo es por declaración);
- la orientación de ningún aliado, cliente o miembro del consejo;
- los dos homónimos del RUES;
- los recuentos por títulos de la API (845, 180, 691/154, 42/5 y 4/15), que no se pudieron verificar;
- la postura de las caricaturas, que no se abrieron.

**¿Aviso de quien dirige?** No procede. No consta candidatura ni cargo público del director ni de la editora. No hay estatuto publicado que dé autoridad editorial al Consejo Directivo.

**¿Centinela?** No tiene entrada en `shared/centinela.js`. Ahora hay un nombre publicado al que agarrarse, el director y editor general. Se podría vigilar su permanencia en el cargo y un cambio en el RUES (representante, estado). Baja prioridad.

**Decisiones para el responsable editorial:**
1. **Valor.** Recomendación: **`bias: null`, «sin medir»**, por la decisión del 16-09 para el mismo tipo de medio. La alternativa literal es −0,40 sin firmar, incompleta y con la tensión escrita. «0,00 con evidencia» queda descartado mientras no exista la precisión que lo permita.
2. **Criterio para los miembros del Consejo Directivo que firman** (hoy, al menos Marcela Anzola e Iván Jaramillo). Recomendación: **terceros por defecto**, declarados aparte como «firmas del órgano de gobierno». Pasarían a voz de la casa solo si un documento del medio da autoridad editorial al consejo, con el mismo criterio que la regla de quien dirige ampliada el 2026-10-07.
3. **«Equipo Razón Pública» y caricaturas.** Recomendación: los boletines y las síntesis atribuidas **no** son voz de la casa, porque cada tesis va a nombre de alguien. Las caricaturas de B&B, que la casa lista como equipo, **sí lo son**, pero solo cuentan si se abren y se clasifican las imágenes. Queda para el recuento de diciembre.
4. **Corregir `mediaOwnership.js`** según lo de arriba, sobre todo el «Consejo editorial» de 2009. Es un error de hecho sobre el presente, y no depende del valor.
