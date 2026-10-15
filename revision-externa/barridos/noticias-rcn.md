# Barrido editorial: Noticias RCN

| | |
|---|---|
| **Medio** | Noticias RCN (`noticias-rcn`), noticiero de televisión nacional de la Organización Ardila Lülle. Portal: noticiasrcn.com |
| **Valor vigente** | **+0,25**, firmado en bloque el 2026-10-10 (`reviewedAt: '2026-10-10'`). Su razón escrita es una frase sin fuente: «énfasis en seguridad y crítica frecuente al gobierno progresista». La propiedad (nivel 1) no da una posición política conocida, y las cinco piezas del nivel 5 de la ficha son crítica al gobierno saliente, que el polo fijo no cuenta. Es decir: **el valor se apoya solo en los niveles 4 y 5**, y por la precisión del 2026-10-10 el barrido manda |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus precisiones del 2026-10-09 y del 2026-10-10 |
| **Ventana** | 2025-10-11 → 2026-10-11 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Lo que pedía la ficha** | Comparar cómo trata al gobierno entrante frente al saliente (REFUTACIÓN, punto 2) |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-11. Es de la misma casa que el autor de la ficha: su acuerdo no es aval |
| **Estado** | **FIRMADO el 2026-10-12: +0,15** (antes +0,25), el valor que proponía este barrido. Aplicado en el registro, la ficha y el texto público (`DECISIONES.md`, 2026-10-12). Lo que más abajo dice «propuesta» o «pendiente de firma» es el estado anterior a la firma y se conserva como historia |
| **Decisión del responsable editorial** | Se firma la propuesta principal, +0,15. No se toma la lectura alternativa de +0,20 que el §6 declaraba defendible |
| **Resultado** | **Cumple los mínimos en la lectura principal, por poco y con piezas leves.** 26 piezas con postura en voz de la casa: **22 D y 4 I (5,5 a 1)**; 10 D antes del cambio y 12 después. Aparte, **27 piezas que fiscalizan a Petro mientras gobierna frente a 2 que fiscalizan a De la Espriella** desde que gobierna. Sin las piezas «leves» no llega a 10 |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas y el
> criterio están aquí para eso. **La clasificación de cada pieza es el juicio
> de un solo lector.**

---

## 1. Método

