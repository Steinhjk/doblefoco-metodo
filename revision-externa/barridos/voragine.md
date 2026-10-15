# Barrido editorial: Vorágine

| | |
|---|---|
| **Medio** | Vorágine (`voragine`), Fundación Vorágine Periodismo Contracorriente. No noticioso (`noNoticioso: true`): fuera del mapa |
| **Valor vigente** | **sin medir** (`bias: null`) en `shared/mediaRegistry.js` desde el 2026-09-18, por decisión del responsable editorial del 2026-09-16. **La ficha y el envío todavía dicen −0,50**: es un error de la ficha (ver la resolución) |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus dos precisiones, y la regla del polo fijo |
| **Ventana** | 2025-10-10 → 2026-10-10 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Resolución de origen** | `revision-externa/respuestas/opus-5-5-voragine.md` (revisor: «el −0,50 no se sostiene»; unas 3 piezas con postura; asimetría de campaña de 12 a 0) |
| **Quién lo hizo** | Claude Opus 5.5 (`claude-opus-5-5`), verificador del ciclo 2, tanda 9, a petición del responsable editorial, el 2026-10-10. Es de la misma casa que el autor de la ficha y que el revisor: su acuerdo no es aval |
| **Estado** | **DECIDIDO el 2026-10-10: sin medir** (se queda; la ficha decía −0,50), por el responsable editorial (`DECISIONES.md`, «2026-10-10 · Tandas 8 y 9 del ciclo 2: el barrido manda sobre los números sin evidencia»). Lo que más abajo dice «propuesta», «recomendada» o «pendiente» es el estado anterior a la decisión y se conserva como historia |
| **Resultado** | **No cumple.** 3 piezas con postura en voz de la casa, las tres leves y en la misma dirección (2 antes del cambio y 1 después), y ningún elogio ni disculpa a nadie. El mínimo es 10. **El patrón es el de fiscalizar a quien manda a los dos lados del cambio**: 6 piezas contra el Gobierno Petro antes y 4 contra el de De la Espriella después |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas y el método
> están aquí para eso. **La clasificación de cada pieza es juicio de un solo
> lector**, de la misma casa que el autor de la ficha y que el revisor, y se
> hizo con titular, entradilla, firma y búsqueda de términos en el cuerpo
> completo, no con lectura íntegra de las 93 piezas.

---

## 1. Método

- **robots.txt** de `voragine.co` (descargado el 2026-10-10): `User-agent: *` con `Disallow` de `/sitio/` y `/bk-sitio/` (y un PDF de 2022). No nombra a ClaudeBot, Claude-Web ni anthropic-ai. `/wp-json/` y `/feed/` no están vetados.
- **Descarga:** `curl -sL --ssl-no-revoke` con User-Agent de navegador (Chrome 126).
- **Universo, sin muestreo:** la API pública de WordPress, `https://voragine.co/wp-json/wp/v2/posts?after=2025-10-10T00:00:00&per_page=100`, con el contenido completo de cada entrada. Cabecera `x-wp-total: 93`, una sola página: todas las entradas publicadas del 2025-10-12 al 2026-10-07. Categorías: `https://voragine.co/wp-json/wp/v2/categories?per_page=100`.
- **Secciones de opinión, comprobadas antes:** «Editorial» tiene **1** entrada en toda su historia (categoría 1154, `count: 1`: la amenaza a un reportero del medio), fuera de la ventana. «Opinión» (categoría 34) tiene 10 en toda su historia y **ninguna** en la ventana. «Comunicado» (1087) tiene 4, **2** en la ventana (n.º 34 y 37).
- **Términos buscados en el cuerpo completo** de las 93: Petro, Espriella, Cepeda, Uribe, Centro Democrático, Pacto Histórico, Benedetti, Sarabia, Pastrana, Paloma, Vital Strategies, Liga Contra el Silencio, Barrientos, Cuestión Pública. Rótulos: ultraderecha, extrema derecha o izquierda, fascis-, tiran-, dictad-, golpis-, neoliberal, progresismo, negacionis-. Elogios: acierto, logró, celebr-, aplaud-, valiente.
- **Búsquedas internas de la API** con `after=2025-10-10T00:00:00`, para cotejar al revisor: `search=Cepeda` 7, `Petro` 24, `De la Espriella` 17, `Uribe` 15, `Barrientos` 1, `Vital Strategies` 17. **Coinciden con las suyas.**
- **Clases.**
  - **F, fiscaliza** (se declara, no cuenta; precisión del responsable editorial del 2026-10-09: no suma para el mínimo por lado). Se anota a quién: Gobierno Petro; Gobierno De la Espriella; candidato o presidente electo de derecha; derecha que no es candidato; empresas; Fuerza Pública; grupos armados; instituciones; otros.
  - **P, postura en voz de la casa** (cuenta): elogio, disculpa o rótulo en voz propia (firma «Vorágine», «Redacción Vorágine» o un periodista de la casa), no atribuido a una fuente. **Aquí solo aparece como «rótulo leve»** dentro de piezas de fiscalización, y se marca en la nota.
  - **Ajena:** firmada por la alianza La Liga Contra el Silencio, por un autor externo «para La Liga» o por un colectivo de firmantes. Se declara; no cuenta (condición 1: comunicados y textos de terceros).
  - **N, neutra:** reportaje, crónica, perfil o servicio (talleres, conversatorios) sin actor político nacional como blanco.
  - **VS:** lleva la leyenda «Esta investigación fue financiada, en parte, por Vital Strategies» o su versión inglesa.
- **El 07-08-2026** cuenta como «después» (día de la posesión). Solo afecta a la n.º 80, que el revisor puso «antes».

---

## 2. Las 93 piezas

