# Respuesta — Claude Opus 5.5 sobre RTVC Noticias

| | |
|---|---|
| **Modelo** | Claude Opus 5.5 |
| **Versión exacta** | `claude-opus-5-5` |
| **Fecha de la consulta** | 2026-10-10 |
| **Quién la hizo** | Claude Code, a petición del responsable editorial (ciclo 2, fase 2, tanda 9; revisor de la misma casa que el autor de las fichas, ver DECISIONES.md 2026-10-07) |
| **¿Tuvo acceso a la red?** | sí |

> **Se pega LITERAL lo que devolvió el modelo, sin editar ni resumir.** Si se
> recorta, se pierde justo lo que pueda incomodar. Los comentarios nuestros van
> al final, en la sección de resolución, claramente separados.
>
> **Edición:** ninguna (ver el principio de la resolución).

---

## RESPUESTA LITERAL

```
DECLARACIÓN PREVIA DE CONFLICTO
Soy Claude Opus 5.5 (claude-opus-5-5), de Anthropic: la misma casa que el modelo que redactó la ficha. Por eso he buscado sobre todo en fuentes que la ficha NO usa (el archivo de rtvcnoticias.com, inravision.gov.co, RUES, SECOP II, las declaraciones de la Misión de Observación Electoral de la UE y prensa de terceros) y no doy por bueno nada solo porque «suene» a lo que la ficha ya dice. Mi acuerdo con cualquier parte de la ficha no debe usarse como aval.
Revisión hecha el 2026-10-10. Todas las citas salen del HTML o PDF crudo descargado ese día (curl -sL con UA de navegador, --ssl-no-revoke), salvo donde digo expresamente que la fuente es secundaria.

MÉTODO Y DÓNDE BUSQUÉ
- robots.txt revisado antes de descargar: rtvcnoticias.com, rtvc.gov.co (redirige a inravision.gov.co), inravision.gov.co, funcionpublica.gov.co, statemediamonitor.com, pulzo.com, eeas.europa.eu, dapre.presidencia.gov.co (normograma.mintic.gov.co devuelve 404 en robots.txt, es decir, sin restricciones). Ninguno excluye a ClaudeBot, Claude-Web ni anthropic-ai. No he tocado eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. No he consultado Wikipedia.
- Archivo propio de RTVC Noticias (la voz de la casa):
  · Barrido completo y reproducible de la sección «Gobierno»: https://www.rtvcnoticias.com/politica/gobierno?page=0 hasta ?page=16. Salen 119 URL únicas, publicadas entre el 2026-04-28 y el 2026-10-09. De cada pieza tomé la fecha (datePublished) y la firma (author.name) del JSON-LD.
  · Además: /politica?page=0..2, /politica/congreso?page=0..3, /actualidad/inravision y ?page=1, /sistema-de-medios-publicos, /categorias/opinion, la portada, sitemap.xml (7 páginas, casi todo taxonomías: no sirve para listar artículos) y rss.xml.
  · «Voz de la casa» = piezas firmadas «RTVC Noticias» o «Redacción Digital», o sin firma. Las de periodista con nombre las anoto aparte y no las cuento en la regla de evidencia editorial.
- inravision.gov.co: /quienes-somos/perfiles-directivos, /directorio, /directorio/funcionarios-colaboradores, /informes-de-empalme, /informacion-general, /quienes-somos, /decretos.
- Registros: RUES (datos.gov.co c82u-588k) y SECOP II (jbjy-vk9h), consultados por NIT 900002583 con igualdad exacta y sin dígito de verificación. No consulté SECOP I (f789-7hwg): SECOP II ya cubre el periodo que importa.
- Registros externos: declaraciones preliminares de la MOE UE Colombia 2026 (PDF en eeas.europa.eu) y State Media Monitor, que la ficha ya cita.
- Prensa de terceros: pulzo.com (listado /noticias/rtvc y 10 artículos). OJO: varias notas de Pulzo dicen de sí mismas «Este artículo fue curado con apoyo de inteligencia artificial». Las trato como secundarias y lo indico cada vez.
- Buscador web: lo usé 5 veces y estuvo DISPONIBLE. No se agotó.

======================================================================
## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No cambió de titular: sigue siendo del Estado. Sí cambió de nombre y figura con OTRA forma jurídica en el registro mercantil:
  · RUES, consultado el 2026-10-10:
    https://www.datos.gov.co/resource/c82u-588k.json?$select=camara_comercio,matricula,razon_social,organizacion_juridica,estado_matricula,ultimo_ano_renovado,fecha_actualizacion&$where=numero_identificacion='900002583'
    Devuelve: «"camara_comercio":"BOGOTA","matricula":"1434314","razon_social":"INRAVISIÓN - SISTEMA DE MEDIOS PÚBLICOS DEL ESTADO COLOMBIANO S.A.S","organizacion_juridica":"SOCIEDADES POR ACCIONES SIMPLIFICADAS SAS","estado_matricula":"ACTIVA","ultimo_ano_renovado":"2026","fecha_actualizacion":"2026/08/21 16:51:25.647000000"».
  · Lo confirma el propio medio el 15-09-2026: «RTVC - Sistema de Medios Públicos del Estado Colombiano S.A.S., presentó ante la Superintendencia de Industria y Comercio una demanda…» (https://www.rtvcnoticias.com/actualidad/rtvc/comunicado-rtvc-uso-indebido-marca).
  · www.rtvc.gov.co redirige hoy a https://www.inravision.gov.co/, cuyo <title> es «Inravisión Sistema de Medios Públicos | Radio, TV y Memoria». La ficha lo había comprobado el 2026-08-08 y sigue igual.

- La persona que la ficha nombra como titular o director, ¿sigue viva y en el cargo?
  La ficha no nombra a nadie: declara el hueco. Su fuente State Media Monitor dice hoy «Hollman Morris manager since April 2024 (still in post 2026)», y eso está DESACTUALIZADO (ver la objeción 2). Comprobado el 2026-10-10.

- ¿Quién dirige hoy la redacción?
  · GERENTE: Ángela María Mora Soto. Fuente primaria, RTVC Noticias del 31-08-2026: «Por instrucciones de la Gerente, Angela María Mora Soto, Inravisión – Sistema de Medios Públicos mantendrá accesible esta rectificación…» (https://www.rtvcnoticias.com/actualidad/inravision/rectificacion). La nombró el Gobierno de Abelardo de la Espriella: Pulzo (secundaria) habla del «Decreto 1196 del 12 de agosto de 2026».
  · DIRECTOR DE NOTICIAS: no encontré nombre posterior al 07-08-2026. El último que consta es William Parra, «director del Sistema Informativo», citado el 06-08-2026 (https://www.rtvcnoticias.com/actualidad/inravision/el-calentao-informativo-se-despide-tras-consolidarse-como-el-programa-que). La nueva gerencia «suspend[ió] la franja noticiosa y de opinión que operó hasta el 6 de agosto» y el 10-09-2026 terminó «contratos relacionados con actividades periodísticas, de presentación y de gestión de contenidos digitales» (https://www.rtvcnoticias.com/actualidad/rtvc/rtvc-avanza-en-la-transformacion-del-sistema-de-medios-publicos). Hecho: no hay director de noticias nombrado públicamente. Inferencia: puede que hoy no exista el cargo.

- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que la ficha cita?
  Sí. El RUES se actualizó el 2026-08-21 (arriba). Las fuentes de la ficha son una norma de 2004 (el enlace está roto, ver la objeción 1), una resolución de 2016 y State Media Monitor (marzo de 2025, con añadidos de 2026).

======================================================================
## OBJECIONES

### OBJECIÓN 1 — La fuente «ROTA» no está caída: el enlace lleva a OTRA norma. Hay sustituta primaria.
- QUÉ AFIRMA LA FICHA: que https://www.funcionpublica.gov.co/eva/gestornormativo/norma.php?i=82339 es la «norma de constitución». El envío la marca como «fetch failed (2 intentos)».
- POR QUÉ: hoy, 2026-10-10, la URL responde 200 (312 430 bytes). Su <title> es «Concepto Sala de Consulta C.E. 00101 de 2016 Consejo de Estado - Sala de Consulta y Servicio Civil». El texto trata de la financiación: «Encuentra la Sala que los recursos que traslada la ANTV a la RTVC para su operación y funcionamiento son transferencias corrientes…». Es un concepto de 2016 sobre recursos, no la norma de constitución. El enlace está mal aunque cargue.
- SUSTITUTA (primaria): el Decreto 3912 de 2004 en la compilación jurídica de MinTIC, https://normograma.mintic.gov.co/mintic/compilacion/docs/decreto_3912_2004.htm (descargado el 2026-10-10). Dice: «Que Radio Televisión Nacional de Colombia, RTVC, autorizada mediante Decreto número 3525 de 26 de octubre de 2004, es una sociedad entre entidades públicas, indirecta, del orden nacional, sometida al régimen de las Empresas Industriales y Comerciales del Estado». Como declaración propia vigente, https://www.inravision.gov.co/quienes-somos/quienes-somos (fechada el 30-05-2023): «es una sociedad entre entidades públicas, descentralizada indirecta, con régimen de Empresa Industrial y Comercial del Estado».
- AVISO: el resumen del buscador dice que notas del normograma de MinTIC atribuyen al Consejo de Estado (sentencia del 27-01-2011, exp. 2005-00030-01) la nulidad del Decreto 3525. NO lo verifiqué en el texto de la sentencia.
- NIVEL: registro externo / declaración del propio medio.

### OBJECIÓN 2 — El hueco de nivel 1 «no se sabe quién lo dirige» ya se puede cerrar
- QUÉ AFIRMA LA FICHA: «EL HUECO, Y ES EL QUE MÁS PESA: no se sabe quién lo dirige hoy».
- POR QUÉ:
  (a) La gerente es Ángela María Mora Soto, desde agosto de 2026. Primaria: RTVC Noticias, 14-08-2026: «Con la llegada de Ángela María Mora Soto a la gerencia, Inravisión arranca un ciclo…» (https://www.rtvcnoticias.com/actualidad/inravision/sistema-medios-publicos-impulsara-la-cultura-el-deporte-y-las-regiones). También la nota del 31-08-2026 citada arriba.
  (b) Quién la nombró y cuándo. Solo tengo fuente secundaria: Pulzo, 2026-08-13, https://www.pulzo.com/nacion/angela-maria-mora-soto-es-nombrada-gerente-de-inravision-claves-y-contexto-en-colombia-PP5274461A: «El gobierno encabezado por Abelardo de la Espriella hizo oficial el nombramiento de Ángela María Mora Soto como gerente de Inravisión […] de acuerdo con lo dispuesto en el Decreto 1196 del 12 de agosto de 2026, firmado por la ministra de Tecnologías de la Información y las Comunicaciones, Alexandra Falla Zerrate». La nota dice ser «curada con apoyo de inteligencia artificial», y el listado de Pulzo describe el mismo decreto como el que «formalizó el regreso de la histórica denominación Inravisión en marzo de 2026». Hay contradicción interna, así que el NÚMERO del decreto queda sin verificar. Lo busqué en dapre.presidencia.gov.co/normativa/normativa/ con dos variantes de nombre de archivo: 404.
  (c) Trayectoria, también de Pulzo (secundaria): «directora [de la ANTV] entre 2015 y 2018»; «asesoró jurídicamente al Departamento Administrativo de la Presidencia de la República entre 2018 y 2019»; en la JEP entre 2019 y 2023. No encontré militancia partidista declarada.
  (d) Otros relevos tras el 07-08-2026, todos con fuente secundaria: Andrea Carolina Holguín, directora de Señal Colombia (Pulzo, 2026-09-03, https://www.pulzo.com/entretenimiento/andrea-carolina-holguin-asume-direccion-de-senal-colombia-modernizacion-y-reto-digital-PP5292328A). En perfiles directivos de inravision.gov.co solo se lee, publicado el «18 de Septiembre de 2026», a «David Tinoco Rosales Cargo: Subgerente de Soporte Corporativo».
  (e) La fuente de la ficha está desactualizada: State Media Monitor (https://statemediamonitor.com/2025/03/radio-y-television-nacional-de-colombia-rtvc-sistema-de-medios-publicos/) sigue diciendo «Hollman Morris manager since April 2024 (still in post 2026)».
- NIVEL: propiedad/gobierno corporativo (primaria para el nombre, secundaria para el decreto).

### OBJECIÓN 3 — La afirmación central «Un mes después de la transición, la comprobación no se puede hacer» es falsa: ya se puede hacer y da OFICIALISMO
- QUÉ AFIRMA LA FICHA: que la asimetría a través del cambio «exige dos fotos, y de la segunda tenemos seis piezas sin una sola de política», y que la previsión del 2026-08-08 «no se puede ni confirmar ni desmentir».
- POR QUÉ: el archivo propio del medio tiene las dos fotos. El problema era la vía de ingesta, no el medio. Barrido de la sección «Gobierno» (119 piezas) más las secciones /politica, /politica/congreso, /actualidad/inravision y algunas piezas de la portada. Abajo, la voz de la casa con postura:

  ANTES del 07-08-2026: favorable al gobierno Petro (la voz de la casa presenta como hecho un logro del Gobierno o adopta su encuadre, sin una voz en contra):
   A1 2026-04-07 «El mayor aumento del salario mínimo en décadas no destruyó empleo en Colombia, según JP Morgan». Firma: RTVC Noticias. https://www.rtvcnoticias.com/economia/el-mayor-aumento-del-salario-minimo-en-decadas-no-destruyo-empleo-en-colombia-segun-jp — cierra: «podría fortalecer el argumento de que incrementos salariales ambiciosos y estabilidad laboral…». Clase: elogio al gobierno.
   A2 2026-04-30 «100 logros del gobierno Petro: menos pobreza, más empleo». Firma: Redacción Digital. https://www.rtvcnoticias.com/politica/gobierno/100-logros-del-gobierno-petro-menos-pobreza-mas-empleo. Clase: elogio.
   A3 2026-05-11 «Decisión del Consejo de Estado deja sin financiación a Colpensiones». Firma: Redacción Digital. https://www.rtvcnoticias.com/politica/gobierno/decision-consejo-estado-financiacion-colpensiones. Clase: adopta el encuadre del Gobierno contra un fallo judicial.
   A4 2026-05-18 «Petro supera el 50 % de imagen positiva en encuesta reciente». Firma: Redacción Digital. https://www.rtvcnoticias.com/politica/gobierno/petro-supera-el-50-de-imagen-positiva-en-encuesta-reciente. Clase: elogio.
   A5 2026-05-27 «Por primera vez, Colombia tiene más clase media que pobres». Firma: Redacción Digital. https://www.rtvcnoticias.com/politica/gobierno/por-primera-vez-colombia-tiene-mas-clase-media-que-pobres. Clase: elogio (titular en voz propia).
   A6 2026-05-29 «Revolución aeroportuaria: 19,6 millones de pasajeros en 4 meses». Firma: Redacción Digital. https://www.rtvcnoticias.com/politica/gobierno/revolucion-aeroportuaria-19-millones-de-pasajeros-en-4-meses. Clase: elogio.
   A7 2026-06-28 «Menos pobres y más empleo: Petro destacó logros de su gobierno». Firma: Redacción Digital. https://www.rtvcnoticias.com/politica/gobierno/menos-pobres-y-mas-empleo-petro-destaco-logros-de-su-gobierno. Clase: elogio.
   Encuadre asimétrico entre candidatos en la misma etapa (voz de la casa que amplifica ataques a De la Espriella sin su réplica):
   A8 2026-05-13 «Petro Pide a Paloma Valencia y De la Espriella retirar demandas». Redacción Digital. https://www.rtvcnoticias.com/politica/gobierno/petro-pide-paloma-valencia-de-la-espriella-retirar-demandas
   A9 2026-06-29 «Pdte. Petro agradece a Karol G por su carta a De la Espriella». Redacción Digital. https://www.rtvcnoticias.com/politica/gobierno/pdte-petro-agradece-karol-g-por-su-carta-de-la-espriella
   A10 2026-06-30 «Iván Cepeda llama a la desobediencia civil y pacífica si De la Espriella no aclara presunta subordinación a EE.UU. …». RTVC Noticias. https://www.rtvcnoticias.com/politica/ivan-cepeda-anuncia-posible-desobediencia-civil-contra-abelardo-de-la-espriella

  DESPUÉS del 07-08-2026: favorable o acrítica con el gobierno De la Espriella (anuncios oficiales reproducidos con el titular del Gobierno, sin voces en contra):
   D1 2026-08-14 «Chocó tendrá prioridad en la reconstrucción tras el terremoto, anuncia presidente De La Espriella». RTVC Noticias. https://www.rtvcnoticias.com/politica/gobierno/choco-tendra-prioridad-en-la-reconstruccion-tras-el-terremoto
   D2 2026-09-28 «Gobierno anuncia conversaciones con el FMI ante el deterioro recibido de las finanzas públicas». RTVC Noticias. https://www.rtvcnoticias.com/politica/gobierno/gobierno-anuncia-conversaciones-con-el-fmi-ante-el-deterioro-recibido-de-las — el titular hace suya, en voz propia, la tesis del Gobierno sobre la herencia de Petro. Clase: adopta el encuadre del Gobierno.
   D3 2026-10-05 «“La seguridad tiene rostro”: presidente De La Espriella anuncia Fuerza Urano con más de mil hombres». RTVC Noticias. https://www.rtvcnoticias.com/politica/gobierno/de-la-espriella-anuncia-fuerza-urano-con-mas-de-mil-hombres
   D4 2026-10-05 «Gobierno inaugura en Montería nuevo estadio de béisbol y sóftbol: "mucho más que un lugar para hacer deporte"». RTVC Noticias. https://www.rtvcnoticias.com/politica/gobierno/gobierno-inaugura-en-monteria-nuevo-estadio-de-beisbol-y-softbol
   D5 2026-10-06 «Presidente De La Espriella plantea un Plan Nacional de Desarrollo con obras, empleo e inversión para las regiones». RTVC Noticias. https://www.rtvcnoticias.com/politica/gobierno/de-la-espriella-plantea-un-plan-nacional-de-desarrollo-con-inversion-para-las
   D6 2026-10-07 «Gobierno anuncia fondo de $1 billón para reconstrucción…». RTVC Noticias. https://www.rtvcnoticias.com/politica/gobierno/gobierno-anuncia-fondo-de-1-billon-para-reconstruccion-y-medidas-para-enfrentar
   D7 2026-10-08 «Presidente De La Espriella ordena plan de austeridad…». RTVC Noticias. https://www.rtvcnoticias.com/politica/gobierno/presidente-de-la-espriella-ordena-plan-de-austeridad-restringe-viajes-y
   D8 2026-10-10 «Gobierno propone agilizar licencias ambientales y consultas previas…». RTVC Noticias. https://www.rtvcnoticias.com/economia/gobierno-propone-agilizar-licencias-ambientales-y-consultas-previas-para-destrabar-grandes — inserta el tuit del ministro («Esta es una de las noticias económicas más importantes de los últimos años!») y no recoge a ninguna comunidad étnica ni a ninguna voz crítica (solo una aclaración propia: «el anuncio no significa que los proyectos queden automáticamente autorizados»).
   Voz INSTITUCIONAL de la casa tras el cambio, que adopta el lema y el relato del nuevo Gobierno:
   D9 2026-08-22 «Usaron la plata de la educación para pagar propaganda». Firma: RTVC Noticias. https://www.rtvcnoticias.com/actualidad/inravision/usaron-la-plata-de-la-educacion-para-pagar-propaganda
   D10 2026-09-03 «Inravisión, Sistema de Medios Públicos ordena cese de emisión de cuatro emisoras de paz que operaban clandestinamente». RTVC Noticias. https://www.rtvcnoticias.com/actualidad/inravision/inravision-sistema-de-medios-publicos-ordena-cese-de-emision-de-cuatro-0 — «el acta de dicha reunión no fue firmada por los dos delegados del gobierno anterior…».
   D11 2026-09-10 «RTVC avanza en la transformación del Sistema de Medios Públicos». RTVC Noticias. https://www.rtvcnoticias.com/actualidad/rtvc/rtvc-avanza-en-la-transformacion-del-sistema-de-medios-publicos — «En la Patria Milagro comienza una nueva etapa para RTVC». «Patria Milagro» es el lema del Gobierno: el mismo medio titula el 13-09 «Los cinco motores con los que el Gobierno De la Espriella busca construir la Patria Milagro».
   Simetría institucional del lado anterior: 2025-12-07 «Pueblo Nasa reconoce al gerente de RTVC…» (RTVC Noticias, https://www.rtvcnoticias.com/actualidad/rtvc/pueblo-nasa-reconoce-al-gerente-de-rtvc-en-historica-cumbre-que-reune-206), que elogia al gerente que había nombrado Petro.

  CONTRAPESOS (voz de la casa crítica con el gobierno de turno):
   - Antes: ninguno en voz de la casa en las 119 piezas de «Gobierno». Con firma personal, 2026-06-05 «Carlos Carrillo renuncia a la UNGRD tras suspensión de la Procuraduría» (https://www.rtvcnoticias.com/politica/gobierno/carlos-carrillo-renuncia-la-ungrd-tras-suspension-de-la-procuraduria), que es fiscalización y no cuenta.
   - Después: ninguno. 2026-08-14 «José Manuel Restrepo desmiente versión…» reproduce un desmentido del propio Gobierno.

  RECUENTO: 7 piezas con postura favorable a Petro antes (A1–A7) y 0 críticas, más 3 de encuadre asimétrico entre candidatos (A8–A10). Después, 8 favorables o acríticas con De la Espriella (D1–D8) más 3 institucionales (D9–D11), y 0 críticas. Hay ≥10 piezas con postura y ≥3 por lado, y la razón es mayor que 3:1 en CADA lado… pero a favor de quien gobierna en cada momento.
  CONCLUSIÓN SEGÚN LA REGLA 7 Y EL POLO FIJO: elogia a Petro antes y a De la Espriella después. Es OFICIALISMO, no orientación. La previsión del 2026-08-08 («cubrir la actualidad desde una posición oficialista con el nuevo gobierno») queda CONFIRMADA por el archivo propio del medio.
  Inferencia mía, que no es un hecho: el −0,35 medía el oficialismo de la etapa Petro, no una posición fija en el eje. Con el polo fijo, ese número no se sostiene como «orientación», y moverlo a la derecha por la etapa De la Espriella sería repetir el error.
  LIMITACIONES: la clasificación «con postura» es mía. Las piezas posteriores al cambio son sobre todo transcripción de anuncios, una postura más débil que los titulares celebratorios de antes. Después no hay campaña, así que no se puede reproducir el encuadre entre candidatos. Y el volumen político cae mucho tras el cierre de la franja informativa: 88 piezas de «Gobierno» antes del cambio en el barrido y 31 después.
- NIVEL: hecho editorial de los últimos 12 meses, voz de la casa con barrido reproducible.

### OBJECIÓN 4 — Falta el registro externo (nivel 3) que documenta la «primera foto»: la MOE de la Unión Europea
- QUÉ AFIRMA LA FICHA: no cita ningún registro externo sobre la conducta del medio. Su único nivel 3 posible es State Media Monitor, que habla de gobernanza.
- POR QUÉ: la Misión de Observación Electoral de la UE midió los informativos de Señal Colombia y Radio Nacional de Colombia, los canales donde se emite RTVC Noticias.
  · Declaración preliminar de la primera vuelta, 2 de junio de 2026: https://www.eeas.europa.eu/sites/default/files/2026/documents/Declaracio%CC%81n%20Preliminar%20primera%20vuelta%20MOE%20UE%20Colombia%202026_0.pdf — «Los medios estatales, que tienen una mayor obligación de neutralidad y equilibrio en su cobertura, favorecieron en su mayoría al presidente, al Gobierno y a Cepeda, mientras que dedicaron mucho menos tiempo a De la Espriella y a Valencia, a menudo en tono negativo». Nota 11: «seguimiento cuantitativo de cuatro medios de comunicación privados (Blu Radio, Caracol Radio, Caracol TV y RCN TV) y dos medios estatales (el canal de televisión Señal Colombia y Radio Nacional de Colombia)», entre el 30 de abril y el 30 de mayo.
  · Declaración de la segunda vuelta, 23 de junio de 2026: https://www.eeas.europa.eu/sites/default/files/2026/documents/MOE%20UE%20DP%20Segunda%20vuelta%20Colombia%202026%20-23%20JUN.pdf — «los medios de comunicación estatales […] ampliaron ligeramente la cobertura de Cepeda, en su mayor parte de forma neutral, mientras que a De la Espriella se le dedicó menos tiempo y, principalmente, en un tono negativo. Al igual que en la primera vuelta, los medios de comunicación estatales favorecieron al presidente y a su Gobierno en su cobertura».
  Esto es encuadre asimétrico entre candidatos, que la regla del polo fijo NO excluye. Pero junto con la objeción 3 lo que muestra es un medio alineado con el gobierno que nombra a su gerente, y no una posición propia que sobreviva al cambio.
- NIVEL: registro externo.

### OBJECIÓN 5 — La ficha interpreta mal la pieza de la rectificación: no es «el Estado rectificando a un medio privado»
- QUÉ AFIRMA LA FICHA: «"Sistema de Medios Públicos rectifica información sobre La Silla Vacía" es el medio del Estado rectificando públicamente a un medio privado […] Rectificar es además legítimo y del oficio. Se anota porque está, no porque diga algo».
- POR QUÉ: es RTVC rectificando SU PROPIA información, por orden judicial. La pieza, firmada «RTVC Noticias» el 2026-08-31 (https://www.rtvcnoticias.com/actualidad/inravision/rectificacion), dice: «en cumplimiento de la sentencia de segunda instancia proferida el treinta (30) de julio de 2026 por el Tribunal Superior de Bogotá, dentro de la acción de tutela instaurada por Juanita León García en representación de la Fundación La Silla Vacía, se permite rectificar lo siguiente». Según Pulzo (secundaria, 2026-07-31, https://www.pulzo.com/nacion/tribunal-superior-de-bogota-ordena-rectificacion-a-rtvc-y-revista-raya-por-caso-proyecto-jupiter-PP5262195A), el Tribunal halló que RTVC y Revista Raya asociaron a La Silla Vacía con un supuesto «Proyecto Júpiter» para «deslegitimar al Gobierno Nacional» y «señaló la falta de veracidad e imparcialidad». No he leído la sentencia: el texto entre comillas es de Pulzo. Es una SENTENCIA sobre la conducta editorial de la etapa Petro, a favor del Gobierno y contra un medio crítico. Tiene más peso que «una pieza que no dice nada».
- NIVEL: registro externo (sentencia) y hecho editorial de los últimos 12 meses.

### OBJECIÓN 6 — El nivel 2 de la ficha está obsoleto y su «medio mudo» no se sostiene
- QUÉ AFIRMA LA FICHA: «SEIS PIEZAS, Y NINGUNA POLÍTICA»; «Lleva ocho días sin entrar una sola pieza»; «Un lector que entre a DobleFoco hoy no encuentra al medio público por ninguna parte».
- POR QUÉ: la conducta medida del propio envío (2026-08-31 → 2026-10-10) da 214 artículos, 59 dentro de alguna historia y 66 historias. Según la regla del envío, «la buena es la de aquí arriba». El sitio publica pieza política firmada «RTVC Noticias» hasta el mismo 2026-10-10 (D8), y la sección «Gobierno» tiene 31 piezas posteriores al 07-08-2026. Lo que la ficha dice del rss.xml sí se confirma hoy: su pubDate más reciente es «Sat, 30 May 2026» y la siguiente salta a «Wed, 26 Jun 2024». El silencio era de la vía de ingesta, no del medio.
- NIVEL: conducta observable.

### OBJECIÓN 7 — La forma jurídica que da la ficha no coincide con el registro mercantil vigente
- QUÉ AFIRMA LA FICHA: «Sociedad entre entidades públicas del orden nacional, constituida en octubre de 2004 y sujeta al régimen de las Empresas Industriales y Comerciales del Estado».
- POR QUÉ: el RUES (actualizado el 2026-08-21) inscribe a la entidad como «INRAVISIÓN - SISTEMA DE MEDIOS PÚBLICOS DEL ESTADO COLOMBIANO S.A.S» con «organizacion_juridica":"SOCIEDADES POR ACCIONES SIMPLIFICADAS SAS"», y el propio medio se llama «S.A.S.» en el comunicado del 15-09-2026. En SECOP II el mismo NIT aparece con dos nombres: «INRAVISIÓN» (14 163 contratos, el último firmado el 2026-07-27) e «INRAVISIÓN - SISTEMA DE MEDIOS PÚBLICOS DEL ESTADO COLOMBIANO S.A.S» (1 755 contratos, el último el 2026-10-07).
  Consulta: https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=nombre_entidad,count(id_contrato) as n,min(fecha_de_firma) as primera,max(fecha_de_firma) as ultima&$where=nit_entidad='900002583'&$group=nombre_entidad
  No mueve el eje, pero el nivel 1 debe citar el registro de 2026 y declarar la tensión entre «sociedad entre entidades públicas» y «S.A.S.». No sé si cambió la forma o si el RUES la clasifica así: no encontré el acto que lo explique.
- NIVEL: propiedad / registro externo.

======================================================================
## LO QUE NO PUDE VERIFICAR
- El número y la fecha del decreto que nombra a la gerente («Decreto 1196 del 12 de agosto de 2026»): solo en Pulzo (curado con IA y contradictorio en su listado). Busqué en dapre.presidencia.gov.co/normativa/normativa/ con dos variantes de nombre (404) y en inravision.gov.co/quienes-somos/decretos, donde la lista termina en 2023.
- El director de noticias tras el 07-08-2026. Busqué en inravision.gov.co (perfiles directivos, directorio, funcionarios), en /actualidad/inravision de rtvcnoticias y con el buscador: nada posterior a William Parra (06-08-2026).
- Que el Consejo de Estado anulara el Decreto 3525 de 2004 (sentencia del 27-01-2011): solo en un resumen del buscador sobre notas del normograma de MinTIC. No leí la sentencia.
- La contratación por Inravisión de dos creadoras de contenido de la campaña de De la Espriella (Pulzo, 2026-10-08, https://www.pulzo.com/nacion/quienes-influencers-que-llegan-inravision-rtvc-con-espriella-PP5325472, que cita a Noticias Caracol). En SECOP II hay contratos de «contenidos del ecosistema digital» firmados el 2026-09-23 (INRA-CPS-1635-2026, 1636 y 1637, cada uno por 15 906 053,01 COP) y una «estrategia digital integral» del 2026-09-02 (INRA-CPS-1617-2026). No vinculé contratistas con la campaña ni publico nombres de personas naturales.
  Consulta: https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=fecha_de_firma,referencia_del_contrato,descripcion_del_proceso,valor_del_contrato&$where=nit_entidad='900002583' AND fecha_de_firma>='2026-08-07'
- El estudio de La Silla Vacía sobre la cobertura de Cepeda (788 notas). Solo lo conozco por Pulzo (2026-07-10, https://www.pulzo.com/nacion/rtvc-fue-maquina-propaganda-cepeda-petro-silla-vacia-PP5243169). No consulté lasillavacia.com porque está prohibido por las reglas.
- La sección /categorias/opinion de rtvcnoticias.com descargó sin enlaces de artículos que pudiera extraer. No encontré editoriales firmados por la casa como tales.

## LO QUE FALTA
1. En el nivel 1: el nombre de la gerente (Ángela María Mora Soto), quién la nombró (el Gobierno De la Espriella, vía MinTIC) y el RUES de 2026 con razón social y forma jurídica.
2. La MOE UE (02-06 y 23-06-2026) como registro externo de la etapa anterior.
3. La sentencia del Tribunal Superior de Bogotá (30-07-2026) y la rectificación que ordenó, leídas como lo que son.
4. Los hechos estructurales de agosto y septiembre de 2026: cierre de la «franja noticiosa y de opinión» (decidido el 15-08, publicado el 16-08: https://www.rtvcnoticias.com/actualidad/inravision/se-acaba-el-aparato-de-propaganda-en-el-sistema-de-medios-publicos), «auditoría editorial» anunciada por MinTIC (Pulzo, 2026-08-23, https://www.pulzo.com/nacion/cambios-medios-publicos-rtvc-decision-gobierno-espriella-PP5280299: «se hará una auditoría editorial del material emitido […] retirar aquellos que, según la entidad, tengan sesgos o intereses políticos»), terminación de contratos periodísticos (10-09) y acciones ante la SIC y la Fiscalía contra excontratistas que montaron «RTC Noticias» (15-09). Cada cambio de gobierno reconfigura la redacción. Eso es estructura vigente.
5. El barrido de la objeción 3, con sus dos fotos, en lugar de las seis piezas de Google News.

## EVIDENCIA QUE NO MUEVE EL NÚMERO
- El cambio de nombre a Inravisión sigue vigente (redirección comprobada el 2026-10-10). No dice nada del eje.
- Estructura de dependencia, igual con los dos gobiernos: State Media Monitor (consultado el 2026-10-10) dice «it has no binding editorial-independence safeguard» y «the government appoints its director, the "manager" (gerente)». La Resolución RTVC 0461 de 2016 (normograma de MinTIC) confirma que el gerente es «nombrado en el cargo mediante Decreto número 1222 del 4 de junio de 2015», es decir, que lo nombra el Ejecutivo por decreto.
- Servicio a la Presidencia con los dos gobiernos: según RTVC Noticias del 22-08-2026 (D9), un «Convenio Interadministrativo No. 390-2026, suscrito con el Departamento Administrativo de la Presidencia (Dapre)» en la etapa Petro. En SECOP II, el 2026-09-28, RTVC-CD-1644-2026 para «toma de fotografía […] del Departamento Administrativo de la Presidencia de la República» en la etapa De la Espriella. Es continuidad estructural, no un giro.
- Antes del cambio, la casa se ofreció a transmitir un debate entre los dos candidatos (2026-06-06, firma personal: https://www.rtvcnoticias.com/actualidad/inravision/inravision-propone-transmitir-debate-presidencial-entre-ivan-cepeda-y). Es conducta de servicio público, con los dos candidatos.
- Mucha producción posterior es servicio (terremoto, incendios con la UNGRD, El Niño, deportes): por ejemplo, 2026-10-06 «UNGRD activa plan nacional…» (RTVC Noticias). No da signo.
- Antes del cambio, el sitio sí publicaba sobre investigaciones a la gerencia de Morris, pero solo en prensa ajena (Pulzo). En el barrido de la sección «Gobierno» de RTVC no encontré piezas propias sobre eso, y eso tampoco mueve el número por sí solo.

## SIN OBJECIÓN
No aplica: hay objeciones arriba. Aclaración: estoy DE ACUERDO con la parte de la ficha que dice que el −0,35 no se puede firmar. La objeción 3 refuerza esa conclusión por otra vía (es oficialismo, no orientación). Ese acuerdo no debe usarse como aval.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** El revisor no copió cédulas, teléfonos ni direcciones de personas naturales, ni la nacionalidad, el origen étnico o el lugar de nacimiento de nadie. Las cifras largas del texto son el NIT de la sociedad, la matrícula mercantil, cuantías y referencias de contrato. Sus consultas a datos.gov.co llevan `$select` con campos que no son documentos de identidad, y se comprobaron:
- RUES: cámara, matrícula, razón social, forma, estado, renovación y actualización;
- SECOP II: entidad y recuento, o fecha, referencia, objeto y valor.

No enlaza procesos de SECOP II. Las personas que nombra lo están por su cargo público o por su papel en un hecho público: la gerente, la ministra TIC, el exgerente, el exdirector del Sistema Informativo, la directora de la fundación que interpuso la tutela (tal como la nombra la propia rectificación del medio) y funcionarios del Gobierno. La trayectoria profesional de la gerente que cita de Pulzo no es un dato de los que excluye la regla. **Esta resolución no nombra a ningún contratista persona natural**, tampoco a los «dos excontratistas» de la denuncia del 15-09.

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada (2026-10-10):
  - `www.rtvcnoticias.com` e `inravision.gov.co`: el de Drupal por defecto, con `User-agent: *`. Excluyen `/core/`, `/profiles/`, `/node/add/` y **`/search/`**: el buscador del sitio no se usó;
  - `funcionpublica.gov.co`: `Disallow:` vacío;
  - `statemediamonitor.com`: solo `/wp-admin/`;
  - `pulzo.com`: reglas para `*` y para robots con nombre, ninguno de Anthropic;
  - `infobae.com`: `User-agent: *` sin exclusiones;
  - `datos.gov.co`: exclusiones de `/browse`, nada sobre `/resource`;
  - `normograma.mintic.gov.co`: 404, sin restricciones.
  - **`www.mintic.gov.co` devolvió 403 al pedir el robots.txt: no se consultó el sitio de MinTIC.** `consejodeestado.gov.co` dio 404 al robots, pero no se buscó la sentencia allí (ver la 1).
  - No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. Las búsquedas web se hicieron excluyendo esos dominios.
- **Descargas**, en crudo, con `curl -sL --ssl-no-revoke` y UA de Chrome 126:
  - **622 piezas únicas de rtvcnoticias.com** en la ventana 2025-10-10 → 2026-10-10: la sección «Gobierno» entera (páginas 0-70), `/actualidad/rtvc` y `/actualidad/inravision` (0-12), `/politica` (0-11), `/categorias/opinion` y las piezas sueltas que cita el revisor. La fecha y la firma salen del JSON-LD;
  - las normas en el normograma de MinTIC (Decreto 3912 de 2004, Decreto 3525 de 2004 y el archivo `js/decreto_3525_2004.js`, con sus notas de vigencia; Resolución RTVC 0461 de 2016) y el concepto de Función Pública `i=82339`;
  - las dos declaraciones de la MOE UE (PDF, leídas con `pdftotext`);
  - State Media Monitor (con el UA de Chrome dio 403; con el de Firefox, 200);
  - inravision.gov.co (portada, «Quiénes somos», perfiles directivos);
  - cinco notas de Pulzo y una de Infobae;
  - `/rss.xml` y `/noticias/rss.xml`.
- **Registros**, en datos.gov.co, por NIT con igualdad exacta, **sin y con dígito de verificación** (`900002583` y `9000025836`):
  - RUES (`c82u-588k`): 1 fila con el NIT sin DV y 0 con el DV pegado;
  - SECOP II (`jbjy-vk9h`), como entidad contratante (`nit_entidad`) y como contratista (`documento_proveedor`): el NIT con DV da 0 filas;
  - **SECOP I (`f789-7hwg`), que el revisor no consultó: 116 filas con el NIT sin DV y 5 más con el NIT con DV.**
- **Buscador web**: 2 consultas, una por el decreto de nombramiento y otra por la «auditoría editorial». De él no se cita nada que no se haya descargado y leído.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | La fuente «rota» carga, pero es otra norma. Sustituta: Decreto 3912 de 2004 | sí | sí, y la nulidad ya consta | **Aceptada y completada.** `i=82339` da 200 y es el «Concepto Sala de Consulta C.E. 00101 de 2016». La cita del Decreto 3912 es literal. **La nulidad del Decreto 3525 de 2004 consta en el normograma oficial de MinTIC**: Consejo de Estado, Sección Primera, sentencia del 27-01-2011, exp. 2005-00030-01. No se leyó la sentencia. La sociedad se protocolizó por la escritura 3138 del 28-10-2004 y sigue activa en el RUES |
| 2 | El hueco «no se sabe quién lo dirige» ya se cierra: Ángela María Mora Soto, nombrada por el Gobierno De la Espriella | sí | sí | **Aceptada.** El nombre y el cargo constan en fuente primaria (RTVC, 14-08 y 31-08). El «Decreto 1196 de 2026» lo dan ahora **dos** secundarias, Pulzo e Infobae (13-08-2026, sin marca de curado con IA), pero sigue sin primaria. El cargo es **gerente**, no «director general». No consta director de noticias, y desde el 07-10 hay un informativo nuevo, «RTVC Ahora». State Media Monitor está desactualizado (cita literal) |
| 3 | La comprobación del cambio ya se puede hacer, y da oficialismo | sí | sí: barrido rehecho y ampliado (622 piezas, 12 meses) | **Aceptada en la conclusión y corregida en el recuento.** Ver `revision-externa/barridos/rtvc.md`. Nivel A: 18 piezas con postura antes y 4 después; con titulares de periodistas de plantilla, 34 y 8. En direcciones opuestas: **ninguna dirección cumple «3 a cada lado y 3 a 1».** D1 y D3-D8 son transcripción atribuida, no elogio, igual que cientos de piezas de la etapa Petro |
| 4 | Falta el registro externo: MOE UE (02-06 y 23-06-2026) | sí | sí | **Aceptada.** Las dos citas son literales. Precisión: la MOE midió **Señal Colombia y Radio Nacional**, los canales del sistema, no el sitio, del 30-04 al 30-05 y del 01-06 al 20-06. Y lo describe como favorecer «al presidente, al Gobierno y a Cepeda»: oficialismo con candidato |
| 5 | La rectificación no es «el Estado rectificando a un medio privado», sino RTVC rectificando lo suyo por una tutela | sí | sí | **Aceptada.** La cita es literal. La rectificación se refiere a información «publicada los días 19, 21 y 26 de abril de 2026 por Inravisión», y dice que «Señal Investigativa» dejó de emitirse el 06-08-2026. Lo que el revisor toma de Pulzo sobre la sentencia sale de una nota marcada «curada con apoyo de inteligencia artificial»: no entra como hecho |
| 6 | El nivel 2 de la ficha está obsoleto; el silencio era de la vía de ingesta | sí | sí | **Aceptada.** `/rss.xml` sigue parado (30-05-2026 y luego 26-06-2024). `/noticias/rss.xml` está vivo (pieza del 10-10-2026). El registro usa esa vía desde el 2026-09-09, pero la ficha nunca se actualizó. Conducta medida vigente: 214 artículos, 59 en historias, 66 historias |
| 7 | La forma jurídica no coincide con el RUES | sí | sí | **Aceptada como tensión declarada.** RUES: «INRAVISIÓN - SISTEMA DE MEDIOS PÚBLICOS DEL ESTADO COLOMBIANO S.A.S», «SOCIEDADES POR ACCIONES SIMPLIFICADAS SAS», matrícula de 2004, renovada el 2026-03-30 y actualizada el 2026-08-21. SECOP II tiene **tres** nombres para el NIT. Ni el medio ni State Media Monitor lo explican como un cambio de naturaleza. No mueve el eje |

### Lo verificado, objeción por objeción

**1 · La norma de constitución.**
- `https://www.funcionpublica.gov.co/eva/gestornormativo/norma.php?i=82339` → 200. `<title>`: «Concepto Sala de Consulta C.E. 00101 de 2016 Consejo de Estado - Sala de Consulta y Servicio Civil - Gestor Normativo - Función Pública». **La ficha y `mediaOwnership.js` lo enlazan como «norma de constitución», y no lo es.** Que el envío dijera «fetch failed» fue un fallo de la descarga, no del enlace.
- **Decreto 3912 de 2004**, en el normograma de MinTIC, literal: «Que Radio Televisión Nacional de Colombia, RTVC, autorizada mediante Decreto número 3525 de 26 de octubre de 2004, es una sociedad entre entidades públicas, indirecta, del orden nacional, sometida al régimen de las Empresas Industriales y Comerciales del Estado».
- **Decreto 3525 de 2004**, en el mismo normograma. El encabezado dice «<NOTA DE VIGENCIA: Decreto declarado NULO>». La nota de vigencia (en `js/decreto_3525_2004.js`, que es lo que la página despliega) dice: «Decreto declarado NULO por el Consejo de Estado, Sección Primera, mediante Sentencia de 27 de enero de 2011, Expediente No. 2005-00030-01, Consejero Ponente Dr. Marco Antonio Velilla Moreno». Destaca el motivo: autorizar que ADPOSTAL participara en la nueva entidad «quebrantó lo dispuesto en el artículo 49 [de la Ley 489 de 1998] … y en el Decreto 2124 de 1992». Otra nota: «La creación de la sociedad … fue protocolizada legalmente mediante Escritura Pública No. 3138 del 28 de octubre de 2004, de la Notaría 34 de Bogotá».
  - **Lo que esto prueba:** que la compilación oficial del sector registra la nulidad.
  - **Lo que no prueba:** qué efectos tuvo sobre la sociedad. Sigue matriculada y activa (ver la 7). La sentencia no se leyó.
