# Barrido editorial: RTVC Noticias (Inravisión, Sistema de Medios Públicos)

| | |
|---|---|
| **Medio** | RTVC Noticias (`rtvc`), sistema de medios públicos nacional. Hoy se presenta como «Inravisión – Sistema de Medios Públicos» |
| **Valor vigente** | **sin medir** (`bias: null`), decisión del responsable editorial del 2026-09-16, aplicada el 2026-09-18 (antes: −0,35) |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus dos precisiones, leída junto con la regla del polo fijo |
| **Ventana** | 2025-10-10 → 2026-10-10 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Resolución de origen** | `revision-externa/respuestas/opus-5-5-rtvc.md` (el revisor contó 7 + 3 piezas antes y 8 + 3 después, sobre 119 piezas de «Gobierno») |
| **Quién lo hizo** | Claude Opus 5.5 (`claude-opus-5-5`), verificador del ciclo 2, tanda 9, a petición del responsable editorial, el 2026-10-10. Es de la misma casa que el autor de la ficha y que el revisor: su acuerdo no es aval |
| **Estado** | **DECIDIDO el 2026-10-10: +0,30, gubernamental** (antes sin medir), por el responsable editorial: un medio del Gobierno nacional toma la dirección del gobierno que lo controla, con la magnitud tope; firmado en bloque el mismo día (`DECISIONES.md`, «2026-10-10 · Tandas 8 y 9 del ciclo 2: el barrido manda sobre los números sin evidencia»). Lo que más abajo dice «propuesta», «recomendada» o «pendiente» es el estado anterior a la decisión y se conserva como historia |
| **Resultado** | **Hay postura en la voz de la casa a los dos lados del cambio, pero en direcciones opuestas en el eje: a favor de quien gobierna en cada momento.** En el nivel A (firma de la casa) hay 18 piezas antes y 4 después; con el nivel B (titulares de periodistas de plantilla) son 34 antes y 8 después. No hay ni una pieza que mantenga la misma dirección en el eje a los dos lados. **La condición 3 («3 a 1 en la misma dirección», con 3 a cada lado) no se cumple para la izquierda ni para la derecha.** Es oficialismo, y la regla no mueve el número. Contrapesos: 2 antes (parciales) y 0 después |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas, el titular y
> el criterio están aquí para eso. **La clasificación de cada pieza es juicio de
> un solo lector**, de la misma casa que el autor de la ficha y que el revisor.

---

## 1. Método

- **robots.txt** de `www.rtvcnoticias.com` (descargado el 2026-10-10): es el de Drupal por defecto, con `User-agent: *`. Excluye `/core/`, `/profiles/`, `/node/add/`, `/search/` y `/index.php/...`. No nombra a ClaudeBot, Claude-Web ni anthropic-ai. Los listados de sección (`?page=N`) y las piezas no están vetados. **El buscador del sitio (`/search/contenidos`) sí lo está, y no se usó.**
- **Descarga:** `curl -sL --ssl-no-revoke --compressed`, con User-Agent de navegador (Chrome 126) y una pausa entre peticiones. La fecha es el `datePublished` y la firma el `author.name` del JSON-LD de cada pieza. Las dos se extrajeron por programa.
- **Universo, sin muestreo dentro de cada sección:**
  1. **«Gobierno» completa**: `https://www.rtvcnoticias.com/politica/gobierno?page=0` hasta `?page=70`. Se cuenta solo el listado principal (7 piezas por página, antes del paginador), no los bloques de «recomendados». Se descargaron 498 piezas y **402 caen en la ventana**: 375 antes del 07-08-2026 y 27 desde ese día. La más antigua del listado es del 2025-08-20, así que la ventana queda cubierta entera.
  2. **Voz institucional**: `/actualidad/rtvc?page=0..12` (del 2025-10-20 al 2026-10-06) y `/actualidad/inravision?page=0..12` (del 2026-04-01 al 2026-09-09; la sección nace con el cambio de nombre).
  3. **«Política» general**: `/politica?page=0..11`. Cubre del 2026-06-02 al 2026-09-13, es decir, la segunda vuelta, la transición y el primer mes del nuevo gobierno. No llega más atrás: es una ampliación, no la sección entera.
  4. **Opinión**: `/categorias/opinion?page=0..12`. La última pieza es del 2026-07-08. **Después del cambio no se publica opinión.** Son columnas firmadas: no cuentan.
  5. Las cuatro piezas sueltas que cita el revisor fuera de esas secciones (dos de `/economia`, una de `/politica` y una de `/actualidad/rtvc` de 2025-12-07).
  - **En total, 622 piezas únicas en la ventana** (deduplicadas por titular: el medio publica a veces la misma pieza con dos slugs, p. ej. `…-cuatro` y `…-cuatro-0`). Son **573 antes y 49 después**. La caída del volumen es en sí un hecho: el 15-08-2026 se cerró la franja informativa (ver la resolución).
