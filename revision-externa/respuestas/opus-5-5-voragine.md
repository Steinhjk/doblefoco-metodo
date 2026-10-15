# Respuesta — Claude Opus 5.5 sobre Vorágine

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
> **Única edición:** se han retirado dos enlaces a un PDF que muestra números
> de cédula y teléfonos de personas naturales (Ley 1581). Se explica al
> principio de la resolución.

---

## RESPUESTA LITERAL

```
DECLARACIÓN PREVIA DE CONFLICTO
Soy Claude Opus 5.5 (claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Para compensarlo he trabajado casi solo con fuentes que la ficha NO usa: el Informe de Transparencia JTI que el propio medio subió en octubre de 2026, sus estados financieros de 2025 (publicados en septiembre de 2026), sus Directrices Editoriales 2026, la API pública de WordPress de voragine.co (barrido de los 12 meses), RUES y SECOP en datos.gov.co. No he usado la página de SembraMedia ni la de GFMD que cita la ficha. Fecha de todas las comprobaciones: 2026-10-10.

MÉTODO Y DÓNDE BUSQUÉ
- robots.txt de voragine.co (descargado el 2026-10-10): solo «User-agent: *» con Disallow de /sitio/ y /bk-sitio/. No excluye a ClaudeBot, Claude-Web ni anthropic-ai. robots.txt de datos.gov.co: solo restringe /browse con parámetros; la API /resource/ no está excluida.
- HTML y PDF crudos con curl -sL (UA de navegador, --ssl-no-revoke), guardados en t89\voragine-dl:
  · https://voragine.co/nosotros/
  · https://voragine.co/documentacion-legal/
  · https://voragine.co/editorial/ (categoría de editoriales)
  · [enlace retirado: el PDF del Informe de Transparencia JTI muestra números de cédula y teléfonos de personas naturales, Ley 1581; se enlaza desde https://voragine.co/nosotros/] («Fecha del informe: septiembre 29, 2026»)
  · https://voragine.co/wp-content/uploads/2026/09/Estados-financieros-comparativos-2025-2024.pdf
  · https://voragine.co/wp-content/uploads/2026/09/Notas-o-revelaciones-a-los-Estados-Financieros-2025-2024.pdf
  · https://voragine.co/wp-content/uploads/2026/08/Directrices-editoriales-de-Voragine-2026.docx.pdf
- Barrido editorial reproducible: https://voragine.co/wp-json/wp/v2/posts?after=2025-10-10T00:00:00&per_page=100&_fields=id,date,link,title,categories → cabecera x-wp-total: 93 (todas las entradas publicadas entre 2025-10-10 y 2026-10-10). Leí titular, entradilla y firma de todas las piezas con actor político identificable (lista abajo). Categorías: https://voragine.co/wp-json/wp/v2/categories?per_page=100. Búsquedas internas en la misma API con search=Cepeda (7), Petro (24), De la Espriella (17), Uribe (15), Barrientos (1).
- Registros: RUES (c82u-588k), SECOP II (jbjy-vk9h), SECOP I (f789-7hwg), por NIT 901406489 (el NIT que el medio declara en su informe JTI, pregunta 5.a), con igualdad exacta y también con el dígito de verificación pegado (9014064891).
- Buscador web: no lo usé. Todo lo necesario estaba en fuentes primarias; no puedo afirmar si estaba disponible porque no lo invoqué.
- Wikipedia: no consultada.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré nada de eso. Es una ESAL sin accionistas. RUES, consultado el 2026-10-10: https://www.datos.gov.co/resource/c82u-588k.json?$select=razon_social,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,camara_comercio,organizacion_juridica&nit=901406489 → «FUNDACIÓN VORAGINE PERIODISMO CONTRACORRIENTE», «ACTIVA», fecha_matricula «20200831», fecha_renovacion «20260319», ultimo_ano_renovado «2026», «MEDELLIN PARA ANTIOQUIA», «FUNDACIONES». Con el DV pegado (9014064891) la consulta devuelve [].

- La persona que la ficha nombra como titular o director, ¿sigue viva y en el cargo?
  La ficha no nombra director. Nombra a cuatro «fundadores»; dos de ellos (Juan Pablo Barrientos y Francisco Escobar) NO figuran hoy en ningún órgano del medio (ver objeción 1). José Guarnizo, que la ficha cita como fundador, sigue en el cargo: «Cofundador y director general de Vorágine» (https://voragine.co/nosotros/, comprobado el 2026-10-10).

- ¿Quién dirige hoy la redacción?
  José Enrique Guarnizo Álvarez. Informe JTI, fechado el 29-09-2026, pregunta 37: «Director de contenidos y director general: José Enrique Guarnizo Álvarez». En la misma respuesta: «Directora ejecutiva y representante legal: María José Jaramillo Berrío»; «Directora de proyectos: Laila Abu Shihab Vergara»; «Directora gráfica y audiovisual: Angélica María Penagos Zerda».

- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que la ficha cita?
  Sí, varios:
  (a) RUES con renovación del 2026-03-19 (arriba).
  (b) El Informe de Transparencia JTI que subió el propio medio (uploads/2026/10, «Fecha del informe: septiembre 29, 2026»), con la composición de sus órganos (preguntas 24 y 26).
  (c) Los estados financieros de 2025 y sus notas (uploads/2026/09), con los ingresos por financiador.
  La ficha no cita ninguno de los tres.

## OBJECIONES

OBJECIÓN 1 — La ficha da una composición de fundadores y control que no es la vigente, y sobre ella monta el «cruce» con Volcánicas
- QUÉ afirma la ficha: que la fundación la crearon «Juan Pablo Barrientos, Francisco Escobar, José Guarnizo y Laila Abu Shihab», y que «Juan Pablo Barrientos, cofundador de esta fundación» es el cruce con Volcánicas que habría que declarar también en la ficha de Vorágine.
- POR QUÉ es incorrecto (HECHO): el medio declara hoy como «Titulares e integrantes activos de la Asamblea General de Fundadores o Asamblea de Gestores (órgano de administración)» a «María José Jaramillo Berrío – José Enrique Guarnizo Álvarez – Angélica María Penagos Zerda – Laila Abu Shihab Vergara» (Informe JTI, pregunta 24, fechado el 2026-09-29). La Junta Directiva («ad honorem») la forman, como titulares, «Luis Miguel De Bedout Hernández – Carlos Alberto García Molina – Fernando Federico Sarmiento Espinosa» y, como suplentes, «Jaime Flórez Suárez – José Enrique Guarnizo Álvarez – Laila Abu Shihab Vergara» (pregunta 26). En /nosotros/ los cuatro cofundadores que figuran son Guarnizo, Abu Shihab, Jaramillo («Cofundadora y directora ejecutiva y administrativa») y Angie Pik («Cofundadora y directora gráfica»). En el HTML de /nosotros/, «Barrientos» aparece 0 veces y «Escobar» 0 veces (grep sobre el HTML crudo, 2026-10-10).
- HECHO: Barrientos sí publica en voragine.co, pero a través de La Liga Contra el Silencio, no como miembro de Vorágine: https://voragine.co/historias/investigacion/presidente-de-la-corte-constitucional-acuso-a-la-madre-de-su-primogenito-de-haberlo-drogado-y-abusado/ (2026-02-19): «Por: La Liga Contra el Silencio, Juan Pablo Barrientos y José Alejandro Castaño. Nota editorial de la La Liga Contra el Silencio y sus aliados». Es su única aparición en las 93 entradas de los 12 meses (search=Barrientos → 1).
- INFERENCIA: hoy el «cruce» no pasa por la gobernanza de Vorágine. Pasa por la alianza La Liga Contra el Silencio, que el 2026-02-27 se describe así: «no es un medio de comunicación, es una alianza de medios independientes… Hoy somos 16 salas de redacción» (https://voragine.co/comunicado/comunicado-de-disculpas-a-las-audiencias-de-la-liga-contra-el-silencio-y-a-los-medios-estigmatizados/). El aviso que la ficha prevé («Si Barrientos pasa a dirigir la redacción…») apunta a la persona equivocada. Quienes controlan hoy la ESAL son los cuatro gestores citados, y la ficha omite a dos de ellos, entre ellos a la representante legal. Además, la ficha da el 1 de junio de 2020 como fecha de creación de la fundación; según el medio, esa es la fecha de lanzamiento del portal y la persona jurídica se constituyó después: «lanzamos públicamente el medio (1 de junio de 2020) antes de la constitución de la persona jurídica (31 de agosto de 2020)» (JTI, pregunta 16.a). Las notas a los estados financieros dicen: «constituida… por Acta del 16 de junio de 2020… inscrita en la Cámara de Comercio de Medellín el 31 de agosto de 2020».
- FUENTE y FECHA: Informe JTI, [enlace retirado: el PDF del Informe de Transparencia JTI muestra números de cédula y teléfonos de personas naturales, Ley 1581; se enlaza desde https://voragine.co/nosotros/] (2026-09-29); https://voragine.co/nosotros/ (consultado el 2026-10-10).
- NIVEL: propiedad / declaración del propio medio.

OBJECIÓN 2 — «Una lista de aliados que rota» no describe la financiación real: está concentrada en cuatro donantes, con un gobierno extranjero y una agencia de la ONU
- QUÉ afirma la ficha: que «el nivel 1 aquí no termina en un dueño, sino en una lista de aliados que rota», con «un modelo en el que quién paga cambia pieza a pieza». No nombra a ningún financiador salvo la nota de Vital Strategies que vio en una pieza.
- POR QUÉ (HECHO): las notas a los estados financieros de 2025 (publicadas en septiembre de 2026) dan unos ingresos totales de 890.653.573 COP (157.594.000 operacionales + 733.059.573 no operacionales). Bajo «Por tercero diversos, donaciones», con cifras de 2025 y 2024:
  «SUBVENCIONES-Vital Strategies, Inc. 255,910,041 141,292,850»
  «SUBVENCIONES-Wellspring Philanthropic Found Inc 159,841,815 153,749,663»
  «SUBVENCIONES-Climate and land use alliance 71,240,439 118,734,065»
  «SUBVENCIONES-Rockefeller Philanthropy Advisors Inc 55,126,283 195,180,691»
  «SUBVENCIONES-Emabaja del Canadá 49,479,131 27,857,142» [sic]
  «SUBVENCIONES-Fundacion Connectas 17,298,645 24,237,777»
  «VAKI 28,381,191 15,660,354»
  Y bajo «Por tercero talleres»: «OFICINA DE LAS NACIONES UNIDAS CONTRA LA DROGA Y EL DELITO 67,620,000». Bajo «Por tercero publicaciones»: «BANCOLOMBIA SA 38,205,000» (las columnas del PDF están desalineadas en esa tabla; cito solo las filas que se leen sin ambigüedad).
- CÁLCULO (mío, reproducible con esas cifras): Vital Strategies = 28,7 % del ingreso total de 2025. Vital Strategies, Wellspring, CLUA y Rockefeller Philanthropy Advisors suman el 60,9 %. Las cuatro aparecen en 2024 y en 2025, así que no es un patrocinio que cambie pieza a pieza: es una base estable de cuatro grant-makers estadounidenses, más la cooperación de un gobierno extranjero (Canadá). El propio medio, en el JTI (pregunta 49, datos de 2023), dice que «el 52,3% corresponden a grants o subvenciones internacionales que financian la operación en general del medio»: apoyo institucional, no por pieza.
- Lo que NO hay (HECHO): no contrata con el Estado colombiano. «No contratamos con el Estado colombiano, en ningún nivel» (/nosotros/), y lo confirman SECOP II y SECOP I (ver «Evidencia que no mueve el número»).
- Por qué importa, aunque «el dueño no determina la orientación»: la ficha tiene que declarar quién la sostiene, y hoy no lo hace con nombres. Esto no mueve el número por sí solo.
- FUENTE y FECHA: https://voragine.co/wp-content/uploads/2026/09/Notas-o-revelaciones-a-los-Estados-Financieros-2025-2024.pdf (ejercicio 2025, subido en 2026-09); Informe JTI (2026-09-29).
- NIVEL: propiedad / registro financiero publicado por el medio.

OBJECIÓN 3 — El mayor financiador sostiene una línea temática continua y declarada, y la ficha la trata como una anécdota
- QUÉ afirma la ficha: que la nota «funded… by Vital Strategies» es una nota de financiación en una de cinco piezas.
- POR QUÉ (HECHO): en las 93 entradas de los 12 meses, 17 llevan la leyenda de Vital Strategies (búsqueda literal «Vital Strategies» en el contenido devuelto por la API, 2026-10-10). Van desde «Los conflictos de interés de la Sociedad Colombiana de Pediatría» (2025-10-16) hasta «Briceño y los intereses detrás de la ofensiva contra los impuestos saludables» (2026-09-27), pasando por la serie Coca-Cola / La Calera y los sellos octagonales, en español y en inglés. La leyenda dice: «Esta investigación fue financiada, en parte, por Vital Strategies. El contenido es editorialmente independiente y su propósito es arrojar una luz tanto sobre las prácticas ilegales o poco éticas de la industria de alimentos y bebidas…» (https://voragine.co/historias/investigacion/briceno-y-los-intereses-detras-de-la-ofensiva-contra-los-impuestos-saludables/, 2026-09-27).
- INFERENCIA: es una agenda temática (salud pública frente a la industria de alimentos y bebidas) que fija el financiador, que se declara y que dura todo el año: el 18 % de lo publicado. No es izquierda ni derecha por sí misma, y no la uso para mover el número. Pero la ficha debe declararla como lo que es: una línea editorial patrocinada y estable, no un patrocinio que rota. La pieza de Briceño apunta a un representante del Centro Democrático y, en la entradilla, al «gobierno de de La Espriella». La causa del financiador coincide aquí con un blanco de un solo lado del espectro, y eso hay que vigilarlo.
- FUENTE y FECHA: las URL de la API citadas en el método; pieza del 2026-09-27.
- NIVEL: hecho editorial de los últimos 12 meses / declaración del propio medio.

OBJECIÓN 4 — El −0,50 no tiene ningún apoyo. El barrido de 12 meses muestra que fiscaliza al gobierno de turno a los dos lados del cambio, con un desequilibrio entre candidatos que no alcanza el umbral de la regla
- QUÉ afirma la ficha: que no hay argumento para −0,50 («ARGUMENTO — no lo hay»). Coincido, pero la ficha no hace el barrido que lo comprobaría. Aquí está.
- BARRIDO (HECHO, reproducible con la URL de la API del método; fecha, titular y ruta literales):
  A) Piezas contra el gobierno de Petro, ANTES del 07-08-2026 (fiscalización del gobierno de turno):
   1. 2025-11-23 «El alto funcionario del Gobierno Petro señalado en la JEP de nexos con paramilitares» /historias/investigacion/el-alto-funcionario-del-gobierno-petro-senalado-en-la-jep-de-nexos-con-paramilitares/
   2. 2026-02-01 «César Manrique: el prófugo al que Petro le ha dado poder dos veces» /historias/perfil/cesar-manrique-el-profugo-al-que-petro-le-ha-dado-poder-dos-veces/
   3. 2026-02-16 «Ministerio de Educación: denuncian presiones a trabajadores para marchar» (marcha «para apoyar al presidente Gustavo Petro») /historias/investigacion/ministerio-de-educacion-denuncian-presiones-a-trabajadores-para-marchar/
   4. 2026-03-07 «26.000 millones en contratos del gobierno a fichas del condenado exsenador Pulgar» (MinInterior «en cabeza de Armando Benedetti»; firma José Guarnizo, el director) /historias/investigacion/26-000-millones-en-contratos-del-gobierno-a-fichas-del-condenado-exsenador-pulgar/
   5. 2026-04-19 «Laura Sarabia y su red de poder: los nombramientos que todavía la persiguen» /historias/investigacion/laura-sarabia-y-su-red-de-poder-los-nombramientos-que-todavia-la-persiguen/
  B) Piezas contra la derecha que estaba en la oposición o en campaña, ANTES del 07-08-2026:
   1. 2025-10-19 «El "Gury" tiene contratado a un exescolta de alias La Madrina» («El concejal uribista de Medellín»)
   2. 2025-11-30 «Santiago Uribe, empresarios y narcos fueron asociados de una temida Convivir»
   3. 2026-01-25 «La apuesta de De la Espriella: arruinar periodistas para silenciarlos»
   4. 2026-02-15 «La tierra de un narcoparamilitar que pasó a manos de Abelardo de la Espriella»
   5. 2026-02-22 «Campesinos firmaron engañados: denuncias contra minera que financió a Paola Holguín»
   6. 2026-03-22 «La chequera uribista que ha impulsado el proyecto político de Oviedo»
   7. 2026-05-24 «Asesor de "Gury" Rodríguez estuvo en la escena de un presunto secuestro» («del Centro Democrático»)
   8. 2026-05-30 «La socia de Abelardo que hizo negocios con un lavador de la mafia»
   9. 2026-05-31 «En campaña de De la Espriella hay miles de funcionarios inscritos…» (firma una alianza: «Cuestión Pública, Vorágine, Rutas del Conflicto, El Veinte y… CLIP»)
   10. 2026-07-10 «Falsos positivos y presunta corrupción: los generales del empalme de De la Espriella» (ya presidente electo)
   11. 2026-07-29 «Acoso y nexos con paras: los señalamientos a los nuevos voceros de Abelardo de la Espriella» (presidente electo)
   12. 2026-08-07 «El negocio del vocero de Abelardo con "el Hombre Malboro", un narco guajiro» (publicada el día de la posesión)
   Además, con postura explícita: 2026-03-08 «#NoAlPactoDeSilencio: 171 mujeres con 20 preguntas para el expresidente Andrés Pastrana Arango» (categoría «comunicado», «Por: Laila Abu Shihab Vergara», directora de proyectos y gestora de la ESAL).
   Piezas contra el candidato de la izquierda (Iván Cepeda / Pacto Histórico) en campaña: NO encontré ninguna en los titulares de las 93 entradas. La búsqueda search=Cepeda devuelve 7 entradas, y ninguna es una investigación sobre él o su campaña (2026-05-28 cómic sobre la Amazonía y «los candidatos»; tres piezas de 2026-05-17 sobre violencia política digital contra mujeres; el comunicado de la Liga del 2026-02-27; la pieza de MinEducación; el análisis sobre Venezuela del 2026-01-11; la pieza del 2025-11-23). Solo leí titulares y entradillas de esas siete.
  C) Piezas contra el gobierno de De la Espriella, DESPUÉS del 07-08-2026:
   1. 2026-08-15 «Los campesinos heridos que De La Espriella no mencionó sobre su primer bombardeo»
   2. 2026-09-20 «Asesinatos contra personas trans: aumenta la violencia y el gobierno desprotege» (el titular de la casa adopta la conclusión)
   3. 2026-09-27 «Briceño y los intereses detrás de la ofensiva contra los impuestos saludables» (contra un representante del Centro Democrático y créditos del «gobierno de de La Espriella»; financiada en parte por Vital Strategies)
   4. 2026-10-04 «Una niña bajo fuego y un asesinato: la denuncia contra el Ejército en Meta»
  D) Piezas contra la izquierda DESPUÉS del 07-08-2026: ninguna (la izquierda ya no gobierna).
- LECTURA según la regla del polo fijo:
  (HECHO) Vorágine fiscalizó al gobierno saliente (A: 5 piezas; una la firma el director) y fiscaliza al entrante (C: 4 piezas). No encontré ninguna pieza que celebre a un gobierno. Es el patrón que el protocolo describe como «periodismo… orientación mixta».
  (INFERENCIA) La única asimetría visible está en la campaña: unas 12 investigaciones sobre la derecha (sobre todo De la Espriella) frente a 0 sobre el candidato de la izquierda. Es «encuadre asimétrico entre candidatos», que el protocolo admite como evidencia. Pero tiene un confusor documentado por el propio medio: De la Espriella era el puntero y luego presidente electo, y la pieza del 2026-01-25 cita a la Flip con «109 denuncias por injuria y calumnia de De la Espriella contra periodistas entre 2008 y 2019». Es decir, era a la vez el candidato con más opciones de poder y el principal litigante contra la prensa.
  (APLICACIÓN DE LA REGLA DEL 2026-10-09) Casi todas las piezas de B y C son investigación, es decir, fiscalización, que no cuenta. Las «piezas con postura» de la voz de la casa que encuentro son pocas: el comunicado sobre Pastrana (2026-03-08), el titular «el gobierno desprotege» (2026-09-20) y el comunicado de la Liga (2026-02-27). No hay editoriales en la ventana (ver «Evidencia que no mueve el número»: la sección Editorial tiene una sola entrada en toda su historia). No llegan a 10 piezas con postura ni a 3 por lado del cambio. LA REGLA NO SE CUMPLE, y esta asimetría NO autoriza a mover el número a −0,50 ni a mantenerlo ahí.
- CONCLUSIÓN de la objeción: no hay evidencia admisible que sostenga −0,50. La única evidencia nueva y fechada a los dos lados del cambio (A y C) es continuidad fiscalizadora, que el protocolo lee como mixta. La asimetría entre candidatos queda por debajo del umbral y tiene un confusor. Con la regla «ante la duda… la más cercana a la mixta», el −0,50 no se sostiene. Esto refuerza la tercera salida que propone la propia ficha («sin medir») o un valor más cercano al centro. No apoya mantener la cifra.
- FUENTE y FECHA: API de voragine.co (93 entradas, del 2025-10-10 al 2026-10-10), consultada el 2026-10-10; cada pieza con su fecha arriba.
- NIVEL: hecho editorial de los últimos 12 meses (nivel 5) + conducta observable.

OBJECIÓN 5 — El hueco del corpus es más grave de lo que la ficha dice, y se come justo las piezas políticas
- QUÉ afirma la ficha: 5 artículos en 30 días; el envío dice 4 artículos y 0 historias en la ventana del 2026-08-31 al 2026-10-10.
- POR QUÉ (HECHO): en esa misma ventana voragine.co publicó 9 entradas, según la API: 2026-08-31 (2), 09-01, 09-06, 09-08, 09-20, 09-27, 10-04 y 10-07. El corpus capturó 4 de 9. Si las 4 capturadas son las de la ficha hasta el 09-08, faltan 09-20 (gobierno de De la Espriella y personas trans), 09-27 (Briceño / Centro Democrático), 10-04 (Ejército) y 10-07 (periodista asesinado). Esto último es inferencia: no veo el corpus.
- INFERENCIA: el hueco no es neutral. Las piezas que no entraron son precisamente las que permitirían ver la conducta posterior al cambio de gobierno. Esto confirma y amplía el «es nuestro y no suyo» de la ficha.
- FUENTE y FECHA: API de voragine.co, 2026-10-10.
- NIVEL: conducta observable (frente a la ingesta propia).

## LO QUE NO PUDE VERIFICAR

- Si Francisco Escobar tuvo alguna vez un papel fundacional: no encontré su nombre en /nosotros/, ni en el JTI de 2026-09, ni en /documentacion-legal/. No busqué en fuentes de terceros. No afirmo que la ficha se equivoque sobre el pasado; afirmo que hoy no figura (objeción 1).
- El papel actual de Barrientos en Volcánicas: no lo comprobé (no visité volcanicas.com). Solo verifiqué que no está en los órganos de Vorágine.
- El conversatorio del 2026-08-12 («La Séptima: una carrera por la memoria») dice que el proyecto lo lideran «la Fundación Carlos Urán, Vorágine y la revista Cambio, con el apoyo de la Consejería Distrital de Paz». No pude determinar si hubo dinero público hacia Vorágine, lo que chocaría con «No contratamos con el Estado colombiano». SECOP no registra contratos con el NIT de Vorágine (abajo), pero el apoyo pudo ir a otra entidad del consorcio.
- La tabla «Por tercero publicaciones» de las notas de 2025 está desalineada en el PDF: no atribuyo con seguridad las cifras de EarthRights, FIAN, Cinep, Brújula ni La Liga.
- Leí completas pocas piezas. La clasificación A/B/C se basa en titular, entradilla y firma, no en un análisis del cuerpo.
- No comprobé quiénes son los tres titulares de la Junta Directiva más allá del nombre que da el medio. No afirmo nada sobre ellos.

## LO QUE FALTA

- La gobernanza vigente con fuente fechada: los cuatro gestores, la Junta Directiva y el director general Guarnizo (Informe JTI del 2026-09-29), en lugar de la lista de cofundadores.
- Los financiadores con nombre y peso (estados financieros de 2025): Vital Strategies 28,7 %; los cuatro grant-makers, 60,9 %; Embajada de Canadá; UNODC; Bancolombia. Y la declaración de que no contrata con el Estado.
- Que es miembro de La Liga Contra el Silencio (alianza de 16 salas) y que copublica con Cuestión Pública, que es uno de los dos medios con los que la ficha la compara (pieza del 2026-05-31). Si el catálogo distingue a Vorágine de Cuestión Pública, conviene saber que firman investigaciones juntas.
- El barrido de los 12 meses de la objeción 4, que es la única forma de llenar el «no hay argumento».
- La línea Vital Strategies (17 piezas) como agenda temática patrocinada y declarada.

## EVIDENCIA QUE NO MUEVE EL NÚMERO

- Sin endoso. La sección Editorial tiene una sola entrada en toda su historia: «La amenaza de muerte», sobre las amenazas al reportero Nicolás Sánchez (https://voragine.co/editorial/, 2026-10-10; la API de categorías da «Editorial» count 1). Ninguna de las 93 entradas de los 12 meses está en «Editorial» ni en «Opinión» (la API de categorías da «Opinión» count 10 en toda la historia, ninguna en la ventana). No encontré ningún endoso electoral en la campaña de 2026.
- Contratación pública: cero. SECOP II, https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=count(*)&documento_proveedor=901406489 → [{"count":"0"}]; con 9014064891 → [{"count":"0"}]. SECOP I, https://www.datos.gov.co/resource/f789-7hwg.json?$select=count(*)&identificacion_del_contratista=901406489 → [{"count":"0"}]; con 9014064891 → [{"count":"0"}]. Consultas del 2026-10-10. Coincide con lo que el medio declara: «Vorágine no contrata con ninguna entidad estatal colombiana, de ningún nivel» (Directrices 2026, §8.7).
- Directrices Editoriales 2026 (subidas en 2026-08), §4.2: «La Junta Directiva no debe influir en las decisiones editoriales del medio, tampoco los aliados comerciales, ni los financiadores». Y §2.3, sobre su foco declarado: «busca contar y hacer visibles historias en las que hay vulneración de Derechos Humanos». Es un foco temático, no una posición en el eje.
- El medio declara la financiación pieza a pieza, como prometen sus Directrices («a través de una leyenda que quedará fijada dentro del mismo contenido»), y se comprueba en las 17 piezas de Vital Strategies.
- Fiscaliza a empresas de los dos lados del dinero político: Santo Domingo, Ardila y Sarmiento financiando a un condenado de Cambio Radical (2026-05-03); Postobón (2026-08-02); Coca-Cola (serie). También fiscaliza instituciones: la pieza sobre el presidente de la Corte Constitucional (2026-02-19, de la Liga) y la del comandante del Ejército (2025-10-26). Fiscalizar no cuenta en ninguna dirección.
- Certificación JTI vigente: el informe está «Publicado el: julio 18, 2024» y tiene «Fecha del informe: septiembre 29, 2026».

## SIN OBJECIÓN
No aplica: presento 5 objeciones.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal (la única, por datos personales).** El revisor no copió cédulas, teléfonos ni direcciones. Pero enlazó dos veces el PDF del Informe de Transparencia JTI (se enlaza desde /nosotros/; no se cita su ruta porque muestra documentos de identidad). Sus preguntas 30 y 37 muestran el **número de cédula y el teléfono móvil de los cuatro gestores**. Los dos enlaces se sustituyeron por «[enlace retirado: … Ley 1581; se enlaza desde https://voragine.co/nosotros/]», que es la página del medio de la que cuelga el PDF. El resto del texto está intacto.

Los PDF de estados financieros que cita el revisor no muestran documentos de identidad (solo las tarjetas profesionales del contador y del revisor fiscal) y se dejan. **Esta resolución no enlaza ningún PDF del medio.** Los nombra y enlaza la página de la que cuelgan:
- el JTI, desde `/nosotros/`;
- los estados financieros, desde `/documentacion-legal/`.

Las consultas a datos.gov.co van con `$select`, limitado a los campos citados (comprobado: no devuelven documentos de identidad).

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada (2026-10-10):
  - voragine.co: `User-agent: *` con `Disallow` de `/sitio/`, `/bk-sitio/` y un PDF de 2022. No nombra a ningún agente de Anthropic. **Literal, como dice el revisor.**
  - datos.gov.co: `Crawl-delay: 1` y exclusiones de `/browse`; se usó solo `/resource`, con más de un segundo entre consultas.
  - casamacondo.co: veta `/wp-admin/`, `/?s=`, los feeds y `/embed/`; `/somos/` está permitido.
  - volcanicas.com, sembramedia.org y gfmd.info: sin restricciones para estas rutas.
  - No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. **No hubo buscador web.**
- **Sitio**, en crudo con `curl -sL --ssl-no-revoke` y User-Agent de Chrome 126, en `t89/voragine-ver`:
  - `/nosotros/`, `/documentacion-legal/`, `/editorial/` y `/feed/`;
  - el Informe de Transparencia JTI, los estados financieros 2025-2024 y sus notas, y las Directrices editoriales 2026, pasados a texto con `pdftotext -layout`;
  - **la API de WordPress con el contenido completo de las 93 entradas** de la ventana (`x-wp-total: 93`), las categorías, y las seis búsquedas internas del revisor.
- **Fuentes de la ficha:** SembraMedia (7-02-2023) y GFMD, las dos con respuesta 200.
- **Cruce del revisor:** `casamacondo.co/somos/` y `volcanicas.com/nosotras/`.
- **Registros**, en datos.gov.co:
  - RUES (`c82u-588k`): `nit` = `901406489` y `9014064891`, y razón social `like '%VORAGINE%'`.
  - SECOP II (`jbjy-vk9h`): `documento_proveedor` = `901406489`, `9014064891` y `901406489-1`; además, `proveedor_adjudicado like '%VORAGINE%'` y `like '%PERIODISMO CONTRACORRIENTE%'`.
  - SECOP I (`f789-7hwg`): `identificacion_del_contratista` con los tres; además, `nom_razon_social_contratista like '%VORAGINE%'`.
- **Repositorio** (rama `revision/ciclo-2-tandas-8-9`, sin tocar):
  - el envío y su `00-LEEME.md`, y `fichas/voragine.md`;
  - las fichas que la nombran: `casa-macondo`, `volcanicas`, `revista-raya`, `las2orillas`, `el-morichal`, `el-colombiano` y `sucre-noticias`;
  - sus entradas en `shared/mediaRegistry.js`, `shared/mediaOwnership.js` y `shared/centinela.js`;
  - el protocolo, `DECISIONES.md` (2026-10-07 a 2026-10-10), `PLAN_PRODUCTO_FINAL.md`, `SESION_DECISIONES.md` y el commit `fa77249`.
- **El barrido**, reproducible, está en `revision-externa/barridos/voragine.md`.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

**Antes de la tabla, un hecho que cambia el marco de las cinco objeciones.** **El valor de Vorágine en el código no es −0,50 desde el 2026-09-18.** El 2026-09-16 el responsable editorial dictó «el trío y RTVC "sin medir"» (`PLAN_PRODUCTO_FINAL.md`, 3.5). El commit `fa77249` (2026-09-18) lo aplicó, y `shared/mediaRegistry.js` dice hoy:

> `SIN MEDIR — decisión del responsable editorial del 2026-09-16, aplicada el 2026-09-18. Llevaba −0,50` · `bias: null`

La cabecera de la ficha («Valor actual | **−0,50**») no se actualizó. De ahí pasó al envío y a `envios/ciclo-2-2026-10-10/00-LEEME.md`. **El revisor ataca un número que ya no está en el código.** Su conclusión («apoya "sin medir"») coincide con lo que ya se aplicó.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | Los fundadores que nombra la ficha no son quienes gobiernan hoy: asamblea de gestores Jaramillo (representante legal), Guarnizo (director general), Penagos y Abu Shihab; Barrientos y Escobar no figuran; el cruce de Barrientos pasa por La Liga | sí | sí | **Aceptada, y va más allá.** Todo literal en el JTI (29-09-2026), en `/nosotros/` y en el RUES, que confirma a la representante legal. **Pero el cruce no es con Volcánicas: es con CasaMacondo.** Barrientos es «Editor de la Unidad Investigativa» en `casamacondo.co/somos/` y no aparece en `volcanicas.com/nosotras/`. La ficha copió mal el medio, y el revisor heredó el error sin comprobarlo. Que fuera fundador consta en SembraMedia (2023), que habla de «siete fundadores», no de cuatro. Es historia |
| 2 | La financiación está concentrada: Vital Strategies 28,7 %; con Wellspring, CLUA y Rockefeller PA, 60,9 %; Embajada de Canadá, UNODC, Bancolombia | sí | sí | **Aceptada, con un matiz.** Las cifras de 2025 son exactas, y en 2024 las cuatro sumaban el **72,3 %**: es una base estable, no rotativa. Matiz que el revisor omite: el mismo JTI (pregunta 49, datos de 2023) dice que el **45,3 %** venía de «alianzas con terceros privados […] para hacer contenidos periodísticos concretos». La ficha no inventó el patrocinio por pieza, pero hoy no es lo principal. La fila de Bancolombia está en una tabla desalineada: se cita con esa reserva |
| 3 | Vital Strategies financia 17 de 93 piezas, declarado en cada una | sí | sí | **Aceptada.** 17 de 93 (18 %), todas sobre la industria de alimentos y bebidas; 8 son versiones en inglés o en cómic. La leyenda es literal. No mueve el número |
| 4 | El −0,50 no se sostiene: fiscaliza a Petro antes y a De la Espriella después; asimetría solo en campaña (12 a 0) con un confusor; unas 3 piezas con postura; la regla no se cumple | sí | sí, con barrido propio de las 93 | **Aceptada en lo sustancial, y ya aplicada desde el 2026-09-18.** El barrido da **6** piezas contra el Gobierno Petro antes del cambio (el revisor contó 5: falta la del pueblo U'wa, 12-07-2026) y **4** contra el Gobierno De la Espriella después. Postura en voz de la casa: **3 rótulos leves**, ninguna celebración. La asimetría de campaña es **12 sobre la derecha** (8 sobre candidatos o el presidente electo y 4 sobre otros políticos de derecha) **frente a 0 sobre Cepeda**. Hay dos contrapesos que el revisor no ve (n.º 55 y 31). La regla no se cumple. Ver el punto 4 |
| 5 | Hueco del corpus: 9 piezas entre el 31-08 y el 10-10, se captaron 4 | sí | parcial | **Aceptada en el hecho.** La API da 9 y **el feed `voragine.co/feed/` las sirve hoy las 9** (10 ítems, del 23-08 al 07-10). El hueco es de la ingesta, no del medio. Qué cuatro se captaron no se pudo comprobar aquí: es inferencia del revisor, como él mismo dice |

### Lo verificado, objeción por objeción

**1 · Gobernanza y cruce.**
- **RUES** (`c82u-588k`, 2026-10-10), literal: «"razon_social":"FUNDACIÓN VORAGINE PERIODISMO CONTRACORRIENTE"», «"nit":"901406489"», «"digito_verificacion":"1"», «"matricula":"1944922"», «"camara_comercio":"MEDELLIN PARA ANTIOQUIA"», «"estado_matricula":"ACTIVA"», «"fecha_matricula":"20200831"», «"fecha_renovacion":"20260319"», «"ultimo_ano_renovado":"2026"», «"organizacion_juridica":"FUNDACIONES"», «"cod_ciiu_act_econ_pri":"5813"», «"representante_legal":"MARÍA JOSÉ JARAMILLO BERRÍO"». Con el dígito de verificación pegado (`9014064891`), `[]`. **Exacto.** Por razón social salen 44 entidades con «VORAGINE» en el nombre, y solo esta es el medio. Consulta: `https://www.datos.gov.co/resource/c82u-588k.json?nit=901406489&$select=razon_social,nit,digito_verificacion,matricula,camara_comercio,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,organizacion_juridica,cod_ciiu_act_econ_pri,representante_legal`.
- **Informe de Transparencia JTI** (enlazado desde `/nosotros/`; «Fecha del informe: septiembre 29, 2026»; «Publicado el: julio 18, 2024»):
  - pregunta 5.a: «901406489-1»;
  - pregunta 24: «Titulares e integrantes activos de la Asamblea General de Fundadores o Asamblea de Gestores (órgano de administración)», con los cuatro nombres que da el revisor;
  - pregunta 26: la Junta Directiva «ad honorem», con tres titulares y tres suplentes, como él dice;
  - pregunta 37: los cuatro cargos;
  - pregunta 16.a: «lanzamos públicamente el medio (1 de junio de 2020) antes de la constitución de la persona jurídica (31 de agosto de 2020)».

  **Todo literal.** La pregunta 25.a remite a `/documentacion-legal/` para los nombres, pero esa página no los publica hoy (0 coincidencias): solo enlaza estados financieros.