- **robots.txt** de `www.noticiasrcn.com`, descargado el 2026-10-11 antes de cualquier otra petición: `User-agent: *` con `Allow: /` y `Disallow: /buscar`. Los bloqueos totales son para agentes con nombre propio (HTTrack, WebZIP, Slurp, etc.), ninguno de los cuales es el nuestro. Declara cinco sitemaps (`/sitemapindex`, `/sitemapnews`, de vídeos, de etiquetas y el de Google News). **No excluye nada de lo que se usó.** No se tocó `/buscar`.
- **User-Agent honesto** en todas las peticiones: `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. No se usó UA de navegador. **Ritmo:** una petición cada 1,2 s como mínimo, en serie; unas 1.350 peticiones en total, todas con respuesta 200.
- **Fuentes de URL: solo las del propio medio.** El `sitemapindex` enlaza un sitemap por mes (`/sitemaps/articles_<Mes>_<Año>.xml.gz`). Se bajaron los 13 de octubre de 2025 a octubre de 2026: **30.656 URL fechadas dentro de la ventana**. Sin buscadores, sin Internet Archive. No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex.
- **Quién es la voz de la casa aquí.** Noticias RCN **no publica editoriales**: no hay sección ni URL con ese nombre en los 12 meses. La sección `/opinion/` (336 piezas en la ventana) es de **columnistas que firman con su nombre** (46 firmas: abogados, gremios, Greenpeace, académicos, periodistas invitados). Por la condición 1 **no cuentan**, y no se clasificaron. En cambio, **todas las notas informativas van firmadas «Noticias RCN»** (campo `author` del JSON-LD: 1.330 de 1.330), es decir, **sin firma personal**. Su titular y su entradilla son voz de la casa cuando la valoración no va entre comillas ni atribuida a una fuente en la misma frase. Eso es lo que se barrió.
- **Filtro sistemático por términos.** De las 30.656 URL se tomaron las de las secciones Colombia, Economía, Salud, Tendencias y Emisiones cuyo slug contiene `petro`, `espriella`, `abelardo`, `cepeda`, `gobierno`, `casa-de-narino`, `presidente-electo` o `mandatario`, y las de Internacional con `petro`, `espriella`, `abelardo` o `gobierno`. Salen **1.330 piezas**, que se descargaron todas: **932 antes del 07-08 y 398 desde ese día**. De cada una se leyó el titular, la entradilla (`description` del JSON-LD) y la fecha (`datePublished`).
- **Lectura.** Se leyeron los 1.330 titulares. Un segundo filtro marcó las 399 piezas cuyo titular o entradilla, quitado lo que va entre comillas, nombran al Gobierno o a un candidato y llevan un término valorativo (polémica, escándalo, golpe, histórico, éxito, ambicioso, etc.); de esas se leyó la entradilla. Las que tenían postura o la rozaban, unas 70, se leyeron por el cuerpo (los primeros párrafos).
- **Qué se clasificó.** Solo piezas con postura **en voz propia** sobre el Gobierno nacional, las candidaturas presidenciales o el presidente (electo o en ejercicio). Lo que va atribuido («expertos cuestionan», «según el alcalde») se declara, pero no cuenta.
  - **D**, dirección derecha: encuadre desfavorable a la candidatura de izquierda (Cepeda, Pacto Histórico) o favorable a De la Espriella como candidato o presidente electo; desde el 07-08, elogio o disculpa al Gobierno De la Espriella, o crítica en voz propia al Gobierno Petro ya fuera del poder (marcada **retro**).
  - **I**, dirección izquierda: lo simétrico.
  - **M**, mixta: reparte a los dos lados en la misma pieza. No suma.
  - **F**, solo fiscaliza a quien gobierna. **No suma** (precisión del 2026-10-09), pero se declara y se usa para comparar el trato.
  - **«leve»**: la postura está en una palabra o en una pregunta del titular, o la entradilla la atribuye a terceros. Cuenta en la lectura principal, como en El Pilón; el §3 da el recuento sin ellas.
- **Descargas y scripts** en la carpeta temporal de la sesión, fuera del repositorio, en carpetas separadas. No se guarda ni se publica el texto de ninguna pieza: aquí solo van titulares literales y fragmentos breves.

---

## 2. Piezas clasificadas

Títulos literales del campo `headline`. Fecha de `datePublished`.

### 2.1 Antes del cambio: 2025-10-11 → 2026-08-06 (gobierna Petro)

| # | Fecha | Título literal | URL | Clase | Por qué |
|---|---|---|---|---|---|
| 1 | 2026-01-17 | Las cuentas no tan claras de las campañas de Carolina Corcho e Iván Cepeda | [enlace](https://www.noticiasrcn.com/colombia/las-cuentas-no-tan-claras-de-las-campanas-de-carolina-corcho-e-ivan-cepeda-981362) | D | El juicio «no tan claras» es del titular. La entradilla: «Una nueva polémica implica a Carolina Corcho e Iván Cepeda» |
| 2 | 2026-03-16 | Controversia por palabras del candidato presidencial Iván Cepeda sobre Antioquia | [enlace](https://www.noticiasrcn.com/colombia/controversia-por-palabras-del-candidato-presidencial-ivan-cepeda-sobre-antioquia-1002549) | D leve | Abre en voz propia: «Hay indignación por declaraciones de Iván Cepeda» |
| 3 | 2026-03-17 | Le respondieron con todo: alcaldes de Antioquia estallaron contra Iván Cepeda por sus polémicas declaraciones | [enlace](https://www.noticiasrcn.com/colombia/alcaldes-de-antioquia-estallaron-contra-ivan-cepeda-por-sus-polemicas-declaraciones-1003149) | D leve | «polémicas declaraciones» y «Le respondieron con todo» en el titular |
| 4 | 2026-04-20 | Retos, condiciones y dudas: ¿Iván Cepeda quiere debatir o está esquivando el cara a cara? | [enlace](https://www.noticiasrcn.com/colombia/cuales-son-las-condiciones-que-puso-ivan-cepeda-para-debatir-1013769) | D leve | La pregunta es del titular; la entradilla la atribuye a «expertos». Contraste: el 21-04 De la Espriella rechaza debatir en el Congreso y el titular es neutro («rechaza invitación para debatir en el Congreso», [enlace](https://www.noticiasrcn.com/colombia/abelardo-de-la-espriella-rechaza-invitacion-para-debatir-en-el-congreso-1014397)) |
| 5 | 2026-04-21 | Las condiciones que puso Iván Cepeda para los debates presidenciales: ¿Un paso atrás? | [enlace](https://www.noticiasrcn.com/colombia/expertos-hablan-sobre-las-condiciones-que-puso-ivan-cepeda-para-los-debates-1014116) | D leve | Misma pauta: el titular hace suya la pregunta de un panelista |
| 6 | 2026-05-31 | ¿Quién es Iván Cepeda, el líder de izquierda que llega a la segunda vuelta presidencial? | [enlace](https://www.noticiasrcn.com/colombia/quien-es-ivan-cepeda-quien-llega-a-segunda-vuelta-presidencial-1026606) | D leve | Perfil en voz propia: «la ortodoxia más pura de ese sector», «ideas revolucionarias». Va en pareja con el n.º 11 |
| 7 | 2026-06-04 | ¿Cepeda pierde terreno en la conquista del centro, previo a la segunda vuelta? | [enlace](https://www.noticiasrcn.com/colombia/cepeda-pierde-terreno-en-la-conquista-del-centro-previo-a-la-segunda-vuelta-1027796) | D | Entradilla en voz propia: «Los días siguientes a elecciones no parecen haber mejorado para el candidato del Pacto, en medio de acusaciones de “fraude” que no respaldan las misiones de observación electoral» |
| 8 | 2026-06-10 | ¿Se está fortaleciendo la campaña de Abelardo de la Espriella tras la polémica por uso de símbolos patrios? | [enlace](https://www.noticiasrcn.com/colombia/se-impulso-la-campana-de-abelardo-de-la-espriella-tras-la-polemica-por-uso-de-simbolos-patrios-1029548) | D leve | El titular plantea el beneficio para el candidato; el fallo se califica de «exagerado» por boca de panelistas |
| 9 | 2026-06-25 | Habló el ‘genio’ detrás de la victoria de Abelardo: reveló el secreto para el éxito de la campaña | [enlace](https://www.noticiasrcn.com/colombia/quien-es-carlos-suarez-el-genio-detras-del-triunfo-de-abelardo-de-la-espriella-1034633) | D leve | Elogio en el titular («genio», «éxito») al presidente electo y su campaña |
| 10 | 2026-07-29 | Gobierno De la Espriella anuncia ambicioso proyecto que cambiará la movilidad en el Caribe | [enlace](https://www.noticiasrcn.com/colombia/de-la-espriella-anuncia-proyecto-para-transformar-corredor-cienaga-barranquilla-1045067) | D leve | «ambicioso» y «cambiará», en voz propia, sobre un anuncio del presidente electo |
| 11 | 2026-05-31 | Abelardo de la Espriella, el ‘outsider’ millonario que se disputa la Presidencia de Colombia | [enlace](https://www.noticiasrcn.com/colombia/quien-es-abelardo-de-la-espriella-el-tigre-candidato-a-la-presidencia-de-colombia-1026581) | **I** | Perfil en voz propia: «El polémico abogado penalista», «controversial», «un discurso antisistema y de desprecio por la izquierda», defensor de «narcotraficantes» |
| 12 | 2026-06-22 | Cepeda responde a la polémica frase de De la Espriella sobre que “'El Tigre' todavía puede morder más duro”: esto dijo | [enlace](https://www.noticiasrcn.com/colombia/que-dijo-cepeda-despues-del-discurso-de-abelardo-tras-conocerse-los-resultados-1033242) | **I leve** | «polémica frase», en voz propia, sobre el presidente electo |

**Fiscalización de Petro mientras gobierna (F: se declara, no suma).** Titulares con la valoración en voz propia; la lista no es exhaustiva, porque F no cuenta:

| Fecha | Título literal | URL |
|---|---|---|
| 2025-10-14 | ¿El Gobierno estaría entablando diálogos de paz con ‘Pipe Tuluá’? Crece la polémica | [enlace](https://www.noticiasrcn.com/colombia/pipe-tulua-asegura-tener-dialogos-de-paz-con-el-gobierno-947393) |
| 2025-10-29 | Disidencias han crecido un 70% y Clan del Golfo, un 60% en Antioquia durante el Gobierno Petro | [enlace](https://www.noticiasrcn.com/colombia/disidencias-han-crecido-un-70-y-clan-del-golfo-un-60-en-antioquia-durante-el-gobierno-petro-953821) |
| 2025-11-10 | Negativa del Gobierno Petro retrasará la construcción del Tren de Cercanías por lo menos un año | [enlace](https://www.noticiasrcn.com/colombia/negativa-del-gobierno-petro-retrasara-la-construccion-del-tren-de-cercanias-por-lo-menos-un-ano-958342) |
| 2026-01-14 | Nuevo remezón en el gobierno Petro a menos de siete meses de terminar su mandato | [enlace](https://www.noticiasrcn.com/colombia/nuevo-remezon-en-el-gobierno-petro-a-menos-de-siete-meses-de-terminar-su-mandato-980403) |
| 2026-01-19 | Serían 24 los funcionarios del gobierno Petro salpicados por irregularidades académicas en la Fundación San José | [enlace](https://www.noticiasrcn.com/colombia/serian-24-los-funcionarios-del-gobierno-petro-que-no-habrian-presentado-la-prueba-saber-pro-981813) |
| 2026-02-02 | Gobierno ‘se echa para atrás’ y retira el proyecto de ley que perjudicaba a las apps de transporte | [enlace](https://www.noticiasrcn.com/colombia/gobierno-retira-el-proyecto-de-ley-que-perjudicaba-a-las-aplicaciones-de-transporte-como-uber-987291) |
| 2026-02-03 | ¿Cuánto le cuesta al país la ’contratitis’ preelectoral del gobierno Petro? | [enlace](https://www.noticiasrcn.com/colombia/cuanto-le-cuesta-al-pais-la-contratitis-preelectoral-del-gobierno-petro-987592) |
| 2026-02-12 | Gobierno Petro hizo contratos por $14 billones antes de que iniciara La Ley de Garantías | [enlace](https://www.noticiasrcn.com/colombia/gobierno-petro-hizo-contratos-por-14-billones-antes-de-que-iniciara-la-ley-de-garantias-990950) |
| 2026-02-25 | César Manrique y Carlos R. González, los dos alfiles del presidente Petro prófugos de la justicia por corrupción | [enlace](https://www.noticiasrcn.com/colombia/cesar-manrique-y-carlos-r-gonzalez-los-dos-alfiles-del-presidente-petro-profugos-de-la-justicia-por-corrupcion-995937) |
| 2026-03-05 | Gobierno gastó más de 4 millones de dólares de recursos públicos en una película en la que actúa el presidente Petro | [enlace](https://www.noticiasrcn.com/colombia/cuanto-costo-la-pelicula-en-la-que-el-presidente-gustavo-petro-es-actor-invirtieron-recursos-del-gobierno-998572) |
| 2026-03-18 | ¿Qué debe pasar con la mamá de Kevin tras la revictimización del gobierno por la muerte de su hijo? | [enlace](https://www.noticiasrcn.com/colombia/que-debe-pasar-con-la-mama-de-kevin-tras-la-revictimizacion-del-gobierno-por-la-muerte-de-su-hijo-1003310) |
| 2026-03-31 | ¿Quiénes son los 23 sanguinarios criminales a los que el gobierno les suspendió órdenes de captura? | [enlace](https://www.noticiasrcn.com/colombia/quienes-son-los-23-sanguinarios-criminales-a-los-que-el-gobierno-les-suspendio-ordenes-de-captura-1007558) |
| 2026-04-06 | Funcionario le habría hecho ofrecimientos a ‘Papá Pitufo’: escándalo sacude al Gobierno Petro | [enlace](https://www.noticiasrcn.com/colombia/jorge-lemus-funcionario-del-gobierno-petro-se-reunio-con-abogado-de-papa-pitufo-1009208) |
| 2026-04-30 | Petro queda contra las cuerdas: del “no convocaré constituyente” a pedir plata y firmas para imponerla | [enlace](https://www.noticiasrcn.com/colombia/contradicciones-de-petro-frente-a-la-constituyente-1017370) |
| 2026-06-03 | Mientras la campaña de Cepeda toma distancia del Gobierno, De La Espriella tendría acercamientos con Álvaro Uribe | [enlace](https://www.noticiasrcn.com/colombia/mientras-la-campana-de-cepeda-toma-distancia-del-gobierno-de-la-espriella-tendria-acercamientos-con-alvaro-uribe-1027737) |
| 2026-06-28 | No solo el Clan del Golfo: operaciones contra las disidencias también se habrían frenado durante el Gobierno Petro | [enlace](https://www.noticiasrcn.com/colombia/no-solo-el-clan-del-golfo-operaciones-contra-las-disidencias-tambien-se-habrian-frenado-durante-el-gobierno-petro-1035397) |
| 2026-06-29 | MinEducación dejaría comprometidos más de 13 billones de pesos antes del cambio de Gobierno | [enlace](https://www.noticiasrcn.com/colombia/mineducacion-dejaria-comprometidos-mas-de-13-billones-de-pesos-antes-del-cambio-de-gobierno-1035649) |
| 2026-07-02 | 65 niños y adolescentes han muerto en bombardeos durante el Gobierno Petro | [enlace](https://www.noticiasrcn.com/colombia/65-ninos-y-adolescentes-han-muerto-en-bombardeos-durante-el-gobierno-petro-1036499) |
| 2026-07-05 | Polémica por nombramientos de notarios interinos ad-portas de finalizar el gobierno actual | [enlace](https://www.noticiasrcn.com/colombia/notarios-de-carrera-piden-frenar-polemicas-designaciones-del-actual-gobierno-1037589) |
| 2026-07-05 | Polémica por decisión del Gobierno Petro: comprometió $13 billones para Defensa a semanas de su salida | [enlace](https://www.noticiasrcn.com/colombia/gobierno-petro-comprometio-13-billones-para-defensa-1037685) |
| 2026-07-06 | Máquina de $27 mil millones que Petro presentó como "la mejor de América Latina" no está funcionando | [enlace](https://www.noticiasrcn.com/colombia/maquina-de-27-mil-millones-que-petro-presento-como-la-mejor-de-america-latina-no-esta-funcionando-1038115) |
| 2026-07-20 | Así fue la relación entre gobierno de Gustavo Petro y el Congreso: entre alianzas y corrupción | [enlace](https://www.noticiasrcn.com/colombia/asi-fue-la-relacion-entre-gobierno-de-gustavo-petro-y-el-congreso-entre-alianzas-y-corrupcion-1042267) |
| 2026-07-22 | 43.000 contratos en 21 días: esta es la millonaria contratación que deja el gobierno saliente | [enlace](https://www.noticiasrcn.com/colombia/por-que-el-gobierno-saliente-concreto-mas-de-40-mil-contratos-1043057) |
| 2026-07-25 | Contrato adjudicado a Alejandro Carranza enciende la polémica a pocos días del cambio de gobierno | [enlace](https://www.noticiasrcn.com/colombia/contrato-adjudicado-a-alejandro-carranza-enciende-la-polemica-a-pocos-dias-del-cambio-de-gobierno-1044003) |
| 2026-07-28 | Polémica solicitud del presidente Petro para transferir $1 billón a la UNGRD a días de dejar el cargo | [enlace](https://www.noticiasrcn.com/colombia/polemica-solicitud-del-presidente-petro-para-transferir-1-billon-a-la-ungrd-a-dias-de-dejar-el-cargo-1044926) |
| 2026-08-01 | Gobierno Petro acelera decretos, contratos y nombramientos a días de finalizar su mandato | [enlace](https://www.noticiasrcn.com/colombia/gobierno-petro-acelera-decretos-y-nombramientos-a-dias-de-finalizar-su-mandato-1046142) |
| 2026-08-03 | Billonarias deudas y elefantes blancos: se prenden las alarmas con el cierre del gobierno Petro | [enlace](https://www.noticiasrcn.com/economia/gobierno-petro-deja-billonarias-deudas-y-elefantes-blancos-1046702) |

No se encontró en los 932 titulares anteriores al cambio **ninguna pieza que elogie en voz propia al Gobierno Petro** o a la candidatura de Cepeda.

### 2.2 Después del cambio: 2026-08-07 → 2026-10-11 (gobierna De la Espriella)

| # | Fecha | Título literal | URL | Clase | Por qué |
|---|---|---|---|---|---|
| 13 | 2026-08-26 | En tan solo 16 días el Gobierno ha firmado más de 30 extradiciones | [enlace](https://www.noticiasrcn.com/colombia/presidente-abelardo-de-la-espriella-ha-firmado-mas-de-30-extradiciones-1054383) | D leve | «En tan solo»: elogio del titular a una cifra que da el propio presidente en X |
| 14 | 2026-08-30 | Documentos reservados revelan plan de desestabilización contra el nuevo gobierno | [enlace](https://www.noticiasrcn.com/colombia/documentos-reservados-revelan-plan-de-desestabilizacion-contra-el-nuevo-gobierno-1055746) | D | Informe propio. En voz de la casa: «la extrema izquierda radical y grupos armados en Colombia habrían diseñado un plan milimétrico» |
| 15 | 2026-09-08 | Gobierno sorprende al anunciar un canal interoceánico: ¿Cómo estaría proyectado? | [enlace](https://www.noticiasrcn.com/colombia/canal-interoceanico-en-colombia-asi-lo-anuncio-el-gobierno-1058686) | D leve | «sorprende» y, en el cuerpo, «importantes anuncios»; sin contraste |
| 16 | 2026-09-13 | Gobierno le sigue cerrando el cerco a las disidencias de Calarcá: le dieron de baja a otro guerrillero | [enlace](https://www.noticiasrcn.com/colombia/gobierno-le-sigue-cerrando-el-cerco-a-las-disidencias-de-calarca-le-dieron-de-baja-a-otro-guerrillero-1060295) | D leve | El logro se atribuye en el titular al Gobierno, sobre un parte del Ejército |
| 17 | 2026-09-22 | ¿En qué consiste el plan de choque que anunció el Gobierno De la Espriella para atender la crisis de salud? | [enlace](https://www.noticiasrcn.com/colombia/en-que-consiste-el-plan-de-choque-que-anuncio-el-gobierno-de-la-espriella-para-atender-la-crisis-de-salud-1063594) | D leve | Entradilla: «el Gobierno tratará de enmendar los daños del sector salud». Disculpa por herencia |
| 18 | 2026-09-26 | Gobierno avanza en soluciones para cumplir con el pago de las pensiones de final de año | [enlace](https://www.noticiasrcn.com/economia/gobierno-avanza-en-soluciones-para-cumplir-con-el-pago-de-las-pensiones-de-final-de-ano-1065383) | D leve | Entradilla: «El gobierno de Abelardo de la Espriella recibió un grave déficit». Disculpa por herencia |
| 19 | 2026-08-18 | ‘Libro de la verdad’ destapa más de 80 casos de presunta corrupción en el gobierno Petro | [enlace](https://www.noticiasrcn.com/colombia/libro-de-la-verdad-destapa-mas-de-80-casos-de-presunta-corrupcion-en-el-gobierno-petro-1051360) | D retro | Hace suyo el informe del Gobierno entrante: «La presentación del informe marca un punto de inflexión en la lucha contra la corrupción» |
| 20 | 2026-08-19 | Las denuncias más controvertidas del 'Libro de la Verdad' con presuntos hechos de corrupción del gobierno Petro | [enlace](https://www.noticiasrcn.com/colombia/las-denuncias-mas-controvertidas-del-libro-de-la-verdad-con-presuntos-hechos-de-corrupcion-del-gobierno-petro-1051823) | D retro leve | Segunda pieza sobre el mismo informe, sin la versión de los señalados en el titular ni en la entradilla |
| 21 | 2026-08-31 | Deuda de las EPS aumentó en 26,5%, pese a intervención del antiguo Gobierno | [enlace](https://www.noticiasrcn.com/colombia/deuda-de-las-eps-aumento-en-26-5-pese-a-intervencion-del-antiguo-gobierno-1056130) | D retro leve | El «pese a» del titular; el dato es de la Contraloría |
| 22 | 2026-09-04 | Ayudas del Gobierno Petro tras accidente aéreo con 69 víctimas nunca llegaron a Puerto Leguízamo | [enlace](https://www.noticiasrcn.com/colombia/ayudas-del-gobierno-petro-tras-accidente-aereo-con-69-victimas-nunca-llegaron-a-puerto-leguizamo-1057750) | D retro | El titular afirma en voz propia lo que dice el alcalde |
| 23 | 2026-09-15 | El macabro prontuario criminal de alias Araña, exgestor de paz del gobierno Petro | [enlace](https://www.noticiasrcn.com/colombia/el-macabro-prontuario-criminal-de-alias-arana-exgestor-de-paz-del-gobierno-petro-que-sera-extraditado-a-ee-uu-1061021) | D retro leve | El titular ata el prontuario al Gobierno anterior |
| 24 | 2026-10-03 | Exclusivo \| Estados financieros de la UNP revelan déficit, elevados costos y una flota duplicada | [enlace](https://www.noticiasrcn.com/colombia/estados-financieros-de-la-unp-revelan-deficit-elevados-costos-y-una-flota-duplicada-en-gobierno-petro-1068079) | D retro leve | Exclusiva propia: el déficit «a pesar de que su presupuesto tuvo un incremento del 91% durante el gobierno Petro» |
| 25 | 2026-08-07 | El regreso de la ultraderecha a Latinoamérica se consolida con el mandato de Abelardo de la Espriella | [enlace](https://www.noticiasrcn.com/internacional/el-regreso-de-la-ultraderecha-a-latinoamerica-se-consolida-con-el-mandato-de-abelardo-de-la-espriella-1048095) | **I leve** | Análisis propio, el día de la posesión: rotula al entrante como «ultraderecha» |
| 26 | 2026-09-02 | ¿Qué pasará con los proyectos férreos en el Gobierno de De la Espriella? Hay anuncio oficial | [enlace](https://www.noticiasrcn.com/colombia/gobierno-confirma-continuidad-de-cinco-proyectos-ferreos-en-colombia-1056968) | **I leve** | Reconoce al saliente: «Tras la reactivación férrea adelantada en el Gobierno anterior […] positiva noticia» |

**Fiscalización de De la Espriella desde que gobierna (F: se declara, no suma):**

| Fecha | Título literal | URL | Por qué |
|---|---|---|---|
| 2026-08-28 | ¿Por qué es mayor el presupuesto general de la nación para 2027 que presentó el Gobierno de De la Espriella? | [enlace](https://www.noticiasrcn.com/economia/por-que-es-mayor-el-presupuesto-general-de-la-nacion-para-2027-que-presento-el-gobierno-de-de-la-espriella-1055140) | Entradilla en voz propia: «Aunque el Gobierno actual llegó a la Casa de Nariño con promesas de austeridad, la cifra creció en 59,3 billones de pesos». El cuerpo da después la explicación del ministro |
| 2026-10-01 | Congresistas se reunieron para coordinar la agenda con el Gobierno y terminaron plantados: ¿qué pasó? | [enlace](https://www.noticiasrcn.com/colombia/congresistas-se-reunieron-para-coordinar-la-agenda-con-el-gobierno-y-terminaron-plantados-1067493) | Leve: un desplante a la coalición, según fuentes |

**Mixta (M):** 2026-09-07, «¿Cuál ha sido el principal acierto y desacierto de De la Espriella tras un mes de gobierno? Esto dicen los analistas» ([enlace](https://www.noticiasrcn.com/colombia/cual-ha-sido-el-principal-acierto-y-desacierto-de-de-la-espriella-tras-un-mes-de-gobierno-1058401)). El balance va atribuido a un analista.

### 2.3 Leídas y no clasificadas (se declaran)

- **Información atribuida o de procedimiento**, en los dos sentidos. Contra el entrante: el fallo que le ordena disculparse por la neutralidad religiosa (27-08), las prohibiciones de usar la camiseta de la Selección y los símbolos patrios en campaña (04-06 y 09-06), la Fiscalía que no halló interceptaciones a su celular (08-04) y las comparaciones con Bukele (26-08). A su favor: la retractación de David Murcia (24-09) y los elogios de Trump (22-09). Contra el saliente: denuncias, sanciones del CNE e imputaciones.
- **Análisis electoral sin postura propia:** «¿Qué salió mal? Los errores que le costaron a Iván Cepeda la victoria en primera vuelta» y «Abelardo de la Espriella: las claves detrás de su sorpresivo triunfo en las urnas», los dos del 01-06 y los dos atribuidos a panelistas.
- **Formatos simétricos:** los dos finalistas pasaron por las entrevistas de la redacción (De la Espriella el 26-03 y el 18-05; Cepeda el 17-05) y tuvieron su «Streaming final» (15-06 y 16-06). «Química en la Fórmula» con De la Espriella y Restrepo (11-05) es un formato ligero; el sitemap no muestra una entrega con Cepeda y Quilcué, pero no se buscó por otra vía y **no cuenta**.
- **El tono de anuncio.** Desde el 07-08, la mayoría de los 398 titulares sobre el Gobierno son anuncios del Ejecutivo en voz neutra («Gobierno anuncia…», «Presidente De la Espriella ordena…»). Es taquigrafía oficial, no postura: no se clasifica, pero se declara en el §4.
- **Columnas firmadas** (`/opinion/`): no cuentan. Entre ellas está «Ni los nadies se salvaron: el balance de corrupción que deja el Gobierno de Gustavo Petro» (27-07-2026), que la ficha llama «la más fuerte» de su nivel 5. **Es una columna firmada por una columnista** (JSON-LD `author`: persona; breadcrumb «Opinión › [columnista]»), así que no es voz de la casa.

---

## 3. Números

| | D | I | M | Con postura | F (no suma) |
|---|---|---|---|---|---|
| Antes del 07-08-2026 (10 meses, 932 piezas leídas) | **10** (2 plenas, 8 leves) | **2** (1 plena, 1 leve) | 0 | 12 | 27 contra Petro |
| Desde el 07-08-2026 (2 meses, 398 piezas leídas) | **12** (3 plenas, 9 leves; 6 retro) | **2** (leves) | 1 | 15 | 2 contra De la Espriella |
| **Total** | **22** | **4** | 1 | **27** | |

**Proporción principal: 22 a 4, es decir, 5,5 a 1.**

Las precisiones sobre el mínimo por lado («solo cuentan los elogios, las disculpas y los rótulos»):
- **antes:** 3 elogios al candidato o presidente electo (n.º 8, 9, 10) y 7 encuadres o rótulos contra la candidatura de izquierda (n.º 1-7);
- **después:** 4 elogios al Gobierno (n.º 13-16) y 2 disculpas por herencia (n.º 17, 18). Las 6 retro son crítica al Gobierno anterior y no son elogio ni disculpa: **sin ellas quedan 6 después del cambio, y el mínimo de 3 se cumple igual.**

Sensibilidad, para que se pueda recontar:

| Lectura | D | I | Proporción | ¿≥10 y ≥3 por lado? |
|---|---|---|---|---|
| Principal | 22 | 4 | **5,5 : 1** | Sí (10 y 12) |
| Sin las retro | 16 | 4 | 4 : 1 | Sí (10 y 6) |
| Sin ninguna «leve» (las de los dos lados pasan a M) | 5 | 1 | 5 : 1 | **No** (6 con postura; 2 y 3 por lado) |
| Los perfiles del 31-05 (n.º 6 y 11) como M | 21 | 3 | 7 : 1 | Sí |

**El trato a quien gobierna (polo fijo).** Con la vara de la voz propia en el titular, la casa fiscalizó a Petro **27 veces en 10 meses (unas 2,7 al mes)** y a De la Espriella **2 veces en 2 meses (1 al mes)**. A Petro, en voz propia, no lo elogió nunca; al entrante, 6 veces en dos meses, entre elogios y disculpas por herencia. No es la misma conducta con los dos gobiernos: es asimetría en el trato, que es lo que la regla mide.

---

## 4. Contrapesos (lo que contradice la dirección, y cuánto pesa)

| Contrapeso | Piezas | Peso |
|---|---|---|
| **Rótulos al entrante en voz propia**: «polémico», «controversial», «desprecio por la izquierda» (31-05) y «ultraderecha» el día de la posesión (07-08) | n.º 11, 12, 25 | **Medio.** Son de la casa y llegan en los dos momentos de más audiencia, pero son cuatro frente a 22 |
| **Fiscalización del entrante en voz propia**: el presupuesto frente a las «promesas de austeridad», el desplante a los congresistas | §2.2 F | **Bajo-medio.** Existe y es de fondo en el caso del presupuesto, pero la cuenta mensual está muy por debajo de la del saliente |
| **Reconocimiento de un programa del saliente** («positiva noticia» la continuidad férrea) | n.º 26 | **Bajo.** Una frase |
| **Formatos y espacios simétricos** para los dos finalistas (entrevistas, streaming final) | §2.3 | **Medio para la magnitud.** No hay trato desigual en el acceso a la pantalla |
| **Sin endoso.** En 12 meses no hay pieza de la casa que pida el voto o declare apoyo a un candidato | — | **Alto para la magnitud.** Mantiene el tope de ±0,30 y lo aleja de quienes endosaron |
| **Densidad baja.** 26 piezas con postura entre 1.330 leídas (2 %). El grueso de la cobertura es información atribuida o taquigrafía de anuncios | §1, §2.3 | **Alto para la magnitud.** La dirección se ve, pero en la palabra del titular, no en un editorial |
| **El tono de anuncio desde el 07-08**: 398 piezas, casi todas anuncio oficial sin contraste | §2.3 | **No es contrapeso; empuja hacia D**, pero no se cuenta porque no es postura en voz propia |

---

## 5. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | **Sí, en titulares y entradillas** | Las notas van firmadas «Noticias RCN» (1.330 de 1.330). El medio no tiene editoriales; sus columnas son de terceros firmantes y no cuentan |
| 2. A los dos lados del cambio, en 12 meses | **Sí** | Con Petro: 27 F, 0 elogios. Con De la Espriella: 2 F, 6 elogios o disculpas. A la candidatura de izquierda, encuadres negativos; al candidato de derecha, elogios leves |
| 3a. ≥10 piezas con postura | **Sí** | 26 (22 D y 4 I) más 1 M |
| 3b. ≥3 a cada lado del cambio | **Sí** | 10 antes y 12 después en la dirección D (6 después, sin las retro) |
| 3c. Proporción ≥3:1 | **Sí** | 5,5:1 (4:1 sin las retro) |
| 4. Contrapesos escritos | **Sí** | §4, con peso |
| 5. Reproducible | **Sí** | §2, con fecha, título literal, URL y clase; §1, con el filtro exacto |

**Las cinco condiciones se cumplen en la lectura principal.** La advertencia va con el veredicto: **depende de las piezas «leves»**. Sin ellas, se queda en 6 piezas y no llega.

---

## 6. Rama de la precisión del 2026-10-10 y valor que resultaría

**Rama: «cumple las cinco condiciones» → el valor del barrido, con el tope de ±0,30** (no hay endoso explícito ni propiedad con posición conocida que lo levante).

**Valor propuesto: +0,15** (juicio declarado). Hoy está en +0,25.

**Por qué no se queda en +0,25:**
- el +0,25 no tenía evidencia propia (§ cabecera), y el barrido manda;
- la dirección D está, pero en la intensidad más baja que admite la regla: casi todo son palabras de titular («en tan solo», «sorprende», «¿un paso atrás?») y el 2 % de las piezas leídas;
- El Diario de Pereira y Vive el Meta, en +0,25, tienen editoriales de la casa con postura explícita. Noticias RCN no tiene editoriales.

**Por qué no +0,20 (El Pilón, El Heraldo):** El Heraldo endosó en editorial; El Pilón dice «apoyamos» en editoriales sin firma. Aquí no hay ni lo uno ni lo otro. Ponerlo a su altura daría la misma magnitud con evidencia más débil. **Se declara como lectura alternativa**: si el responsable editorial pesa más la asimetría del trato (27 contra 2) que la densidad, +0,20 es defendible y no pasa del tope.

**Por qué no 0,00:** el 0,00 con evidencia pide la misma conducta con los dos gobiernos y la postura por debajo de 3 a 1. Aquí ni lo uno ni lo otro.

**Vecinos:**
- La República (+0,15), del mismo dueño y bajo la misma consejería de medios: misma magnitud;
- Noticias Caracol (+0,10), el otro noticiero privado: por debajo;
- La FM (+0,35), de la misma casa, con editorial diario firmado por su director: muy por encima, y la diferencia la explica el formato, como ya decía la ficha.

**Qué lo refutaría:**
- hacia arriba: un editorial o una pieza sin firma que pida el voto en 2027, o que los elogios al Gobierno pasen de la palabra del titular a la valoración del cuerpo;
- hacia abajo: que la fiscalización en voz propia del Gobierno De la Espriella se acerque al ritmo que tuvo con Petro (unas 2,7 al mes);
- y, en cualquier sentido, un recuento que no dé por buenas las «leves»: ese recuento no llega a los mínimos, y la rama sería **«sin medir» con la dirección declarada como tensión** (la dirección es clara, pero no hay mínimos).

---

## 7. Cobertura, huecos y avisos

- **Lo que no se leyó.** La **emisión de televisión**, que es el producto principal del medio: este barrido es del portal. Tampoco las piezas cuyo slug no lleva ninguno de los términos del §1 (por ejemplo, las que solo dicen «presidente», «ministro» o «MinHacienda»), ni las secciones Deportes y Tendencias fuera del filtro. Una nota sobre el Gobierno con un slug sin esos términos se escapa.
- **F no es exhaustiva.** La lista de fiscalización a Petro es de titulares con la valoración en voz propia, leídos uno por uno, y no un recuento cerrado. La de De la Espriella sí se buscó a fondo, con términos de crítica, sobre las 398 piezas posteriores. Si la de Petro está incompleta, la asimetría sería mayor, no menor.
- **Cuerpos leídos en parte.** De unas 70 piezas se leyeron los primeros párrafos, no el texto entero. La clase se apoya en el titular y la entradilla, que es lo que la regla cuenta.
- **El lado posterior es corto:** dos meses y 398 piezas, frente a diez meses y 932.
- **Robots y red.** El robots.txt no excluyó nada de lo usado. No hubo bloqueos ni respuestas distintas de 200, y no se reintentó nada.
- **Una sola lectura**, de la misma casa que el autor de la ficha. Las piezas límite van marcadas «leve» y el §3 da el recuento con y sin ellas.
- **Datos personales.** No se copia ningún número de documento, teléfono ni dirección. Las personas nombradas son cargos públicos o candidatos. La columnista de la pieza del 27-07 no se nombra.
