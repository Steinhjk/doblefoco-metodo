# Respuesta — Claude Opus 5.5 sobre CasaMacondo

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
> **Sin ediciones.** El revisor no copió cédulas, teléfonos, direcciones,
> nacionalidad, origen étnico ni lugar de nacimiento, y no enlazó ninguna
> consulta que muestre un documento de identidad. Se explica al principio de
> la resolución.

---

## RESPUESTA LITERAL

```
DECLARACIÓN PREVIA DE CONFLICTO
Soy Claude Opus 5.5 (claude-opus-5-5), de Anthropic. Es la misma casa que el modelo que escribió la ficha, así que lo que yo coincida con ella no prueba nada. Por eso he buscado sobre todo en fuentes que la ficha no usa: la página «Así nos financiamos» y su PDF de 2025, las Directrices editoriales 2025, RUES (c82u-588k), SECOP I y II, la API pública de WordPress del propio medio (la usé para un barrido de 12 meses), las biografías de autor del propio sitio y las capturas de Wayback Machine de las dos páginas que cita la ficha. Fecha de todas las comprobaciones: 2026-10-10, salvo que diga otra.

MÉTODO Y DÓNDE BUSQUÉ
- robots.txt de casamacondo.co (2026-10-10): «User-agent: *», con Disallow de /wp-admin/, /?s=, /feed/, /*/feed/ y /*/embed/. No menciona a ClaudeBot, Claude-Web ni anthropic-ai. robots.txt de voragine.co: solo excluye /sitio/ y /bk-sitio/. datos.gov.co: solo pide Crawl-delay 1. jti-app.com no tiene robots.txt (redirige a la portada de JTI). No toqué ninguno de los dominios vetados ni /feed/.
- Descargas con curl -sL, UA de navegador y --ssl-no-revoke, guardadas en t89\macondo-dl. Páginas descargadas: /somos/, /financiacion/, el PDF https://casamacondo.co/wp-content/uploads/2026/03/Asi-nos-financiamos-2025.pdf, el PDF https://casamacondo.co/wp-content/uploads/2025/05/Directrices-editoriales-2025.pdf, sitemap_index y category-sitemap, y https://voragine.co/nosotros/.
- Barrido editorial: https://casamacondo.co/wp-json/wp/v2/posts?after=2025-10-01T00:00:00 (campos id, date, link, title, categories, author; 214 entradas). Autores sacados de /wp-json/wp/v2/users. Entre 2025-10-10 y 2026-10-10 hay 208 entradas: 73 caricaturas en todo el lote y 138 piezas de texto en esos 12 meses. Leí el HTML crudo de 30 piezas: todas las de Opinión con contenido político, más investigaciones, denuncias y noticias sobre actores políticos de los dos lados.
- Wayback CDX y capturas id_: casamacondo.co/financiacion/ (2025-07-09, 2025-11-07, 2026-03-11) y voragine.co/nosotros/ (2024-09-09, 2025-10-06, 2026-07-20).
- RUES c82u-588k: $where razon_social LIKE '%MACONDO%', sin personas naturales, con $select limitado a cámara, matrícula, razón social, NIT, organización jurídica, fecha de matrícula, último año renovado, estado y CIIU.
- SECOP II jbjy-vk9h (documento_proveedor) y SECOP I f789-7hwg (identificacion_del_contratista): igualdad exacta por los dos NIT, sin DV y con cada DV del 0 al 9 pegado. Además, en SECOP II, proveedor_adjudicado LIKE '%CASA MACONDO%'. Resultado: cero filas en todas.
- Buscador web: disponible. Lo usé una sola vez («Juan Pablo Barrientos Vorágine fundador CasaMacondo») y no dio nada pertinente: solo resultados sobre la novela La vorágine. Ninguna afirmación de esta respuesta sale del buscador.
- Una incidencia de método: por un error de directorio, dos PDF (Asi-nos-financiamos-2025.pdf y Directrices-editoriales-2025.pdf) cayeron un momento en la carpeta de trabajo del repositorio. Los moví de inmediato a t89\macondo-dl sin abrir ningún otro archivo del repositorio.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré nada de eso. Las dos personas jurídicas que encontré siguen activas en RUES y renovadas en 2026 (ver objeción 2). Sin embargo, la estructura de socios no es pública en RUES, así que un cambio en la composición accionaria no se vería por esa vía. Tampoco he podido descartarlo.
- La persona que la ficha nombra como titular o director, ¿sigue viva y en el cargo? (comprobado el 2026-10-10)
  Christopher Tibble aparece hoy en https://casamacondo.co/somos/ como «Director general», y su biografía de autor dice «Director general. [...] Cofundador de CasaMacondo» (https://casamacondo.co/wp-json/wp/v2/users/15, 2026-10-10). José Alejandro Castaño figura como «Editor general» en /somos/ y firma piezas hasta el 2026-10-10. Juan Pablo Barrientos figura en /somos/ como «Editor de la Unidad Investigativa», no como quien «dirige» la unidad. Su biografía dice «Jefe de la Unidad Investigativa [...] Nieman Fellow 2026-2027» (users/5). Su última pieza firmada en el barrido es del 2026-08-15 (/investigacion/enriquecimiento-jorge-eliecer-laverde/). La beca Nieman se cursa en residencia en Harvard, así que es posible que hoy no lleve la unidad en el día a día. Eso es una inferencia y no tengo fuente que lo confirme.
- ¿Quién dirige hoy la redacción?
  En dirección, Christopher Tibble. Al frente de la edición, José Alejandro Castaño como editor general (https://casamacondo.co/somos/, 2026-10-10). Él firma además casi todas las piezas políticas propias recientes.
- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que la ficha cita?
  Sí, y la ficha no tiene ninguno: no nombra ninguna persona jurídica. RUES (datos.gov.co c82u-588k, consulta del 2026-10-10) devuelve dos:
  · «CASA MACONDO - SOMOS HISTORIAS SAS», NIT 901747859, Cámara de Comercio de Bogotá, matrícula del 2023-08-29, SAS, ACTIVA, último año renovado 2026, CIIU 6391.
  · «FUNDACIÓN CASA MACONDO - SOMOS HISTORIAS», NIT 901857339, Bogotá, matrícula del 2024-07-02, «LAS DEMÁS ORGANIZACIONES CIVILES,CORPORACIONES,FUNDACIONES», ACTIVA, renovado 2026, CIIU 6391, fecha de actualización 2026/09/02.
  La fecha de la SAS coincide con lo que dice el propio medio: «Nacimos como empresa el 29 de agosto de 2023» (PDF Así nos financiamos 2025).

## OBJECIONES

OBJECIÓN 1 — La financiación no está «SIN DOCUMENTAR», y la que está publicada contradice la ficha
- QUÉ afirma la ficha: «Se sostiene con suscripciones y donaciones. Su web anuncia una sección "Así nos financiamos", pero el enlace directo devolvía 404 el 2026-08-08. La composición de sus ingresos queda sin documentar». También compara el caso con Volcánicas, que sí «publica sus donantes con porcentajes».
- POR QUÉ es incorrecto:
  (a) https://casamacondo.co/financiacion/ responde 200 hoy, y el enlace sale de la propia página /somos/ («"url":"https:\/\/casamacondo.co\/financiacion\/"»). La página tiene article:modified_time 2026-06-20T19:28:38-05:00, antes de la fecha del supuesto 404. Wayback la registra con 200 el 2025-07-09, el 2025-11-07 y el 2026-03-11, y la captura del 2026-03-11 ya incrusta el PDF de 2025. Lo más probable es que la ficha probara otra URL. Esto es inferencia: no sé qué URL usó.
  (b) La página publica donantes y porcentajes, igual que Volcánicas. Cito literal del PDF Asi-nos-financiamos-2025.pdf: «CasaMacondo tuvo cuatro fuentes de financiación en el año 2025: [...] Audiencias 3.100.886,00 4,1% / Donación Vaki 3.100.886,00 / Especiales y proyectos 62.680.111,91 83,3% [...] Talleres de formación 5.761.344,58 7,7% [...] Subvenciones 3.715.828,00 4,9% / Sembra Media 3.715.828,00 / Total 75.258.170,49». Entre los financiadores de «Especiales y proyectos» nombra a Cámara Colombiana del Libro, CONSORCIO NACIONAL DE MEDIOS S.A.S, EDICIONES FONDO DE CULTURA ECONOMICA SAS, Estrella Grupo Empresarial SAS, Fundación Algo en Común, Fundación Confiar, Fundación Gloria Zea, Fundación Para El Fomento De La Lectura, Universal Group Agencia De Comunicaciones S A S y UNIVERSIDAD DE LOS ANDES. En talleres aparece Caro y Cuervo. Nota: la extracción del PDF a texto alinea las cifras con cada línea; las he citado en ese orden.
  (c) Por tanto, «se sostiene con suscripciones y donaciones» es falso con los datos del propio medio: las audiencias pesan el 4,1 % en 2025. En la versión de 2024 (captura de Wayback del 2025-11-07) pesaban el 2,44 %: «Durante 2024 los ingresos de CasaMacondo ascendieron a [...] ($91.760.215) [...] 94,92 % [...] financiación de los proyectos como el especial «Sonidos para la paz», «Los 50 mejores libros del 2024» [...] 2,63 % [...] aportes realizados por los socios [...] 2,44 % [...] aportes realizados por la audiencia».
  (d) Lo que esto dice sobre la orientación: en 2025, el 83 % de los ingresos son patrocinios de proyectos culturales (sobre todo «Los 50 mejores libros»), pagados por editoriales, fundaciones empresariales o culturales, una universidad privada y agencias de comunicación. Ninguno es un financiador de perfil partidista reconocible. Esto es inferencia y no lo he investigado financiador por financiador. Así, la evidencia de nivel 1 que la ficha esperaba («puede mover el valor en cualquier dirección», refutación 1) ya existe, y no apunta a la izquierda.
- FUENTE Y FECHA: https://casamacondo.co/financiacion/ (consultada el 2026-10-10; modificada el 2026-06-20); https://casamacondo.co/wp-content/uploads/2026/03/Asi-nos-financiamos-2025.pdf (subido en marzo de 2026, datos de 2025); Wayback https://web.archive.org/web/20251107121725/https://casamacondo.co/financiacion/ y https://web.archive.org/web/20260311004840/https://casamacondo.co/financiacion/.
- NIVEL: propiedad y financiación, como declaración documentada del propio medio, con cifras.

OBJECIÓN 2 — El «Nivel 1» de la ficha no dice de quién es el medio
- QUÉ afirma la ficha: su nivel 1 se reduce a «Quién dirige, hoy», con tres nombres. No nombra ninguna persona jurídica, socio ni NIT.
- POR QUÉ: el editor del medio existe, está registrado y es localizable. Es CASA MACONDO - SOMOS HISTORIAS SAS (NIT 901747859), junto con una fundación hermana, FUNDACIÓN CASA MACONDO - SOMOS HISTORIAS (NIT 901857339), ambas activas y renovadas en 2026 (RUES; datos en NIVEL 1). En cuanto a la propiedad, las Directrices 2025 hablan de «los trece socios de CasaMacondo» (Directrices-editoriales-2025.pdf, apartado c), y las biografías del sitio presentan como «Cofundador de CasaMacondo» a Tibble (users/15), a Castaño (users/9), a Barrientos (users/5) y a Ricardo Mendivil (users/3). El informe de 2024 dice que los socios aportaron el 2,63 % de los ingresos. Ni RUES abierto ni el medio publican la composición accionaria de la SAS, y no encontré un certificado de existencia y representación de 2026. Es una laguna declarable, pero la regla «se declara siempre de quién es» exige al menos nombrar la entidad y decir que la propiedad está repartida entre unos trece socios-periodistas sin accionista dominante conocido. Esto último es inferencia a partir del «trece socios» y no tengo la composición. Contratación pública: cero contratos en SECOP I y SECOP II con cualquiera de los dos NIT, con o sin DV (consultado el 2026-10-10).
- FUENTE Y FECHA: datos.gov.co c82u-588k, jbjy-vk9h y f789-7hwg (2026-10-10); https://casamacondo.co/wp-content/uploads/2025/05/Directrices-editoriales-2025.pdf (mayo de 2025, enlazado hoy desde /somos/); https://casamacondo.co/wp-json/wp/v2/users/{15,9,5,3} (2026-10-10).
- NIVEL: propiedad y registro externo.

OBJECIÓN 3 — El «CRUCE QUE HAY QUE DECLARAR» con Vorágine no lo sostiene la fuente que cita
- QUÉ afirma la ficha: «Juan Pablo Barrientos es a la vez uno de los cuatro periodistas fundadores de la Fundación Vorágine», con fuente en https://voragine.co/nosotros/. A partir de ahí plantea si «los dos valores se están fijando por la misma intuición».
- POR QUÉ: hoy, https://voragine.co/nosotros/ nombra cuatro cofundadores y ninguno es Barrientos: «José Guarnizo Cofundador y director general de Vorágine», «Laila Abu Shihab Vergara Cofundadora y directora de proyectos de Vorágine», «María José Jaramillo Cofundadora y directora ejecutiva y administrativa de Vorágine» y «Angie Pik Cofundadora y directora gráfica de Vorágine». El apellido «Barrientos» aparece 0 veces en el HTML de hoy y también en las capturas de Wayback del 2024-09-09, el 2025-10-06 y el 2026-07-20. Además, su biografía en CasaMacondo pone Vorágine en pasado: «Fue corresponsal en Washington [...]; periodista de La Fm, W Radio, Caracol Radio y Vorágine. [...] Cofundador de CasaMacondo.» Con la regla del presente, el cruce es como mucho historia. No hay papel vigente en dos medios, así que este no es «el segundo caso» tras Daniel Coronell. Puede que Barrientos fundara Vorágine en su día, pero no encontré fuente que lo diga, y la que cita la ficha no lo dice.
- FUENTE Y FECHA: https://voragine.co/nosotros/ (2026-10-10); https://web.archive.org/web/20240909181307/https://voragine.co/nosotros/, https://web.archive.org/web/20251006011143/https://voragine.co/nosotros/ y https://web.archive.org/web/20260720084619/https://voragine.co/nosotros/; https://casamacondo.co/wp-json/wp/v2/users/5 (2026-10-10).
- NIVEL: propiedad o dirección (estructura vigente) y declaración del propio medio.

OBJECIÓN 4 — La lectura del nivel 4 es selectiva: el propio medio dice hoy no tener militancia ideológica
- QUÉ afirma la ficha: «Todo el peso recae en una declaración vigente de misión», en concreto «promover la justicia social, la divulgación ambiental y la complejidad cultural».
- POR QUÉ: el documento editorial vigente, enlazado hoy desde /somos/ como «Directrices editoriales», declara lo contrario de una afiliación: «CasaMacondo contrapone una práctica periodística emancipada de cualquier militancia ideológica y es, respecto de sus audiencias, un medio de comunicación soberano, confiable, creíble e íntegro». En /somos/, la misma frase de misión que cita la ficha va precedida de «Buscamos incidir en el debate público y contar al país desde su pluralidad». La misión de las Directrices también habla de «vulneración de derechos humanos, ambientales y animales, lo mismo que denuncias sobre corrupción y abusos de poder», y eso es fiscalización. Con sus propios criterios, la ficha tendría que haber puesto esta declaración en el CONTRA. Esto no hace mixto al medio, porque las autodeclaraciones valen poco. Pero sí deja sin apoyo la única pata de la ficha: el nivel 4 completo es ambivalente, no apunta a la izquierda.
- FUENTE Y FECHA: https://casamacondo.co/wp-content/uploads/2025/05/Directrices-editoriales-2025.pdf (mayo de 2025, vigente y enlazado el 2026-10-10); https://casamacondo.co/somos/ (2026-10-10).
- NIVEL: declaración del propio medio, hoy.

OBJECIÓN 5 — El valor −0,35 no se puede alcanzar con la evidencia admitida, ni siquiera sumando la voz de la casa (barrido contado)
- QUÉ afirma la ficha: −0,35 apoyado «solo en nivel 4». La ficha misma reconoce que eso incumple el protocolo, pero mantiene el número, y otras fichas lo usan como referencia.
- POR QUÉ: con las objeciones 1 a 4, el nivel 1 hoy documentado (entidad, socios-periodistas y financiación cultural sin financiador partidista) no apunta a la izquierda, y el nivel 4 es ambivalente. Solo queda la vía de la regla de evidencia editorial histórica, así que hice el barrido.
  Voz de la casa considerada: piezas firmadas por el editor general y cofundador Castaño (autor 9), por la cuenta institucional «CasaMacondo» (autor 12) y por otros cofundadores de la plantilla. Excluí las columnas de terceros (por ejemplo Daniella Sánchez Russo, Luis Tejada, Cerosetenta) y las caricaturas, porque no las leí, solo vi los títulos. También excluí como «postura» las piezas que fiscalizan al poder de turno.
  Antes del 07-08-2026 (gobierno Petro), piezas con postura en un eje izquierda-derecha:
   1. 2025-11-08, Castaño, https://casamacondo.co/opinion/miguel-polo-polo-el-rico-mas-pobre-en-su-album-de-fotografias/. Contra la derecha, con un contrapeso dentro del texto: «La crueldad de la extrema izquierda no justifica la crueldad de la extrema derecha.» Lo cuento como postura izquierda y anoto el contrapeso.
   2. 2026-06-06, Castaño, https://casamacondo.co/opinion/abelardo-de-la-espriella/: «El candidato de la extrema derecha colombiana parece construido para esa mutación cultural.» Izquierda. Es encuadre de un candidato en campaña, no fiscalización del poder.
   3. 2026-06-24, Castaño, https://casamacondo.co/opinion/no-tenemos-miedo-cronica-eleccion-colombia/: «por suerte, el ciclo reciente de reformas sociales no desaparecerá [...] la sorprendente votación de algunos sectores populares en favor del modelo económico que más los ha explotado y envilecido». Izquierda, con postura explícita sobre las reformas. El og:description la presenta como «Crónica de CasaMacondo», y el autor escribe «como enviado especial de CasaMacondo».
   4. 2026-07-18, Castaño, https://casamacondo.co/opinion/ignorantes-desvergonzados-jose-castano/: «el legado del sátrapa» (sobre Álvaro Uribe) y «Abelardo de la Espriella resulta minúsculo [...] su ignorancia y [...] sus dogmas». Izquierda. Es antes de la posesión y De la Espriella era presidente electo, no gobernante.
   C1. 2025-11-22, Castaño, https://casamacondo.co/opinion/las-mentiras-de-la-verdad-absoluta-opinion/. CONTRAPESO simétrico: llama «embustes» a mitos de la derecha («que Gustavo Petro es un capo del narcotráfico internacional») y de la izquierda («que las sanciones de Donald Trump a Gustavo Petro [...] fueron un complot uribista», «sabotajes [...] para derrocar al gobierno del cambio»).
   C2. 2026-07-04, Ricardo Mendivil (cofundador), https://casamacondo.co/opinion/importancia-periodismo-independiente/. CONTRAPESO: «los seguidores de Abelardo de la Espriella hicieron señalamientos [...] muchos de los que nos defendían comenzaron a atacarnos por confrontar también al poder de turno: el de Gustavo Petro».
  Después del 07-08-2026 (gobierno De la Espriella):
   5. 2026-08-22, Castaño, https://casamacondo.co/opinion/donald-trump/ (og: «Un periodista lamenta el triunfo electoral del candidato de la extrema derecha»). Izquierda, pero sobre política extranjera.
   6. 2026-10-03, Castaño, https://casamacondo.co/opinion/milei-y-de-la-espriella-felinos-asustados/. Sobre De la Espriella es fiscalización o burla del poder de turno y no cuenta. La parte sobre Milei («El león es manso con los poderosos y fiero con los débiles»), que tampoco es fiscalización interna, la cuento como postura izquierda.
  Recuento: 6 piezas con postura (4 antes del cambio y 2 después, las dos sobre presidentes extranjeros) más 2 contrapesos. No llega al mínimo de 10 piezas ni al de 3 después del cambio. La razón antes del cambio es 4:1 o 4:2 según cómo se pese C2, así que el umbral de 3:1 tampoco queda claro. La regla de nivel 2 no se cumple. Si se cumpliera, el tope sería ±0,30, y −0,35 lo supera.
  El protocolo dice «Sin evidencia de nivel 1-3, no se mueve el número» y «ante la duda, la más cercana a la mixta». Con eso, −0,35 no se puede sostener: o se rebaja hacia la banda mixta, o se declara expresamente como valor de alta no firmable y fuera de comparación.
  Consecuencia que hay que decir: otras fichas usan CasaMacondo en −0,35 como punto de comparación («menos marcado que Vorágine (−0,50) o Cuestión Pública (−0,45)», y a la inversa). Si este valor baja, esas comparaciones pierden su ancla y hay que revisarlas.
- Nota en sentido contrario, para no sesgar: los puntos 2 a 4 son encuadre asimétrico entre candidatos, que la regla del polo fijo NO excluye. En la campaña de 2026 el editor general atacó a De la Espriella en tres piezas y no encontré ninguna pieza de opinión suya contra Cepeda. El perfil «El dedo acusador de Iván Cepeda» (2026-04-30, Pacho Escobar, de plantilla, https://casamacondo.co/perfiles/el-dedo-acusador-de-ivan-cepeda/) es mayoritariamente biográfico, aunque recoge a sus críticos: «Algunas etapas de esa defensa son su talón de Aquiles. Sus opositores lo presentan como un político cuya figura se entrelaza con viejos fantasmas de la guerra». Hay, por tanto, una inclinación observable en la voz del editor general. Es evidencia real y la ficha no la tiene, pero no alcanza el umbral cuantitativo.
- FUENTE Y FECHA: las URL listadas, leídas en HTML crudo el 2026-10-10; lista completa en https://casamacondo.co/wp-json/wp/v2/posts?after=2025-10-01T00:00:00&per_page=100 (páginas 1 a 3).
- NIVEL: hechos editoriales de los últimos 12 meses (voz de la casa) y protocolo.

OBJECIÓN 6 — La «Conducta medida» parte de una fuente que el robots.txt del medio excluye, y la cifra de la ficha está desfasada
- QUÉ afirma la ficha: «Su feed da 10 ítems con mediana de 255 h».
- POR QUÉ: el robots.txt de casamacondo.co dice «Disallow: /feed/» y «Disallow: /*/feed/» (2026-10-10). Si el corpus de DobleFoco lee el RSS de CasaMacondo, lo hace contra la exclusión expresa del medio. No sé qué URL usa el ingestor, así que es una inferencia que conviene comprobar. Sobre las cifras: la API del medio da 24 entradas entre el 2026-08-31 y el 2026-10-10, coherente con las 22 del corpus, y 208 en 12 meses (138 sin contar caricaturas). Eso es unas 4 por semana, no «10 ítems». La medición de nivel 2 (2 piezas en historias) no sirve para nada, como reconoce el propio envío.
- FUENTE Y FECHA: https://casamacondo.co/robots.txt (2026-10-10); API WP del medio (2026-10-10).
- NIVEL: conducta observable y método.

## LO QUE NO PUDE VERIFICAR
- La composición accionaria de CASA MACONDO - SOMOS HISTORIAS SAS y si alguno de los «trece socios» la controla. RUES abierto no trae socios. No pedí certificado de Cámara de Comercio porque es de pago y no tengo acceso. El enlace «Autoevaluación Normas JTI» (https://www.jti-app.com/report/aMlNE9LmzpR61JvK) devuelve la portada de JTI y no el informe, así que no pude leer lo que el medio declaró allí sobre propiedad.
- Quién dirige de hecho la Unidad Investigativa mientras Barrientos está en la beca Nieman 2026-2027. Busqué en /somos/, en su biografía y en las firmas del barrido.
- Qué URL probó la ficha el 2026-08-08 para obtener el 404. Wayback no tiene capturas de /financiacion/ entre el 2026-03-11 y hoy.
- Quiénes están detrás de CONSORCIO NACIONAL DE MEDIOS S.A.S, Estrella Grupo Empresarial SAS y Universal Group Agencia De Comunicaciones S A S, financiadores de 2025. No los investigué. Es la siguiente comprobación útil para el nivel 1.
- El contenido de las 73 caricaturas de Leo Parra (director de arte y caricaturista de plantilla). Solo leí los títulos y no los cuento. Los títulos apuntan a los dos lados: antes del cambio, «Personaje del (d)año» (Benedetti), «El infiltrado» (consulta del Pacto Histórico), «Excusa "médica"» (ministro de Salud), «El tigre de papel», «"El tigre" al desnudo» y «Postura de Centro... Democrático»; después del cambio, «"Administración milagro"» y «"Interlocución milagro"».

## LO QUE FALTA
- La entidad editora (NIT 901747859), la fundación hermana (NIT 901857339), la cifra de «trece socios» y los cuatro cofundadores identificados en el sitio.
- La tabla de financiación de 2025 y la de 2024, con sus porcentajes. Además, que en 2024 el principal proyecto se hizo «con el apoyo del Ministerio de las Culturas»: «Este texto hace parte de un especial sobre el programa Sonidos para la Construcción de Paz y cuenta con el apoyo del Ministerio de las Culturas» (https://casamacondo.co/cronicas/cuando-la-musica-tiende-puentes-donde-antes-solo-habia-abismos/, 2024-12-01). Es dinero de un ministerio del gobierno saliente y queda fuera de la ventana de 12 meses. No aparece en SECOP con los NIT del medio, quizá porque llegó por un intermediario (inferencia). En 2025 no hay fondos públicos en la tabla. Debe declararse como historia reciente, no como estructura vigente.
- Un posible conflicto de interés del tipo que pide el envío: el director general ganó en 2021 el Simón Bolívar con «El rey se pasea desnudo: corrupción en el Fondo de Cultura Económica Colombia» (users/15), y EDICIONES FONDO DE CULTURA ECONOMICA SAS financia en 2025 el especial de libros (PDF 2025). No mueve la orientación, pero es un dato de independencia que conviene registrar.
- El barrido de la objeción 5, con sus contrapesos.
- La declaración «emancipada de cualquier militancia ideológica» en el CONTRA.

## EVIDENCIA QUE NO MUEVE EL NÚMERO
- Después del cambio de gobierno, CasaMacondo fiscaliza a los dos lados, y eso es periodismo, no orientación:
  · Al gobierno entrante: «Viceministro de Vivienda se presenta con una maestría que no ha completado» (2026-09-24, institucional, https://casamacondo.co/investigacion/reynaldo-dsilva-uribe-maestria-externado/) y «Otro viceministro del Tigre presume de un título que no tiene» (2026-10-10, https://casamacondo.co/investigacion/viceministro-ambiente-gustavo-guerrero/).
  · Al gobierno saliente y a Comunes: «Gobierno de Petro entregó tierras a Pablo Catatumbo cuando era senador» (2026-09-19, institucional, https://casamacondo.co/noticia/petro-entrego-tierras-pablo-catatumbo/) y «La ANT le tituló tierras a Germán Gómez cuando era representante a la Cámara» (2026-10-03, https://casamacondo.co/noticia/tierra-firmantes-catatumbo-gomez-ant/).
- Antes del cambio, fiscalizó al gobierno Petro con dureza. «El gobierno que prometió no matar niños asesinó más que el anterior» (2026-06-27, Barrientos, https://casamacondo.co/investigacion/ninos-muertos-en-bombardeos-durante-gobierno-petro/): «Durante el de Gustavo Petro, 57, a un ritmo de 15,2 por año, un 41 por ciento más.» En campaña investigó a candidatos de los dos lados: Carlos Caicedo (2026-05-16, https://casamacondo.co/casamacondo/carlos-caicedo-candidato-embargado/), Santiago Botero (2026-05-22) y De la Espriella (2026-06-13, https://casamacondo.co/investigacion/abelardo-de-la-espriella-fiscalia/).
- El objetivo más constante de la unidad investigativa en 12 meses es la Iglesia católica (Archivo Secreto: Tobón, Ratzinger, Cely Silva, Reyes, entre otros), un eje que no es izquierda-derecha.
- No encontré endoso electoral explícito («votaremos», «apoyamos a») en la sección de Opinión ni en la cuenta institucional durante la campaña de 2026. Busqué en todas las piezas de Opinión y de la categoría «CasaMacondo» entre mayo y junio de 2026 del listado de la API.
- No hay contratos públicos con los NIT del medio en SECOP I ni en SECOP II (2026-10-10).

## SIN OBJECIÓN
No aplica: hay seis objeciones.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** El revisor no escribe ningún documento de identidad ni enlaza consultas de datos.gov.co (nombra los conjuntos, `c82u-588k`, `jbjy-vk9h` y `f789-7hwg`, sin URL). Los dos PDF del medio que enlaza se leyeron enteros y **no traen documentos de identidad**: el de financiación de 2025 da conceptos, financiadores (personas jurídicas) y cifras; las Directrices 2025 solo traen un número de atención pública (línea de ayuda de Medellín). Se pueden enlazar. Las biografías de `/wp-json/wp/v2/users/` muestran el correo profesional que el propio medio publica; esta resolución no los copia. **Esta resolución tampoco escribe ni enlaza ningún documento**: las consultas que cita llevan `$select` (comprobado: devuelven las mismas filas sin datos personales).

**Incidencia del revisor, comprobada.** Dijo que dos PDF cayeron en la carpeta del repositorio. `git status` al empezar esta verificación: limpio. No queda nada suyo ni de esta verificación fuera de los dos archivos que se entregan.

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada (2026-10-10):
  - casamacondo.co: `User-agent: *` con `Disallow` de `/wp-admin/`, `/?s=`, `/feed/`, `/*/feed/` y `/*/embed/`. No excluye `/wp-json/` ni los sitemaps. **Literal, como dice el revisor.** **No se leyó `/feed/`.**
  - voragine.co: solo `/sitio/` y `/bk-sitio/`. datos.gov.co: `Crawl-delay: 1`; se usó solo `/resource`, con un segundo entre consultas. jti-app.com: `/robots.txt` redirige a la portada de journalismtrustinitiative.org.
  - web.archive.org: el índice CDX respondió; las capturas, **429** (bloqueo por tráfico) salvo una (`financiacion/`, 2025-11-07).
  - No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. **No hubo buscador web.**
- **Sitio**, en crudo con `curl -sL --ssl-no-revoke -A "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/126.0 Safari/537.36"`:
  - `/somos/`, `/financiacion/`, `/asi-nos-financiamos/` (404), los dos PDF, `sitemap_index.xml`;
  - la API de WordPress: `/wp-json/wp/v2/users/{3,5,9,12,15}`, `users?per_page=100`, `categories`, `types` y **las 208 entradas de 12 meses con su cuerpo**;
  - `voragine.co/nosotros/`; la crónica del 2024-12-01 sobre «Sonidos para la paz».
- **Registros**, en datos.gov.co:
  - RUES (`c82u-588k`): `nit=901747859`, `nit=901857339` y `razon_social like '%MACONDO%'`.
  - SECOP II (`jbjy-vk9h`), `documento_proveedor`, y SECOP I (`f789-7hwg`), `identificacion_del_contratista`: **cada NIT sin DV, con el DV pegado y con guion** (`901747859`, `9017478594`, `901747859-4`; `901857339`, `9018573398`, `901857339-8`). Y por nombre: `proveedor_adjudicado like '%MACONDO%'`, `like '%CASA MACONDO%'`, `like '%SOMOS HISTORIAS%'`; en SECOP I, `nom_razon_social_contratista` con los dos últimos.
- **Repositorio:** el envío, `fichas/casa-macondo.md`, sus entradas en `shared/mediaRegistry.js`, `shared/mediaOwnership.js` y `shared/centinela.js`, `auditoria/estado.json`, `auditoria/hallazgos.json`, `data/conducta.json`, el lector de feeds (`server/services/ingestDaemon.js`, `fetchFeed`), `shared/userAgent.js`, el protocolo (§1 «Evidencia editorial histórica» y «Datos personales», §2, §5), DECISIONES.md del 2026-10-07 al 2026-10-10, `fichas/voragine.md` (la decisión del 2026-09-16) y todas las menciones de CasaMacondo (lista abajo).
- **El barrido**, reproducible, está en `revision-externa/barridos/casa-macondo.md`.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | La financiación está documentada: 75,3 M en 2025; audiencias 4,1 %; proyectos culturales 83,3 %; sin financiador partidista; en 2024, audiencias 2,44 % | sí | sí | **Aceptada.** Cifras y financiadores literales. La página existe desde el **2025-06-28** (`article:published_time`), no solo desde julio. La URL que da 404 hoy es `/asi-nos-financiamos/`: probablemente la que probó la ficha (inferencia) |
| 2 | Entidades: SAS (NIT 901747859) y fundación (NIT 901857339), activas y renovadas en 2026; «trece socios»; cuatro cofundadores; 0 contratos en SECOP | sí | sí | **Aceptada, con un dato que el revisor no da:** el RUES consigna como **representante legal de las dos a Juan Pablo Barrientos Hoyos**. SECOP: 0 con todas las variantes de NIT y nombre |
| 3 | El cruce Barrientos–Vorágine no lo sostiene la fuente | sí | sí | **Aceptada.** La página de hoy nombra a cuatro cofundadores y ninguno es él; su biografía pone Vorágine en pasado. Las capturas de Wayback existen (CDX) pero no se pudieron abrir (429) |
| 4 | Nivel 4 leído a medias: las Directrices dicen «emancipada de cualquier militancia ideológica», y /somos/, «pluralidad» | sí | sí | **Aceptada.** Literal en el PDF y en /somos/ |
| 5 | El −0,35 no se sostiene; el barrido no llega (6 piezas, todas a la izquierda, 4 y 2; 2 contrapesos) | sí | sí, pieza por pieza | **Aceptada en la conclusión; el recuento se corrige.** Lectura amplia: **5 antes (una leve que él no cuenta) y 0 después**. Sus 2 «después» no entran: «Donald Trump» es una **columna de noviembre de 2024 con fecha nueva**, y lo de Milei es internacional. Omite una opinión **institucional** que fiscaliza al gobierno entrante (28-08-2026). En la lectura estricta del protocolo, **0** |
| 6 | El robots.txt excluye `/feed/` y el registro lo lee; la cifra de la ficha está desfasada | sí | sí | **Aceptada en lo principal; parcial en las cifras.** La ingesta lee `https://casamacondo.co/feed/` (`mediaRegistry.js:303`; la auditoría lo da «sano» el 2026-10-08). Pero «10 ítems» es cierto: el feed da 10 (por defecto de WordPress), no es una frecuencia. Lo desfasado es la mediana de 255 h |