- **`/nosotros/`** (2026-10-10), literal: «José Guarnizo Cofundador y director general de Vorágine», «Laila Abu Shihab Vergara Cofundadora y directora de proyectos», «María José Jaramillo Cofundadora y directora ejecutiva y administrativa», «Angie Pik Cofundadora y directora gráfica». «Barrientos» y «Escobar» aparecen **0 veces**. **Exacto.**
- **Notas a los estados financieros 2025-2024:** «constituida […] por Acta del 16 de junio de 2020 […] inscrita en la Cámara de Comercio de Medellín el 31 de agosto de 2020». Exacto. El «1 de junio de 2020» de la ficha es la fecha de lanzamiento del portal («Nacimos el primero de junio de 2020», `/nosotros/`). Es una efeméride y no pesa.
- **De dónde salían los cuatro nombres de la ficha.** SembraMedia (7-02-2023), literal: Guarnizo «se reunió con otros dos periodistas […] ‘Pacho’ Escobar y Juan Pablo Barrientos»; Barrientos invitó a Abu Shihab «a formar parte del equipo de fundadores»; y el medio arrancó con «siete millones de pesos […] que salieron del bolsillo de los siete fundadores». **Siete, no cuatro.** La ficha eligió cuatro nombres de una fuente de 2023 y los presentó como vigentes. Por la regla del presente, quién fundó no cuenta; cuenta quién controla hoy.
- **El cruce.**
  - La ficha dice que Barrientos «dirige la unidad investigativa de Volcánicas». En `volcanicas.com/nosotras/` (2026-10-10) «Barrientos» aparece **0 veces**. En `casamacondo.co/somos/` figura como «Juan Pablo Barrientos Editor de la Unidad Investigativa».
  - El código ya lo tenía bien: `mediaOwnership.js`, `casamacondo-direccion`; `centinela.js`, `casa-macondo`; y `fichas/casa-macondo.md`.
  - **Error de la ficha de Vorágine**, que el revisor no detecta: dice «Volcánicas» y afirma que el registro lo anota «en la ficha de propiedad de Volcánicas». Lo anota en la de CasaMacondo.