- **Declaración propia vigente**, inravision.gov.co/quienes-somos/quienes-somos (fechada el «30 de Mayo de 2023»), literal: «es una sociedad entre entidades públicas, descentralizada indirecta, con régimen de Empresa Industrial y Comercial del Estado».

**2 · Quién la dirige.**
- RTVC Noticias, 2026-08-14 (firma personal; sección institucional): «Con la llegada de Ángela María Mora Soto a la gerencia, Inravisión arranca un ciclo…». Literal salvo las etiquetas `<strong>`.
- RTVC Noticias, 2026-08-31, firma «RTVC Noticias»: «Por instrucciones de la Gerente, Angela María Mora Soto, Inravisión – Sistema de Medios Públicos mantendrá accesible esta rectificación…» (literal).
- **El decreto**, solo en secundarias:
  - Pulzo (2026-08-13): «de acuerdo con lo dispuesto en el Decreto 1196 del 12 de agosto de 2026, firmado por la ministra de Tecnologías de la Información y las Comunicaciones, Alexandra Falla Zerrate». La nota lleva «Este artículo fue curado con apoyo de inteligencia artificial».
  - Infobae (2026-08-13, firmada, sin esa marca), literal: «una transición que ya quedó oficializada con el Decreto 1196 de 2026».
  - Dos secundarias concordantes. El número es **probable, no verificado**: falta el decreto mismo.
