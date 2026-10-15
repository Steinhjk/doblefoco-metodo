# Respuesta — Claude Opus 5.5 sobre Revista RAYA

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
> **Sin ninguna edición.** El revisor no copió cédulas, teléfonos ni
> direcciones, y no enlazó consultas de SECOP ni del RUES: cita los conjuntos
> y los procesos como texto. Ninguno de sus enlaces muestra un documento de
> identidad.

---

## RESPUESTA LITERAL

```
DECLARACIÓN PREVIA DE CONFLICTO
Soy Claude Opus 5.5 (claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Que coincida o no con ella mide fiabilidad, no validez. Para reducir ese sesgo me apoyé sobre todo en fuentes que la ficha NO usa: el manifiesto y la página de financiación del propio medio, sus listados de secciones, RUES, SECOP II/I, la página del Tribunal Superior de Bogotá recogida por El Colombiano, e Infobae. Solo leí el archivo de envío; no abrí ningún otro archivo del repositorio. La clasificación de cada pieza como «con postura» es MÍA, de un solo codificador, y la tiene que revisar una persona.

MÉTODO Y DÓNDE BUSQUÉ (todo consultado el 2026-10-10)
- robots.txt revisado antes de descargar: revistaraya.com (solo excluye rutas de sistema de Joomla y no nombra a ClaudeBot, Claude-Web ni anthropic-ai); directorio.sembramedia.org (robots.txt devuelve 404); datos.gov.co (User-agent *, crawl-delay 1; no excluye /resource/); elcolombiano.com (pone «User-agent: Anthropic-ai / Allow: /»); infobae.com (User-agent *, sin exclusiones para estos bots). No toqué lasillavacia.com, cambiocolombia.com, eltiempo.com ni vlex.
- HTML crudo con curl -sL y user-agent de navegador (--ssl-no-revoke). La portada y los feeds de revistaraya.com devolvieron 429 (protección anti-bots de Deflect/eQualit.ie). Las páginas interiores sí respondieron con 200.
- Páginas del medio: /staff.html, /manifiesto.html, /financiacion.html, /subraya.html (investigación: 99 piezas con fecha, del 2025-11-24 al 2026-10-06), /enlaraya.html (96 entradas, sin fecha en el listado), /opinion.html (99 columnas, sin fecha en el listado), la página de certificación JTI y el buscador interno /buscar.html con los términos «libertad de prensa», «editorial» y «Cepeda». Además abrí 11 piezas sueltas para ver su fecha, autor, sección y notas de transparencia.
- Registros: RUES (c82u-588k) buscando «REVISTA RAYA» en razon_social; SECOP II (jbjy-vk9h) por documento_proveedor = 901644009 y = 9016440098 (el NIT con el dígito de verificación pegado), y por proveedor_adjudicado con «REVISTA RAYA»; SECOP I (f789-7hwg) por identificacion_del_contratista con las dos variantes. Todas las consultas llevaron $select limitado a los campos citados.
- Buscador web: lo usé una sola vez («"Señal Investigativa" Revista RAYA RTVC 2026», excluyendo los dominios vetados). Estuvo disponible.
- Hueco declarado: el listado de SubRaya empieza el 2025-11-24, así que no barrí del 2025-10-10 al 2025-11-23. Tampoco barrí los programas audiovisuales pieza por pieza.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré nada de eso. Sigue siendo una fundación. Según RUES (c82u-588k, consultado el 2026-10-10), «FUNDACIÓN REVISTA RAYA», NIT 901644009, Cámara de Comercio de Bogotá, tiene estado_matricula «ACTIVA», fecha_matricula 20220930, fecha_renovacion 20260515 y ultimo_ano_renovado 2026.
  Lo que sí cambió en los últimos 12 meses es la FINANCIACIÓN: entraron contratos públicos grandes con RTVC y una alianza pagada con el Ministerio de Educación del gobierno saliente (ver las objeciones 1 y 2), y uno de esos contratos figura como «terminado» tres días antes del cambio de gobierno.

- La persona que la ficha nombra como director, ¿sigue viva y en el cargo?
  Sí, a 2026-10-10. Página /staff.html: «Edinson Arley Bolaños — Cofundador, integrante del consejo directivo, director de la Revista RAYA.»
  La otra persona que la ficha presenta como «su editora», Isabel Caballero, NO aparece en el staff actual (cero coincidencias de «Caballero» en /staff.html). El manifiesto la nombra solo entre los «Otros fundadores: … Isabel Caballero Samper» (ver la objeción 5).

- ¿Quién dirige hoy la redacción?
  El director es Edinson Arley Bolaños. La editora general y defensora del lector es Fabiola León Posada, según /staff.html (2026-10-10): «Fabiola León Posada — Editora general de la Revista RAYA y defensora del lector».
  La página de financiación añade: «La dirección de nuestro proyecto es colectiva. Los cargos de dirección, incluyendo la editorial, se eligen mediante votación de quiénes integramos el equipo.»

- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que la ficha cita?
  Sí: la renovación en RUES del 2026-05-15 (citada arriba). El conjunto abierto de RUES no trae ni la junta ni el representante legal. Más importante para el expediente es SECOP II, con cuatro contratos firmados entre 2025-02 y 2026-01 (objeción 1). La ficha no cita ningún registro público.

## OBJECIONES

### OBJECIÓN 1 — La ficha omite la financiación pública del gobierno saliente, que es la más grande documentada

- QUÉ afirma la ficha: «Su ingreso principal son servicios prestados a organizaciones sin ánimo de lucro, seguidos de consultoría; completan la financiación campañas de micromecenazgo, donaciones…». La fuente es SembraMedia, y el propio SembraMedia advierte: «Este perfil fue elaborado a partir de información proporcionada por el propio medio… no garantiza su exactitud o vigencia».

- POR QUÉ es incorrecto: SECOP II (jbjy-vk9h, documento_proveedor = 901644009, consultado el 2026-10-10) registra cuatro contratos de coproducción con INRAVISIÓN/RTVC, el sistema de medios públicos. Hecho:
  · RTVC-COPRO- 253-2025, firmado el 2025-02-07: «COPRODUCIR CON RTVC EL PROYECTO PERIODISTICO SEÑAL INVESTIGATIVA». Valor del contrato: 783.000.000. Estado: «Modificado».
  · RTVC-COPRO-2421-2025, firmado el 2025-09-04: «…PROYECTO PERIODISTICO SEÑAL INVESTIGATIVA… ENTRE RTVC NOTICIAS Y LA FUNDACIÓN REVISTA RAYA». Valor: 417.600.000.
  · RTVC-COPRO-2468-2025, firmado el 2025-09-12: «…SEÑAL INVESTIGATIVA DEBATES…». Valor: 100.000.000.
  · RTVC-COPRO-304-2026, firmado el 2026-01-21: «Aunar esfuerzos… para desarrollar conjuntamente el programa de investigación Señal Investigativa y el programa de opinión Parte y Contraparte». Valor: 1.361.295.000. Fecha de fin: 2026-12-31. Estado: «terminado». Última actualización: 2026-08-04.
  · Suma de los valores registrados: 2.661.895.000 COP. SECOP I y SECOP II con el dígito de verificación pegado (9016440098) no devolvieron nada.

- Cautelas:
  · Los valores son los registrados en SECOP. valor_pagado figura en 0 en los cuatro contratos, así que no hay dato fiable de lo pagado.
  · Infobae (2025-11-03) atribuye al contrato de febrero de 2025 un aporte de RTVC de 357 millones (68 %) más un aporte en especie de RAYA de 165 millones: «RTVC destina un aporte económico de 357 millones de pesos, que representa el 68% del valor del proyecto». Esa cifra no cuadra con los 783 millones de SECOP (contrato «Modificado»). La discrepancia queda declarada.
  · Infobae recoge una denuncia de un concejal de oposición. Es la fuente del dato, no un aval de su lectura («Propaganda»).

- Inferencia (no es un hecho): que el contrato de 2026, previsto hasta diciembre, figure «terminado» con última actualización tres días antes del 07-08-2026 sugiere una terminación anticipada en la transición. No encontré la causa.

- El medio lo reconoce él mismo: /financiacion.html (actualizada el 26-09-2024) dice «En junio de 2024 realizamos un acuerdo con Señal Colombia, de RTVC, para la coproducción de Señal investigativa». La misma página declara contratos de 2023 y 2024 con la Agencia de Reincorporación y Normalización y con la Agencia de Renovación Territorial. Esos dos no aparecen en SECOP bajo su NIT; no los verifiqué.

- FUENTES:
  · SECOP II, conjunto jbjy-vk9h, procesos RTVC-COPRO- 253-2025, RTVC-COPRO-2421-2025, RTVC-COPRO-2468-2025 y RTVC-COPRO-304-2026 (consultado el 2026-10-10).
  · https://www.infobae.com/colombia/2025/11/03/denuncian-que-hollman-morris-aprobo-pagos-millonada-a-revista-raya-para-investigaciones-independientes-en-rtvc/ (2025-11-03).
  · https://revistaraya.com/financiacion.html (actualización 2024-09-26; consultada el 2026-10-10).

- NIVEL: propiedad/financiación (nivel 1) y registro externo (nivel 3).

### OBJECIÓN 2 — «No admite publicidad dentro del contenido editorial» ya no es exacto: en julio de 2026 publicó contenido pagado por el Ministerio de Educación que elogia al gobierno saliente

- QUÉ afirma la ficha: «No cobra por leer ni admite publicidad dentro del contenido editorial.»

- POR QUÉ es incorrecto. Hecho: en la sección Síntesis aparecen tres piezas con esta nota: «Este producto hace parte de una alianza entre Revista RAYA y el Ministerio de Educación Nacional, con recursos destinados a su producción y divulgación. RAYA mantiene su independencia editorial…». Son:
  · «Cuatro años de gratuidad en la universidad pública: qué logró en la educación superior en el gobierno Petro» (publicada el 17-07-2026).
  · «De la enseñanza tradicional a la formación integral: la revolución educativa del Gobierno del Cambio» (30-07-2026). La nota de alianza también figura en el HTML crudo de esta pieza.
  · «Llevar la educación superior al territorio: el legado del Cambio» (31-07-2026). El texto dice: «Durante el Gobierno del Cambio, el Ministerio de Educación atacó ambos males al mismo tiempo.»
  La política de financiación ya lo preveía: «La Revista RAYA ha decidido aceptar recursos por vía de pauta o asociaciones de coproducción… que pueden provenir de organizaciones privadas o estatales» (/financiacion.html). Lo declara con transparencia, y eso cuenta a su favor. Aun así, es contenido pagado por un gobierno, publicado en sección editorial, con titulares que celebran a ese gobierno una semana antes de que saliera.
  No encontré en SECOP, bajo el NIT de RAYA, el contrato con el Ministerio de Educación; no sé por qué vía se pagó.

- FUENTES (consultadas el 2026-10-10):
  · https://revistaraya.com/cuatro-anos-de-gratuidad-en-la-universidad-publica-que-logro-en-la-educacion-superior-en-el-gobierno-petro.html (2026-07-17)
  · https://revistaraya.com/de-la-ensenanza-tradicional-a-la-formacion-integral-la-revolucion-educativa-del-gobierno-del-cambio.html (2026-07-30)
  · https://revistaraya.com/llevar-la-educacion-superior-al-territorio-el-legado-del-cambio.html (2026-07-31)

- NIVEL: financiación (nivel 1) y hecho editorial de los últimos 12 meses (nivel 5).

### OBJECIÓN 3 — El ARGUMENTO de la ficha se apoya en columnas de terceros, no en la voz de la casa

- QUÉ afirma la ficha: que «Los migrantes, víctimas del fascismo» y otros titulares son «elección léxica de la casa, y esa sí es evidencia de línea».

- POR QUÉ es incorrecto. Hecho: el listado /opinion.html atribuye esas piezas a columnistas:
  · «Los migrantes, víctimas del fascismo» — Mauricio Jaramillo Jassir (/mauricio-jaramillo/1807-…).
  · «De la Paz Total a la Guerra Total» — Laura Espinosa Macías (/laura-espinosa-macias/1808-…).
  · «El PGN 2027: lo técnico y sus contradicciones» — Laura Espinosa Macías (/laura-espinosa-macias/1820-…).
  La regla del 2026-10-09 excluye expresamente las «columnas de terceros». Tres de los siete titulares de la ficha no son admisibles como voz de la casa.
  Dos de los otros sí lo son, aunque la ficha no lo comprobó:
  · El de Cerimedo es de David González M., periodista de plantilla, en SubRaya.
  · «Un mes de ataques del gobierno De la Espriella a la libertad de prensa» es de Tatiana Portela, de plantilla, en la sección Síntesis, publicado el 07-09-2026.

- Consecuencia: el ARGUMENTO, tal como está escrito, no sostiene la tesis de «léxico de la casa». La evidencia de voz de la casa existe, pero hay que construirla con otras piezas (objeción 4).

- FUENTES (consultadas el 2026-10-10):
  · https://revistaraya.com/opinion.html
  · https://revistaraya.com/un-mes-de-ataques-del-gobierno-de-la-espriella-a-la-libertad-de-prensa.html («Publicado el: 07 Septiembre 2026 / Por: Tatiana Portela»)

- NIVEL: conducta observable / hecho editorial de los últimos 12 meses.

### OBJECIÓN 4 — El −0,55 no tiene el soporte que exige el protocolo; el barrido de la voz de la casa sostiene como mucho el tope de −0,30, salvo que la financiación pública se trate como nivel 1

- QUÉ afirma la ficha: un valor de −0,55, apoyado en 7 titulares de 30 días que la propia ficha reconoce insuficientes.

- POR QUÉ es incorrecto:
  (a) Sin endoso y sin nivel 1 con posición conocida, la excepción de voz de la casa topa en ±0,30. No encontré endoso de la casa. La única pieza de voto que hallé es una columna firmada por un tercero: /pablo-montoya/1706-es-menester-votar-por-cepeda.html. La autodeclaración «progresista» es de nivel 4 y no puede sostener sola el valor.
  (b) Hice un barrido reproducible de SubRaya: las 99 piezas del 2025-11-24 al 2026-10-06, más búsquedas internas. El listado está en https://revistaraya.com/subraya.html. Conté como «con postura» las piezas cuyo titular o entradilla CALIFICA, adopta una tesis de parte o defiende a un gobierno, y no las que solo fiscalizan. Codificación mía, un solo codificador.

  Antes del cambio (gobierno Petro), a favor del lado del gobierno o con calificación contra la derecha:
   1. 2025-12-02 — «El audio con el que El Tiempo construyó un falso escándalo contra la DNI». Entradilla: «La maniobra coincide con una ofensiva política para golpear al Gobierno Petro.» (Unidad Investigativa) /el-audio-con-el-que-el-tiempo-construyo-un-falso-escandalo-contra-la-dni.html
   2. 2025-12-19 — «Coronel Publio Hernán Mejía: el héroe de la extrema derecha condenado por crímenes de guerra». (Padilla y Fragozo) /coronel-publio-hernan-mejia-…html
   3. 2026-02-01 — «El informe reservado que el Gobierno envió a Washington para demostrar las cifras erróneas sobre la cocaína». Hace suya en el titular la tesis del gobierno. (Forero)
   4. 2026-02-15 — «El pulso por el salario mínimo: ¿quiénes lograron frenar el aumento?». Retrata a los demandantes del decreto como gremios y Centro Democrático. (Padilla y Portela)
   5. 2026-04-21 — «Juanita León cambia de versión cuatro veces sobre participación de La Silla Vacía en el "Proyecto Júpiter"». Es parte de la serie que presentaba a un medio crítico como pieza de una operación «para deslegitimar al Gobierno Nacional». El Tribunal Superior de Bogotá ordenó rectificarla (objeción 6).
   6. 2026-05-30 — «Zandalio Durán, el parapolítico y corrupto ex alcalde de Puerto Wilches que apoya a Paloma Valencia». (Unidad Investigativa)
   7. 2026-06-04 — «"El Tigre" y el clan Char: una alianza con los de siempre, señalados de corrupción». (Redacción)
   8. 2026-06-05 — «Justicia le da la razón a RAYA y Señal Colombia: niega tutela con que La Silla Vacía buscaba censura». (Redacción)
   9. 2026-07-02 — «La red trumpista que rodea a De la Espriella y la pregunta por la soberanía de Colombia». (David González M., Rayuela)
   10. 2026-07-17, 07-30 y 07-31 — las tres piezas del Ministerio de Educación de la objeción 2. Las cuento como una sola unidad, porque son contenido pagado.
   Dudosa en el eje (la cuento aparte, no en el total): 2026-02-21, «Exclusivo: 112 colombianos han participado del genocidio en Gaza» (entradilla: «el lobby progenocidio opera impunemente»).

  Después del cambio (gobierno De la Espriella), contra el gobierno con calificación:
   11. 2026-08-14 — «El primer bombardeo del gobierno De la Espriella podría ser un "falso positivo"…, aseguran líderes sociales». Atribuida; es débil.
   12. 2026-08-23 — «Radio Nacional sin noticias: Gobierno De la Espriella pone mordaza a la voz de las regiones». (Fabiola León Posada, editora general, Síntesis)
   13. 2026-09-07 — «Un mes de ataques del gobierno De la Espriella a la libertad de prensa». (Tatiana Portela, Síntesis)
   14. 2026-09-08 — «La red de manipulación de Cerimedo y Negre, al servicio de la extrema derecha latinoamericana…». (David González M.)
   15. 2026-09-16 — «La política del cadáver: por qué la extrema derecha necesita un enemigo muerto y exhibido». (Juan Sebastián Lozano, de plantilla, Rayuela)
   16. 2026-09-27 — «En el sepelio de Ricardo Martínez: inconsistencias apuntan al primer falso positivo del Gobierno De la Espriella». (Forero)

  Contrapesos que busqué, piezas que fiscalizan a figuras del lado contrario:
   · 2025-11-27, «Los miles de millones de pesos detrás de la pelea de Ismael Peña por la rectoría de la U. Nacional».
   · 2026-09-22, «Ismael Peña, rector de la Nacional, busca millonaria indemnización…».
   · 2026-10-06, «La maestría exprés del jefe de Planeación de la ANT». Es un funcionario del gobierno actual, así que no es un contrapeso.
   Ninguno de estos lleva postura calificativa. No pude verificar desde una fuente admisible la cercanía de Peña con el gobierno saliente, así que su valor como contrapeso es una inferencia.
   En las 99 piezas no encontré NINGUNA investigación con postura contra el gobierno Petro mientras gobernaba. Las piezas de fiscalización anteriores al 07-08-2026 apuntan sobre todo a candidatos y políticos de oposición (De la Espriella, Paloma Valencia, Uribe, Char, Centro Democrático), no al gobierno en ejercicio.

  Recuento: 16 entradas con postura (10 antes del cambio, contando el punto 10 como una sola aunque agrupa tres piezas, y 6 después) contra 0 en sentido contrario. La razón supera holgadamente 3:1. A mi juicio esto CUMPLE el umbral de nivel 2 de la regla del 2026-10-09, pero lo codifiqué yo solo y lo tiene que recodificar una persona. Aun así, lo que esto justifica es −0,30 (el tope), no −0,55.
  La distancia hasta −0,55 solo se sostendría si el comité tratara como «nivel 1 con posición conocida» la financiación del gobierno saliente: los contratos de RTVC de la objeción 1 y el contenido pagado por el Ministerio de Educación de la objeción 2. La ficha no hace ese razonamiento. Tiene que hacerlo explícitamente o bajar a −0,30.

- FUENTES: las URLs de revistaraya.com citadas arriba, con su fecha de publicación (consultadas el 2026-10-10), y el listado https://revistaraya.com/subraya.html (consultado el 2026-10-10).

- NIVEL: hecho editorial de los últimos 12 meses, voz de la casa a ambos lados del cambio.

### OBJECIÓN 5 — Equipo directivo mal descrito: Isabel Caballero no es «su editora»

- QUÉ afirma la ficha: «su director y su editora vienen de Cambio», refiriéndose a Edinson Bolaños e Isabel Caballero.

- POR QUÉ es incorrecto. Hecho: en /staff.html (2026-10-10) la editora general es Fabiola León Posada e Isabel Caballero no aparece. El manifiesto la lista solo como «Otros fundadores: Pablo Navarrete, Cristian Garavito, Isabel Caballero Samper, Maria Camila Diaz». El párrafo de «procedencia que conviene tener a la vista» queda sin base para la editora. Para Bolaños sí se sostiene: su biografía en /staff.html dice «fue parte del proyecto… de la Revista CAMBIO».

- Dato que la ficha no tiene, del mismo staff: Sebastián Forero, periodista de investigación, «Fue Director de Comunicaciones del Ministerio de Agricultura» y es periodista «en la Revista RAYA y el programa Señal Investigativa». No encontré en qué gobierno ocupó ese cargo.

- FUENTES (consultadas el 2026-10-10): https://revistaraya.com/staff.html ; https://revistaraya.com/manifiesto.html

- NIVEL: declaración del propio medio (nivel 4) sobre quién dirige.

### OBJECIÓN 6 — Falta un hecho de los últimos 12 meses con consecuencia verificable: la rectificación judicial ordenada en el caso «Proyecto Júpiter»

- QUÉ afirma la ficha: que el único hecho judicial (la inspección de 2023) queda fuera por la regla del presente. Es correcto, pero no recoge el hecho judicial de este año.

- POR QUÉ: El Colombiano (2026-07-31) informa sobre el fallo de tutela del Tribunal Superior de Bogotá del 30-07-2026: «los medios accionados tergiversaron la información para presentar a La Silla Vacía como un aliado o agencia digital del denominado "Proyecto Júpiter"… no fue demostrada ni siquiera de manera indiciaria». Y añade: «la Revista Raya distorsionó sus respuestas para sugerir una contradicción inexistente».
  RAYA cumplió: su pieza del 21-04-2026 lleva ahora la «Nota de rectifiación ordenada por la Sala Penal del Tribunal Superior de Bogotá en su fallo de tutela, con radicado No. 2026-00219-01». La propia nota de RAYA subraya que el Tribunal «negó la pretensión de retirar los contenidos», y lo registro como contrapeso.
  Relevancia para la orientación: la serie, coproducida con el medio público del gobierno saliente, presentaba a un medio crítico como parte de una operación «con el objetivo de deslegitimar al Gobierno Nacional». Así lo resume El Colombiano. Es conducta de defensa del gobierno en ejercicio, no fiscalización. Y el 05-06-2026 RAYA tituló en voz propia «Justicia le da la razón a RAYA y Señal Colombia: niega tutela con que La Silla Vacía buscaba censura», sobre su socio contractual.

- FUENTES:
  · https://www.elcolombiano.com/inicio/rtvc-raya-retractar-la-silla-vacia-proyecto-jupiter-AG39485115 (datePublished 2026-07-31)
  · https://revistaraya.com/juanita-leon-cambia-de-version-cuatro-veces-sobre-participacion-de-la-silla-vacia-en-el-proyecto-jupiter.html (consultada el 2026-10-10)

- NIVEL: registro externo, por ser sentencia (nivel 3), y hecho editorial de los últimos 12 meses (nivel 5).

### OBJECIÓN 7 — Las cifras de nivel 2 de la ficha son caducas y su «25,9×» descansa en una sola pieza

- QUÉ afirma la ficha: 8 artículos y 3 historias, y libertad de prensa al 16,7 %, «25,9×».

- POR QUÉ es incorrecto:
  · La medición del envío (2026-10-10, 40 días) da 29 artículos, 1 en historia y 1 historia. Por la regla del propio envío, vale esta.
  · Además, 16,7 % = 1/6 y 50 % = 3/6. El «perfil temático más extremo del catálogo» se calcula sobre unas seis piezas, y el «25,9×» es UNA pieza. La ficha lo destaca en negrita y lo usa en el ARGUMENTO («cubre libertad de prensa 26 veces más»). Con n=1 no debería figurar como evidencia, ni siquiera de especialidad.

- FUENTE: la sección «Conducta medida» de este mismo envío (2026-10-10), frente a la tabla de la ficha (2026-09-08).

- NIVEL: conducta medida (nivel 2).

## LO QUE NO PUDE VERIFICAR

- Si los fundadores fueron «nueve periodistas». SembraMedia dice «Fundadoras mujeres: 4 / Fundadores hombres: 5». No todos son periodistas: el staff incluye a un ingeniero de sistemas y a una diseñadora. No verificado.
- Que Isabel Caballero venga de Cambio: no podía usar cambiocolombia.com, y no encontré otra fuente.
- La fuente de La Silla Vacía que cita la ficha («Presentan la Revista RAYA»): dominio vetado para mí, no la abrí.
- El punto 3 del CONTRA, «Cerimedo trabaja abiertamente para candidaturas de esa familia política… etiqueta que el propio actor reivindica»: la ficha no da fuente y yo no encontré ninguna. No encuentro fuente para esto.
- La causa del estado «terminado» del contrato RTVC-COPRO-304-2026, y si Señal Investigativa sigue en antena con el gobierno nuevo. No busqué más para ahorrar buscador.
- Los contratos con la ARN (2023), la ART (2024) y el Ministerio de Educación (2026): no aparecen en SECOP I ni en SECOP II bajo el NIT 901644009, con o sin dígito de verificación. Pudieron ir por otra vía; no lo sé.
- El punto 4 del CONTRA (orden relativo frente a Vorágine y Cuestión Pública): no puedo evaluarlo sin leer esas fichas, y tengo prohibido abrir otros archivos.
- El periodo del 2025-10-10 al 2025-11-23 y las entradas de /enlaraya.html, que no tienen fecha en el listado. Por eso quedaron fuera del recuento.

## LO QUE FALTA

- Los contratos de SECOP II con RTVC (objeción 1), con número de proceso como texto. Son el primario del presente que sustituye a SembraMedia, que es autodeclarado.
- La autodeclaración vigente del manifiesto: «Queremos aportar al debate social con información de calidad desde una postura democrática y progresista» (/manifiesto.html, 18-08-2022, todavía en línea). La repite la página JTI del 31-07-2025: «desde una postura democrática y progresista». Es nivel 4 y la ficha no la cita.
- La alianza pagada con el Ministerio de Educación (objeción 2) y la sentencia de rectificación (objeción 6).
- El barrido de voz de la casa a ambos lados del cambio (objeción 4), en lugar de 7 titulares de 30 días.
- El nombre de la editora general actual (Fabiola León Posada) y el modelo de dirección colectiva electa.

## EVIDENCIA QUE NO MUEVE EL NÚMERO

- Certificación JTI de Reporteros sin Fronteras, anunciada por el medio el 31-07-2025: «RAYA se convirtió en uno de los primeros medios nacionales en recibir esta certificación» (https://revistaraya.com/revista-raya-recibe-certificacion-internacional-de-transparencia-y-periodismo-confiable-del-jti.html). Es un estándar de proceso, no una orientación.
- RAYA declara de forma visible la financiación del Ministerio de Educación al pie de cada pieza pagada. Es conducta de transparencia.
- RAYA cumplió la orden de rectificación y la publicó en la pieza original.
- Fiscalizó a un funcionario del gobierno nuevo con vínculo con el clan Char (2026-10-06) y al rector Ismael Peña en dos ocasiones (2025-11-27 y 2026-09-22). Fiscalizar no cuenta para la orientación.
- No encontré endoso editorial de la casa en la elección de 2026. El «Es menester votar por Cepeda» que hallé es una columna firmada por Pablo Montoya.
- Es especialista en conflicto armado y tierras: varias piezas de 2026 sobre Drummond, Hidroituango, El Aro y falsos positivos. Es formato, y la ficha lo trata bien.
- Su revelación sobre acoso en Red+ Noticias de Claro (2026-05-23 y 2026-05-29) y la de Gabriel Meluk (2026-05-28) afectan a medios grandes, sin eje partidista claro.
- Una pieza del 2026-05-28 sobre una bananera lleva en su titular la marca «[Aclarado por fallo de tutela]». Es un segundo ajuste judicial en 2026; no lo leí, así que no lo valoro.

## SIN OBJECIÓN
No aplica: hay 7 objeciones.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** Ver el aviso de arriba.

**Antes de nada: el número que se juzga no es −0,55.** En `shared/mediaRegistry.js`, `revista-raya` lleva `bias: null` y `biasRationale: 'SIN MEDIR. …'` desde el 2026-09-18 (commit `fa77249`, «El sesgo sin medir existe en el codigo»), por la decisión del responsable editorial del 2026-09-16 sobre el trío de investigación (Vorágine, Cuestión Pública y RAYA) y RTVC. Lo fija `shared/sinMedir.test.js` (`SIN_MEDIR_DECIDIDOS`). Pero la cabecera de `fichas/revista-raya.md` sigue diciendo «Valor actual | −0,55», y el envío la copió, así que el revisor atacó un valor que ya no está en el catálogo. **Sus objeciones se leen aquí contra el valor vigente, «sin medir»**, y la pregunta que resuelven es otra: **¿hay evidencia para pasar de «sin medir» a un número?** Además, **la decisión del 2026-09-16 no tiene entrada en `DECISIONES.md`**: consta en el comentario del registro, en el commit, en la prueba y en `PLAN_PRODUCTO_FINAL.md` (3.5).

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada (2026-10-10):
  - revistaraya.com: el de Joomla por defecto; `User-agent: *` con `Disallow` solo de carpetas técnicas. No nombra a ningún agente de Anthropic. **Como dice el revisor.**
  - datos.gov.co: `Crawl-delay: 1` y exclusiones de `/browse`; se usó solo `/resource`, con más de un segundo entre consultas.
  - elcolombiano.com: «User-agent: Anthropic-ai / Allow: /». infobae.com: `User-agent: *` sin exclusiones para la ruta usada. directorio.sembramedia.org: `/robots.txt` da 404. **Como dice el revisor.**
  - No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. **No hubo buscador web.**
- **Sitio**, en crudo con `curl -sL --ssl-no-revoke` y User-Agent de navegador (Chrome 126), **de 4 a 6 segundos entre peticiones**, sin pedir la portada (antibots, 429): `/staff.html`, `/manifiesto.html`, `/financiacion.html`, la nota de la certificación JTI, los listados `/subraya.html`, `/sintesis.html`, `/rayuela.html`, `/rayainvestiga.html` y `/opinion.html`, y **143 piezas una por una** (las 78 primeras de Síntesis, las 50 de Rayuela, las 5 de RAYA Investiga y 10 de SubRaya). 153 peticiones, todas 200.
- **Registros**, en datos.gov.co: RUES (`c82u-588k`) por `nit=901644009` y por razón social; SECOP II (`jbjy-vk9h`) por `documento_proveedor` = `901644009`, `9016440098` y `901644009-8`, por `proveedor_adjudicado like '%REVISTA RAYA%'` y por objeto (`SEÑAL INVESTIGATIVA`, `PARTE Y CONTRAPARTE`, `REVISTA RAYA`); SECOP I (`f789-7hwg`) por `identificacion_del_contratista` con las tres variantes y por razón social. Además, contratos del Ministerio de Educación Nacional en 2026 con «RAYA» o «divulgación» en el objeto.
- **Prensa:** Infobae (03-11-2025), El Colombiano (31-07-2026) y la ficha de SembraMedia.
- **Repositorio:** el envío; `fichas/revista-raya.md`; las entradas de `revista-raya` y `raya-fundacion` en `shared/mediaOwnership.js` y la de `shared/mediaRegistry.js`; `shared/centinela.js` (RAYA no está); las menciones en `fichas/voragine.md`, `fichas/volcanicas.md` y `fichas/colombia-informa.md`; `shared/sinMedir.test.js`; el protocolo; DECISIONES.md (2026-10-07 a 2026-10-10); el barrido modelo de El Informador.
- **El barrido**, reproducible, está en `revision-externa/barridos/revista-raya.md`: 225 piezas de 12 meses, con URL, fecha, lado del cambio y clase.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | SECOP II: 4 contratos de coproducción con Inravisión/RTVC por 2.661.895.000 COP; el de 2026, «terminado» y actualizado el 04-08; Infobae da otras cifras | sí | sí | **Aceptada.** Los cuatro procesos, valores, fechas, estados y objetos son exactos; la suma también. SECOP I: 0, con y sin dígito de verificación. Las cifras de Infobae son literales y no cuadran con SECOP: discrepancia declarada. **Pero no es nivel 1** (ver abajo): entra como contratación pública y tensión |
| 2 | Julio de 2026: contenido pagado por el Ministerio de Educación en Síntesis, con nota de alianza, que elogia al gobierno saliente | sí | sí | **Aceptada, y se queda corta.** Son **7 piezas**, no 3 (17-07 a 06-08-2026), y hay **6 más pagadas por el CNE** (27-05 a 20-06-2026). Contradice la frase de la ficha y el propio manifiesto («sin muros de pago, propaganda ni publicidad dentro de nuestro contenido editorial») |
| 3 | El ARGUMENTO de la ficha se apoya en columnas de terceros | sí | sí | **Aceptada.** Las tres columnas son de firmas que no están en la plantilla. Las otras dos piezas que cita sí son de plantilla |
| 4 | Barrido de SubRaya: 16 con postura (10 y 6), 0 en contra; tope −0,30 salvo que la financiación cuente como nivel 1 | sí | sí, pieza por pieza | **Aceptada en la dirección y en el tope; el recuento cambia.** De sus 16 se sostienen 12. Barriendo también Síntesis, Rayuela y RAYA Investiga: **35 piezas con postura (22 antes y 13 después; 19 sin las leves) frente a 3 contrapesos parciales**. Cumple las cinco condiciones. La financiación **no** es nivel 1: rige el tope |
| 5 | La editora general es Fabiola León Posada; Isabel Caballero no está en el staff; Bolaños sigue | sí | sí | **Aceptada.** Literal en `/staff.html` y `/manifiesto.html` |
| 6 | Rectificación judicial (Tribunal Superior de Bogotá, 30-07-2026) por la serie del «Proyecto Júpiter»; RAYA la publicó | sí | sí | **Aceptada.** El Colombiano lo recoge literal y RAYA publicó la nota con el radicado. Además: la pieza del 05-06 que celebraba la primera instancia no lleva nota de que el Tribunal la revirtió en parte |
| 7 | Las cifras de nivel 2 de la ficha están caducas y el «25,9×» es una pieza | sí | sí | **Aceptada.** La medición vigente del envío es 29 artículos, 1 en historia, 1 historia (40 días) |

### Lo verificado, objeción por objeción

**1 · Contratación pública.**
- **SECOP II**, `documento_proveedor=901644009` (2026-10-10), 4 filas, proveedor «FUNDACIÓN REVISTA RAYA», todas «Contratación régimen especial», `valor_pagado` 0 en las cuatro:
  - RTVC-COPRO- 253-2025 (INRAVISIÓN), firmado el 2025-02-07, fin 2025-08-31, $783.000.000, «Modificado»: «COPRODUCIR CON RTVC EL PROYECTO PERIODISTICO SEÑAL INVESTIGATIVA.»
  - RTVC-COPRO-2421-2025 (INRAVISIÓN), 2025-09-04, fin 2025-12-31, $417.600.000, «En ejecución»: «…ENTRE RTVC NOTICIAS Y LA FUNDACIÓN REVISTA RAYA».
  - RTVC-COPRO-2468-2025 (INRAVISIÓN), 2025-09-12, fin 2025-12-31, $100.000.000, «En ejecución»: «…SEÑAL INVESTIGATIVA DEBATES…».
  - RTVC-COPRO-304-2026 (INRAVISIÓN - SISTEMA DE MEDIOS PÚBLICOS DEL ESTADO COLOMBIANO S.A.S), 2026-01-21, fin 2026-12-31, $1.361.295.000, «terminado», `ultima_actualizacion` 2026-08-04: «…el programa de investigación Señal Investigativa y el programa de opinión Parte y Contraparte…».
  - **Suma: $2.661.895.000. Exacto.** Con `9016440098` y `901644009-8`: 0 filas. Por razón social: las mismas 4. Por objeto: ningún otro proveedor ni contrato con «Señal Investigativa» o «Parte y Contraparte».
- **SECOP I** (`f789-7hwg`), las tres variantes y por razón social: **0**. Exacto.
- **Últimos 12 meses (2025-10-10 → 2026-10-10): 1 contrato, $1.361.295.000** (el 304-2026).
- **¿Contrató el gobierno nuevo?** **No consta.** Ningún contrato de SECOP con el NIT es posterior al 2026-01-21, y ninguna pieza de los 12 meses lleva nota de alianza con una entidad después del 06-08-2026. El 304-2026, previsto hasta diciembre, figura «terminado» con actualización del 04-08. Que se terminara antes de tiempo en la transición es **inferencia** (no consta la causa); también lo es que RAYA Investiga, el formato propio que arranca el 08-09 («En su primer capítulo…»), sustituya a Señal Investigativa.
- **Infobae** (`datePublished` 2025-11-03T04:55:03Z), literal: «RTVC destina un aporte económico de 357 millones de pesos, que representa el 68% del valor del proyecto , mientras que la Fundación Raya realiza un aporte en especie estimado en 165 millones de pesos». También: «pagos mensuales por más de 71 millones de pesos» y «un contrato de coproducción de veinte programas». La cita «Propaganda» es del concejal denunciante. **No cuadra con los $783.000.000 de SECOP** para el contrato de febrero de 2025, que figura «Modificado». Discrepancia declarada; vale SECOP, y siempre como valor **contratado**.
- **El propio medio** (`/financiacion.html`, «Publicado el: 11 Octubre 2022», «Última actualización: 26 Septiembre 2024»): «En junio de 2024 realizamos un acuerdo con Señal Colombia, de RTVC, para la coproducción de Señal investigativa». Declara también proyectos de 2023 con la Agencia de Reincorporación y Normalización y de 2024 con la Agencia de Renovación Territorial, y que acepta «recursos por vía de pauta o asociaciones de coproducción … que pueden provenir de organizaciones privadas o estatales». Los de la ARN y la ART **no aparecen en SECOP bajo su NIT**: laguna, como dice el revisor.
- **RUES** (`c82u-588k`), una fila: «FUNDACIÓN REVISTA RAYA», NIT 901644009-8, matrícula 90061613, Cámara de Comercio de Bogotá, «ACTIVA», matriculada el 20220930, renovada el 20260515, último año 2026, «LAS DEMÁS ORGANIZACIONES CIVILES,CORPORACIONES,FUNDACIONES», CIIU 5813, actualizada el 2026/09/29. **Exacto** en lo que cita el revisor.
- Consultas sin datos personales (comprobadas el 2026-10-10):
  - `https://www.datos.gov.co/resource/c82u-588k.json?nit=901644009&$select=razon_social,nit,digito_verificacion,matricula,camara_comercio,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,organizacion_juridica,cod_ciiu_act_econ_pri,fecha_actualizacion`
  - `https://www.datos.gov.co/resource/jbjy-vk9h.json?documento_proveedor=901644009&$select=referencia_del_contrato,nombre_entidad,fecha_de_firma,fecha_de_fin_del_contrato,valor_del_contrato,valor_pagado,estado_contrato,modalidad_de_contratacion,descripcion_del_proceso,proveedor_adjudicado,ultima_actualizacion`
  - `https://www.datos.gov.co/resource/f789-7hwg.json?identificacion_del_contratista=901644009&$select=numero_de_constancia,nombre_entidad,fecha_de_firma_del_contrato,cuantia_contrato,detalle_del_objeto_a_contratar,nom_razon_social_contratista` (devuelve `[]`)