- **Cómo aparece hoy Barrientos en voragine.co.** Una sola vez en 12 meses: la n.º 32 (19-02-2026), «Por: La Liga Contra el Silencio, Juan Pablo Barrientos y José Alejandro Castaño». La nota editorial explica que es la **republicación por La Liga de una investigación de CasaMacondo** retirada por una tutela: «los medios que integramos la alianza de La Liga Contra el Silencio republicamos de manera íntegra la nota censurada». El comunicado del 27-02 dice: «no es un medio de comunicación, es una alianza de medios independientes» y «Hoy somos 16 salas de redacción». **Literal.**
- **Lectura.** El vínculo vigente entre Vorágine y CasaMacondo es la alianza La Liga, no una persona con papel en los dos. Barrientos no tiene papel hoy en Vorágine. **El cruce de persona deja de ser vigente** y pasa a historia (SembraMedia 2023). Debe corregirse en las dos puntas. Se anota la alianza.

**2 · Financiación.**
- **Notas a los estados financieros 2025-2024**, enlazadas desde `/documentacion-legal/`. Literal:
  - «Total ingresos operacionales 157,594,000»;
  - «Total ingresos no operacionales 733,059,573»;
  - total «890,653,573».
  - Bajo «Por tercero diversos, donaciones», las filas que cita el revisor, con las mismas cifras (incluida la errata «Emabaja del Canadá»): Vital Strategies 255.910.041, Wellspring 159.841.815, Climate and Land Use Alliance 71.240.439, Rockefeller Philanthropy Advisors 55.126.283, Embajada de Canadá 49.479.131, Fundación Connectas 17.298.645 y VAKI 28.381.191.
  - Bajo «Por tercero talleres»: «OFICINA DE LAS NACIONES UNIDAS CONTRA LA DROGA Y EL DELITO 67,620,000».

  **Exacto.**