- **Que lo nombra el Ejecutivo** ya constaba como estructura. La Resolución RTVC 0461 de 2016 dice del gerente de entonces, literal: «nombrado en el cargo mediante Decreto número 1222 del 4 de junio de 2015». State Media Monitor, literal: «the government appoints its director, the "manager" (gerente)».
- **Director de noticias.** El último que consta es William Parra, «director del Sistema Informativo», en la pieza del 06-08-2026 (literal). Después no consta ninguno.
  - **Hecho nuevo, que el revisor no trae:** el 06-10-2026 el medio anunció «RTVC Ahora», «un nuevo informativo» que se estrenó el 07-10, «con emisiones cada hora … desde las 6:00 a. m. hasta las 6:00 p. m.» y «periodistas y equipos desplegados en diferentes territorios del país» (literal). **Hay redacción informativa otra vez desde hace tres días**, sin director nombrado.
- **State Media Monitor**, literal hoy: «Hollman Morris manager since April 2024 (still in post 2026)». Desactualizado.
- **Perfiles directivos de inravision.gov.co** (publicado el «18 de Septiembre de 2026»): solo un subgerente de Soporte Corporativo.

**3 · El barrido.** Está entero en `revision-externa/barridos/rtvc.md`. Resumen:
- **Universo:** 622 piezas únicas (573 antes, 49 después). Solo en «Gobierno» son 402 (375 y 27).
- **Con postura, en voz de la casa en sentido estricto (firma «RTVC Noticias» o «Redacción Digital»):**
  - **18 antes**: 14 elogios, 2 rótulos contra el candidato o el presidente electo de la derecha, y 2 piezas institucionales alineadas. Una es «¡Atención! RTVC rechaza amenazas intervencionistas de Trump contra Colombia e invita a la movilización por la soberanía nacional de este miércoles» (2026-01-06), el mismo día en que el Gobierno «llama a movilización en respaldo al presidente Petro».
  - **4 después**: «… ante el deterioro recibido de las finanzas públicas» (28-09), «Usaron la plata de la educación para pagar propaganda» (22-08), el cese de las emisoras «que operaban clandestinamente» (03-09) y «En la Patria Milagro comienza una nueva etapa para RTVC» (10-09).