**2 · Contenido pagado.**
- Las tres piezas que cita existen, con su fecha y con la nota literal: «Este producto hace parte de una alianza entre Revista RAYA y el Ministerio de Educación Nacional, con recursos destinados a su producción y divulgación. RAYA mantiene su independencia editorial, sus criterios de verificación y su responsabilidad periodística sobre el contenido publicado.» La frase «Durante el Gobierno del Cambio, el Ministerio de Educación atacó ambos males al mismo tiempo» es literal (31-07).
- **Son siete, todas en Síntesis:** 17-07, 28-07, 30-07, 31-07 (dos), 01-08 y 06-08-2026. La última, la víspera del cambio de gobierno. Lista en el barrido, §6.
- **Y hay otra alianza que el revisor no vio:** 6 piezas de pedagogía electoral (27-05 a 20-06-2026, Síntesis y Rayuela) con «una alianza comunicativa financiada por el Consejo Nacional Electoral». El CNE no es el gobierno, y las piezas no tienen postura en el eje.
- **Contra la ficha y contra el manifiesto.** La ficha dice «No cobra por leer ni admite publicidad dentro del contenido editorial»; el manifiesto (vigente, del 18-08-2022), «Somos un medio independiente sin muros de pago, propaganda ni publicidad dentro de nuestro contenido editorial». Las 13 piezas pagadas están en secciones editoriales y declaradas al pie. Lo declara, y eso cuenta a su favor; lo que la ficha afirma ya no es exacto.
- **Una corrección menor al revisor:** el titular del 17-07 es «Cuatro años de gratuidad en la universidad pública: ¿qué logró la educación superior en el gobierno Petro?», no «qué logró en la educación superior».
- En SECOP II no aparece un contrato del Ministerio de Educación con RAYA ni con «RAYA» en el objeto en 2026. Por qué vía se pagó: laguna.