- **Cálculo.** Vital Strategies es el 28,73 % del total de 2025, y las cuatro juntas, el 60,87 %. **Exacto.** En 2024 las cuatro sumaban 608.957.269 de 842.845.418, el **72,3 %**. Las donaciones son el 73,9 % de los ingresos de 2025. La Embajada de Canadá pesa el 5,6 % y UNODC el 7,6 %.
- **Bancolombia SA, 38.205.000.** Está en la tabla «Por tercero publicaciones», con las columnas desalineadas en el PDF. La fila se lee, pero no consta con seguridad a qué año corresponde. El revisor ya lo advierte. **Se cita con reserva.**
- **El matiz que el revisor omite.**
  - JTI, pregunta 49 (año 2023): «el 52,3% corresponden a grants o subvenciones internacionales que financian la operación en general del medio; el 45,3% corresponden a alianzas con terceros privados (nacionales e internacionales) para hacer contenidos periodísticos concretos, y el resto (2,4%) corresponden a donaciones de los lectores».
  - `/nosotros/`: «cuatro fuentes de ingresos principales: los aportes de los lectores, los talleres, las subvenciones o grants internacionales y las alianzas con entidades y organizaciones privadas».

  La frase de la ficha («aliados que patrocinan investigaciones concretas») describe una parte real del modelo. **Lo que no se sostiene es «una lista de aliados que rota» como descripción del conjunto.**