| # | Fecha | Pieza | Lado del 07-08 | Clase | Nota |
|---|---|---|---|---|---|
| 1 | 2025-10-12 | [Las sombras de la Casa Castaño que rondan a una congresista de víctimas](https://voragine.co/historias/investigacion/las-sombras-de-la-casa-castano-que-rondan-a-una-congresista-de-victimas/) | antes | F · otros | congresista de una curul de paz (Urabá) |
| 2 | 2025-10-16 | [Los conflictos de interés de la Sociedad Colombiana de Pediatría](https://voragine.co/comic/los-conflictos-de-interes-de-la-sociedad-colombiana-de-pediatria/) | antes | F · empresas · VS | industria y Sociedad Colombiana de Pediatría |
| 3 | 2025-10-19 | [El “Gury” tiene contratado a un exescolta de alias La Madrina](https://voragine.co/historias/investigacion/el-gury-tendria-contratado-a-un-escolta-personal-con-recursos-del-concejo-de-medellin/) | antes | F · derecha, no candidato | concejal uribista de Medellín · rótulo leve en voz de la casa: «se destaca por su agresividad» |
| 4 | 2025-10-22 | [Un poder ‘endulzado’ por la industria de ultraprocesados](https://voragine.co/noticias-especiales/un-poder-endulzado-por-la-industria-de-ultraprocesados/) | antes | F · empresas | industria de ultraprocesados |
| 5 | 2025-10-26 | [Las denuncias por falsos positivos contra el comandante de Educación y Doctrina del Ejército](https://voragine.co/historias/investigacion/las-denuncias-por-falsos-positivos-contra-el-comandante-de-educacion-y-doctrina-del-ejercito/) | antes | F · Fuerza Pública | general del Ejército en servicio bajo Petro |
| 6 | 2025-10-27 | [Nukak: desterrados y ahora usados en un turbio negocio de créditos de carbono](https://voragine.co/historias/investigacion/nukak-siguen-desterrados-y-ahora-son-usados-en-un-turbio-negocio-de-creditos-de-carbono/) | antes | F · otros | negocio de créditos de carbono |
| 7 | 2025-10-27 | [Conflicts of Interest in the Colombian Pediatric Society](https://voragine.co/comic/conflicts-of-interest-in-the-colombian-pediatric-society/) | antes | F · empresas · VS | (versión en inglés de la n.º 2) |
| 8 | 2025-10-29 | [Las inundaciones no sólo son climáticas, también son políticas: así funciona la gestión de riesgo de desastres en el Meta](https://voragine.co/historias/reportaje/las-inundaciones-no-solo-son-climaticas-tambien-son-politicas-asi-funciona-la-gestion-de-riesgo-de-desastres-en-el-meta/) | antes | F · otros | gestión de riesgo, gobiernos locales del Meta |
| 9 | 2025-11-04 | [Madres, migrantes y vendedoras ambulantes: el rostro femenino del rebusque en la frontera con Venezuela](https://voragine.co/historias/reportaje/madres-migrantes-y-vendedoras-ambulantes-el-rostro-femenino-del-rebusque-en-la-frontera-con-venezuela/) | antes | N |  |
| 10 | 2025-11-05 | [Sellos octagonales: balance agridulce](https://voragine.co/comic/sellos-octagonales-balance-agridulce/) | antes | F · empresas · VS | política de sellos y la industria |
| 11 | 2025-11-07 | [Lo que significan para la libertad de expresión los segundos silenciados de “Noviembre”](https://voragine.co/historias/analisis/lo-que-significan-para-la-libertad-de-expresion-los-segundos-silenciados-de-noviembre/) | antes | N | libertad de expresión, censura judicial de una película (con La Liga) |
| 12 | 2025-11-09 | [Lagos para esquí náutico: el club de La Calera que consume más agua que Coca Cola](https://voragine.co/historias/investigacion/lagos-para-esqui-nautico-el-club-de-la-calera-que-consume-mas-agua-que-coca-cola/) | antes | F · empresas · VS | club de La Calera y Coca-Cola |
| 13 | 2025-11-13 | [El mar avanza más rápido que el Estado sobre la costa norte de Nariño](https://voragine.co/historias/reportaje/el-mar-avanza-mas-rapido-que-el-estado-sobre-la-costa-norte-de-narino/) | antes | N |  |
| 14 | 2025-11-16 | [Las empresas israelíes más cuestionadas por espionaje y sus contratos con la Fiscalía y Policía](https://voragine.co/historias/investigacion/david-ghitis-el-ingeniero-detras-de-la-red-israeli-de-inteligencia-en-colombia/) | antes | F · otros | empresas israelíes de espionaje con contratos con Fiscalía y Policía; activista cercano al CD |
| 15 | 2025-11-23 | [El alto funcionario del Gobierno Petro señalado en la JEP de nexos con paramilitares](https://voragine.co/historias/investigacion/el-alto-funcionario-del-gobierno-petro-senalado-en-la-jep-de-nexos-con-paramilitares/) | antes | F · Gobierno Petro | alto funcionario del Gobierno Petro |
| 16 | 2025-11-27 | [Lakes for Water Skiing: The Club in La Calera That Consumes More Water Than Coca-Cola](https://voragine.co/historias/investigacion/lakes-for-water-skiing-the-club-in-la-calera-that-consumes-more-water-than-coca-cola/) | antes | F · empresas · VS | (inglés) |
| 17 | 2025-11-28 | [Octagonal Seals: A Bittersweet Balance Sheet](https://voragine.co/comic/octagonal-seals-a-bittersweet-balance-sheet/) | antes | F · empresas · VS | (inglés) |
| 18 | 2025-11-30 | [Santiago Uribe, empresarios y narcos fueron asociados de una temida Convivir](https://voragine.co/historias/investigacion/santiago-uribe-empresarios-y-narcos-fueron-asociados-de-una-temida-convivir/) | antes | F · derecha, no candidato | Santiago Uribe y una Convivir |
| 19 | 2025-11-30 | [Niñez migrante en medio del conflicto: entre el reclutamiento, y el desplazamiento forzado](https://voragine.co/historias/investigacion/ninez-migrante-en-medio-del-conflicto-entre-el-reclutamiento-y-el-desplazamiento-forzado/) | antes | N |  |
| 20 | 2025-12-10 | [La lucha de mujeres migrantes para ser atendidas en hospitales en Colombia](https://voragine.co/historias/cronica/la-lucha-de-mujeres-migrantes-para-ser-atendidas-en-hospitales-en-colombia/) | antes | N |  |
| 21 | 2026-01-11 | [El daño colateral: Lo que viene para Colombia en medio de la crisis venezolana](https://voragine.co/historias/analisis/el-dano-colateral-lo-que-viene-para-colombia-en-medio-de-la-crisis-venezolana/) | antes | N | análisis de la crisis venezolana; cita encuestas de los dos candidatos |
| 22 | 2026-01-18 | [El cuestionado estudio que presentó Coca Cola sobre el agua en La Calera](https://voragine.co/historias/investigacion/el-cuestionado-estudio-que-presento-coca-cola-sobre-el-agua-en-la-calera/) | antes | F · empresas · VS | Coca-Cola |
| 23 | 2026-01-19 | [Grupos armados y mercurio: la tragedia silenciosa en la frontera amazónica entre Colombia y Venezuela](https://voragine.co/historias/reportaje/grupos-armados-y-mercurio-la-tragedia-silenciosa-en-la-frontera-amazonica-entre-colombia-y-venezuela/) | antes | N |  |
| 24 | 2026-01-25 | [La apuesta de De la Espriella: arruinar periodistas para silenciarlos](https://voragine.co/historias/investigacion/la-apuesta-de-de-la-espriella-arruinar-periodistas-para-silenciarlos/) | antes | F · candidato o presidente electo de derecha | De la Espriella, demandas contra periodistas (cifras de la Flip) |
| 25 | 2026-01-26 | [Tiros de gracia: las dudas sobre la matanza de disidentes en Guaviare](https://voragine.co/historias/investigacion/tiros-de-gracia-las-dudas-sobre-la-matanza-de-disidentes-en-guaviare/) | antes | Ajena (no es voz de la casa) | firma un autor externo «para La Liga Contra el Silencio»; matanza de disidentes |
| 26 | 2026-01-26 | [Acorralado por mineros y narcos, el único pueblo no contactado identificado en Colombia podría extinguirse](https://voragine.co/historias/reportaje/acorralado-por-mineros-y-narcos-el-unico-pueblo-no-contactado-identificado-en-colombia-podria-extinguirse/) | antes | N |  |
| 27 | 2026-02-01 | [César Manrique: el prófugo al que Petro le ha dado poder dos veces](https://voragine.co/historias/perfil/cesar-manrique-el-profugo-al-que-petro-le-ha-dado-poder-dos-veces/) | antes | F · Gobierno Petro | funcionario prófugo nombrado por Petro |
| 28 | 2026-02-08 | [La opacidad de los financiadores de la última encuesta presidencial de Cifras y Conceptos](https://voragine.co/historias/investigacion/la-opacidad-de-los-financiadores-de-la-ultima-encuesta-presidencial-de-cifras-y-conceptos/) | antes | F · otros | financiadores de una encuesta presidencial |
| 29 | 2026-02-12 | [The Controversial Study Regarding Water in La Calera Presented by Coca-Cola](https://voragine.co/historias/investigacion/the-controversial-study-regarding-water-in-la-calera-presented-by-coca-cola/) | antes | F · empresas · VS | (inglés) |
| 30 | 2026-02-15 | [La tierra de un narcoparamilitar que pasó a manos de Abelardo de la Espriella](https://voragine.co/historias/investigacion/la-tierra-de-un-narcoparamilitar-que-paso-a-manos-de-abelardo-de-la-espriella/) | antes | F · candidato o presidente electo de derecha | tierra de un narcoparamilitar en manos de De la Espriella |
| 31 | 2026-02-16 | [Ministerio de Educación: denuncian presiones a trabajadores para marchar](https://voragine.co/historias/investigacion/ministerio-de-educacion-denuncian-presiones-a-trabajadores-para-marchar/) | antes | F · Gobierno Petro | presiones en MinEducación para marchar a favor de Petro (en campaña) |
| 32 | 2026-02-19 | [Presidente de la Corte Constitucional acusó a la madre de su primogénito de haberlo drogado y abusado](https://voragine.co/historias/investigacion/presidente-de-la-corte-constitucional-acuso-a-la-madre-de-su-primogenito-de-haberlo-drogado-y-abusado/) | antes | Ajena (no es voz de la casa) | pieza de La Liga; firman Barrientos y Castaño; presidente de la Corte Constitucional |
| 33 | 2026-02-22 | [Campesinos firmaron engañados: denuncias contra minera que financió a Paola Holguín](https://voragine.co/historias/investigacion/campesinos-firmaron-enganados-denuncias-contra-minera-que-financio-a-paola-holguin/) | antes | F · derecha, no candidato | minera que financió a una senadora del CD |
| 34 | 2026-02-27 | [COMUNICADO DE DISCULPAS A LAS AUDIENCIAS DE LA LIGA CONTRA EL SILENCIO Y A LOS MEDIOS ESTIGMATIZADOS](https://voragine.co/comunicado/comunicado-de-disculpas-a-las-audiencias-de-la-liga-contra-el-silencio-y-a-los-medios-estigmatizados/) | antes | Ajena (no es voz de la casa) | comunicado de La Liga (alianza de 16 salas): disculpa a medios estigmatizados tras una pieza sobre Iván Cepeda · postura, no de la casa |
| 35 | 2026-03-01 | [Así saqueó el Clan del Golfo la salud y el PAE en Antioquia y Chocó](https://voragine.co/historias/investigacion/asi-saqueo-el-clan-del-golfo-la-salud-y-el-pae-en-antioquia-y-choco/) | antes | F · grupos armados | Clan del Golfo, salud y PAE |
| 36 | 2026-03-07 | [26.000 millones en contratos del gobierno a fichas del condenado exsenador Pulgar](https://voragine.co/historias/investigacion/26-000-millones-en-contratos-del-gobierno-a-fichas-del-condenado-exsenador-pulgar/) | antes | F · Gobierno Petro | contratos de MinInterior (Benedetti); firma el director |
| 37 | 2026-03-08 | [#NoAlPactoDeSilencio: 171 mujeres con 20 preguntas para el expresidente Andrés Pastrana Arango](https://voragine.co/comunicado/noalpactodesilencio-171-mujeres-con-20-preguntas-para-el-expresidente-andres-pastrana-arango/) | antes | Ajena (no es voz de la casa) | manifiesto de 171 firmantes a Pastrana, categoría Comunicado · postura, no de la casa |
| 38 | 2026-03-15 | [El Clan del Golfo se ensañó con el Cinep](https://voragine.co/historias/investigacion/el-clan-del-golfo-se-ensano-con-el-cinep/) | antes | F · grupos armados | Clan del Golfo contra el Cinep |
| 39 | 2026-03-22 | [La chequera uribista que ha impulsado el proyecto político de Oviedo](https://voragine.co/historias/investigacion/la-chequera-uribista-que-ha-impulsado-el-proyecto-politico-de-oviedo/) | antes | F · candidato o presidente electo de derecha | aportes uribistas a la fórmula vicepresidencial de Paloma Valencia |
| 40 | 2026-03-22 | [Narcos extorsionados: las redes de corrupción que involucran a policías y fiscales](https://voragine.co/historias/investigacion/narcos-extorsionados-las-redes-de-corrupcion-que-involucran-a-policias-y-fiscales/) | antes | F · instituciones | policías y fiscales |
| 41 | 2026-03-29 | [La estrategia de Coca-Cola para limpiar su imagen en el Mundial de Fútbol](https://voragine.co/historias/investigacion/la-estrategia-de-coca-cola-para-limpiar-su-imagen-en-el-mundial-de-futbol/) | antes | F · empresas · VS | Coca-Cola |
| 42 | 2026-04-16 | [Coca-Cola’s strategy to clean up its image at the World Cup](https://voragine.co/historias/reportaje/coca-colas-strategy-to-clean-up-its-image-at-the-world-cup/) | antes | F · empresas · VS | (inglés) |
| 43 | 2026-04-19 | [Informantes asesinados y recompensas robadas: una olla podrida en la Fuerza Pública](https://voragine.co/historias/investigacion/informantes-asesinados-y-recompensas-robadas-una-olla-podrida-en-la-fuerza-publica/) | antes | F · Fuerza Pública | informantes y recompensas |
| 44 | 2026-04-19 | [Goles y canciones: una conversación irrepetible con el Bambino Pons](https://voragine.co/historias/hernan-pelaez-y-el-bambino-pons-dos-conversaciones-irrepetibles-en-la-escuelavoragine/) | antes | N | taller |
| 45 | 2026-04-19 | [Laura Sarabia y su red de poder: los nombramientos que todavía la persiguen](https://voragine.co/historias/investigacion/laura-sarabia-y-su-red-de-poder-los-nombramientos-que-todavia-la-persiguen/) | antes | F · Gobierno Petro | Laura Sarabia |
| 46 | 2026-04-26 | [Oro, miedo y poder: el río que se marchita en Ataco, Tolima](https://voragine.co/historias/investigacion/oro-miedo-y-poder-el-rio-que-se-marchita-en-ataco-tolima/) | antes | F · otros | minería en Ataco |
| 47 | 2026-04-26 | [Coca Cola en La Calera: la resistencia social que redujo la explotación de agua](https://voragine.co/historias/cronica/coca-cola-en-la-calera-la-resistencia-social-que-redujo-la-explotacion-de-agua/) | antes | F · empresas · VS | Coca-Cola |
| 48 | 2026-04-26 | [Ciencia para encontrarles: el camino científico para buscar a los desaparecidos](https://voragine.co/historias/ciencia-para-encontrarles-el-camino-cientifico-para-buscar-a-los-desaparecidos/) | antes | N |  |
| 49 | 2026-05-03 | [Santodomingo, Ardila y Sarmiento financiaron a un condenado por compra de votos](https://voragine.co/historias/investigacion/santodomingo-ardila-y-sarmiento-financiaron-a-un-condenado-por-compra-de-votos/) | antes | F · empresas | grandes empresarios que financiaron a un condenado de Cambio Radical |
| 50 | 2026-05-10 | [El futuro asesinado: la historia de Mateo, el joven reportero](https://voragine.co/historias/perfil/el-futuro-asesinado-la-historia-de-mateo-el-joven-reportero/) | antes | N | perfil de un periodista asesinado por el frente de «Calarcá», «nombrado gestor de paz» |
| 51 | 2026-05-13 | [En Chocó los bonos de carbono esconden un “extractivismo verde sofisticado”](https://voragine.co/historias/investigacion/en-choco-los-bonos-de-carbono-esconden-un-extractivismo-verde-sofisticado/) | antes | F · empresas | bonos de carbono |
| 52 | 2026-05-17 | [7.837 falsos positivos: las historias íntimas de los abrazos en la JEP](https://voragine.co/historias/cronica/7-837-falsos-positivos-las-historias-intimas-de-los-abrazos-en-la-jep/) | antes | N | crónica de la JEP |
| 53 | 2026-05-17 | [‘Chalá’, el señalado asesino del periodista Mateo Pérez, es el “sicario de confianza” de ‘Calarcá’](https://voragine.co/historias/investigacion/chala-el-senalado-asesino-del-periodista-mateo-perez-es-el-sicario-de-confianza-de-calarca/) | antes | F · grupos armados | asesino de un periodista |
| 54 | 2026-05-17 | [Campañas bajo ataque digital: el doble desafío de las mujeres en la política colombiana](https://voragine.co/historias/investigacion/campanas-bajo-ataque-digital-el-doble-desafio-de-las-mujeres-en-la-politica-colombiana/) | antes | N | violencia digital contra candidatas de los dos lados |
| 55 | 2026-05-17 | [Ecosistema del ataque: quiénes y cómo impulsan la violencia política contra las mujeres](https://voragine.co/historias/investigacion/ecosistema-del-ataque-quienes-y-como-impulsan-la-violencia-politica-contra-las-mujeres/) | antes | F · otros | ecosistema de ataques a candidatas; nombra cuentas «a favor del gobierno Petro y el candidato presidencial oficialista Iván Cepeda» · contrapeso parcial |
| 56 | 2026-05-17 | [Cuando la violencia política digital llega a la mensajería interna](https://voragine.co/historias/investigacion/cuando-la-violencia-politica-digital-llega-a-la-mensajeria-interna/) | antes | N |  |
| 57 | 2026-05-17 | [Candidatas bajo ciberataque: así funciona la violencia política digital](https://voragine.co/historias/investigacion/candidatas-bajo-ciberataque-asi-funciona-la-violencia-politica-digital/) | antes | N |  |
| 58 | 2026-05-24 | [Asesor de “Gury” Rodríguez estuvo en la escena de un presunto secuestro](https://voragine.co/historias/investigacion/asesor-de-gury-rodriguez-estuvo-en-la-escena-de-un-presunto-secuestro/) | antes | F · derecha, no candidato | asesor de un concejal del CD · rótulo leve en voz de la casa: «se ha caracterizado por intimidar la protesta social» |
| 59 | 2026-05-25 | [Tierra y periodismo: taller de herramientas para investigar y cubrir el catastro multipropósito](https://voragine.co/historias/tierra-y-periodismo-taller-de-herramientas-para-investigar-y-cubrir-el-catastro-multiproposito/) | antes | N | taller |
| 60 | 2026-05-28 | [La Amazonía se desangra: ¿Por qué les importa tan poco a los candidatos presidenciales?](https://voragine.co/comic/la-amazonia-se-desangra-por-que-les-importa-tan-poco-a-los-candidatos-presidenciales/) | antes | N | cómic: la Amazonía y todos los candidatos |
| 61 | 2026-05-30 | [La socia de Abelardo que hizo negocios con un lavador de la mafia](https://voragine.co/historias/investigacion/la-socia-de-abelardo-que-hizo-negocios-con-un-lavador-de-la-mafia/) | antes | F · candidato o presidente electo de derecha | socia de De la Espriella |
| 62 | 2026-05-31 | [En campaña de De la Espriella hay miles de funcionarios inscritos, incluyendo policías activos](https://voragine.co/historias/investigacion/en-campana-de-de-la-espriella-hay-miles-de-funcionarios-inscritos-incluyendo-policias-activos/) | antes | F · candidato o presidente electo de derecha | base de datos de la campaña de De la Espriella (alianza con Cuestión Pública y otros) |
| 63 | 2026-06-09 | [Tierra y periodismo: taller de herramientas para investigar y cubrir el catastro multipropósito en Boyacá](https://voragine.co/historias/tierra-y-periodismo-taller-de-herramientas-para-investigar-y-cubrir-el-catastro-multiproposito-en-boyaca/) | antes | N | taller |
| 64 | 2026-06-14 | [Tráfico de mercurio: de un cartel mexicano a envenenar los ríos amazónicos en Colombia](https://voragine.co/historias/trafico-de-mercurio-de-un-cartel-mexicano-a-envenenar-los-rios-amazonicos-en-colombia/) | antes | F · grupos armados | tráfico de mercurio |
| 65 | 2026-06-18 | [Nukak: cercados por un baño de sangre y la ganadería](https://voragine.co/historias/reportaje/nukak-cercados-por-un-bano-de-sangre-y-la-ganaderia/) | antes | N |  |
| 66 | 2026-06-20 | [El crimen de Cristian Herrera y la orfandad del periodismo en Cúcuta](https://voragine.co/historias/el-crimen-de-cristian-herrera-y-la-orfandad-del-periodismo-en-cucuta/) | antes | N |  |
| 67 | 2026-06-23 | [Buscar justicia para su abuela la convirtió en una de las científicas indígenas más visibles de América Latina](https://voragine.co/historias/perfil/buscar-justicia-para-su-abuela-la-convirtio-en-una-de-las-cientificas-indigenas-mas-visibles-de-america-latina/) | antes | N |  |
| 68 | 2026-06-28 | [En el pueblo donde el calor desmaya, las niñas y niños enseñan a cuidar el planeta](https://voragine.co/historias/cronica/en-el-pueblo-donde-el-calor-desmaya-las-ninas-y-ninos-ensenan-a-cuidar-el-planeta/) | antes | N |  |
| 69 | 2026-06-28 | [Le ponen freno a Coca-Cola en La Calera](https://voragine.co/historias/le-ponen-freno-a-coca-cola-en-la-calera/) | antes | F · empresas · VS | Coca-Cola |
| 70 | 2026-07-05 | [Venezuela: la tragedia de desenterrar todo lo que amas](https://voragine.co/historias/cronica/venezuela-la-tragedia-de-desenterrar-todo-lo-que-amas/) | antes | N |  |
| 71 | 2026-07-08 | [Coca-Cola in La Calera: Water Exploitation Curtailed Through Social Resistance](https://voragine.co/historias/coca-cola-in-la-calera-water-exploitation-curtailed-through-social-resistance/) | antes | F · empresas · VS | (inglés) |
| 72 | 2026-07-10 | [Falsos positivos y presunta corrupción: los generales del empalme de De la Espriella](https://voragine.co/historias/investigacion/falsos-positivos-y-presunta-corrupcion-los-generales-del-empalme-de-de-la-espriella/) | antes | F · candidato o presidente electo de derecha | generales del empalme del presidente electo |
| 73 | 2026-07-12 | [El Estado colombiano sigue en deuda con el pueblo U’wa](https://voragine.co/historias/reportaje/el-estado-colombiano-sigue-en-deuda-con-el-pueblo-uwa/) | antes | F · Gobierno Petro | el Gobierno Nacional y la sentencia U’wa (marzo de 2026) |
| 74 | 2026-07-16 | [Brakes on for Coca-Cola in La Calera](https://voragine.co/comic/brakes-on-for-coca-cola-in-la-calera/) | antes | F · empresas · VS | (inglés) |
| 75 | 2026-07-17 | [El millonario y cuestionado negocio de Coca-Cola con el Mundial de Fútbol y los Juegos Olímpicos](https://voragine.co/comic/el-millonario-y-cuestionado-negocio-de-coca-cola-con-el-mundial-de-futbol-y-los-juegos-olimpicos/) | antes | F · empresas · VS | Coca-Cola |
| 76 | 2026-07-29 | [Acoso y nexos con paras: los señalamientos a los nuevos voceros de Abelardo de la Espriella](https://voragine.co/historias/investigacion/acoso-y-nexos-con-paras-los-senalamientos-a-los-nuevos-voceros-de-abelardo-de-la-espriella/) | antes | F · candidato o presidente electo de derecha | voceros del presidente electo |
| 77 | 2026-07-31 | [La guerra entre “Calarcá” y “Mordisco” que desangra al Chiribiquete](https://voragine.co/historias/investigacion/la-guerra-entre-calarca-y-mordisco-que-desangra-al-chiribiquete/) | antes | F · grupos armados | «Calarcá» y «Mordisco» |
| 78 | 2026-08-02 | [Engañados para viajar, obligados a delinquir: la nueva trata de colombianos en Camboya](https://voragine.co/historias/investigacion/enganados-para-viajar-obligados-a-delinquir-la-nueva-trata-de-colombianos-en-camboya/) | antes | F · otros | trata de personas |
| 79 | 2026-08-02 | [“Qué culos te importa si a Postobón le meten una multa”: denuncian humillaciones y despidos ilegales en la compañía](https://voragine.co/historias/investigacion/que-culos-te-importa-si-a-postobon-le-meten-una-multa-denuncian-humillaciones-y-despidos-ilegales-en-la-compania/) | antes | F · empresas | Postobón |
| 80 | 2026-08-07 | [El negocio del vocero de Abelardo con “el Hombre Malboro”, un narco guajiro](https://voragine.co/historias/investigacion/el-negocio-del-vocero-de-abelardo-con-el-hombre-malboro-un-narco-guajiro/) | después | F · candidato o presidente electo de derecha | vocero del gobierno entrante (publicada el día de la posesión) |
| 81 | 2026-08-12 | [Conversatorio: La Séptima: una carrera por la memoria](https://voragine.co/historias/analisis/conversatorio-la-septima-una-carrera-por-la-memoria/) | después | N | conversatorio |
| 82 | 2026-08-15 | [Los campesinos heridos que De La Espriella no mencionó sobre su primer bombardeo](https://voragine.co/historias/investigacion/los-campesinos-heridos-que-de-la-espriella-no-menciono-sobre-su-primer-bombardeo/) | después | F · Gobierno De la Espriella | primer bombardeo del Gobierno |
| 83 | 2026-08-16 | [Chocó en carne viva: el terremoto que dejó al desnudo un siglo de promesas incumplidas](https://voragine.co/historias/cronica/choco-en-carne-viva-el-terremoto-que-dejo-al-desnudo-un-siglo-de-promesas-incumplidas/) | después | N | crónica del terremoto |
| 84 | 2026-08-23 | [Buenaventura sin escuelas: el terremoto agravó el riesgo de reclutamiento](https://voragine.co/historias/reportaje/buenaventura-sin-escuelas-el-terremoto-agravo-el-riesgo-de-reclutamiento/) | después | N |  |
| 85 | 2026-08-31 | [Fronteras de la desaparición: las personas que los gobiernos no buscan](https://voragine.co/historias/fronteras-de-la-desaparicion-las-personas-que-los-gobiernos-no-buscan/) | después | N |  |
| 86 | 2026-08-31 | [Nariño: Buscar un rastro de vida en una frontera silenciada](https://voragine.co/historias/investigacion/narino-buscar-un-rastro-de-vida-en-una-frontera-silenciada/) | después | N |  |
| 87 | 2026-09-01 | [El imperio de alias “Calarcá” que devora el bosque en Caquetá](https://voragine.co/historias/investigacion/el-imperio-de-alias-calarca-que-devora-el-bosque-en-caqueta/) | después | F · grupos armados | «Calarcá» |
| 88 | 2026-09-06 | [De la página a la pantalla, taller con Camila Brugés, guionista de “Cien años de soledad”](https://voragine.co/historias/de-la-pagina-a-la-pantalla-taller-con-camila-bruges-guionista-de-cien-anos-de-soledad/) | después | N | taller |
| 89 | 2026-09-08 | [Coca-Cola’s Million Dollar Controversial Business Deal with the FIFA World Cup and the Olympic Games](https://voragine.co/comic/coca-colas-million-dollar-controversial-business-deal-with-the-fifa-world-cup-and-the-olympic-games/) | después | F · empresas · VS | (inglés) |
| 90 | 2026-09-20 | [Asesinatos contra personas trans: aumenta la violencia y el gobierno desprotege](https://voragine.co/historias/reportaje/asesinatos-contra-personas-trans-aumenta-la-violencia-y-el-gobierno-desprotege/) | después | F · Gobierno De la Espriella | retiro de una coalición de derechos y violencia contra personas trans · rótulo leve en voz de la casa: titular «el gobierno desprotege» y «influencer de extrema derecha» |
| 91 | 2026-09-27 | [Briceño y los intereses detrás de la ofensiva contra los impuestos saludables](https://voragine.co/historias/investigacion/briceno-y-los-intereses-detras-de-la-ofensiva-contra-los-impuestos-saludables/) | después | F · Gobierno De la Espriella · VS | representante del CD e intereses azucareros; créditos del Gobierno |
| 92 | 2026-10-04 | [Una niña bajo fuego y un asesinato: la denuncia contra el Ejército en Meta](https://voragine.co/historias/reportaje/una-nina-bajo-fuego-y-un-asesinato-la-denuncia-contra-el-ejercito-en-meta/) | después | F · Fuerza Pública | denuncia contra el Ejército (Gobierno De la Espriella) |
| 93 | 2026-10-07 | [Las últimas horas de Julián, el periodista hallado muerto en un bosque en Antioquia](https://voragine.co/historias/reportaje/las-ultimas-horas-de-julian-el-periodista-hallado-muerto-en-un-bosque-en-antioquia/) | después | N | periodista asesinado |

---

## 3. Recuento

| Clase | Antes del 07-08 | Desde el 07-08 | Total |
|---|---:|---:|---:|
| F · Gobierno Petro | 6 (n.º 15, 27, 31, 36, 45, 73) | — | 6 |
| F · Gobierno De la Espriella | — | 3 (n.º 82, 90, 91) | 3 |
| F · Fuerza Pública bajo el Gobierno De la Espriella | — | 1 (n.º 92) | 1 |
| F · candidato o presidente electo de derecha | 7 (n.º 24, 30, 39, 61, 62, 72, 76) | 1 (n.º 80, el día de la posesión) | 8 |
| F · derecha que no es candidato | 4 (n.º 3, 18, 33, 58) | — (la n.º 91 va con el Gobierno) | 4 |
| F · empresas | 19 | 1 | 20 |
| F · Fuerza Pública (antes), grupos armados, instituciones, otros | 16 | 1 | 17 |
| Ajena (La Liga, autor externo, colectivo) | 4 (n.º 25, 32, 34, 37) | 0 | 4 |
| N, neutra | 23 | 7 | 30 |
| **Total** | **79** | **14** | **93** |

**Postura en voz de la casa (lo único que cuenta para la regla):**

| | Antes | Desde el 07-08 | Dirección |
|---|---:|---:|---|
| Rótulos leves | 2 (n.º 3, 58) | 1 (n.º 90) | contra la derecha |
| Elogios o disculpas a un gobierno, partido o candidato | 0 | 0 | — |
| **Total con postura** | **2** | **1** | **3, todas en la misma dirección** |

**Contrapesos.** No son postura; se anotan porque contradicen la lectura de «asimetría»:
- 6 piezas de fiscalización al Gobierno Petro antes del cambio, una de ellas firmada por el director (n.º 36);
- la n.º 55, en plena campaña, nombra entre los atacantes de una congresista a cuentas «a favor del gobierno Petro y el candidato presidencial oficialista Iván Cepeda»;
- la n.º 31, también en campaña, documenta presiones en un ministerio para marchar a favor de Petro;
- la n.º 50 llama a «Calarcá» «nombrado gestor de paz» al contar el asesinato de un periodista por su frente.

**Vital Strategies:** 17 de 93 piezas (n.º 2, 7, 10, 12, 16, 17, 22, 29, 41, 42, 47, 69, 71, 74, 75, 89, 91), todas sobre la industria de alimentos y bebidas. 8 son versiones en inglés o en cómic de piezas de la misma serie.

---

## 4. Lo que dice cada condición

1. **Voz de la casa.** La hay: casi todo va firmado por la casa o por periodistas de su redacción. **Pero no hay editoriales en la ventana** y la sección Opinión está vacía. Lo que queda en voz de la casa es investigación, y la postura aparece solo en 3 rótulos sueltos.
2. **A los dos lados del cambio.** Hay piezas a los dos lados, pero de fiscalización: 6 contra el gobierno saliente y 4 contra el entrante. Con postura: 2 y 1. **No llega a 3 por lado.**
3. **Sostenida.** 3 piezas con postura, contra un mínimo de 10. **No se cumple.** La proporción (3 a 0) no significa nada con ese volumen.
4. **Contrapesos.** Escritos arriba.
5. **Reproducible.** Esta tabla.

**Veredicto: no cumple.** Por la segunda precisión del responsable editorial (2026-10-09), «un barrido que no llega a los mínimos no deshace nada»: se conserva el valor vigente. **Y el valor vigente es «sin medir», no −0,50** (ver §6).

---

## 5. La asimetría de campaña: ¿postura o fiscalización del puntero?

**El hecho.** Entre el 2026-01-25 y el 2026-07-29, Vorágine publicó 7 investigaciones sobre De la Espriella: él mismo, su campaña, su socia, su empalme y sus voceros. Publicó también una sobre la fórmula vicepresidencial de Paloma Valencia (n.º 39). Sobre Iván Cepeda o su campaña no publicó **ninguna**. De las 7 entradas que dan «Cepeda», dos se refieren a otras personas con ese apellido: Efraín Cepeda en la n.º 15 e Iván Camilo Cepeda en la n.º 31.

**Cómo lo lee el protocolo, literal.**
- Polo fijo, «Qué NO toca esta regla»: «Lo mismo vale para el encuadre asimétrico entre candidatos». Es decir, **el encuadre asimétrico entre candidatos es evidencia admisible** y no queda excluido como fiscalización.
- Pero «Evidencia editorial histórica», primera precisión: para el mínimo «solo cuentan los elogios, las disculpas y los rótulos. Una pieza que solo fiscaliza a quien manda se declara, pero no suma». Y el §5, regla 3: sin nivel 1-3 el número no se mueve, salvo por esa vía.
- La propia ficha fija qué contaría (REFUTACIÓN): «trato distinto a dos actores comparables», no «dureza con quien manda».

**Lectura.** Ocho investigaciones sobre un candidato no son un encuadre: son una **frecuencia de blancos**. Para hablar de encuadre asimétrico hay que mostrar que el medio trató distinto a dos actores comparables con material comparable, y este barrido no lo muestra:
- **Confusor 1, documentado por el propio medio.** De la Espriella era puntero en las encuestas que cita la n.º 21, y después presidente electo. La n.º 24 cita a la Flip: «109 denuncias por injuria y calumnia de De la Espriella contra periodistas entre 2008 y 2019». Investigar al candidato con más opciones de poder, que es además el mayor litigante contra la prensa, es fiscalizar el poder probable.
- **Confusor 2.** Tres de las ocho son de después de la elección, con De la Espriella como presidente electo, y otra es del día de la posesión. Eso ya es fiscalizar a quien va a mandar.
- **Contrapesos.** En campaña, la n.º 55 toca el ecosistema digital del candidato oficialista, y la n.º 31, al Gobierno que lo respaldaba.

**Conclusión.** La asimetría de campaña **se declara como tensión** (nivel 5, conducta observable) y **no suma** para la regla. Aun contándola como postura, no se llega al mínimo: son 8 piezas, todas de un lado, pero ninguna es elogio, disculpa ni rótulo. Y la regla pide 10 piezas con postura y 3 a cada lado del cambio.

---

## 6. De dónde salía el −0,50, y qué valor queda

- **La ficha lo dice ella misma:** «El −0,50 no viene de ninguna medición, ni antigua ni nueva: es una colocación entre RAYA y Cuestión Pública» (CONTRA, punto 4). Ninguna entrada de `DECISIONES.md` lo justifica con evidencia.
- **El responsable editorial lo retiró el 2026-09-16:** «el trío y RTVC "sin medir"» (`PLAN_PRODUCTO_FINAL.md`, tarea 3.5). Se aplicó el 2026-09-18 (commit `fa77249`). Desde entonces, `shared/mediaRegistry.js` lleva `bias: null` con el comentario «SIN MEDIR — decisión del responsable editorial del 2026-09-16, aplicada el 2026-09-18. Llevaba −0,50».
- **La cabecera de la ficha no se actualizó** («Valor actual | −0,50»). De ahí pasó al envío del 2026-10-10 y a su `00-LEEME.md`. El revisor atacó un valor que ya no está en el código.
- **Reglas 2 y 3.** No hay evidencia de nivel 1-3 que sitúe al medio en el eje, y el barrido no llega a los mínimos, así que el número no se mueve: se queda en **sin medir**.
- **Lo que el barrido sí permite, si el responsable editorial lo quiere.** El protocolo dice: «Un barrido que muestra la misma conducta con los dos gobiernos sostiene el 0,00 como evidencia». Aquí la conducta es la misma con los dos gobiernos: fiscaliza a los dos y no celebra a ninguno. Es el caso de Chocó 7 Días, 0,00 con evidencia desde el 2026-10-09.
- **En contra del 0,00:**
  - la asimetría de campaña del §5, que Chocó 7 Días no tenía;
  - que el 16-09 se decidió para el trío entero (Vorágine, Cuestión Pública y Revista RAYA).

  **Ningún valor negativo tiene apoyo.**

---

## 7. PROPUESTA (pendiente de la firma del responsable editorial)

- **Valor: sin medir (`bias: null`), sin cambios en el código.** Alternativa declarada: **0,00 provisional, con evidencia**, con la asimetría de campaña escrita como tensión. Ningún valor de izquierda tiene apoyo.
- **Corregir la cabecera de la ficha y el `00-LEEME.md` del envío:** «−0,50» → «sin medir (decisión del 2026-09-16)».
- **Revisión: recontar en enero de 2027**, con cinco meses de Gobierno De la Espriella. Hay dos cosas que mirar:
  - si aparece postura en voz de la casa (editoriales, comunicados propios o titulares con rótulo) en cantidad suficiente, se aplica la regla;
  - si el medio publica sobre Cepeda o el Pacto Histórico algo comparable a lo de De la Espriella, o si sigue sin hacerlo teniendo material, se anota.