**3 · Columnas de terceros.** En `/opinion.html`: `/mauricio-jaramillo/1807-los-migrantes-victimas-del-fascismo.html`, `/laura-espinosa-macias/1808-de-la-paz-total-a-la-guerra-total.html` y `/laura-espinosa-macias/1820-el-pgn-2027-lo-tecnico-y-sus-contradicciones.html`. Ninguno de los dos firmantes está en `/staff.html`. **Exacto.** El de Cerimedo (SubRaya, 08-09-2026) y «Un mes de ataques…» (Síntesis, «Publicado el: 07 Septiembre 2026», «Por: Tatiana Portela», de plantilla) sí son voz de la casa.

**4 · El barrido** (completo en `revision-externa/barridos/revista-raya.md`).
- **Universo:** SubRaya entera (99, del 2025-11-24 al 2026-10-06) y, además, todo Síntesis, Rayuela y RAYA Investiga dentro de la ventana (71 + 50 + 5). **225 piezas**: 173 antes del 07-08 y 52 después.
- **Su barrido no era el que declara.** Dice «las 99 piezas» de SubRaya, pero 5 de sus 16 entradas son de Síntesis o Rayuela, elegidas sin barrer esas secciones.
- **De sus 16 se sostienen 12** (P o L). No: el salario mínimo (solo identifica a los demandantes), el bombardeo «falso positivo» (atribuido a líderes sociales) y el sepelio (fiscaliza al gobierno en ejercicio): las tres son F. Y **el contenido del Ministerio de Educación no puede contar**: la condición 1 excluye «la propaganda o el contenido pagado».
- **El recuento sistemático:** **35 con postura en la misma dirección**: 22 antes (11 P y 11 leves) y 13 después (8 P y 5 leves). **3 contrapesos, los tres parciales y de antes** (falsos positivos del Ejército en Antioquia, 12-2025; la docente baleada por la Policía en Arauca, 05-2026; el silencio oficial en la frontera, 02-2026). **Ningún contrapeso pleno.**
- **Mínimos:** ≥ 10 → 35 (19 sin leves). ≥ 3 por lado, solo con elogios, disculpas y rótulos → 22 y 13 (11 y 8). ≥ 3:1 → 35:3 (19:3). **Cumple las cinco condiciones.**
- **La prueba del polo fijo.** Los mismos rótulos aparecen a los dos lados: «el héroe de la extrema derecha» (19-12-2025), «Trumpismo colombiano: la estrategia de la derecha para manipular las elecciones de 2026» (14-01-2026), «el linaje conservador antiderechos» (05-03-2026), cuando la derecha era oposición; «dos derechas y un mismo fascismo» (22-08), «para imponer ideología de extrema derecha» (01-09) y «¿por qué la extrema derecha necesita un enemigo muerto y exhibido?» (16-09), cuando gobierna. Antes del cambio la fiscalización apunta a la oposición y a los partidos tradicionales, y la casa defiende al gobierno («La maniobra coincide con una ofensiva política para golpear al Gobierno Petro», 02-12-2025); después, fiscaliza al entrante. Nunca fiscalizó al ejecutivo de Petro mientras gobernaba. **No depende de quién mande.**
- **Lo que no cuenta y se declara:** 37 piezas de terceros en Síntesis y Rayuela («Análisis especial para RAYA», firmas externas, entrevistas, una carta), casi todas contra la derecha y ninguna en sentido contrario; las 13 pagadas; las columnas. Es **selección**, no voz.