- **Contratación pública:** 0. Comprobado con las seis consultas por NIT (con y sin DV, y con guion) y por razón social:
  - SECOP II: 8 registros con «VORAGINE» en el nombre, todos de otras entidades (un hogar infantil, varios consorcios);
  - SECOP I: 25 registros, todos de otras entidades (un conservatorio, una estación de servicio…);
  - ninguno es la fundación.

  `/nosotros/`: «No contratamos con el Estado colombiano, en ningún nivel». Directrices 2026, §8.7: «Vorágine no contrata con ninguna entidad estatal colombiana, de ningún nivel». **Exacto.**
- **Lo que no se resuelve.** Si la Consejería Distrital de Paz pagó algo a Vorágine por el conversatorio del 12-08 (n.º 81). SECOP no lo registra con este NIT. Queda como el revisor lo deja.

**3 · Vital Strategies.**
- 17 de las 93 entradas llevan la leyenda (`search=Vital Strategies` con `after` da 17; el recuento en el cuerpo da las mismas 17). Las fechas van del 2025-10-16 al 2026-09-27. **Exacto.** La de Briceño (n.º 91), literal: «Esta investigación fue financiada, en parte, por Vital Strategies. El contenido es editorialmente independiente y su propósito es arrojar una luz tanto sobre […]».
- Ocho de las 17 son versiones en inglés o en cómic de otras de la misma serie. **Investigaciones distintas hay 9.** El «18 % de lo publicado» es cierto en entradas; en investigaciones, menos.
- **Tensión que se declara, no mueve el número.** El mayor financiador fija una línea temática estable: salud pública frente a la industria de alimentos y bebidas. Esa línea apunta en septiembre de 2026 a un congresista del Centro Democrático y a créditos del Gobierno De la Espriella. Hay que vigilarlo, como dice el revisor. La causa no es de izquierda ni de derecha por sí misma.