- **Con los titulares de periodistas de plantilla** se suman 16 antes y 4 después. Ahí está casi todo el encuadre de la segunda vuelta, por ejemplo:
  - «La ola Cepeda: artistas, académicos, movimientos sociales e influencers respaldan su llegada a la Casa de Nariño» (14-06);
  - «Abelardo de la Espriella: de abogado de Álex Saab y David Murcia a candidato presidencial» (11-06);
  - «El Instituto de Pensamiento Progresista desmiente el mito del "voto fusil" promovido por la ultraderecha» (23-06).

  Y después:
  - «Se acaba el aparato de propaganda en el Sistema de Medios Públicos de Colombia» (16-08);
  - «Los cinco motores con los que el Gobierno De la Espriella busca construir la Patria Milagro» (13-09);
  - «Gobierno anterior dejó sin un peso el Sistema de Medios Públicos» (25-09).
- **Contrapesos:** 2 parciales antes (las suspensiones de la Procuraduría a funcionarios del Gobierno Petro, 02-06 y 05-06) y **0 después**. La oposición desaparece del archivo después del 07-08: ninguna de las 49 piezas posteriores trata de Cepeda ni del Pacto Histórico.
- **Lo que no suma y se declara:** la transcripción del Ejecutivo. En «Gobierno», el Ejecutivo es el sujeto del titular en el 85 % de las piezas antes y en el 63 % después.
- **La regla no se activa en ninguna dirección.** Hacia la izquierda hay 34 piezas antes y 0 después; hacia la derecha, 0 antes y 8 después. Ninguna dirección tiene 3 piezas a cada lado. Es la conducta que el polo fijo describe como medir al gobierno y no al medio.