**¿Es la financiación del gobierno saliente «nivel 1 con posición conocida»? No.**
- **El §2 del protocolo:** el nivel 1 es «**Propiedad documentada** — Quién controla la empresa, con fuente citable y persona natural». Los contratos de coproducción y el contenido pagado dicen quién paga, no quién controla. RAYA es una fundación con dirección electa por su equipo («Los cargos de dirección, incluyendo la editorial, se eligen mediante votación de quiénes integramos el equipo», `/financiacion.html`). Nada de eso da a Inravisión ni al ministerio control sobre la fundación.
- **«CONTRATACIÓN PÚBLICA»:** «Es **desvelamiento, no acusación** … No mueve la clasificación por sí sola. Si los editoriales elogian a quien contrata, eso se declara como tensión».
- **El polo fijo:** cobrar del gobierno de turno no es orientación; lo que se mide es la asimetría a través del cambio. Y esa asimetría **ya está medida**, por el barrido, sin necesidad de la financiación.
- **Los precedentes:** Telecafé (tanda 6): «pauta informativa pagada y queda como tensión», y 0,00. Ecos del Combeima (tanda 7): la pauta informativa vendida fue motivo para **no dar de alta**, no evidencia del eje. El Informador (tanda 7): los contratos con la Alcaldía y los editoriales que elogian al alcalde entraron como **tensión**; lo que lo llevó a +0,45 fue el **endoso**, no los contratos. RAYA se trata igual: **tensión declarada**, y el tope sigue.
- **¿Hubo contratos o contenido pagado del gobierno nuevo?** No consta (punto 1). Si lo hubiera, sería la misma tensión con el otro signo, y tampoco movería el eje.
- **La consecuencia:** el tope de ±0,30 rige, y el −0,55 no tiene base en ninguna lectura.