- **Voz de la casa (condición 1), en dos niveles. Se cuentan por separado:**
  - **Nivel A**, voz de la casa en sentido estricto: firma «RTVC Noticias» o «Redacción Digital», o sin firma. Es el criterio del revisor.
  - **Nivel B**: titular propio de una pieza informativa firmada por un periodista de la plantilla. El protocolo cuenta como voz de la casa «los titulares, entradillas y análisis propios no atribuidos a una fuente», y excluye «las columnas firmadas por terceros». Un periodista de plantilla no es un tercero, pero el nivel A es el más seguro, y por eso se dan los dos. **Aquí no se escriben nombres de periodistas**: basta con «firma personal».
  - Se usa el titular del JSON-LD (`headline`). Cuando el `<title>` del HTML (título SEO) dice otra cosa en voz propia, se anota. El revisor citó a veces ese `<title>`: no es una deformación, es otro campo del mismo medio.
- **Clases:**
  - **E, elogio o celebración** del gobierno de turno o de su candidato, en voz propia: el logro se da como hecho («histórico», «éxito», «revolución»), sin atribuirlo. **Cuenta.**
  - **R, rótulo o encuadre contra el adversario** del gobierno de turno (candidato rival, presidente electo, gobierno anterior), en voz propia. **Cuenta.**
  - **I, voz institucional de la entidad alineada con el gobierno de turno**: invitar a su movilización, adoptar su lema, declararse «medio aliado». **Cuenta** como nivel A.
  - **T, transcripción** de un anuncio o una declaración del Ejecutivo, atribuida y sin contraste. **No cuenta**: no es elogio ni rótulo, y la precisión del responsable editorial del 2026-10-09 solo deja sumar elogios, disculpas y rótulos. Se declara su peso.
  - **C, contrapeso**: crítica o reparo al gobierno de turno, en voz propia o en información propia sobre sanciones a sus funcionarios.
  - **Fuera:** servicio (desastres, programación, premios), autopromoción institucional que no toca el eje y columnas.
- **Dirección en el eje.** Antes del 07-08, E y R favorecen al Gobierno Petro y a su candidato frente a la derecha: apuntan a la izquierda. Después, E y R favorecen al Gobierno De la Espriella frente al gobierno anterior: apuntan a la derecha.
- **Límite declarado.** Las piezas R sobre el presidente electo y sus nombramientos antes del 07-08 (n.º 31 y 34 de la tabla «antes») pueden leerse como fiscalización. Van como «límite». Quitarlas no cambia el resultado.

---

## 2. Tablas de piezas que cuentan

Todas las URL son de `https://www.rtvcnoticias.com`. El titular es el literal del JSON-LD (2026-10-10). «Nivel» A o B, según el §1.

### 2.1 Antes del cambio: 2025-10-10 → 2026-08-06 (gobierna Petro)