### Lo verificado, objeción por objeción

**1 · Financiación.**
- `https://casamacondo.co/financiacion/`, 200, `article:published_time` 2025-06-28T09:00:04-05:00, `article:modified_time` 2026-06-20T19:28:38-05:00. Enlazada desde /somos/ (`"url":"https:\/\/casamacondo.co\/financiacion\/"`). Incrusta [el PDF de 2025](https://casamacondo.co/wp-content/uploads/2026/03/Asi-nos-financiamos-2025.pdf). Wayback CDX: capturas con 200 el 2025-07-09, el 2025-11-07 y el 2026-03-11, exacto.
- **Tabla de 2025, extraída en modo `-raw`** (que deja cada cifra en su línea; la extracción por columnas del revisor las desalinea, como él mismo avisó). Literal:
  - «Audiencias 3.100.886,00 4,1%» (Donación Vaki).
  - «Especiales y proyectos 62.680.111,91 83,3%»:
    - «Especial 50 mejores libros 2024 10.075.068,91»: Cámara Colombiana del Libro 5.075.068,91; CONSORCIO NACIONAL DE MEDIOS S.A.S 5.000.000,00.
    - «Especial 50 mejores libros 2025 52.605.043,00»: EDICIONES FONDO DE CULTURA ECONOMICA SAS 4.201.681,00; Estrella Grupo Empresarial SAS 10.000.000,00; Fundación Algo en Común 4.201.681,00; Fundación Confiar 5.000.000,00; **Fundación Gloria Zea 11.500.000,00** (el mayor); Fundación Para El Fomento De La Lectura 4.201.681,00; Universal Group Agencia De Comunicaciones S A S 8.500.000,00; UNIVERSIDAD DE LOS ANDES 5.000.000,00.
  - «Talleres de formación 5.761.344,58 7,7%»: «Talles Casa Macondo 2.400.000,00», «Talles Caro y Cuervo 3.361.344,58».
  - «Subvenciones 3.715.828,00 4,9%»: Sembra Media.
  - «Total 75.258.170,49». Y: «Nacimos como empresa el 29 de agosto de 2023».
  - La suma cuadra al céntimo. **Todo el 83,3 % es un solo producto, «Los 50 mejores libros»**, patrocinado por editoriales, fundaciones culturales o empresariales, una universidad y dos agencias. Ninguno es partido político ni entidad pública.
- **2024**, en la captura de Wayback del 2025-11-07 (la única que respondió), literal: «Durante 2024 los ingresos de CasaMacondo ascendieron a […] ($91.760.215). […] correspondiente al 94,92 % de los ingresos, se encuentra la financiación de los proyectos como el especial «Sonidos para la paz», «Los 50 mejores libros del 2024» y «Los 50 mejores libros del 2023». En segundo lugar, correspondiente a un 2,63 % se encuentran los aportes realizados por los socios, en tercer lugar están los aportes realizados por la audiencia, los cuales corresponden al 2,44 %». **Exacto.** La página de hoy ya no trae ese texto: solo el PDF de 2025.
- **Ministerio de las Culturas (2024)**, literal en la [crónica del 2024-12-01](https://casamacondo.co/cronicas/cuando-la-musica-tiende-puentes-donde-antes-solo-habia-abismos/): «Este texto hace parte de un especial sobre el programa Sonidos para la Construcción de Paz y cuenta con el apoyo del Ministerio de las Culturas.» Fuera de la ventana: historia, no estructura. No hay contrato con los NIT del medio en SECOP; por qué vía llegó, no consta.
- **Lo que la ficha decía** («Se sostiene con suscripciones y donaciones»; «404»; «sin documentar») **es falso hoy y era falso el 2026-08-08**: la página llevaba más de un año publicada.

**2 · Entidades.**
- RUES, literal (2026-10-10):
  - «CASA MACONDO - SOMOS HISTORIAS SAS», NIT 901747859, DV 4, Cámara de Bogotá, matrícula 3723800, «SOCIEDADES POR ACCIONES SIMPLIFICADAS SAS», matriculada el 2023-08-29, renovada el 2026-04-03, último año 2026, ACTIVA, CIIU 6391, actualizada el 2026-04-03. **Representante legal: JUAN PABLO BARRIENTOS HOYOS.**
  - «FUNDACIÓN CASA MACONDO - SOMOS HISTORIAS», NIT 901857339, DV 8, Bogotá, matrícula 90064810, «LAS DEMÁS ORGANIZACIONES CIVILES,CORPORACIONES,FUNDACIONES», matriculada el 2024-07-02, renovada el 2026-04-03, ACTIVA, CIIU 6391, actualizada el 2026-09-02. **Representante legal: el mismo.**
  - Consulta sin datos personales: `https://www.datos.gov.co/resource/c82u-588k.json?nit=901747859&$select=razon_social,nit,matricula,camara_comercio,organizacion_juridica,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,estado_matricula,cod_ciiu_act_econ_pri,representante_legal,fecha_actualizacion` (y lo mismo con `901857339`).
  - La fecha de la SAS coincide con la del PDF: «29 de agosto de 2023».
- **«Trece socios»**, literal en las Directrices 2025, apartado «c) Profesionales contratados en modalidad freelance»: «el mismo valor que se les retribuye a los trece socios de CasaMacondo». La composición accionaria **no consta**: el RUES abierto no la da.
- **Cofundadores en el sitio**, literal en `/wp-json/wp/v2/users/`: Tibble (15, «Director general. […] Cofundador de CasaMacondo»), Castaño (9, «Cofundador de CasaMacondo»), Barrientos (5, «Jefe de la Unidad Investigativa. […] Nieman Fellow 2026-2027. Cofundador de CasaMacondo») y Mendivil (3, «Cofundador de CasaMacondo»). En /somos/: Tibble «Director general», Castaño «Editor general», Barrientos «Editor de la Unidad Investigativa».
- **SECOP**: 0 filas con los seis valores de NIT, en SECOP I y en SECOP II. Por nombre: `'%CASA MACONDO%'` y `'%SOMOS HISTORIAS%'`, 0 en los dos. `'%MACONDO%'` en SECOP II da 31 filas, todas de siete proveedores ajenos (Corporación Cultural Macondo, Macondo Corp, juntas de acción comunal de barrios Macondo, una papelería…). Consulta: `https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=count(*)&documento_proveedor=901747859`.
- **Regla de quien dirige:** no consta candidatura ni cargo público vigente de Tibble, Castaño ni Barrientos. No salta el aviso.
- **Que Barrientos esté de becario Nieman en 2026-2027** lo dice su biografía. Que eso le aparte del día a día es inferencia del revisor, y aquí no se usa. Su última firma en la API es del 2026-08-15. Desde entonces, las investigaciones salen con la firma de la cuenta institucional o del editor general.

**3 · El cruce con Vorágine.**
- `https://voragine.co/nosotros/` (2026-10-10): «Cofundador y director general de Vorágine» (José Guarnizo), «Cofundadora y directora de proyectos», «Cofundadora y directora ejecutiva y administrativa» y «Cofundadora y directora gráfica de Vorágine». «Barrientos»: **0 apariciones** en el HTML.
- Capturas de Wayback de esa página: el índice CDX confirma 200 el 2024-09-09, el 2025-10-06 y el 2026-07-20 (y otras desde 2024). **Su contenido no se pudo abrir (429)**: lo de que tampoco lo nombran queda en palabra del revisor.
- Biografía (users/5), literal: «Fue corresponsal en Washington de La Fm y Noticias RCN; director de Teleantioquia Noticias; periodista de La Fm, W Radio, Caracol Radio y Vorágine.» **Pasado.**
- **El cruce se cae.** Está escrito en cinco sitios del repositorio (lista abajo). El «segundo caso, después de Daniel Coronell» también.

**4 · Nivel 4.**
- [Directrices editoriales 2025](https://casamacondo.co/wp-content/uploads/2025/05/Directrices-editoriales-2025.pdf), enlazadas hoy desde /somos/, apartado VISIÓN, literal: «CasaMacondo contrapone una práctica periodística emancipada de cualquier militancia ideológica y es, respecto de sus audiencias, un medio de comunicación soberano, confiable, creíble e íntegro». MISIÓN: «investiga y publica historias sobre vulneración de derechos humanos, ambientales y animales, lo mismo que denuncias sobre corrupción y abusos de poder». Y principios: «imparcialidad y ecuanimidad».
- /somos/, literal: «Buscamos incidir en el debate público y contar al país desde su pluralidad. […] El compromiso con nuestras audiencias es promover la justicia social, la divulgación ambiental y la complejidad cultural.»
- **La ficha citó la última frase y omitió la de la pluralidad y las Directrices.** El nivel 4 completo es ambivalente. Autodeclaraciones: pesan poco en las dos direcciones.

**5 · El barrido** (completo en `revision-externa/barridos/casa-macondo.md`).
- **Universo:** las 208 entradas de la API del 2025-10-10 al 2026-10-10, igual que el revisor: 70 caricaturas y 138 de texto; 169 antes del 07-08 y 39 después. Sin `/feed/`.
- **Las 6 del revisor existen**, con esas fechas, URL y citas literales. Pero:
  - **«Donald Trump» (id 5953), contada como «después», es de noviembre de 2024.** Su id está entre el 5948 (caricatura del 2024-11-07) y el 5974 (2024-11-10). El texto habla de Trump «transfigurado por segunda vez en presidente electo». La API la fecha el 2026-08-22, con `modified` del 2026-07-22, anterior a la publicación. Además es política extranjera. **Fuera.**
  - «Milei y De la Espriella…» (2026-10-03): lo de Milei es internacional (fuera, como en los barridos de El Diario y El Informador); lo de De la Espriella, crítica del presidente en ejercicio (F, no suma). **Fuera.**
  - Falta una leve antes del cambio: 18-06-2026, [«La Virgen del Cobre…»](https://casamacondo.co/opinion/economia-campesina-victimas-conflicto-uraba/), Castaño, que encuadra el programa del candidato («propone desmontar una parte de la arquitectura institucional que hizo posibles procesos como este»).
  - **Omite una opinión con la firma de la cuenta institucional**: 28-08-2026, [«Viviane Morales y el credo de los curas en los colegios públicos»](https://casamacondo.co/opinion/viviane-morales-curas-colegios-publicos/): «que la misma institución que ha encubierto sistemáticamente a abusadores de menores ahora contemple, con el beneplácito del nuevo gobierno, administrar colegios públicos». Fiscaliza al gobierno entrante: no suma, pero es la única pieza de Opinión **de la casa** en el año, y va contra la derecha en el poder.
- **Recuento:**

| Lectura | Antes (I / D) | Después (I / D) | Contrapesos | ¿Cumple? |
|---|---|---|---|---|
| Estricta (cuenta de la casa y director) | 0 / 0 | 0 / 0 | — | No |
| Amplia (+ editor general, cofundadores, plantilla) | 5 (4 + 1 leve) / 0 | 0 / 0 | 2, antes | No: 5 de 10; 0 después; 5:2 |
| La del revisor | 4 / 0 | 2 / 0 | 2 | No |

- **Fiscaliza a los dos gobiernos.** Antes, al de Petro en ejercicio (27-06-2026, niños muertos en bombardeos). Después, al de De la Espriella (28-08, 24-09, 10-10) **y** actos del de Petro y de congresistas de Comunes (19-09 y 03-10). Ninguna celebración del entrante ni disculpa del saliente después del 07-08.
- **La tensión que sí existe,** y el revisor la ve bien: entre el 06-06 y el 18-07, el editor general escribió tres columnas contra De la Espriella y ninguna contra Cepeda. Las investigaciones de campaña fueron sobre Caicedo, Botero, De la Espriella y un exsenador conservador; sobre Cepeda, un perfil biográfico que recoge a sus críticos. Es encuadre asimétrico entre candidatos, firmado y por debajo de todos los mínimos. Se declara; no mueve.

**6 · Feed y robots.**
- Registro, `shared/mediaRegistry.js:303`: `feed: { url: 'https://casamacondo.co/feed/', via: 'direct', category: 'Judicial' }`. Auditoría, `auditoria/estado.json`, 2026-10-08: «sano», 10 ítems, 10 tomados. **La ingesta lee la ruta que el robots.txt excluye para `User-agent: *`**, que incluye a `DobleFocoBot`. Lo que el revisor dejó como inferencia, consta.
- **Desde cuándo lo excluye: no consta.** El CDX de Wayback registra cambios del robots.txt el 2025-05, 2025-07, 2026-02 y 2026-04, y el archivo de hoy tiene otra huella que la última captura (2026-05-02). Su contenido no se pudo leer (429).
- **«10 ítems»** es el tamaño del feed (por defecto de WordPress), no una frecuencia: en eso el revisor se equivoca. **«Mediana de 255 h»** sí está desfasada: la auditoría del 08-10 da un hueco típico de 34,1 h, y la API, 208 entradas en 12 meses (138 de texto). Del 2026-08-31 al 2026-10-10: 24 entradas, 16 de texto, frente a las 22 que mide el corpus.

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se corrigen estas partes:
- **Obj. 5, recuento:** «4 antes y 2 después» → **5 antes (1 leve) y 0 después**. «Donald Trump» es de 2024 con fecha nueva; lo de Milei es internacional.
- **Obj. 5, «voz de la casa»:** el revisor la extiende al editor general sin decir que el protocolo solo nombra al director. Aquí se cuenta en las dos lecturas; el resultado no cambia.
- **Obj. 6, «eso es unas 4 por semana, no "10 ítems"»:** compara un tamaño de feed con una frecuencia. Lo desfasado es la mediana.
- **Obj. 1 (b), alineación de cifras:** su cita sale del modo por columnas, que desalinea los financiadores. Las cifras por financiador, en el punto 1.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente ni cita inventada.** Las URL resuelven, las citas son literales y los registros coinciden al dato. Lo que hay:
- un error de fecha: toma por pieza de 2026 una columna de 2024 (no podía verlo sin mirar el id);
- dos omisiones: el representante legal en el RUES y la opinión institucional del 28-08;
- una comparación mal hecha en la objeción 6;
- y tres capturas de Wayback de Vorágine que aquí no se pudieron reabrir (429). No es fuente falsa: queda sin comprobar.

**Errores de la propia ficha, para no repetirlos:**
- **«404» y «SIN DOCUMENTAR»:** la página de financiación existía desde el 2025-06-28 y estaba enlazada desde /somos/. La ficha probó una URL adivinada en vez de seguir el enlace (inferencia: `/asi-nos-financiamos/` da 404).
- **«Se sostiene con suscripciones y donaciones»:** sin fuente, y falso: el 4,1 % en 2025.
- **El cruce con Vorágine:** atribuido a una página que no lo dice. Pasó sin comprobar a `mediaRegistry.js`, `mediaOwnership.js` y `centinela.js`, que lleva dos meses vigilando un vínculo que no existe.
- **Nivel 1 sin persona jurídica, sin RUES y sin la línea de contratación pública**, obligatoria desde el 2026-10-07.
- **Nivel 4 citado a medias**: la frase de la justicia social sin la de la pluralidad, y sin las Directrices, que dicen lo contrario de una militancia.
- **Un valor relativo a dos vecinos que ya no tienen número**: «menos marcado que Vorágine (−0,50) o Cuestión Pública (−0,45)». Los dos pasaron a «sin medir» el 2026-09-16, por ser colocaciones relativas.
- **Lo que la ficha sí tenía bien:** que el valor descansaba solo en nivel 4, que eso incumplía el protocolo, y que la financiación podía moverlo «en cualquier dirección». Lo dijo y lo dejó sin resolver.

---

**Propuesta para la firma**

**Valor: 0,00, orientación mixta, provisional y sin firmar.** Sale del −0,35.

- **Por qué se mueve, si el barrido no llega.** El barrido no es lo que lo mueve: por la segunda precisión del responsable editorial, un barrido que no llega no deshace nada. Lo que deja sin apoyo el −0,35 es que **las razones por las que se puso han caído**:
  - Se puso solo con nivel 4, y el §2 del protocolo no lo admite: «Una clasificación no puede apoyarse solo en los niveles 4 y 5». La ficha lo reconocía.
  - Ese nivel 4, leído completo, es ambivalente: «emancipada de cualquier militancia ideológica» y «desde su pluralidad» (obj. 4).
  - Y ahora hay **nivel 1**: editora en el RUES, trece socios y una financiación publicada sin financiador de posición conocida. Era justo lo que la refutación 1 de la ficha esperaba.
- **Regla 3.** «Sin evidencia de nivel 1-3, no se mueve el número.» Aquí la hay, de nivel 1, y no señala dirección.
- **Regla 2.** Entre «izquierda moderada» y «orientación mixta», con la duda que queda (la asimetría del editor general), se elige **la más cercana a la mixta**.
- **Y con el barrido como apoyo, no como motor.** La casa fiscaliza a los dos gobiernos a los dos lados del 07-08. Es la conducta que el protocolo describe como periodismo, aunque no llega a sostener el 0,00 «con evidencia» porque la voz de la casa en sentido estricto apenas opina. **Se escribe como 0,00 por ausencia de evidencia de posición, con la tensión declarada**, igual que El Isleño o El Manduco.

**Alternativas declaradas:**
- **Sin medir (`bias: null`)**, como Vorágine, Cuestión Pública y RAYA el 2026-09-16. A favor: es el tipo «no noticioso», y el −0,35 era una colocación relativa frente a dos vecinos que ya no tienen número. En contra: aquí sí hay material (208 piezas, 138 de texto) y se ha leído; «sin medir» diría que no se sabe lo que sí se ha mirado.
- **Mantener −0,35** (lectura literal de «un barrido que no llega no deshace nada»). **No se recomienda:** esa precisión protege valores puestos por otras razones, y aquí la razón era un nivel 4 en solitario que el protocolo no admite y que ya no dice lo que la ficha le atribuía.
- **No se sostiene** ninguna banda a la derecha.

**El feed: retirarlo hoy, con nota, y escribir al medio.**
- **Por qué.** El robots.txt del medio excluye `/feed/` y `/*/feed/` para todo agente, y la decisión que recoge `shared/userAgent.js` es que «los bloqueos de robots se respetan». Seguir leyéndolo contradice lo que el motor declara de sí mismo.
- **Cómo:** comentar la línea, como la de El Isleño (`mediaRegistry.js:1689`), que es el precedente de un medio en el catálogo sin feed. (El Manduco no sirve de precedente para esto: su feed se retiró el 2026-09-02 por otras razones y se reactivó el 2026-10-10.)
- **Qué se pierde:** CasaMacondo deja de entrar en las historias y, por tanto, en el panel de no noticiosos, hasta que haya otra vía. Hoy aporta 22 piezas en 40 días, 2 en historias.
- **Las alternativas, comprobadas:**
  - **`/wp-json/wp/v2/posts`:** el robots.txt **no lo excluye**, y da título, fecha, enlace y extracto. Pero la ingesta solo lee RSS: `fetchFeed` llama a `parser.parseURL` (`rss-parser`) y no hay otra vía que `direct` y `gnews`. Haría falta código (una `via: 'wpjson'`). Y es leer por la puerta de al lado lo que el medio cerró por la de delante: la letra lo permite; la intención, no está clara.
  - **Sitemap** (`post-sitemap4.xml`): permitido, pero tampoco lo lee la ingesta, y no trae títulos.
  - **Google News (`gnews`)**: **no es alternativa.** El robots.txt de news.google.com veta `/rss` a `User-agent: *` (solo permite `/`, `/home`, `/topics/`, `/publications/`, `/stories/`, `/swg/` y `/about`). Ver los avisos.
- **Recomendación:** retirar hoy y escribir al medio pidiendo que permita `/feed/` a `DobleFocoBot` (`userAgent.js`: «Un medio que nos cierra la puerta merece que le escribamos»). Si dice que sí, se reactiva. La `via: 'wpjson'` queda como decisión del responsable editorial, no como atajo.

**Bloque propuesto para `shared/mediaRegistry.js`** (no se escribe en código):

```js
    {
        id: 'casa-macondo', name: 'CasaMacondo', shortName: 'CasaMacondo',
        domain: 'casamacondo.co', country: 'CO', group: 'Investigación independiente',
        /**
         * NO NOTICIOSO — (se conserva el comentario del tipo, tal como está).
         *
         * DE −0,35 A 0,00 (ciclo 2, tanda 8, 2026-10-10). El −0,35 descansaba
         * solo en nivel 4 y citaba media misión. Las Directrices 2025 dicen
         * «emancipada de cualquier militancia ideológica», y el nivel 1 ya
         * consta: editora en el RUES, trece socios, y el 83,3 % de los
         * ingresos de 2025 en patrocinios de «Los 50 mejores libros». El
         * barrido (`revision-externa/barridos/casa-macondo.md`) no llega a los
         * mínimos y muestra fiscalización a los dos gobiernos.
         *
         * FEED RETIRADO EL 2026-10-10: su robots.txt excluye `/feed/` y
         * `/*/feed/` para todo agente, y los bloqueos de robots se respetan
         * (`shared/userAgent.js`). Se leyó hasta ese día. Se reactiva si el
         * medio lo autoriza. `/wp-json/` no está excluido, pero la ingesta
         * solo lee RSS.
         */
        noNoticioso: true,
        bias: 0.0, factuality: 0.88, reviewedAt: null,
        biasRationale: 'Medio de periodismo investigativo, ambiental y cultural. Lo edita CASA MACONDO - SOMOS HISTORIAS SAS (NIT 901747859, ACTIVA), con una fundación hermana; sus Directrices hablan de trece socios. En 2025, el 83,3 % de sus ingresos vino de patrocinios de un especial de libros (editoriales, fundaciones, una universidad); las audiencias, el 4,1 %; ningún financiador de posición conocida. Declara una práctica «emancipada de cualquier militancia ideológica». Su casa fiscaliza a los dos gobiernos a ambos lados del 07-08-2026; las columnas de su editor general atacaron al candidato de la derecha y no al de la izquierda en la campaña, por debajo de los mínimos. 0,00 provisional por ausencia de evidencia de posición — ver fichas/casa-macondo.md.',
        // feed: { url: 'https://casamacondo.co/feed/', via: 'direct', category: 'Judicial' },
    },
```

Y **retirar el comentario huérfano** de las líneas 231-246 (encima de Las2Orillas), que es la antigua nota de CasaMacondo con el cruce de Vorágine.

**Bloque propuesto para `shared/mediaOwnership.js`** (no se escribe en código):

```js
    'casamacondo-direccion': {
        label: 'CasaMacondo — sus cofundadores y su equipo directivo',
        sectores: [],
        personas: [
            { nombre: 'Christopher Tibble', papel: 'Director general y cofundador.', desde: null,
              fuentes: ['https://casamacondo.co/somos/', 'https://casamacondo.co/wp-json/wp/v2/users/15'] },
            { nombre: 'José Alejandro Castaño', papel: 'Editor general y cofundador.', desde: null,
              fuentes: ['https://casamacondo.co/somos/', 'https://casamacondo.co/wp-json/wp/v2/users/9'] },
            { nombre: 'Juan Pablo Barrientos', papel: 'Editor (jefe) de la Unidad Investigativa, cofundador y representante legal de la SAS y de la fundación (RUES, 2026-10-10).', desde: null,
              fuentes: ['https://casamacondo.co/somos/', 'https://www.datos.gov.co/resource/c82u-588k.json?nit=901747859&$select=razon_social,nit,estado_matricula,representante_legal,fecha_actualizacion'] },
            { nombre: 'Ricardo Mendivil', papel: 'Responsable de la operación digital y cofundador.', desde: null,
              fuentes: ['https://casamacondo.co/wp-json/wp/v2/users/3'] },
        ],
    },
```

```js
    'casa-macondo': {
        // 2026-10-10 (ciclo 2, tanda 8): editora y fundación en el RUES,
        // financiación publicada por el medio; la composición de los trece
        // socios no consta. DATOS PERSONALES: las consultas de datos.gov.co
        // van con $select.
        ownerType: 'independiente',
        controlGroup: 'casamacondo-direccion',
        holdings: [
            'Lo edita CASA MACONDO - SOMOS HISTORIAS SAS, NIT 901747859, matrícula 3723800 de la Cámara de Comercio de Bogotá (desde el 29-08-2023), ACTIVA, renovada el 03-04-2026, CIIU 6391. Tiene una fundación hermana, FUNDACIÓN CASA MACONDO - SOMOS HISTORIAS (NIT 901857339, matrícula 90064810, desde el 02-07-2024, ACTIVA). Representante legal de las dos: Juan Pablo Barrientos (RUES, 2026-10-10).',
            'Sus Directrices editoriales 2025 hablan de «los trece socios de CasaMacondo». Cuatro se presentan en el sitio como cofundadores: Christopher Tibble, José Alejandro Castaño, Juan Pablo Barrientos y Ricardo Mendivil. La composición accionaria no consta.',
            'Financiación de 2025, publicada por el medio: 75.258.170 pesos. Especiales y proyectos, 83,3 % (todo del especial «Los 50 mejores libros», patrocinado por la Cámara Colombiana del Libro, Consorcio Nacional de Medios, Ediciones Fondo de Cultura Económica, Estrella Grupo Empresarial, las fundaciones Algo en Común, Confiar, Gloria Zea y para el Fomento de la Lectura, Universal Group y la Universidad de los Andes); talleres, 7,7 %; subvención de Sembra Media, 4,9 %; audiencias, 4,1 %. En 2024: 91.760.215 pesos, 94,92 % proyectos, 2,63 % socios, 2,44 % audiencias.',
        ],
        notes: [
            'Contratación pública (SECOP I y II, NIT 901747859 y 901857339, con y sin dígito de verificación, y por nombre; consultado 2026-10-10): ninguna.',
            'Historia, no estructura: en 2024 su especial «Sonidos para la paz» contó «con el apoyo del Ministerio de las Culturas». No aparece en SECOP con sus NIT.',
            'Desvelamiento de independencia: su director ganó en 2021 el Premio Simón Bolívar con una investigación sobre corrupción en el Fondo de Cultura Económica Colombia, y en 2025 Ediciones Fondo de Cultura Económica patrocinó su especial de libros (4.201.681 pesos). No mueve el eje.',
        ],
        sources: [
            'https://casamacondo.co/somos/',
            'https://casamacondo.co/financiacion/',
            'https://casamacondo.co/wp-content/uploads/2026/03/Asi-nos-financiamos-2025.pdf',
            'https://casamacondo.co/wp-content/uploads/2025/05/Directrices-editoriales-2025.pdf',
            'https://www.datos.gov.co/resource/c82u-588k.json?nit=901747859&$select=razon_social,nit,matricula,camara_comercio,organizacion_juridica,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,estado_matricula,cod_ciiu_act_econ_pri,representante_legal,fecha_actualizacion',
            'https://www.datos.gov.co/resource/c82u-588k.json?nit=901857339&$select=razon_social,nit,matricula,camara_comercio,organizacion_juridica,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,estado_matricula,cod_ciiu_act_econ_pri,representante_legal,fecha_actualizacion',
        ],
        verifiedAt: '2026-10-10',
    },
```

`ownerType: 'independiente'` se mantiene: no hay grupo ni dueño dominante conocido. Su descripción («financiado por donaciones, membresías o cooperación internacional») le encaja a medias: es una SAS de socios-periodistas que vive de patrocinios por proyecto. No hay categoría mejor. `verifiedAt` pasa a 2026-10-10: la comprobación del 2026-08-08 tenía el 404 y el cruce erróneos.

**`shared/centinela.js`, líneas 393-401:** la consulta «Barrientos» vigila un vínculo que no existe. Sustituirla por la financiación, que es lo que puede cambiar el nivel 1: consulta «Así nos financiamos» o «Los 50 mejores libros», con `vigila: 'Su página de financiación y el especial que da el 83 % de sus ingresos. Si aparece un financiador de posición conocida o cambia la composición, el 0,00 se revisa.'`

**Textos a corregir** (los aplica quien el responsable editorial decida; aquí no se toca nada):

En `fichas/casa-macondo.md`:
1. Cabecera: «**−0,35** · Izquierda moderada» → «**0,00** · Orientación mixta, provisional (ciclo 2, 2026-10-10)».
2. **Nivel 1**: tabla nueva con la SAS y la fundación (NIT, matrícula, estado, renovación, representante legal), «trece socios» y los cuatro cofundadores; Barrientos como «Editor de la Unidad Investigativa» (/somos/), no «dirige». **Retirar entero el «CRUCE QUE HAY QUE DECLARAR»** y el enlace a Vorágine. Línea de contratación pública: ninguna.
3. **Financiación — SIN DOCUMENTAR** → «Financiación — documentada por el medio», con la tabla de 2025, la de 2024 y la nota del Ministerio de las Culturas como historia. Retirar «Se sostiene con suscripciones y donaciones», el «404» y la comparación con Volcánicas.
4. **Nivel 4**: añadir «contar al país desde su pluralidad» y la frase de las Directrices.
5. **Nivel 2**: retirar «Su feed da 10 ítems con mediana de 255 h». Poner el barrido (5 y 0 en lectura amplia; 0 en estricta; fiscaliza a los dos gobiernos) con enlace, y que el feed está retirado por su robots.txt.
6. **ARGUMENTO**: retirar «menos marcado que Vorágine (−0,50) o Cuestión Pública (−0,45)» (los dos están sin medir desde el 2026-09-16) y la frase de Volcánicas. Razón nueva: la de esta propuesta.
7. **CONTRA**: la tensión del editor general, con las tres columnas y el perfil de Cepeda.
8. **REFUTACIÓN**: 1 se cumple (se documentó la financiación). Nueva: «Si la voz de la casa toma postura con nombre después del 07-08, o deja de fiscalizar a uno de los dos gobiernos (recuento en enero de 2027); si aparece un financiador de posición conocida».
9. **ESTADO** y una sección **REVISIÓN** con esta resolución.

**Todas las menciones de CasaMacondo como referencia, con lo que habría que ajustar:**

| Archivo:línea | Qué dice | Qué hacer |
|---|---|---|
| `fichas/las2orillas.md:35` | «Es un hueco de nivel 1 y se deja constar, como en CasaMacondo» | Falso ya: CasaMacondo publica su financiación. Quitar «como en CasaMacondo» |
| `fichas/las2orillas.md:73` | «El valor de hoy se propuso "por comparación con CasaMacondo (−0,35) y por debajo de la investigación militante (Vorágine, Cuestión Pública)"» | La ficha ya dice que esa justificación no es evidencia. Añadir que el ancla pasa a 0,00 y que Vorágine y Cuestión Pública están sin medir. **Las2Orillas está en esta misma tanda**: lo decide su resolución |
| `shared/mediaRegistry.js:278` | biasRationale de Las2Orillas: «Valor propuesto por comparacion con CasaMacondo (-0,35) y por debajo de la investigacion militante (Voragine, Cuestion Publica)» | Lo mismo |
| `shared/mediaOwnership.js:1351` | nota de Las2Orillas: «Queda sin documentar […] igual que en CasaMacondo» | Quitar «igual que en CasaMacondo» |
| `shared/mediaRegistry.js:231-246` | Comentario huérfano: «CRUCE QUE HAY QUE DECLARAR: Juan Pablo Barrientos […] uno de los cuatro periodistas fundadores de la Fundación Vorágine» | Retirar |
| `shared/mediaRegistry.js:300-303` | `bias: -0.35`, biasRationale y feed | Bloque de arriba |
| `shared/mediaRegistry.js:307` | Volcánicas: «Ver la nota de CasaMacondo sobre la regla del presente» | Apunta al comentario huérfano: cambiar por «ver `fichas/casa-macondo.md`» o quitar |
| `shared/mediaOwnership.js:1145-1171` | `casamacondo-direccion`, con el cruce | Bloque de arriba |
| `shared/mediaOwnership.js:1357-1369` | `casa-macondo`: «se sostiene con suscripciones y donaciones», «404», cruce | Bloque de arriba |
| `shared/centinela.js:393-401` | Vigila «Barrientos» por el cruce | Sustituir (arriba) |
| `src/docs/catalogo_medios.txt:72` y `:75-80` | Copia del biasRationale de Las2Orillas y de CasaMacondo («sesgo −0.35») | Se regenera solo |
| `revision-externa/pendientes.md:282` | «CasaMacondo \| −0,35 \| … \| **Lista.** Medio nuevo, valor derivado de su declaración vigente» | Actualizar al decidir |
| `revision-externa/envios/ciclo-2-2026-10-10/00-LEEME.md:51` | Índice del envío: «**−0,35** · Izquierda moderada» | Es el envío tal como se mandó: no se toca |
| `fichas/choco-7-dias.md:318` | «~~[…] con el precedente de CasaMacondo~~» | Sin número. Nada |
| `fichas/el-morichal.md:308` | «Es el mismo problema que en Chocó 7 Días y en CasaMacondo» | Sin número. Nada |
| `ESTUDIO_PUNTOS_CIEGOS.md:300`, `:395`, `:452` | Mediciones de agosto con CasaMacondo como «izq» | Documento fechado: nada, o una nota de que el valor cambió |
| `CONTEXTO_ALGORITMO_SESGO.md:85` | «Bloque 3 — 1 medio · sesgo declarado −0,35» | Medido el 2026-07-31, antes del alta de CasaMacondo (08-08): **no es CasaMacondo**. Nada |
| `dist/` y `dist-server/` | Copias compiladas | Se regeneran |

**Lo que NO entra como hecho:**
- la composición accionaria de la SAS ni quién la controla;
- que la beca Nieman aparte a Barrientos de la unidad;
- qué URL probó la ficha el 2026-08-08 (lo de `/asi-nos-financiamos/` es inferencia);
- el contenido de las capturas de Wayback de Vorágine y del robots.txt de mayo (429);
- quién está detrás de Consorcio Nacional de Medios, Estrella Grupo Empresarial y Universal Group;
- por qué vía llegó el apoyo del Ministerio de las Culturas en 2024;
- el contenido de las 70 caricaturas (solo títulos).

**¿Aviso de quien dirige?** No procede: no consta candidatura ni cargo público vigente de nadie de la dirección.

**Decisiones para el responsable editorial:**
1. **Valor.** Recomendación: **0,00 provisional**, por las razones de arriba. Alternativas: «sin medir», como el trío del 2026-09-16; o mantener −0,35, que no se recomienda.
2. **Feed.** Recomendación: **retirarlo hoy** (comentado, con nota) y **escribir al medio**. La `via: 'wpjson'` (permitida por su robots.txt, pero hay que programarla) queda a tu juicio.
3. **El cruce con Vorágine.** Recomendación: retirarlo de los cinco sitios a la vez, y cambiar la vigilancia del centinela a la financiación.
4. **¿Las columnas del editor general son «voz de la casa»?** El protocolo nombra solo al director. Recomendación: precisarlo para los medios sin editorial sin firma (CasaMacondo, y seguramente Volcánicas, Razón Pública y RAYA en esta tanda). Propuesta: cuentan las del director y las de quien firma como editor general **si** el medio no publica editoriales, y se marcan aparte.
5. **Las2Orillas.** Su valor se apoyaba en el de CasaMacondo. Recomendación: que lo decida su propia resolución de esta tanda, con este cambio delante.

**Avisos fuera de esta ficha:**
- **Google News veta `/rss` en su robots.txt** para `User-agent: *` (2026-10-10). El catálogo tiene **9 feeds con `via: 'gnews'`**. Si «los bloqueos de robots se respetan», esos nueve están en la misma situación que este. No se ha revisado uno por uno.
- **Fechas reescritas en WordPress:** al menos una pieza de CasaMacondo de 2024 («Donald Trump», id 5953) lleva fecha de 2026. Un barrido que se fíe solo de `date` puede contar piezas viejas como nuevas. Conviene mirar el id o `modified` cuando una pieza no cuadra con su contexto.