**5 · Dirección.**
- `/staff.html` (2026-10-10): «Edinson Arley Bolaños — Cofundador, integrante del consejo directivo, director de la Revista RAYA», y su biografía: «fue parte del proyecto … de la Revista CAMBIO». «Fabiola León Posada — Editora general de la Revista RAYA y defensora del lector». «Caballero»: 0 coincidencias. **Exacto.**
- `/manifiesto.html`: «Otros fundadores: Pablo Navarrete, Cristian Garavito, Isabel Caballero Samper, Maria Camila Diaz». **Exacto.** Que Isabel Caballero venga de Cambio no se puede verificar sin cambiocolombia.com (vetado): se retira.
- SembraMedia (actualizado el 20-10-2025) da 4 fundadoras y 5 fundadores y como directores a Bolaños («editorial»), al editor web, a la editora gráfica y a una productora. Son nueve fundadores, pero no todos periodistas: el staff incluye a un ingeniero de sistemas y a una diseñadora. **«Nueve periodistas» → «nueve fundadores».**
- El dato sobre el periodista que fue director de comunicaciones de un ministerio es literal en `/staff.html`, pero **no dispara aviso de quien dirige**: es un cargo pasado de un periodista, no de quien dirige ni de quien tiene la autoridad editorial.

**6 · Rectificación judicial.**
- **El Colombiano** (`datePublished` 2026-07-31), literal: «los medios accionados tergiversaron la información para presentar a La Silla Vacía como un aliado o agencia digital del denominado “Proyecto Júpiter” y que la supuesta alianza para manipular las elecciones o deslegitimar al Gobierno Nacional no fue demostrada ni siquiera de manera indiciaria»; «la Revista Raya distorsionó sus respuestas para sugerir una contradicción inexistente»; «El fallo judicial con fecha del 30 de julio de 2026». **Exacto.**
- **RAYA lo publicó:** la pieza del 21-04-2026 lleva arriba «* Nota de rectifiación ordenada por la Sala Penal del Tribunal Superior de Bogotá en su fallo de tutela, con radicado No. 2026-00219-01» y al final «De conformidad con lo dispuesto en la sentencia del 30 de julio de 2026, Inravisión – Sistema de Medios Públicos y la Fundación Revista RAYA proceden a realizar la rectificación ordenada respecto de las publicaciones efectuadas los días 19, 21 y 26 de abril de 2026». Y subraya que el Tribunal «dejó en firme los programas». **Exacto**, incluido el contrapeso que anota el revisor.
- **Lo que no dice:** la pieza del 05-06-2026, «Justicia le da la razón a RAYA y Señal Colombia: niega tutela con que La Silla Vacía buscaba censura», era de **primera instancia** («La decisión es de primera instancia y puede ser impugnada») y **no lleva nota** de que el Tribunal ordenó después rectificar.
- **Nivel:** sentencia, nivel 3, y hecho de los últimos 12 meses. Entra en la ficha como hecho; **no levanta el tope** (solo lo levantan el endoso y el nivel 1 con posición).