| # | Fecha | Nivel | Clase | Titular (enlace) | Por qué |
|---|---|---|---|---|---|
| 1 | 2025-10-14 | A | E (leve) | ['Vías para la Paz': la apuesta de 15 billones de pesos del Gobierno para conectar regiones históricamente olvidadas](https://www.rtvcnoticias.com/politica/gobierno/15-billones-para-reconectar-el-pais-con-vias-para-la-paz) | «la apuesta … para conectar regiones históricamente olvidadas», en voz propia |
| 2 | 2025-10-15 | B | E | [CELAG: Gustavo Petro supera a Álvaro Uribe y Juan Manuel Santos en índice de 'Mejor Presidente de la historia de Colombia'](https://www.rtvcnoticias.com/politica/gobierno/celag-gustavo-petro-supera-alvaro-uribe-y-juan-manuel-santos-en-indice-de-mejor) | «Petro supera a Álvaro Uribe y Juan Manuel Santos en índice de "Mejor Presidente de la historia"» |
| 3 | 2025-11-15 | A | E (leve) | [Colombia firma histórico acuerdo con Suecia para adquirir 17 aviones de combate Gripen](https://www.rtvcnoticias.com/politica/gobierno/colombia-firma-historico-acuerdo-con-suecia-para-adquirir-17-aviones-de-combate) | «histórico acuerdo», en voz propia |
| 4 | 2026-01-06 | A | I | [¡Atención! RTVC rechaza amenazas intervencionistas de Trump contra Colombia e invita a la movilización por la soberanía nacional de este miércoles](https://www.rtvcnoticias.com/actualidad/rtvc/rtvc-rechaza-amenazas-intervencionistas-de-trump-contra-colombia-e-invita-la) | la entidad «invita a la movilización por la soberanía nacional» del mismo día que convoca el Gobierno (pieza hermana: «Gobierno colombiano … llama a movilización en respaldo al presidente Petro», 2026-01-06) |
| 5 | 2026-02-02 | A | E | [El Gobierno del presidente Petro ha incautado 3.000 toneladas de cocaína](https://www.rtvcnoticias.com/politica/gobierno/gobierno-petro-ha-incautado-3000-toneladas-de-cocaina) | logro del Gobierno como hecho, en el titular |
| 6 | 2026-02-03 | A | E | [Tres claves que marcan el éxito de la reunión de Estado Petro – Trump](https://www.rtvcnoticias.com/politica/gobierno/tres-claves-que-marcan-el-exito-de-la-reunion-de-estado-petro-trump) | «el éxito de la reunión», en voz propia |
| 7 | 2026-03-01 | A | E (leve) | [Encuesta del CNC revela que presidente Petro alcanza su mayor índice de aprobación: 54,5% de imagen positiva](https://www.rtvcnoticias.com/politica/gobierno/encuesta-del-cnc-revela-que-presidente-petro-alcanza-su-mayor-indice-de) | encuesta favorable como titular |
| 8 | 2026-03-10 | A | E | [Gobierno del presidente Petro ha realizado más de 400 mil operaciones antinarcóticos](https://www.rtvcnoticias.com/politica/gobierno/gobierno-petro-ha-hecho-mas-de-400-mil-operaciones-antinarcoticos) | logro del Gobierno como hecho, en el titular |
| 9 | 2026-04-01 | B | E | [El gobierno del Presidente Gustavo Petro democratiza el acceso a la carrera diplomática en Colombia](https://www.rtvcnoticias.com/politica/gobierno/petro-democratiza-el-acceso-la-carrera-diplomatica-en-colombia) | «democratiza», en voz propia |
| 10 | 2026-04-01 | B | E (leve) | [Encuesta Celag: Presidente Petro alcanza 46,7% de imagen positiva y se destaca por encima de la mayoría de líderes en América Latina](https://www.rtvcnoticias.com/politica/gobierno/encuesta-celag-petro-imagen-positiva) | «se destaca por encima de la mayoría de líderes en América Latina» |
| 11 | 2026-04-07 | A | E | [El mayor aumento del salario mínimo en décadas no destruyó empleo en Colombia, según JP Morgan](https://www.rtvcnoticias.com/economia/el-mayor-aumento-del-salario-minimo-en-decadas-no-destruyo-empleo-en-colombia-segun-jp) | cierre: «podría fortalecer el argumento de que incrementos salariales ambiciosos…» |
| 12 | 2026-04-14 | A | E | [Salario vital sigue en firme a pesar de que el Consejo de Estado ratificó suspensión del decreto](https://www.rtvcnoticias.com/politica/gobierno/salario-vital-firme-decision-consejo-estado) | «sigue en firme a pesar de que el Consejo de Estado ratificó la suspensión»: el encuadre del Gobierno, en voz propia |
| 13 | 2026-04-14 | A | E (leve) | [Campaña Colombia, el País de la Belleza, ha alcanzado 650 millones de vistas en el mundo](https://www.rtvcnoticias.com/politica/gobierno/colombia-el-pais-de-la-belleza-ha-alcanzado-650-millones-de-vistas) | campaña del Gobierno presentada por su alcance |
| 14 | 2026-04-23 | A | I (leve) | [Santa Marta será sede de la Conferencia para la Transición más allá de los Combustibles Fósiles: Inravisión, medio aliado](https://www.rtvcnoticias.com/actualidad/inravision/santa-marta-sede-de-conferencia-para-la-transicion-energetica) | «Inravisión, medio aliado» de la conferencia del Gobierno |
| 15 | 2026-04-30 | A | E | [100 logros del gobierno Petro: de la reducción de la pobreza y el desempleo histórico, hasta la transición energética](https://www.rtvcnoticias.com/politica/gobierno/100-logros-del-gobierno-petro-menos-pobreza-mas-empleo) | «100 logros del gobierno Petro…» (título SEO: «menos pobreza, más empleo») |
| 16 | 2026-05-08 | A | E (leve) | [Por primera vez en la historia, las madres comunitarias son empleadas públicas del Estado colombiano](https://www.rtvcnoticias.com/politica/gobierno/las-madres-comunitarias-son-empleadas-publicas-del-estado) | «Por primera vez en la historia…», en voz propia |
| 17 | 2026-05-18 | A | E (leve) | [Pdte. Petro supera el 50 % de imagen positiva en encuesta reciente de CELAG Data](https://www.rtvcnoticias.com/politica/gobierno/petro-supera-el-50-de-imagen-positiva-en-encuesta-reciente) | encuesta favorable como titular |
| 18 | 2026-05-27 | A | E | [Pdte. Petro afirma que Colombia tiene más clase media que pobres por primera vez en su historia](https://www.rtvcnoticias.com/politica/gobierno/por-primera-vez-colombia-tiene-mas-clase-media-que-pobres) | título SEO en voz propia: «Por primera vez, Colombia tiene más clase media que pobres» (el titular visible lo atribuye: «Pdte. Petro afirma…») |
| 19 | 2026-05-29 | A | E | [Revolución aeroportuaria en Colombia: 19,6 millones de pasajeros en 4 meses y turismo como reemplazo del petróleo y el carbón](https://www.rtvcnoticias.com/politica/gobierno/revolucion-aeroportuaria-19-millones-de-pasajeros-en-4-meses) | «Revolución aeroportuaria en Colombia…», en voz propia |
| 20 | 2026-06-02 | A | R | [Intervención en la política colombiana: Trump anuncia a De la Espriella como su candidato](https://www.rtvcnoticias.com/politica/donald-trump-anuncia-abelardo-espriella-candidato) | «Intervención en la política colombiana:», rótulo en voz propia sobre un candidato |
| 21 | 2026-06-04 | B | E (leve) | [Histórico: declaran la Sierra Nevada de Santa Marta como reserva libre de minería y petróleo](https://www.rtvcnoticias.com/politica/gobierno/gobierno-sierra-nevada-libre-de-petroleo-e-hidrocarburos) | «Histórico:», en voz propia |
| 22 | 2026-06-07 | B | R (candidato) | [Defensores del porte de armas y “de la Patria”: la ciencia los desmiente y advierte los riesgos](https://www.rtvcnoticias.com/politica/la-ciencia-advierte-los-riesgos-del-porte-de-armas) | «Defensores del porte de armas y "de la Patria": la ciencia los desmiente» |
| 23 | 2026-06-09 | B | E (candidato) | [La historia de Iván Cepeda: cómo el dolor de su familia se convirtió en una lucha por la justicia, la paz y los derechos humanos](https://www.rtvcnoticias.com/politica/vida-de-ivan-cepeda-su-familia-y-la-lucha-por-la-paz) | perfil laudatorio del candidato del Gobierno |
| 24 | 2026-06-11 | B | R (candidato) | [Abelardo de la Espriella: de abogado de Álex Saab y David Murcia a candidato presidencial](https://www.rtvcnoticias.com/politica/abelardo-de-la-espriella-de-abogado-de-alex-saab-y-david-murcia-candidato-presidencial) | «de abogado de Álex Saab y David Murcia a candidato presidencial» |
| 25 | 2026-06-13 | B | R (candidato) | [Argumentos técnicos desvirtúan propuesta de Restrepo: Impuestos saludables sí protegen la vida y la nutrición](https://www.rtvcnoticias.com/politica/datos-desmienten-jose-manuel-restrepo-impuesto-saludable-colombia) | «Argumentos técnicos desvirtúan propuesta de Restrepo» |
| 26 | 2026-06-14 | B | E (candidato) | [La ola Cepeda: artistas, académicos, movimientos sociales e influencers respaldan su llegada a la Casa de Nariño](https://www.rtvcnoticias.com/politica/artistas-influencers-academicos-apoyo-ivan-cepeda) | «La ola Cepeda: … respaldan su llegada a la Casa de Nariño» |
| 27 | 2026-06-16 | B | E (leve) | [El peso colombiano consolida una revaluación histórica: el dólar cae cerca del 30% bajo el gobierno del presidente Gustavo Petro](https://www.rtvcnoticias.com/politica/gobierno/el-dolar-cae-cerca-del-30-bajo-el-gobierno-del-presidente-petro) | «revaluación histórica … bajo el gobierno del presidente Gustavo Petro» |
| 28 | 2026-06-17 | B | R (candidato) | [¿Independiente? Estas son las maquinarias políticas y tradicionales que impulsan a Abelardo de la Espriella](https://www.rtvcnoticias.com/politica/maquinarias-politicas-y-tradicionales-que-apoyan-de-la-espriella) | «¿Independiente? Estas son las maquinarias…» |
| 29 | 2026-06-23 | B | R (candidato) | [El Instituto de Pensamiento Progresista desmiente el mito del "voto fusil" promovido por la ultraderecha](https://www.rtvcnoticias.com/politica/el-instituto-de-pensamiento-progresista-desmiente-el-mito-del-voto-fusil) | «… promovido por la ultraderecha» |
| 30 | 2026-06-25 | B | E | [Gobierno del presidente Petro fue el que más invirtió en carreteras del país en comparación a los 3 cuatrienios previos](https://www.rtvcnoticias.com/politica/gobierno/carreteras-gobierno-petro-mayor-inversion-infraestructura-vial) | logro del Gobierno como hecho |
| 31 | 2026-06-29 | A | R (límite) | [Abelardo de la Espriella nombraría como ministro de Vivienda a exalcalde investigado por corrupción](https://www.rtvcnoticias.com/politica/minvivienda-que-nombraria-de-la-espriella-investigado-por-corrupcion) | presidente electo, aún sin gobernar; puede leerse como fiscalización |
| 32 | 2026-07-01 | B | E (leve) | [Más derechos para los trabajadores colombianos: este mes el recargo dominical sube al 90% y la jornada laboral se reduce](https://www.rtvcnoticias.com/politica/gobierno/en-mes-de-julio-el-recargo-dominical-sube-al-90-y-la-jornada-laboral-se-reduce) | «Más derechos para los trabajadores colombianos:» |
| 33 | 2026-07-02 | B | E | [El histórico 8% de desempleo que el presidente Gustavo Petro le entrega al próximo gobierno](https://www.rtvcnoticias.com/politica/gobierno/el-historico-8-de-desempleo-que-el-presidente-gustavo-petro-le-entrega-al-proximo) | «El histórico 8 % de desempleo que … le entrega al próximo gobierno» |
| 34 | 2026-07-08 | B | R (límite) | [Jaime Andrés Beltrán liderará MinVivienda con un escándalo de corrupción sin respuesta por más de $23 mil millones](https://www.rtvcnoticias.com/politica/jaime-andres-beltran-caso-23-mil-millones-minvivienda) | «con un escándalo de corrupción sin respuesta» (ministro designado, aún sin gobernar) |

### 2.2 Después del cambio: 2026-08-07 → 2026-10-10 (gobierna De la Espriella)

| # | Fecha | Nivel | Clase | Titular (enlace) | Por qué |
|---|---|---|---|---|---|
| 1 | 2026-08-16 | B | R | [Se acaba el aparato de propaganda en el Sistema de Medios Públicos de Colombia](https://www.rtvcnoticias.com/actualidad/inravision/se-acaba-el-aparato-de-propaganda-en-el-sistema-de-medios-publicos) | «Se acaba el aparato de propaganda»; «En la Patria Milagro se vivirá una nueva etapa» |
| 2 | 2026-08-22 | A | R | [Usaron la plata de la educación para pagar propaganda](https://www.rtvcnoticias.com/actualidad/inravision/usaron-la-plata-de-la-educacion-para-pagar-propaganda) | «Increíble hallazgo»; «propaganda» para la etapa anterior, con la ministra y la gerente como fuente |
| 3 | 2026-09-03 | A | R (leve) | [Inravisión, Sistema de Medios Públicos ordena cese de emisión de cuatro emisoras de paz que operaban clandestinamente](https://www.rtvcnoticias.com/actualidad/inravision/inravision-sistema-de-medios-publicos-ordena-cese-de-emision-de-cuatro) | «que operaban clandestinamente»; «el acta … no fue firmada por los dos delegados del gobierno anterior» |
| 4 | 2026-09-10 | A | I | [RTVC avanza en la transformación del Sistema de Medios Públicos](https://www.rtvcnoticias.com/actualidad/rtvc/rtvc-avanza-en-la-transformacion-del-sistema-de-medios-publicos) | «En la Patria Milagro comienza una nueva etapa para RTVC»: el lema del Gobierno |
| 5 | 2026-09-13 | B | E (leve) | [Los cinco motores con los que el Gobierno De la Espriella busca construir la Patria Milagro](https://www.rtvcnoticias.com/politica/los-cinco-motores-con-los-que-el-gobierno-de-la-espriella-busca-construir-la-patria) | el lema del Gobierno («Patria Milagro») en el titular |
| 6 | 2026-09-19 | B | E (leve) | [Gobierno Nacional inyecta $2 billones de pesos para proteger la red de salud golpeada por el terremoto](https://www.rtvcnoticias.com/politica/gobierno/gobierno-nacional-inyecta-2-billones-de-pesos-para-proteger-la-red-de-salud) | «inyecta … para proteger», encuadre del anuncio |
| 7 | 2026-09-25 | B | R | [Gobierno anterior dejó sin un peso el Sistema de Medios Públicos](https://www.rtvcnoticias.com/actualidad/rtvc/gobierno-anterior-dejo-sin-un-peso-el-sistema-de-medios-publicos) | «Gobierno anterior dejó sin un peso…»; «la administración anterior asumió compromisos … sin contar con recursos» |
| 8 | 2026-09-28 | A | R | [Gobierno anuncia conversaciones con el FMI ante el deterioro recibido de las finanzas públicas](https://www.rtvcnoticias.com/politica/gobierno/gobierno-anuncia-conversaciones-con-el-fmi-ante-el-deterioro-recibido-de-las) | «el deterioro recibido»: la tesis del Gobierno sobre la herencia, en voz propia |

---

## 3. Lo que no cuenta pero se declara

### 3.1 Transcripción del Ejecutivo (T), a los dos lados

La sección «Gobierno» es, ante todo, la voz del presidente de turno. En los titulares de las 402 piezas de la ventana, el sujeto es el Ejecutivo («Presidente…», «Pdte.…», «Gobierno…», un ministerio o la Cancillería):

| | Piezas de «Gobierno» | Con el Ejecutivo de sujeto | Firma de la casa (A) |
|---|---:|---:|---:|
| Antes del 07-08 | 375 | 318 (85 %) | 257 |
| Desde el 07-08 | 27 | 17 (63 %) | 15 |

Ejemplos, después: «Chocó tendrá prioridad en la reconstrucción tras el terremoto, anuncia presidente De La Espriella» (2026-08-14), «“La seguridad tiene rostro”: presidente De La Espriella anuncia Fuerza Urano…» (2026-10-05), «Presidente De La Espriella ordena plan de austeridad…» (2026-10-08), «Gobierno propone agilizar licencias ambientales y consultas previas…» (2026-10-10, en `/economia`). Ejemplos, antes: «“Ni un paso atrás y jamás de rodillas”: presidente Petro responde a su inclusión en la Lista Clinton» (2025-10-24), «Un clan de pedófilos quiere acabar la democracia en Colombia: presidente Petro» (2025-11-10), «Presidente Petro denuncia que "fuerzas uribistas dentro de Ecopetrol" sabotean…» (2026-03-30).

Son la misma conducta con los dos gobiernos: reproducir al Ejecutivo sin contraste. **No suma para el mínimo**, pero es el rasgo más estable del archivo.

### 3.2 Contrapesos (C)

- **Antes, 2 parciales, ambos de nivel B** e informativos, sobre sanciones a funcionarios del Gobierno Petro: «Procuraduría suspende de sus cargos al director de la UNGRD, Carlos Carrillo, y al embajador en Brasil, Alfredo Saade» (2026-06-02, `/politica/carlos-carrillo-alfredo-saade-suspendidos-procuraduria`) y «Carlos Carrillo renunció a la UNGRD tras suspensión de la Procuraduría» (2026-06-05, `/politica/gobierno/carlos-carrillo-renuncia-la-ungrd-tras-suspension-de-la-procuraduria`). Ninguno en voz de la casa.
- **Después, 0.** Lo más parecido es «Presidente De la Espriella le pide la renuncia al presidente de Colpensiones» (2026-09-24, nivel B), que cuenta una decisión del propio Gobierno. Las piezas de control posteriores apuntan a la etapa anterior: «Contraloría instaló la Auditoría de cumplimiento de los contratos del Sistema de Medios Públicos RTVC» (2026-08-24) y «Contraloría … adelanta revisión de los recursos administrados por MinIgualdad» (2026-09-29).
- **La oposición desaparece del archivo después del cambio.** En las 49 piezas posteriores no hay ninguna sobre Iván Cepeda ni sobre el Pacto Histórico. Antes, solo en `/politica` entre el 02-06 y el 06-08, hay decenas.

### 3.3 Servicio público con los dos lados (no mueve el número)

- «Inravisión convoca a los candidatos presidenciales a definir un debate nacional antes del 31 de mayo» (2026-04-30, A).
- «Inravisión expresa su disposición para organizar debate entre Iván Cepeda y Abelardo de la Espriella» (2026-06-06, B).
- «Inravisión sí tuvo disposición para producir y transmitir la posesión presidencial de Abelardo de la Espriella» (2026-08-04, B).
- Después del cambio, gran parte de la producción es servicio: el terremoto, El Niño y los incendios. Un ejemplo es «UNGRD activa plan nacional para combatir incendios forestales en 18 departamentos» (2026-10-06, A).

### 3.4 Columnas

En `/categorias/opinion` hay 6 piezas en la ventana, firmadas por columnistas, por ejemplo «El Escudo de las Américas o la guerra contra la izquierda latinoamericana» (2026-03-30). No cuentan. La última es del 2026-07-08.

---

## 4. Recuento y aplicación de la regla

| | Antes (Petro) | Después (De la Espriella) |
|---|---:|---:|
| **Nivel A** (firma de la casa): E / R / I | 14 / 2 / 2 = **18** | 0 / 3 / 1 = **4** |
| **Nivel B** (titular de periodista de plantilla): E / R | 10 / 6 = **16** | 2 / 2 = **4** |
| **Total A + B** | **34** | **8** |
| Dirección en el eje | izquierda (a favor del Gobierno Petro y de su candidato; contra el candidato y el presidente electo de la derecha) | derecha (a favor del Gobierno De la Espriella; contra la etapa anterior) |
| Contrapesos | 2 parciales (B) | 0 |

**Las cinco condiciones:**

1. **Voz de la casa.** Sí, en el nivel A (22 piezas) y, si se acepta, en el B (20 más).
2. **A los dos lados del cambio.** Hay postura a los dos lados, pero **en sentidos opuestos**.
3. **Sostenida: ≥ 10 piezas, ≥ 3 a cada lado y ≥ 3 a 1 en la misma dirección.**
   - Hacia la izquierda: 34 antes y **0 después**. No llega al mínimo por lado.
   - Hacia la derecha: **0 antes** y 8 después. Tampoco.
   - Sumar las 42 en una sola cuenta («34 a 8 hacia la izquierda») sería contar como izquierda lo que solo es el doble de volumen de la etapa anterior. Después del cierre de la franja informativa, la producción política cae de 573 a 49 piezas.
   - **No se cumple para ninguna dirección.**
4. **Contrapesos escritos.** Ver §3.2.
5. **Reproducible.** Las tablas del §2 y el método del §1.

**Conclusión.** La regla no mueve el número. Lo que el barrido muestra es lo que el polo fijo llama «medir contra quién le tocó ejercer»: el medio celebra a Petro con Petro, y al Gobierno De la Espriella con De la Espriella. La prueba de la regla («si el gobierno cambiara mañana y el medio mantuviera exactamente la misma conducta, ¿cambiaría su clasificación?») da sí en los dos sentidos: −0,35 antes y algo a la derecha ahora. Eso es medir al gobierno, no al medio. **Oficialismo, como preveía el responsable editorial el 2026-08-08.**

**El encuadre asimétrico entre candidatos de la etapa anterior** (las piezas de la segunda vuelta marcadas «candidato» en la tabla «antes», más la MOE UE) es lo único que la regla del polo fijo no excluye, y lo trata la resolución. Tiene dos límites:

- el candidato favorecido era el del Gobierno;
- la redacción que lo produjo se desmontó en agosto y septiembre de 2026.

---

## 5. Comparación con el barrido del revisor

- **Sus 119 piezas son las de las páginas 0 a 16 de «Gobierno».** Recontadas con el `datePublished` del JSON-LD, dan **92 antes y 27 después**. El revisor da 88 y 31: la diferencia es de fechas en el límite. Este barrido llega hasta la página 70, es decir, a 12 meses.
- **Coinciden** en lo esencial (oficialismo) y en 9 de sus piezas: A1, A2, A4, A5 (por su título SEO), A6, D2, D9, D10 y D11. A3, A7, A8, A9 y A10 son, aquí, transcripción atribuida. A3 y A7 llevan un título SEO más afirmativo que el titular, y contarlas no cambia nada.
- **Difieren en la clase de D1 y D3 a D8.** El revisor las cuenta como «favorables o acríticas». Aquí son transcripción (T): reproducen el anuncio con su titular, pero no lo celebran en voz propia. Si se contaran, habría que contar también como T los cientos de transcripciones de la etapa Petro, y la simetría quedaría igual.
- **Lo que este barrido añade:**
  - 12 meses en vez de 5;
  - el nivel B, donde está casi todo el encuadre entre candidatos de la segunda vuelta;
  - la pieza institucional que «invita a la movilización» convocada por el Gobierno (2026-01-06);
  - la constatación de que la oposición desaparece del archivo después del cambio.

---

## 6. Para rehacerlo

1. Descargar `https://www.rtvcnoticias.com/politica/gobierno?page=N` (N = 0..70) y quedarse con los enlaces `<a href="/…" hreflang="es">` anteriores a `class="rtvc-pager"`.
2. Lo mismo con `/actualidad/rtvc`, `/actualidad/inravision` y `/categorias/opinion` (N = 0..12) y con `/politica` (N = 0..11).
3. De cada pieza, el `datePublished`, el `author.name` y el `headline` del bloque `application/ld+json`. Filtrar del 2025-10-10 al 2026-10-10 y deduplicar por titular.
4. Clasificar con las clases del §1. Las piezas que cuentan están en el §2. Todas las demás son T, servicio, autopromoción o columnas.