**4 · La MOE UE.**
- 2 de junio, literal: «Los medios estatales, que tienen una mayor obligación de neutralidad y equilibrio en su cobertura, favorecieron en su mayoría al presidente, al Gobierno y a Cepeda, mientras que dedicaron mucho menos tiempo a De la Espriella y a Valencia, a menudo en tono negativo». Nota 11: «dos medios estatales (el canal de televisión Señal Colombia y Radio Nacional de Colombia)», «Entre el 30 de abril y el 30 de mayo». Nota 10: Señal Colombia y Radio Nacional «informaron con frecuencia sobre las acusaciones del presidente Petro relativas a un posible fraude».
- 23 de junio, literal: «los medios de comunicación estatales … ampliaron ligeramente la cobertura de Cepeda, en su mayor parte de forma neutral, mientras que a De la Espriella se le dedicó menos tiempo y, principalmente, en un tono negativo. Al igual que en la primera vuelta, los medios de comunicación estatales favorecieron al presidente y a su Gobierno en su cobertura». Y algo que el revisor no cita: «el Consejo de Estado prohibió a Gustavo Petro utilizar los medios de comunicación estatales a favor o en contra de un movimiento político».
- **Es nivel 3 y es de la etapa anterior.** Mide los canales, no el sitio. No dice nada de cómo trata el medio al Gobierno entrante.