**7 · Nivel 2.** La medición del envío (2026-10-10, ventana 2026-08-31 → 2026-10-10): «29 | 1 | 1 | 100 % | 0 | — | —». La ficha (2026-09-08) dice 8 artículos, 3 historias y un perfil temático en sextos (16,7 % y 50 %): el «25,9×» es una pieza. Vale la del envío, y ninguna mueve el número.

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se corrigen estas partes:
- **Obj. 1 y 4, «nivel 1» por la financiación:** no es nivel 1 (§2: control, no pago). Es contratación pública y tensión.
- **Obj. 2, «tres piezas»:** son siete del Ministerio, más seis del CNE.
- **Obj. 4, el recuento:** el punto 10 (Ministerio) no puede contar (condición 1); los puntos 4, 11 y 16 son solo fiscalización (precisión del 2026-10-09). El barrido no era solo de SubRaya. El recuento sistemático da 35 frente a 3, no 16 frente a 0.
- **Obj. 4, «contrapesos»:** las piezas sobre Ismael Peña no se cuentan en ningún sentido (no consta su relación con el gobierno saliente); los tres contrapesos parciales que sí hay no los vio.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente ni cita inventada.** Los cuatro procesos de SECOP, la fila del RUES, las citas de Infobae, El Colombiano, el staff, el manifiesto, la financiación y las piezas son literales. Lo que hay:
- un titular citado con una palabra de más («qué logró en la educación superior»);
- «tres» piezas pagadas donde hay siete, y la alianza con el CNE sin ver;
- un barrido que se presenta como de SubRaya y mezcla piezas de otras secciones elegidas a mano.