**4 · El barrido** (completo en `revision-externa/barridos/voragine.md`).
- **Universo:** las 93 entradas de la API con el contenido completo, sin muestreo. No hay editoriales en la ventana: la categoría Editorial tiene 1 entrada en toda su historia y Opinión, 0 en la ventana. **Exacto, como dice el revisor.**
- **Recuento:**

| | Antes del 07-08 | Desde el 07-08 |
|---|---:|---:|
| Fiscaliza al Gobierno Petro | **6** (n.º 15, 27, 31, 36, 45, 73) | — |
| Fiscaliza al Gobierno De la Espriella (incluye al Ejército bajo su mando, n.º 92) | — | **4** (n.º 82, 90, 91, 92) |
| Fiscaliza a candidatos de derecha o al presidente electo | 7 | 1 (n.º 80, el día de la posesión) |
| Fiscaliza a otra derecha (no candidatos) | 4 | — |
| Postura en voz de la casa (rótulos leves) | 2 (n.º 3, 58) | 1 (n.º 90) |
| Elogios o disculpas a un gobierno, partido o candidato | 0 | 0 |
| Ajenas: La Liga, autor externo, colectivo | 4 (n.º 25, 32, 34, 37) | 0 |

- **Diferencias con el revisor:**
  - suma la n.º 73 (12-07-2026, «El Estado colombiano sigue en deuda con el pueblo U'wa»), que reprocha al Gobierno Nacional la sentencia de la Corte IDH: son 6, no 5;
  - pone la n.º 80 (publicada el 07-08) del lado «después»;
  - **no cuenta como postura de la casa** el comunicado de La Liga (n.º 34) ni el manifiesto de las 171 firmantes (n.º 37). El primero es voz de una alianza de 16 salas. El segundo es un texto colectivo en categoría Comunicado. Los dos se declaran y no suman (condición 1).
  - **sí cuenta** dos rótulos leves que él no ve: la n.º 3 («se destaca por su agresividad») y la n.º 58 («se ha caracterizado por intimidar la protesta social»), ambas sobre un concejal del CD. Y la n.º 90, con su titular y «influencer de extrema derecha». **Total: 3 con postura, como él estima, pero otras tres.**
- **Contrapesos que el revisor no ve:**
  - la n.º 55 (17-05-2026, en campaña) nombra entre los atacantes de una congresista a «@Xpost1A, cuenta anónima de propaganda política a favor del gobierno Petro y el candidato presidencial oficialista Iván Cepeda»;
  - la n.º 31 (16-02-2026) documenta presiones en MinEducación para marchar a favor de Petro, también en campaña.
- **Un error menor del revisor:** de las 7 entradas de `search=Cepeda`, cuenta «tres piezas de 2026-05-17», y son **dos** (n.º 54 y 55). La lista suma 7 igual porque incluye otras. Además, la n.º 15 nombra a Efraín Cepeda y la n.º 31 a Iván Camilo Cepeda, no al candidato.
- **¿La asimetría de campaña (12 a 0) es postura o fiscalización del puntero?** El protocolo, literal:
  - polo fijo, «Qué NO toca esta regla»: «Lo mismo vale para el encuadre asimétrico entre candidatos»;
  - «Evidencia editorial histórica», primera precisión: «Para llegar a 3 piezas a cada lado del cambio de gobierno solo cuentan los elogios, las disculpas y los rótulos. Una pieza que solo fiscaliza a quien manda se declara, pero no suma»;
  - la REFUTACIÓN de la propia ficha pide «trato distinto a dos actores comparables».

  **Ocho investigaciones sobre un candidato son frecuencia de blancos, no encuadre.** Para que fuera encuadre habría que mostrar trato distinto con material comparable. Y hay dos confusores documentados por el propio medio: De la Espriella era puntero y, según la Flip citada en la n.º 24, el mayor litigante contra periodistas («109 denuncias»). Cuatro de las ocho son de después de la elección. **Se declara como tensión (nivel 5) y no suma.** Aun contándola como postura, no hay ningún elogio, disculpa ni rótulo en esas ocho, y faltaría el mínimo de 10 y el de 3 por lado.
- **Aplicación literal de las reglas:**
  - condición 3: «al menos 10 piezas con postura» → 3; **no se cumple**;
  - condición 2 con la precisión: «3 a cada lado» → 2 y 1; **no se cumple**;
  - segunda precisión: «Un barrido que no llega a los mínimos no deshace nada. La ficha conserva el valor que tenía»;
  - §5, regla 3: «Sin evidencia de nivel 1-3, no se mueve el número»;
  - regla 2: «Ante la duda entre dos bandas, se elige la más cercana a la mixta».
- **¿Cómo se llegó a −0,50, y se apoyaba en algo?** En nada medido. La ficha, CONTRA 4: «El −0,50 no viene de ninguna medición, ni antigua ni nueva: es una colocación entre RAYA y Cuestión Pública». Ninguna entrada de `DECISIONES.md` lo justifica, y `fichas/casa-macondo.md` y `fichas/volcanicas.md` lo usan como vecino, no como medida. **No es que la evidencia de −0,50 «ya no se sostenga»: nunca la hubo.** Por eso el responsable editorial lo retiró el 16-09. La regla «no deshace nada» protege un valor puesto por otras razones; el valor vigente es **sin medir**, y el barrido no lo mueve.
- **Lo que sí permite el barrido.** El protocolo dice: «Un barrido que muestra la misma conducta con los dos gobiernos sostiene el 0,00 como evidencia». Aquí la conducta con los dos gobiernos es la misma: fiscaliza a los dos y no celebra a ninguno. Es lo que llevó a Chocó 7 Días a 0,00 con evidencia el 2026-10-09. **En contra** están la asimetría de campaña, que Chocó 7 Días no tenía, y que el «sin medir» del 16-09 se decidió para el trío entero. Es decisión del responsable editorial: ver la propuesta.

**5 · Hueco del corpus.**
- API: 9 entradas del 31-08 al 07-10 (n.º 85-93). **Exacto.**
- `https://voragine.co/feed/` (2026-10-10, 200, `application/rss+xml`): 10 ítems, del 23-08 al 07-10, y **contiene las 9**. Las n.º 85 y 86 traen de resumen la plantilla «The post … appeared first on», y la n.º 89 la leyenda de Vital Strategies en inglés: es el defecto que la ficha ya documentó.
- **El hueco es de la ingesta, no del feed.** El envío da 4 artículos en la ventana. Qué cuatro no se pudo comprobar aquí sin la base; el revisor lo marca como inferencia. Confirma el «LO QUE ES NUESTRO Y NO SUYO» de la ficha y lo agrava: las cuatro piezas posteriores al 08-09, que son las primeras del Gobierno De la Espriella, no están medidas.

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se corrigen estas partes:
- **Obj. 1, «el cruce con Volcánicas»:** el cruce del catálogo es con **CasaMacondo**. El revisor aceptó la premisa de la ficha y declaró no haber visitado volcanicas.com; allí Barrientos no figura.
- **Obj. 2, «no es un patrocinio que cambie pieza a pieza»:** es cierto del grueso de 2025, pero el propio JTI da un 45,3 % de alianzas por contenido concreto en 2023. La ficha describía mal la proporción, no un hecho inexistente.
- **Obj. 3, «el 18 % de lo publicado»:** cierto en entradas, pero 8 de las 17 son versiones de otras. Son 9 investigaciones distintas.
- **Obj. 4, recuento y clases:**
  - Petro, antes: 5 → **6**;
  - la n.º 80 pasa al lado «después»;
  - las piezas «con postura de la casa» no son el comunicado de La Liga ni el manifiesto, que son ajenos, sino tres rótulos leves (n.º 3, 58 y 90);
  - faltan los contrapesos n.º 55 y 31;
  - «tres piezas de 2026-05-17» → **dos**.
- **Obj. 4, «el −0,50»:** ya no es el valor del código desde el 2026-09-18. La objeción llega tarde por un error de la ficha, no del revisor.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente ni cita inventada.** Todas las URL de voragine.co y de datos.gov.co responden, y las citas son literales en el HTML, en el PDF o en el JSON. Lo que hay:
- **Enlaces a un PDF que muestra cédulas y teléfonos** (retirados de la literal, ver arriba). No es fuente falsa, es dato personal.
- Hereda de la ficha el error de Volcánicas.
- Cuenta como «postura de la casa» textos que no son de la casa, y no ve dos rótulos que sí lo son.
- Un recuento menor equivocado (dos piezas del 17-05, no tres).

**Errores de la propia ficha, para no repetirlos:**
- **«Valor actual | −0,50»:** desactualizado desde el 2026-09-18 (`bias: null`, decisión del 16-09). Pasó al envío y a su `00-LEEME.md`, y el revisor gastó la objeción decisiva contra un número retirado. Hay que comprobar el registro antes de armar un envío.
- **«Juan Pablo Barrientos […] dirige la unidad investigativa de Volcánicas»** y «el registro lo anota en la ficha de propiedad de Volcánicas»: es CasaMacondo. El código y `fichas/casa-macondo.md` lo tenían bien.
- **Los cuatro «fundadores» como titulares vigentes:** salen de SembraMedia (2023), que habla de siete. Hoy controlan la ESAL cuatro gestores, dos de ellos distintos de los que nombra la ficha, y la ficha omite a la representante legal. Es la regla del presente.
- **«Creada el 1 de junio de 2020»:** es el lanzamiento del portal. La persona jurídica es del 16-06-2020 (acta) y del 31-08-2020 (inscripción).
- **«Una lista de aliados que rota»:** cuatro grant-makers dan el 60,9 % de 2025 y el 72,3 % de 2024.
- **Sin la línea de contratación pública**, obligatoria desde el 2026-10-07. Son 0 contratos, y también se escribe.
- **No miró la sección Editorial ni el archivo.** Habría encontrado que no hay editoriales y que el medio fiscaliza a los dos gobiernos, que era la prueba que la propia ficha pedía en la REFUTACIÓN.
- **Lo que la ficha sí tenía bien, hoy:** que el −0,50 no venía de ninguna medición; que fiscalizar no es orientación; que el hueco del corpus es «nuestro»; y que la salida «sin medir» era la que menos inventaba. El responsable editorial la tomó el 16-09.

---

**Propuesta para la firma**

**Valor: sin medir (`bias: null`), sin cambios en el código.**
- **Por qué no se mueve.** El barrido no cumple «Evidencia editorial histórica» (3 piezas con postura frente a 10; 2 y 1 por lado), y por la segunda precisión del 09-10 no deshace nada. No hay nivel 1-3 que sitúe al medio en el eje (regla 3). **El −0,50 no vuelve**: nunca tuvo evidencia.
- **Alternativa declarada: 0,00 provisional, con evidencia.** El protocolo admite el 0,00 cuando un barrido muestra la misma conducta con los dos gobiernos, y aquí la hay: 6 piezas fiscalizan antes del cambio y 4 después, sin celebrar a nadie. Es el precedente de Chocó 7 Días. **Por qué no se recomienda:** hay una asimetría de campaña (12 a 0) que Chocó 7 Días no tenía, el «sin medir» se decidió el 16-09 para el trío, y el medio es no noticioso, así que el número no se ve en el mapa.
- **Ningún valor de izquierda tiene apoyo.** Un −0,20 o un −0,30 exigiría que la asimetría de campaña contara como postura, y ni así llega a los mínimos.

**`ownerType` y `verifiedAt`:**
- `ownerType: 'independiente'` se mantiene: es una ESAL sin accionistas, gobernada por cuatro periodistas gestores (JTI y RUES).
- `verifiedAt: '2026-10-10'`: la gobernanza, la financiación y la contratación quedan verificadas hoy en fuentes primarias (RUES, JTI, estados financieros y SECOP). Hoy dice `VERIFICADO` (`'2026-07-29'`).

**Bloque propuesto para `shared/mediaOwnership.js`, entrada `voragine`** (no se escribe en código):

```js
    'voragine': {
        // 2026-10-10 (ciclo 2, tanda 9): gobernanza del JTI (29-09-2026) y del
        // RUES; financiación de las notas a los estados financieros 2025.
        // Los «cuatro fundadores» que decía esta entrada salían de SembraMedia
        // (2023), que habla de siete; dos de los cuatro no figuran hoy.
        //
        // DATOS PERSONALES: el PDF del informe JTI muestra cédulas y teléfonos
        // de los gestores; se enlaza la página de la que cuelga (/nosotros/).
        ownerType: 'independiente',
        controlGroup: 'voragine-fundacion',
        holdings: [
            'Lo publica la FUNDACIÓN VORAGINE PERIODISMO CONTRACORRIENTE, NIT 901406489-1, fundación sin ánimo de lucro y sin accionistas, matrícula 1944922 de la Cámara de Comercio de Medellín para Antioquia (inscrita el 31-08-2020), ACTIVA, renovada el 19-03-2026. Representante legal: María José Jaramillo Berrío (RUES).',
            'La gobierna una Asamblea de Gestores de cuatro periodistas: María José Jaramillo Berrío (directora ejecutiva y representante legal), José Enrique Guarnizo Álvarez (director general y de contenidos), Laila Abu Shihab Vergara (directora de proyectos) y Angélica María Penagos Zerda (directora gráfica y audiovisual). Tiene además una Junta Directiva ad honorem (informe JTI del 29-09-2026).',
            'Se financia sobre todo con subvenciones internacionales. En 2025 ingresó 890,7 M COP; cuatro donantes estadounidenses dieron el 60,9 %: Vital Strategies (28,7 %), Wellspring Philanthropic Fund, Climate and Land Use Alliance y Rockefeller Philanthropy Advisors (en 2024, el 72,3 %). También la Embajada de Canadá (5,6 %) y talleres para la Oficina de Naciones Unidas contra la Droga y el Delito (7,6 %). Notas a los estados financieros 2025-2024.',
            'Vital Strategies financia, y el medio lo declara en cada pieza, una línea estable sobre la industria de alimentos y bebidas: 17 de sus 93 entradas de los últimos 12 meses (9 investigaciones distintas).',
        ],
        notes: [
            'Contratación pública (SECOP I y II, NIT 901406489, consultado 2026-10-10): 0 contratos en SECOP I y II a 2026-10-10, también con el dígito de verificación. El medio declara: «No contratamos con el Estado colombiano, en ningún nivel».',
            'Es miembro de La Liga Contra el Silencio, una alianza de 16 salas de redacción, y copublica investigaciones con otros medios del catálogo: con Cuestión Pública (31-05-2026), y con CasaMacondo, cuya investigación republicó por La Liga (19-02-2026). Juan Pablo Barrientos, editor de la unidad investigativa de CasaMacondo, fue uno de los fundadores de Vorágine (SembraMedia, 2023), pero hoy no figura en sus órganos.',
        ],
        sources: [
            'https://voragine.co/nosotros/',
            'https://voragine.co/documentacion-legal/',
            'https://www.datos.gov.co/resource/c82u-588k.json?nit=901406489&$select=razon_social,nit,digito_verificacion,matricula,camara_comercio,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,organizacion_juridica,cod_ciiu_act_econ_pri,representante_legal',
            'https://www.datos.gov.co/resource/jbjy-vk9h.json?documento_proveedor=901406489&$select=count(*)',
            'https://www.datos.gov.co/resource/f789-7hwg.json?identificacion_del_contratista=901406489&$select=count(*)',
        ],
        verifiedAt: '2026-10-10',
    },
```

Y en `'voragine-fundacion'`, el campo `personas` pasa a los cuatro gestores, con su papel y `fuentes: ['https://voragine.co/nosotros/']`, en lugar de «Juan Pablo Barrientos, Francisco Escobar, José Guarnizo y Laila Abu Shihab […] desde 2020-06-01».

**Textos a corregir** (los aplica quien el responsable editorial decida; aquí no se toca nada):

En `fichas/voragine.md`:
1. **Cabecera.** «Valor actual | **−0,50**» → «**sin medir** (`bias: null`, decisión del responsable editorial del 2026-09-16, aplicada el 2026-09-18)». «Propuesta»: se mantiene «sin medir»; alternativa, 0,00 con evidencia.
2. **Nivel 1.** Sustituir el párrafo de los cuatro fundadores por la gobernanza del bloque de arriba: RUES, asamblea de gestores, Junta Directiva y representante legal. «Creada el 1 de junio de 2020» → «lanzada el 1 de junio de 2020; persona jurídica inscrita el 31-08-2020». Los «siete millones» de SembraMedia pasan, si se quieren, a una línea de historia que no pesa. Fuentes: `/nosotros/` (de la que cuelga el JTI), `/documentacion-legal/` y el RUES con `$select`.
3. **«EL PATROCINIO POR INVESTIGACIÓN…»** → «LA FINANCIACIÓN, CON NOMBRES»: el 60,9 % y el 72,3 %, el 45,3 % de 2023 en alianzas por contenido y la línea de Vital Strategies (17 de 93). Se retira «una lista de aliados que rota».
4. **«EL CRUCE QUE HAY QUE DECLARAR»** → el cruce es con **CasaMacondo**, y por la alianza La Liga Contra el Silencio, no por una persona con papel en los dos. Barrientos fue fundador (2023) y hoy no figura en los órganos de Vorágine.
5. **Sección nueva «CONTRATACIÓN PÚBLICA»:** la primera nota del bloque.
6. **Nivel 2:** añadir el barrido de 12 meses (`revision-externa/barridos/voragine.md`), con este resumen:
   - fiscaliza a los dos gobiernos (6 y 4) y no hay editoriales;
   - 3 rótulos leves, muy por debajo del mínimo;
   - asimetría de campaña de 12 a 0 como tensión, con sus confusores y contrapesos.
   Y el hueco: el feed sirve las 9 piezas y la ingesta captó 4.
7. **«ARGUMENTO — no lo hay»** → «POR QUÉ SIN MEDIR». El barrido no llega a los mínimos y no hay nivel 1-3. El 0,00 con evidencia queda como alternativa declarada.
8. **REFUTACIÓN.**
   - El punto 4 (Barrientos) se retira.
   - Se añade: «Si en el recuento de enero de 2027 aparecen 10 o más piezas con postura en voz de la casa, con 3 a cada lado del cambio, se aplica la regla. Y si el medio investiga a Cepeda o al Pacto Histórico con la misma intensidad que a De la Espriella, o sigue sin hacerlo teniendo material comparable, se anota».
9. **REVISIÓN EXTERNA:** esta resolución, con modelo, versión y fecha.

En `revision-externa/envios/ciclo-2-2026-10-10/00-LEEME.md`, línea 54: «**−0,50** · `reviewedAt: null`» → «**sin medir** (2026-09-16) · `reviewedAt: null`».

En `shared/mediaRegistry.js` (entrada `voragine`): `bias: null` se queda. Al comentario «SIN MEDIR — decisión del responsable editorial del 2026-09-16» se añade: «Barrido de 12 meses del 2026-10-10 (tanda 9): fiscaliza a los dos gobiernos, 3 piezas con postura; no mueve el número. Ver `revision-externa/barridos/voragine.md`».

**Fichas y archivos que se comparan con Vorágine o repiten el cruce** (el valor cambia de −0,50 a sin medir, y el cruce de persona deja de ser vigente):
- `fichas/casa-macondo.md`:
  - líneas 22-28, «uno de los cuatro periodistas fundadores de la Fundación Vorágine, que también está en este catálogo con un valor de −0,50» → «fue uno de los fundadores de Vorágine (SembraMedia, 2023); hoy no figura en sus órganos. Las dos son miembros de La Liga Contra el Silencio, y Vorágine republicó una investigación suya el 19-02-2026»;
  - línea 63, «menos marcado que Vorágine (−0,50) o Cuestión Pública (−0,45)»: los dos están sin medir desde el 2026-09-18. La comparación se cae, y el −0,35 de CasaMacondo queda sin vecino de referencia.
- `fichas/volcanicas.md`, línea 78: «(Vorágine −0,50, Revista RAYA −0,55, Cuestión Pública −0,45)»: los tres están sin medir. El −0,50 de Volcánicas pierde su «mismo rango».
- `fichas/revista-raya.md`:
  - líneas 118-119, «más a la izquierda que Vorágine (−0,50) y que Cuestión Pública (−0,45)», y línea 136;
  - **su propia cabecera dice «−0,55» y el registro, `bias: null`**: el mismo error que la de Vorágine (aviso fuera de esta tanda).
- `fichas/las2orillas.md`, línea 74: cita el rationale antiguo («por debajo de la investigación militante (Vorágine, Cuestión Pública)»). Es una cita y puede quedarse, con la nota «hoy los dos, sin medir».
- `fichas/el-morichal.md`, líneas 183 y 194: cita las directrices de Vorágine, no su valor. **Sin cambios.**
- `fichas/razon-publica.md`: no nombra a Vorágine (comprobado con grep). Las2Orillas, sí (arriba).
- `shared/mediaOwnership.js`:
  - `voragine-fundacion` y `voragine`: como arriba;
  - `casa-macondo`, nota: «cofundó la Fundación Vorágine, también en este catálogo» → «fue uno de los fundadores de Vorágine (2020); hoy no figura en sus órganos»;
  - `casamacondo-direccion`, Barrientos: «es también uno de los cuatro periodistas fundadores de la Fundación Vorágine […] Segundo caso de una persona con papel en dos medios nuestros» → se retira «con papel en dos medios», que hoy no es cierto;
  - `ntc-television`, comentario: «Juan Pablo Barrientos tiene papel en Casa Macondo y en Vorágine» → solo en CasaMacondo.
- `shared/centinela.js`, `casa-macondo`: la vigilancia «Barrientos» describe un vínculo que ya no está vigente. O se retira, o se cambia a «La Liga Contra el Silencio».

**Lo que NO entra como hecho:**
- cédulas, teléfonos o correos de los gestores, que el JTI publica;
- los nombres de personas naturales que aparecen como fuentes de ingreso en las notas;
- los nombres de los miembros de la Junta Directiva más allá de su papel. Se citan como «Junta Directiva ad honorem», sin perfil;
- que Barrientos tenga hoy papel en Volcánicas o en Vorágine;
- que la Consejería Distrital de Paz pagara a Vorágine;
- qué piezas captó la ingesta;
- que la línea de Vital Strategies sea de izquierda o de derecha;
- que la asimetría de campaña sea postura.

**¿Aviso de quien dirige?** No procede. Nadie de la dirección consta con candidatura ni cargo público.

**Decisiones para el responsable editorial:**
1. **Valor.** Recomendación: **sin medir**, como está en el código. Alternativa: 0,00 provisional con evidencia (precedente de Chocó 7 Días). Ningún valor negativo.
2. **La cabecera de la ficha y el `00-LEEME.md` del envío.** Recomendación: corregir «−0,50» hoy. Además, comprobar el registro contra la cabecera en el resto de fichas del trío (RAYA tiene el mismo error) y en las de RTVC antes de enviar más.
3. **El cruce Barrientos.** Recomendación: retirarlo como cruce de persona en las dos puntas y anotar la alianza La Liga Contra el Silencio. Corregir «Volcánicas» → «CasaMacondo» en la ficha de Vorágine.
4. **`ownerType` y `verifiedAt`.** Recomendación: `'independiente'` y `'2026-10-10'`, con el bloque de arriba.
5. **El hueco de la ingesta.** El feed sirve las 9 piezas, pero se captaron 4. Recomendación: revisarlo antes del recuento de enero; es la misma causa que deja sin medir al trío.
6. **Recuento.** Recomendación: enero de 2027, con cinco meses de Gobierno De la Espriella.