**5 · La rectificación.**
- 2026-08-31, firma «RTVC Noticias», literal: «en cumplimiento de la sentencia de segunda instancia proferida el treinta (30) de julio de 2026 por el Tribunal Superior de Bogotá, dentro de la acción de tutela…». Y: «A raíz de información publicada los días 19, 21 y 26 de abril de 2026 por Inravisión – Sistema de Medios Públicos, no está acreditada la existencia de una alianza … con el Proyecto Júpiter». Y: «Inravisión – Sistema de Medios Públicos dejó de emitir el programa Señal Investigativa el 6 de agosto de 2026».
- **Es una orden judicial sobre la conducta informativa de abril de 2026.** Nivel 3 (sentencia) por lo que ordena, que se lee en la rectificación. El razonamiento del Tribunal, solo por Pulzo con marca de curado con IA, no entra.

**6 · Nivel 2.** El envío del 2026-10-10 trae lo vigente: 40 días, 214 artículos, 59 en alguna historia, 66 historias, agenda propia del 14 %. Con 59 piezas en historias no sostiene nada, pero desmiente «seis piezas», «ocho días sin entrar» y «hoy no está en el sitio».

**7 · El registro mercantil.**
- RUES, consulta del 2026-10-10:
  `https://www.datos.gov.co/resource/c82u-588k.json?$select=camara_comercio,matricula,razon_social,organizacion_juridica,estado_matricula,fecha_matricula,ultimo_ano_renovado,fecha_renovacion,fecha_actualizacion&$where=numero_identificacion='900002583'`
  Devuelve: «BOGOTA», «1434314», «INRAVISIÓN - SISTEMA DE MEDIOS PÚBLICOS DEL ESTADO COLOMBIANO S.A.S», «SOCIEDADES POR ACCIONES SIMPLIFICADAS SAS», «ACTIVA», `fecha_matricula` «20041129», renovado en «2026» el «20260330» y actualizado el «2026/08/21».
- SECOP II, como entidad: «INRAVISIÓN» (14 163 contratos, del 2017-01-10 al 2026-07-27) y «INRAVISIÓN - SISTEMA DE MEDIOS PÚBLICOS DEL ESTADO COLOMBIANO S.A.S» (1 755, el último el 2026-10-07). Como contratista aparece además «RADIO TELEVISIÓN NACIONAL DE COLOMBIA RTVC S.A.S» (2 filas): **la etiqueta «S.A.S.» es anterior a 2026.**
- **En contra de leerlo como cambio de naturaleza:** State Media Monitor dice que el cambio de nombre de abril de 2026 «does not alter the entity's legal nature as a society between public entities». Y el propio medio, el 15-09-2026, se llama «RTVC - Sistema de Medios Públicos del Estado Colombiano S.A.S.» (literal).
- No hay un acto que explique la forma «SAS». **Tensión declarada; no mueve el eje.**

### Los hechos estructurales de agosto a octubre, en fuente primaria

Son lo más grave para la independencia y se verificaron en el sitio del propio medio:

| Fecha | Hecho | Fuente y cita literal |
|---|---|---|
| 15-08-2026 (publicado el 16-08) | **Cierre de la franja informativa y de opinión**, revisión de contenidos y de contratos | «Se acaba el aparato de propaganda en el Sistema de Medios Públicos de Colombia» (`/actualidad/inravision/se-acaba-el-aparato-de-propaganda-en-el-sistema-de-medios-publicos`, firma personal): «la ministra de Tecnologías de la Información y las Comunicaciones, Alexandra Falla, y la directora de Inravisión, Ángela Mora, definieron un plan de acción inmediato»; «Finalización de la franja noticiosa y de opinión en radio y televisión que hasta el 6 de agosto pasado ocupaba una parte significativa de los recursos humanos y técnicos»; «aproximadamente el 90 % de los recursos y del personal disponible destinados a actividades "periodísticas"»; «Revisión inmediata de los contenidos y formatos actualmente al aire»; «durante los días 6 y 7 de agosto se suscribieron 87 contratos por aproximadamente $4.000 millones»; «En la Patria Milagro se vivirá una nueva etapa para el Sistema de Medios Públicos» |
| 22-08-2026 | La casa acusa a la etapa anterior de usar contratos para «propaganda» | «Usaron la plata de la educación para pagar propaganda» (firma «RTVC Noticias»): «Increíble hallazgo en el Sistema de Medios Públicos». Cita el «Convenio Interadministrativo No. 390-2026, suscrito con el Departamento Administrativo de la Presidencia (Dapre)» |
| «Auditoría editorial» | **Solo en secundaria** | Pulzo (sin marca de IA): «El Ministerio señaló que se hará una auditoría editorial del material emitido, con el objetivo de revisar los contenidos y retirar aquellos que, según la entidad, tengan sesgos o intereses políticos». **En la fuente primaria del medio la medida se llama «revisión inmediata de los contenidos y formatos»**, y no dice «auditoría» ni «retirar». El sitio de MinTIC no se consultó (su robots.txt dio 403) |
| 10-09-2026 | **Terminación anticipada de contratos periodísticos** | «RTVC avanza en la transformación del Sistema de Medios Públicos» (firma «RTVC Noticias»): «decidió dar por terminados anticipadamente algunos contratos de prestación de servicios, entre los cuales se encuentran contratos relacionados con actividades periodísticas, de presentación y de gestión de contenidos digitales»; «el pasado 15 de agosto se dispuso suspender la franja noticiosa y de opinión que operó hasta el 6 de agosto»; «En la Patria Milagro comienza una nueva etapa para RTVC». **SECOP II no permite contarlos:** de los 384 contratos de 2026 con persona natural y objeto periodístico, 236 siguen «En ejecución» y 14 constan «terminado», con datos actualizados al 2026-10-08. El hecho descansa en el comunicado |
| 15-09-2026 | **Demanda ante la SIC y denuncia ante la Fiscalía** contra excontratistas | «RTVC - Sistema de Medios Públicos denuncia el uso no autorizado de la marca RTVC Noticias…» (firma «RTVC Noticias»): «presentó ante la Superintendencia de Industria y Comercio una demanda por infracción de derechos de propiedad industrial y, ante la Fiscalía General de la Nación, denuncia penal por la presunta comisión del delito de usurpación de derechos de propiedad industrial. Las acciones se dirigen contra dos excontratistas de la entidad». Pide a la SIC «el bloqueo del sitio web» y «la suspensión de las cuentas asociadas». Aquí no se nombra a nadie |
| 25-09-2026 | La casa sobre la etapa anterior | «Gobierno anterior dejó sin un peso el Sistema de Medios Públicos» (firma personal): «La administración anterior asumió compromisos relacionados con conciertos y eventos sin contar con recursos efectivamente disponibles» |
| 06/07-10-2026 | **Vuelve un informativo** | «‘RTVC Ahora’ donde pasa, estamos…» (firma «RTVC Noticias»): «Este miércoles 7 de octubre, el Sistema de Medios Públicos estrenará RTVC Ahora, un nuevo informativo» |

Leídos juntos:
- cada cambio de gobierno trae otra redacción;
- la nueva administración desmontó la anterior con el lenguaje del nuevo Gobierno («aparato de propaganda», «Patria Milagro»);
- acudió a la SIC y a la Fiscalía contra quienes siguieron informando fuera.

Es **estructura vigente de dependencia**, y no posición en el eje. State Media Monitor, literal: «it has no binding editorial-independence safeguard».

### Contratación pública (protocolo, 2026-10-07)

- **Como contratista** (lo que pide el protocolo):
  - **SECOP II** (`documento_proveedor='900002583'`): 265 contratos firmados por $389.681 millones desde el 2017-04-26, más 6 filas sin fecha de firma.
    - **En los últimos 12 meses, 14 contratos por $30.421.937.496**, todos con entidades del Gobierno nacional y **todos firmados antes del 07-08-2026**. El último es el DAPRE 555-26, del 2026-07-27, por $2.450 millones, en estado «terminado». **Después del 07-08, 0.**
    - Por entidad: DAPRE (3 contratos, $10.680 millones: 487-25, 390-296 y 555-26), Ministerio de Educación ($10.600 millones, 2026-01-29, «para difundir las acciones del Ministerio de Educación Nacional»), ICBF ($5.047 millones), MinTransporte ($1.390 millones, «central de medios»), MinHacienda ($857 millones), MinVivienda ($652 millones), UAPA ($600 millones), MinCIT ($297 millones), Superservicios ($150 millones), JEP (2 contratos, $103 millones) y Canal TRO ($47 millones).
  - **SECOP I** (`identificacion_del_contratista`, con y sin DV): 121 contratos por $107.651 millones, del 2017-10-23 al 2022-01-28. **0 en los últimos 12 meses.**
- **Consultas** (texto, con `$select`):
  - `https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=nombre_entidad,fecha_de_firma,referencia_del_contrato,estado_contrato,valor_del_contrato,descripcion_del_proceso&$where=documento_proveedor='900002583' AND fecha_de_firma>='2025-10-10'`
  - `https://www.datos.gov.co/resource/f789-7hwg.json?$select=count(*),sum(cuantia_contrato),min(fecha_de_firma_del_contrato),max(fecha_de_firma_del_contrato)&$where=identificacion_del_contratista in('900002583','9000025836')`