**Errores de la propia ficha, para no repetirlos:**
- **La cabecera dice −0,55 y el registro lleva «sin medir» desde el 2026-09-18.** La ficha no se actualizó con la decisión del 2026-09-16, y el envío salió con el valor viejo. Es el error que hizo atacar al revisor un número que no existe.
- **«No admite publicidad dentro del contenido editorial»:** desmentido por 13 piezas pagadas en 2026, declaradas por el propio medio.
- **La financiación sin el primario del presente:** cita a SembraMedia, autodeclarado, y no a SECOP, donde hay $2.661.895.000 contratados con Inravisión. **Sin la línea de contratación pública**, obligatoria desde el 2026-10-07.
- **«Su director y su editora vienen de Cambio»:** la editora general es otra persona; Isabel Caballero es cofundadora y no está en el staff; su paso por Cambio no se puede verificar.
- **«Nueve periodistas»:** nueve fundadores, no todos periodistas.
- **El ARGUMENTO, sobre columnas de terceros:** tres de los siete titulares son columnas, que la regla del 2026-10-09 excluye. La ficha no miró las secciones propias, donde estaba la evidencia.
- **El nivel 2 del 2026-09-08**, caducado, y el «25,9×» sobre una pieza.
- **El punto 3 del CONTRA** («Cerimedo trabaja abiertamente para candidaturas de esa familia política… la etiqueta que el propio actor reivindica»): sin fuente. Se retira o se le pone fuente.
- **Lo que la ficha sí tenía bien:** que la inspección de 2023 no cuenta por la regla del presente; que la especialidad en conflicto armado es formato, no eje; y que siete titulares no sostienen «sostenidamente».

---

**Propuesta para la firma**

**Valor: de «sin medir» a −0,30, izquierda moderada, provisional y sin firmar.**
- **Por qué sale de «sin medir».** El «sin medir» del 2026-09-16 se puso porque el volumen del corpus no permitía medirla, y el registro lo dice así: «el volumen que publica no permite medirla». La regla del 2026-10-09 mide el archivo del medio y no el corpus, y «se aplica a la vez a todas las fichas afectadas». El barrido cumple las cinco condiciones con margen. Dejarla sin medir teniendo esto delante sería lo que la regla vino a corregir.
- **Por qué no pasa de −0,30.** Ni endoso de la casa (la única petición de voto es una columna firmada) ni nivel 1 con posición conocida (la financiación es contratación, no control). La autodeclaración «progresista» es nivel 4. La sentencia es nivel 3, pero no levanta el tope. Rige el §1: «la magnitud no pasa de ±0,30».
- **Por qué −0,30 y no −0,25.** La asimetría es completa: ningún contrapeso pleno en 12 meses y los mismos rótulos a los dos lados del cambio. Archipiélago Press llegó a +0,30 con 26 piezas y sin endoso; aquí son 35 (19 sin leves). El País (−0,25) se apoya en cinco editoriales que fiscalizan a los dos gobiernos; Abra Noticias se quedó en 0,00 porque su barrido no llegó a 10.
- **Alternativas declaradas:** **−0,25** si el responsable editorial pesa más que 16 de las 35 son leves y que la codificación es de un solo lector de la misma casa (regla 2). **Seguir «sin medir»** solo si el responsable editorial decide expresamente que los no noticiosos quedan fuera de la regla del 2026-10-09; en ese caso hay que escribirlo. **−0,55 no lo sostiene ninguna lectura.**

**Lo que cambia en código y fichas si se aplica** (los aplica quien el responsable editorial decida; aquí no se toca nada):

En `shared/mediaRegistry.js` (entrada `revista-raya`):
- `bias: null` → `bias: -0.30`; `reviewedAt: null` se queda.
- El comentario «SIN MEDIR — decisión del responsable editorial del 2026-09-16…» se conserva como historia y se añade debajo: «2026-10-10 (ciclo 2, tanda 8): −0,30 por el barrido de la voz de la casa (`revision-externa/barridos/revista-raya.md`); tope de ±0,30 por falta de endoso y de nivel 1 con posición».
- `biasRationale`: «Fundación de periodistas de investigación (Bogotá), no noticiosa. Izquierda moderada, −0,30, por el barrido de 12 meses de sus secciones propias (10-10-2026): 35 piezas con postura en voz de la casa, todas en la misma dirección —22 antes del 07-08 y 13 después—, frente a 3 contrapesos parciales; los mismos rótulos («extrema derecha», «antiderechos») con la derecha en la oposición y en el gobierno. Sin endoso de la casa: tope de ±0,30. TENSIÓN: Inravisión (RTVC) le contrató $2.661.895.000 entre 2025 y 2026, y publicó 7 piezas pagadas por el Ministerio de Educación que elogian al gobierno saliente. Rectificación judicial ordenada el 30-07-2026 por su serie del «Proyecto Júpiter». Ver fichas/revista-raya.md.» (Sin «SIN MEDIR».)

En `shared/sinMedir.test.js`: `SIN_MEDIR_DECIDIDOS` pasa a `['voragine', 'cuestion-publica', 'rtvc']`, y los textos que dicen «cuatro» pasan a «tres». Si no, la prueba falla, que es para lo que está.

En `shared/biasAnalysis.js` (comentario de `classifySpectrum`, línea 627): «marcó «sin medir» a Vorágine, Cuestión Pública, Revista RAYA y RTVC» se conserva como historia, con «(RAYA salió el 2026-10-10 con su barrido)».

`src/docs/catalogo_medios.txt`, línea 748: «Revista RAYA · sesgo sin medir» → «−0,30». Si se genera, regenerar.

En `shared/mediaOwnership.js`, entrada `revista-raya` (`ownerType: 'independiente'` se queda: es una fundación de periodistas y nadie con posición conocida la controla):
- `holdings[0]` → «FUNDACIÓN REVISTA RAYA, NIT 901644009-8, matrícula 90061613 de la Cámara de Comercio de Bogotá (desde el 30-09-2022), ACTIVA, renovada el 15-05-2026. Fundación sin ánimo de lucro de nueve fundadores; la dirige Edinson Bolaños, y la editora general y defensora del lector es Fabiola León Posada. Los cargos de dirección, también el editorial, los elige el equipo por votación.»
- `holdings[1]` → «Se financia con servicios a organizaciones sin ánimo de lucro, consultoría, micromecenazgo, donaciones y producción de contenidos para otros medios (SembraMedia, autodeclarado, 20-10-2025), y con coproducción y alianzas con entidades públicas, que declara al pie de cada pieza. No cobra por leer.» (Sale «ni admite publicidad dentro del contenido editorial».)
- `notes`, añadir:
  - «Contratación pública (SECOP I y II, NIT 901644009, consultado 2026-10-10): 1 contrato por $1.361.295.000 contratados en los últimos 12 meses (2025-10-10 → 2026-10-10); 4 por $2.661.895.000 en total desde 2025. Contratante único: Inravisión – RTVC, sistema de medios públicos del Estado, cuya gerencia depende del gobierno nacional, que el medio cubre. Son coproducciones de Señal Investigativa, Señal Investigativa Debates y el programa de opinión Parte y Contraparte (régimen especial). El de 2026, previsto hasta el 31-12-2026, figura «terminado» con actualización del 04-08-2026. SECOP I: 0. Es valor contratado: SECOP marca 0 pagado.»
  - «CONTENIDO PAGADO EN SECCIÓN EDITORIAL: 7 piezas de Síntesis (17-07 a 06-08-2026) de una «alianza entre Revista RAYA y el Ministerio de Educación Nacional, con recursos destinados a su producción y divulgación», con titulares que celebran al gobierno saliente («el legado del Cambio», «la revolución educativa del Gobierno del Cambio»); y 6 de pedagogía electoral financiadas por el CNE (27-05 a 20-06-2026). Las declara al pie. Ninguna alianza consta en SECOP bajo su NIT.»
  - «TENSIÓN DECLARADA: bajo el gobierno saliente defendió a su contratante («Justicia le da la razón a RAYA y Señal Colombia», 05-06-2026); bajo el entrante, su editora general titula contra la nueva gerencia de Inravisión («Gobierno De la Espriella pone mordaza», 23-08-2026). Desvelamiento, no acusación.»
  - «RECTIFICACIÓN JUDICIAL: el 30-07-2026 la Sala Penal del Tribunal Superior de Bogotá ordenó a Inravisión y a la Fundación Revista RAYA rectificar las piezas del 19, 21 y 26-04-2026 sobre La Silla Vacía y el «Proyecto Júpiter» (radicado 2026-00219-01; El Colombiano, 31-07-2026). RAYA publicó la rectificación; el Tribunal no ordenó retirar los contenidos.»
  - La nota de la inspección de 2023 se queda, como está.
- `sources`, añadir: `https://revistaraya.com/manifiesto.html`, `https://revistaraya.com/financiacion.html`, la consulta del RUES y la de SECOP II con `$select` de arriba (como texto los procesos), `https://www.elcolombiano.com/inicio/rtvc-raya-retractar-la-silla-vacia-proyecto-jupiter-AG39485115`, `https://revistaraya.com/juanita-leon-cambia-de-version-cuatro-veces-sobre-participacion-de-la-silla-vacia-en-el-proyecto-jupiter.html` y `https://revistaraya.com/cuatro-anos-de-gratuidad-en-la-universidad-publica-que-logro-en-la-educacion-superior-en-el-gobierno-petro.html`. La de La Silla Vacía (2022) no se ha podido comprobar en este ciclo (dominio vetado para el verificador); la sustituye el RUES.
- `verifiedAt: VERIFICADO_AGO` → **`'2026-10-10'`** cuando estén aplicadas estas correcciones (hasta entonces, lo que dice `holdings` no está verificado).
- `controlGroup 'raya-fundacion'`: `label` «Fundación RAYA — sus nueve periodistas fundadores» → «Fundación Revista RAYA — nueve fundadores, dirección elegida por el equipo»; `personas[0]`: `nombre` «Edinson Bolaños, con otros ocho fundadores», `papel` «Fundadores de la fundación sin ánimo de lucro; Bolaños es cofundador, integrante del consejo directivo y director.», `fuentes` + `https://revistaraya.com/manifiesto.html`.

En `fichas/revista-raya.md`:
1. **Cabecera:** «Valor actual | −0,55» → «Valor actual | **sin medir** (`bias: null`, decisión del 2026-09-16)» y «Valor propuesto | **−0,30**, izquierda moderada, provisional (barrido, `revision-externa/barridos/revista-raya.md`)». Nueva fila «Contratación pública» con la línea de arriba.
2. **Nivel 1:** retirar «nueve periodistas», «su editora», «ambos procedentes de la revista Cambio» y «ni admite publicidad dentro del contenido editorial»; poner los datos del RUES, la dirección y la editora general de `/staff.html` y la dirección electa de `/financiacion.html`. El párrafo «Un dato de procedencia…» queda solo para el director, con su fuente.
3. **Sección nueva «CONTRATACIÓN PÚBLICA Y CONTENIDO PAGADO»**: la línea del protocolo, los cuatro procesos como texto, las 7 piezas del Ministerio y las 6 del CNE, y la tensión con Inravisión. Desvelamiento, no acusación; no mueve el eje.
4. **Nivel 3 / 5 (hechos de 12 meses):** la rectificación judicial del 30-07-2026, con la nota de RAYA, y que la pieza del 05-06 no lleva nota de la segunda instancia.
5. **Nivel 2:** la medición del envío (29 / 1 / 1, 40 días) en lugar de la del 2026-09-08; retirar el «25,9×» del ARGUMENTO.
6. **ARGUMENTO:** sustituir los siete titulares por el resumen del barrido (35 frente a 3; 22 y 13; los rótulos a los dos lados), con el enlace al barrido, y por qué el tope (sin endoso, sin nivel 1 con posición).
7. **CONTRA:** el 1 cambia (ya no es «todo lo que hay es de un mes»: es un solo codificador de la misma casa y 16 leves); el 2 se queda; el 3 se retira o se le pone fuente; el 4 se reescribe: Vorágine y Cuestión Pública siguen sin medir y se barren con la misma regla; añadir que 37 piezas de terceros y 13 pagadas no cuentan.
8. **REFUTACIÓN:** «Si en los próximos seis meses la casa publica piezas propias con rótulo contra la izquierda o elogio al Gobierno De la Espriella en proporción mayor de 1 a 3»; «Si aparece un contrato o contenido pagado del gobierno entrante y la casa cambia de tono con él» (sería tensión con el otro signo); «Si un segundo lector recodifica el barrido y no llega a los mínimos».
9. **REVISIÓN EXTERNA:** esta resolución, con modelo, versión y fecha.

Las fichas que se comparan con RAYA, y que hay que tocar si el valor cambia:
- `fichas/voragine.md` (líneas 12-17, 144, 160, 171): habla del trío «−0,50, −0,45, −0,55». Añadir que RAYA salió del «sin medir» con un barrido del archivo y que Vorágine y Cuestión Pública deben pasar por el mismo (lo dice la regla: «se aplica a la vez a todas las fichas afectadas»).
- `fichas/volcanicas.md` (línea 78): «Vorágine −0,50, Revista RAYA −0,55, Cuestión Pública −0,45» ya era falso desde el 2026-09-18 (las tres sin medir); con esto, «Revista RAYA −0,30 (barrido), Vorágine y Cuestión Pública sin medir».
- `fichas/colombia-informa.md` (línea 243): cita el error de especialidad de la ficha de RAYA; no cambia.
- `PLAN_PRODUCTO_FINAL.md` (3.5): historia; no se toca.

**Comparación con los vecinos de la escala** (para que la decisión se vea entera): con −0,30, RAYA queda **a la derecha** de Volcánicas (−0,50), Razón Pública (−0,40), Cambio (−0,40), Las2Orillas (−0,35) y CasaMacondo (−0,35). Volcánicas y CasaMacondo tienen el número por su misión declarada (nivel 4), sin barrido. **No es que RAYA sea más moderada que ellos**: es que es la primera de ese grupo con un número medido y con tope. Conviene barrer a esos con la misma regla antes de leer el orden.

**Lo que NO entra como hecho:**
- que algún contrato o alianza haya comprado una pieza concreta o una línea;
- por qué se terminó el contrato 304-2026, y que RAYA Investiga sustituya a Señal Investigativa;
- por qué vía pagó el Ministerio de Educación;
- la relación de Ismael Peña con el gobierno saliente;
- que Isabel Caballero venga de Cambio;
- el contenido de la fuente de La Silla Vacía de 2022 (dominio vetado para el verificador);
- la valoración que hace El Colombiano de RAYA al describirla; solo se toma el fallo que reporta.

**¿Aviso de quien dirige?** No procede. No consta candidatura ni cargo público vigente del director ni de la editora general.

**Decisiones para el responsable editorial:**
1. **Valor.** Recomendación: **−0,30**, de «sin medir» a número, sin firmar. Alternativas: −0,25 (regla 2, 16 leves y un solo lector) o seguir sin medir (si los no noticiosos quedan fuera de la regla del 2026-10-09, y escribiéndolo).
2. **La financiación pública como nivel 1.** Recomendación: **no**; tensión declarada, igual que Telecafé, Ecos y El Informador. Si el responsable editorial la quisiera como nivel 1, levantaría el tope también para cualquier medio que contrate con su gobierno, y eso contradice el polo fijo.
3. **El contenido pagado del Ministerio de Educación en sección editorial.** Recomendación: anotarlo en la ficha de propiedad como hecho y tensión, y corregir la frase «no admite publicidad». No es motivo de baja: está declarado al pie.
4. **Vorágine y Cuestión Pública** (y los demás no noticiosos). En esta misma tanda hay barridos suyos en curso, de otros verificadores, que esta resolución no ha leído. Recomendación: decidir los seis no noticiosos juntos, con la misma regla, para no tener una para RAYA y otra para ellos.
5. **La decisión del 2026-09-16 en `DECISIONES.md`.** Recomendación: añadir la entrada que falta (trío y RTVC sin medir), con fecha, para que el registro y la ficha no vuelvan a separarse. Y antes de armar un envío, comprobar que la cabecera de la ficha coincide con `bias` en el registro.
6. **Segundo lector.** La clasificación es de un solo lector de la misma casa. Recomendación: que el responsable editorial recuente una muestra del §9 del barrido (por ejemplo, las 35 que cuentan y las 79 F) antes de firmar.