- **Como entidad contratante**, que no es la línea del protocolo pero se declara: 46 contratos firmados desde el 07-08-2026, 39 con personas naturales. Entre ellos, los de «gestión de contenidos del ecosistema digital» que cita el revisor (INRA-CPS-1635, 1636 y 1637-2026, del 2026-09-23, por $15.906.053,01 cada uno; INRA-CPS-1617-2026, del 2026-09-02, «estrategia digital integral»). También RTVC-CD-1644-2026 (2026-09-28), «toma de fotografía … del Departamento Administrativo de la Presidencia de la República». **La relación de servicio con la Presidencia sigue con el nuevo Gobierno.** La vinculación de contratistas con la campaña de De la Espriella (Pulzo, 2026-10-08) **no entra**: no consta en fuente que la acredite, y aquí no se nombra a personas naturales.

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. No entran como hecho, o se corrigen, estas partes:
- **Obj. 3: D1 y D3 a D8 como piezas «favorables o acríticas» que cuentan.** Son transcripción atribuida de anuncios del Gobierno. La precisión del responsable editorial del 2026-10-09 solo deja sumar elogios, disculpas y rótulos. Pasa lo mismo con A3 y A7 a A10 del lado anterior. La simetría no cambia.
- **Obj. 3: «119 piezas, 88 antes y 31 después».** Con el `datePublished` son 92 y 27. Y el universo de 12 meses es de 402 piezas en «Gobierno».
- **Hechos estructurales: la «auditoría editorial anunciada por MinTIC» como hecho.** Solo la da Pulzo. La primaria dice «revisión inmediata de los contenidos y formatos».
- **Obj. 2: el «Decreto 1196» como hecho.** Ahora lo dan dos secundarias. Sigue sin primaria.
- **Obj. 5: lo que «halló» el Tribunal**, citado de una nota de Pulzo curada con IA. Entra solo lo que dice la rectificación.
- **Obj. 1, aviso del revisor sobre la nulidad «no verificada»:** ya consta en la compilación oficial de MinTIC. Lo que sigue sin leerse es la sentencia.

### Fuentes falsas, inexistentes o deformadas

**Ninguna inexistente.** Todas las URL del revisor resuelven, y sus citas literales del medio, del RUES, de SECOP, de la MOE UE, del normograma y de State Media Monitor coinciden. Matices:
- Varios de sus titulares (A3, A5, A7, A8, A2) son el `<title>` SEO de la página, no el titular visible. Por ejemplo, A5 dice en el `<title>` «Por primera vez, Colombia tiene más clase media que pobres», y el titular dice «Pdte. Petro afirma que Colombia tiene más clase media que pobres por primera vez en su historia». Es literal de otro campo del mismo medio, no una invención. Donde cambia la clase, se anota.
- La nota de Pulzo sobre «Proyecto Júpiter» lleva la marca de curado con IA, y el revisor no la señaló en esa cita (sí en general).

**Errores de la propia ficha, para no repetirlos:**
- «Función Pública — norma de constitución» (`i=82339`): es un concepto de 2016 sobre recursos.
- Omite que el decreto que autorizó la sociedad (3525 de 2004) fue **declarado nulo** en 2011, y que el registro mercantil vigente la inscribe como **S.A.S.**
- «DESIGNA a su director general»: el cargo es **gerente**, nombrado por decreto.
- «no se sabe quién lo dirige hoy»: es Ángela María Mora Soto, gerente desde agosto de 2026.
- «Un mes después de la transición, la comprobación no se puede hacer» y «la previsión no se puede ni confirmar ni desmentir»: el archivo del medio la permite, y **la confirma**.
- Nivel 2 entero («SEIS PIEZAS», «ocho días sin entrar», «Hoy no está en el sitio»): obsoleto desde el 09-09, cuando entró `/noticias/rss.xml`.
- La rectificación «a un medio privado»: es la suya, por orden judicial, sobre lo que publicó en abril.
- **REFUTACIÓN, punto 2:** «si … su cobertura política resulta favorable al gobierno entrante de forma sostenida … el número se mueve hacia la derecha». **Contradice la regla del polo fijo**, que la propia ficha invoca en el ARGUMENTO 2: moverlo a la derecha por favorecer al entrante sería medir al gobierno.
- Faltan la línea de contratación pública, la MOE UE y los hechos de agosto a octubre.
- El medio no está en el centinela, y no puede estar por su buscador: `/search/` está excluido en su robots.txt.

**Lo que la ficha sí tenía bien, hoy:**
- es el único medio público nacional del catálogo;
- la gerencia la nombra el Ejecutivo y el control pasa por MinTIC;
- `rtvc.gov.co` redirige a `inravision.gov.co` (comprobado el 2026-10-10);
- `/rss.xml` está abandonado;
- y, sobre todo, que el −0,35 no se podía sostener.

**La decisión de nombre del 08-08 sale reforzada:** desde septiembre el propio medio vuelve a firmar como «RTVC - Sistema de Medios Públicos…» y llama «RTVC Ahora» a su informativo nuevo.

---

**Propuesta para la firma**

**Valor: de «sin medir» (`null`) a 0,00, con la nota de oficialismo. Sin firmar.**

Por qué ese valor y no otro, con el protocolo en la mano:
- **La previsión del 08-08 se confirma con las piezas delante, que es lo que la decisión «sin medir» esperaba.** La MINUTA del 2026-09-16 (punto 6), literal: «"Sin medir", re-medición a principios de octubre con ~30 días de su feed propio. La previsión del 08-08 queda como contraste — el responsable editorial espera oficialismo, y el número se moverá solo si las piezas lo dicen». El registro, literal: «SE RE-MIDE A PRINCIPIOS DE OCTUBRE … El número se moverá si las piezas lo dicen». La MINUTA del 05-10 la fijó «hacia el 15-10». El barrido de 12 meses dice oficialismo, a los dos lados.
- **El polo fijo dice qué hacer con el oficialismo.** «Izquierda y derecha son posiciones ideológicas. No son "a favor del gobierno" y "en contra del gobierno": si lo fueran, el mismo medio cambiaría de signo cada cuatro años sin haber cambiado de línea». Y su prueba: «Si el gobierno cambiara mañana y el medio mantuviera exactamente la misma conducta, ¿cambiaría su clasificación? Si la respuesta es sí, no se está midiendo al medio». Con RTVC, el gobierno cambió, el medio mantuvo la conducta (celebrar a quien manda), y un valor por dirección daría −0,35 antes y algo positivo ahora. **No hay posición fija que medir. El número que no mide al gobierno es el 0,00.**
- **La regla de evidencia editorial histórica lo permite y no da otro.** Su condición 3 («al menos 3 a cada lado … y una proporción de al menos 3 a 1 en la misma dirección») no se cumple para ninguna dirección. Y: «Lo que también hace: el 0,00 con evidencia. Un barrido que muestra la misma conducta con los dos gobiernos sostiene el 0,00 como evidencia». La conducta es la misma con los dos: postura a favor de quien gobierna y transcripción sin contraste.
- **«Orientación mixta» describe esto, aunque no lo parezca.** El contexto del protocolo lo dice: «"Orientación mixta" NO significa neutral, imparcial ni "sin línea" … Significa que la suya no se sitúa en el eje izquierda-derecha». La línea de RTVC es clarísima, pero es la de quien gobierne. La regla 2 apunta igual: «Ante la duda entre dos bandas, se elige la más cercana a la mixta».
- **Coherencia con el catálogo.** Los otros medios públicos están en 0,00 por la misma razón estructural:
  - Telemedellín: «su línea sigue al gobierno local de turno»;
  - Canal Capital: «su línea sigue al gobierno distrital de turno»;
  - Telecaribe;
  - Telecafé, decidido el 2026-10-10 (DECISIONES). La resolución de Telecafé propuso: «0,00, igual que los otros canales públicos del catálogo: su línea sigue a quien lo dirige».

  RTVC sería el primero en que eso **se ha medido** a los dos lados de un cambio de gobierno, y no solo supuesto.
- **El encuadre entre candidatos de la segunda vuelta** (nivel B y MOE UE) es lo único que el polo fijo no excluye, y es lo que más empuja hacia la izquierda. No lo hace por tres razones:
  - el candidato favorecido era el del Gobierno, y la MOE lo describe así («al presidente, al Gobierno y a Cepeda»);
  - **la regla del presente**: la redacción que lo produjo se desmontó entre el 15-08 y el 10-09 (franja cerrada, «Señal Investigativa» fuera del aire, contratos periodísticos terminados). La prueba («si ese hecho dejara de ser cierto mañana, ¿cambiaría la clasificación?») ya se cumplió, porque dejó de ser cierto;
  - lo que sobrevive es la dependencia, que produce oficialismo y no un polo.

  Se declara en CONTRA.
- **Lo que pesa en contra de mover ya, y es la alternativa**, del responsable editorial: el informativo nuevo («RTVC Ahora») tiene tres días. Si se quiere medir la redacción nueva y no la transición, cabe mantener «sin medir» hasta que tenga unos 30 días (hacia mediados de noviembre). **Recomendación: 0,00 ahora.** El «sin medir» se decidió porque no había material, y ya lo hay en los dos lados. Mantenerlo diría «no lo sabemos» de algo que el archivo ya muestra.

**`biasRationale` propuesto:** «Sistema de medios públicos nacional (Inravisión): el Gobierno nombra a su gerente por decreto y no hay salvaguarda vinculante de independencia editorial. Oficialista: su voz propia celebró al Gobierno Petro hasta el 06-08-2026 y al Gobierno De la Espriella desde el 07-08 (barrido de 622 piezas, 2026-10-10). Con el polo fijo eso no es una posición en el eje, y el 0,00 no dice que sea neutral: dice que su línea sigue al gobierno de turno. Ver fichas/rtvc.md.»

**Correcciones de hecho**

En `fichas/rtvc.md`:
1. **Cabecera**: valor «sin medir» → 0,00 propuesto, con la fecha y la referencia a este expediente. Hoy la cabecera dice «−0,35», que es anterior a la decisión del 16-09.
2. **Nivel 1, primer párrafo** → «Sistema de medios públicos nacional. Sociedad entre entidades públicas del orden nacional, sometida al régimen de las Empresas Industriales y Comerciales del Estado (Decreto 3912 de 2004; inravision.gov.co). Se protocolizó por la escritura pública 3138 del 28-10-2004. El decreto que autorizó su creación (3525 de 2004) fue declarado nulo por el Consejo de Estado el 27-01-2011, según el normograma de MinTIC. En el registro mercantil figura hoy como «INRAVISIÓN - SISTEMA DE MEDIOS PÚBLICOS DEL ESTADO COLOMBIANO S.A.S», sociedad por acciones simplificada, activa, renovada en 2026 (RUES, actualizado el 2026-08-21). No consta el acto que explique la forma SAS. El Gobierno nombra a su gerente por decreto, y el control pasa por MinTIC.»
3. **Nivel 1, gerente**, en lugar de «EL HUECO» → «Gerente: Ángela María Mora Soto, desde agosto de 2026, nombrada por el Gobierno De la Espriella (lo dice el propio medio el 14-08 y el 31-08; el «Decreto 1196 de 2026» lo dan Pulzo e Infobae, sin fuente primaria). No consta director de noticias desde el 07-08-2026. El último fue el director del Sistema Informativo de la etapa anterior, citado el 06-08. Desde el 07-10-2026 emite un informativo nuevo, «RTVC Ahora».»
4. **Fuentes del nivel 1**: quitar `i=82339`. Poner los decretos 3912 y 3525 de 2004 (normograma de MinTIC), la consulta RUES con `$select` y la pieza del 14-08-2026.
5. **«La previsión…»** → «Contraste, 2026-10-10: **la previsión se confirma.** Barrido de 12 meses (`revision-externa/barridos/rtvc.md`): postura en voz de la casa a favor del Gobierno Petro antes del 07-08 y a favor del Gobierno De la Espriella después, sin contrapesos después.»
6. **Nivel 2** → sustituir entero por las cifras del 2026-10-10 (40 días, 214 artículos, 59 en historias, 66 historias, agenda propia del 14 %), con la advertencia de que no sostienen nada. Y una línea sobre el cambio de vía: `/noticias/rss.xml` desde el 2026-09-09.
7. **«La sexta pide un párrafo…»** → «"Sistema de Medios Públicos rectifica información sobre La Silla Vacía" (31-08) es el medio rectificando lo que él mismo publicó el 19, 21 y 26 de abril de 2026, por una sentencia de tutela de segunda instancia del Tribunal Superior de Bogotá (30-07-2026). Es un registro judicial sobre su conducta informativa en la etapa anterior.»
8. **«LO QUE ES NUESTRO Y NO SUYO»**: los puntos 1, 2 y 4 pasan a historia de la ficha («resuelto el 2026-09-09»).
9. **ARGUMENTO**: sustituir por el razonamiento de arriba (polo fijo, condición 3 no cumplida, «el 0,00 con evidencia», regla 2, coherencia con los medios públicos).
10. **CONTRA**: añadir el encuadre entre candidatos de la segunda vuelta (nivel B y MOE UE) como el mejor caso a favor de un valor a la izquierda, con sus dos límites (candidato del Gobierno y redacción desmontada). Añadir también «el informativo nuevo tiene tres días».
11. **REFUTACIÓN**: quitar el punto 2 («se mueve hacia la derecha»), que contradice el polo fijo. Poner:
    - (a) «si RTVC Ahora, en 90 días, fiscaliza al Gobierno De la Espriella como fiscalizaría a otro, con piezas propias críticas, eso rompe el oficialismo, y la lectura pasa a ser la de cualquier medio»;
    - (b) «si en la próxima campaña (2030) su encuadre favorece a un candidato que no es el del Gobierno, aparece una posición propia»;
    - (c) «si cambia el régimen de nombramiento del gerente (salvaguarda vinculante de independencia)».
12. **Sección nueva: HECHOS ESTRUCTURALES 2026**: la tabla de arriba (15-08, 22-08, 10-09, 15-09, 25-09 y 07-10), solo con fuente primaria. La «auditoría editorial» va como secundaria.
13. **Sección nueva: CONTRATACIÓN PÚBLICA**, en el formato del protocolo:

> Contratación pública (SECOP I y II, NIT 900002583, consultado 2026-10-10): 14 contratos por $30.422 millones contratados en los últimos 12 meses, todos en SECOP II y todos firmados antes del 07-08-2026; 386 por unos $497.000 millones en total desde 2017 (SECOP II: 265 por $389.681 millones; SECOP I: 121 por $107.651 millones), con valores que en SECOP II pueden incluir adiciones. Principales contratantes de los últimos 12 meses: Presidencia de la República (DAPRE, 3 contratos, $10.680 millones), Ministerio de Educación ($10.600 millones), ICBF ($5.047 millones) y Ministerio de Transporte ($1.390 millones). Todos son entidades del Gobierno nacional, el mismo que el medio cubre y que nombra a su gerente. Sus objetos son de producción, emisión y divulgación de la propia entidad («para difundir las acciones del Ministerio de Educación Nacional»). Con el Gobierno De la Espriella no hay contratos en los que el medio sea contratista a 2026-10-10. Como contratante, el 2026-09-28 firmó un servicio de fotografía para la Presidencia (RTVC-CD-1644-2026).

14. **REVISIÓN EXTERNA**: anotar esta respuesta y su resolución.

En `shared/mediaOwnership.js`, entrada `rtvc`:
15. `holdings[0]` → el texto del punto 2, abreviado. Tiene que conservar la nulidad de 2011 y la forma SAS del RUES como tensión.
16. `holdings[1]` → «El Gobierno nombra a su gerente por decreto, y el control pasa por MinTIC. Gerente desde agosto de 2026: Ángela María Mora Soto, nombrada por el Gobierno De la Espriella.»
17. `notes[1]` → «El período presidencial cambió el 7 de agosto de 2026. La gerencia cambió el 12-13 de agosto, la franja informativa y de opinión se cerró el 15-08 y los contratos periodísticos se terminaron el 10-09. Desde el 07-10 hay un informativo nuevo, "RTVC Ahora". Cada cambio de gobierno trae otra redacción.»
18. `notes[2]` (la previsión): se **conserva literal** y se añade debajo: «CONTRASTE (2026-10-10): confirmada. Ver revision-externa/barridos/rtvc.md.»
19. `notes`, nuevas: la línea de contratación pública; la tensión «sociedad entre entidades públicas / S.A.S.»; y «Rectificó por orden judicial (Tribunal Superior de Bogotá, tutela, 30-07-2026) información que publicó el 19, 21 y 26 de abril de 2026».
20. `sources`: quitar `https://www.funcionpublica.gov.co/eva/gestornormativo/norma.php?i=82339`. Añadir:
    - `https://normograma.mintic.gov.co/mintic/compilacion/docs/decreto_3912_2004.htm`
    - `https://normograma.mintic.gov.co/mintic/compilacion/docs/decreto_3525_2004.htm`
    - la consulta RUES con `$select` de arriba
    - `https://www.rtvcnoticias.com/actualidad/inravision/sistema-medios-publicos-impulsara-la-cultura-el-deporte-y-las-regiones`
    - `https://www.rtvcnoticias.com/actualidad/rtvc/rtvc-avanza-en-la-transformacion-del-sistema-de-medios-publicos`
    - los dos PDF de la MOE UE

    Mantener la Resolución 0461 de 2016 y State Media Monitor (este, con la nota «gerente desactualizado a 2026-10-10»).
21. `ownerType: 'publico'` y `controlGroup: 'estado-colombiano'` **se mantienen**. **`verifiedAt`**: hoy hereda `VERIFICADO = '2026-07-29'`; propuesta `'2026-10-10'` cuando se apliquen estas correcciones. La gerente sale de fuente primaria y la forma jurídica del RUES de 2026. Queda declarada la falta del decreto de nombramiento.

En `shared/mediaRegistry.js`, entrada `rtvc`:
22. `bias: null` → `0.0`, con el `biasRationale` de arriba. Al comentario «SIN MEDIR» se le añade debajo el cierre: «RE-MEDIDO EL 2026-10-10 con un barrido de 12 meses: oficialismo a los dos lados del cambio; 0,00 por el polo fijo.» `reviewedAt: null` (sin firmar). **`factuality: 0.82` no se toca aquí** (ver las decisiones).

En `shared/centinela.js`:
23. **No se puede añadir con consultas al buscador del sitio**: `/search/` está excluido en su robots.txt. Propuesta, fuera del centinela:
    - comprobación mensual de los listados `/actualidad/rtvc` y `/actualidad/inravision`, que es donde el medio publica sus relevos y comunicados (el gerente, el informativo, las acciones judiciales);
    - comprobación anual de la `fecha_actualizacion` y la `organizacion_juridica` del RUES.

    Si el centinela llega a aceptar URL de listado además de consultas, se vigilaría «Mora Soto» y «gerente» en esas dos páginas.

**Lo que NO entra como hecho:**
- el número del decreto de nombramiento (dos secundarias, sin primaria);
- la «auditoría editorial» de MinTIC con retirada de contenidos (solo Pulzo; la primaria dice «revisión de contenidos y formatos»);
- lo que «halló» el Tribunal, según Pulzo curado con IA;
- la vinculación de contratistas con la campaña de De la Espriella;
- el estudio de La Silla Vacía sobre la cobertura de Cepeda (solo por Pulzo; la fuente está vetada);
- que la forma «SAS» suponga un cambio de naturaleza jurídica;
- cuántos contratos periodísticos se terminaron (SECOP no lo refleja).

**¿Aviso de quien dirige?** No procede. No consta candidatura ni cargo de elección de la gerente. Ser gerente de una sociedad pública nombrada por el Gobierno es la dependencia que ya declara la ficha de propiedad, no el cargo que dispara la regla. Es el mismo criterio que en Telecafé.

**Decisiones para el responsable editorial:**
1. **Valor.** Recomendación: **0,00 con la nota de oficialismo**, sin firmar. La alternativa es mantener «sin medir» hasta que «RTVC Ahora» tenga unos 30 días (hacia el 15-11) y re-medir solo la redacción nueva.
2. **Nivel B del barrido** (titulares de periodistas de plantilla como voz de la casa). Aquí no cambia el resultado, pero es un criterio para todo el catálogo: el protocolo cuenta los «titulares … propios no atribuidos» y solo excluye las columnas de terceros. Recomendación: admitirlo, siempre separado del nivel A.
3. **El encuadre entre candidatos de la segunda vuelta.** Recomendación: tratarlo como conducta de una redacción desmontada (regla del presente), declarado en CONTRA, sin mover el número.
4. **`verifiedAt`.** Recomendación: ponerlo (2026-10-10) al aplicar las correcciones.
5. **Centinela.** Recomendación: las dos comprobaciones manuales del punto 23. No lo hay por buscador.
6. **Factualidad (0,82).** Fuera del encargo, pero sale de aquí. Hay una sentencia de tutela que ordenó rectificar información de abril de 2026 por falta de acreditación. Es de la redacción anterior. Se anota por si el responsable editorial quiere revisarla con el criterio de factualidad del catálogo.
