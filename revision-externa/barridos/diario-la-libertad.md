# Barrido editorial: Diario La Libertad

| | |
|---|---|
| **Medio** | Diario La Libertad, Barranquilla, Atlántico (`diario-la-libertad`) |
| **Valor vigente** | 0,00, provisional y sin firmar, «ya no por Regla 2». La ficha declara que los editoriales de septiembre «apuntan a la derecha» y que solo la regla 3 impidió mover el número (DECISIONES.md, 2026-10-07, «Ciclo 2, tanda 1») |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09) |
| **Ventana** | 2025-10-09 → 2026-10-09 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5 (`claude-opus-5-5`), a petición del responsable editorial, el 2026-10-09. Es de la misma casa que el autor de la ficha y que quien escribió la resolución del ciclo 2: su acuerdo no es aval |
| **Estado** | **DECIDIDO el 2026-10-09: +0,20** (antes 0,00), por el responsable editorial; firmado en bloque el 2026-10-10 (`DECISIONES.md`, «2026-10-09 · Reexamen de cinco fichas cerradas con la regla nueva»). Lo que más abajo dice «propuesta» o «pendiente» es el estado anterior a la decisión y se conserva como historia |
| **Decisión (2026-10-09)** | el responsable editorial: **de 0,00 a +0,20.** La celda 3b de este barrido cuenta también la fiscalización; con la precisión del mismo día (fiscalizar no cuenta por lado) quedan 4 piezas antes, favorables al presidente electo, y 11 después, así que sigue cumpliéndose. El cambio de redactor es un indicio, no un hecho (`DECISIONES.md`, «Reexamen de cinco fichas cerradas con la regla nueva»; ver la ficha) |

---

## 1. Método

- **robots.txt** de diariolalibertad.com (descargado el 2026-10-09): `User-agent: * / Crawl-delay: 10`. No excluye ninguna ruta. **Se respetó el retardo de 10 s** entre peticiones.
- **No se tocaron** eltiempo.com, cambiocolombia.com ni lasillavacia.com. No hubo buscador web.
- **Descarga.** `curl -sL --ssl-no-revoke` con el UA de un navegador (Chrome 128 en Windows), el 2026-10-09. Todas las páginas respondieron 200. La fecha de cada pieza es la de su URL, que coincide con `datePublished`. El feed da a veces el día siguiente, por la hora UTC.
- **Por qué no los sitemaps.** `sitemap.xml` es un índice de 1.123 `post-sitemap` de hasta 200 URL cada uno, pero **se dejó de regenerar el 16-07-2026**: `post-sitemap1.xml` acaba en esa fecha. Para tres meses del año, el sitemap no sirve. La API REST sigue cerrada (`401`, ya anotado en la ficha).
- **Cómo se armó la lista. Es un barrido por sección y por término.**
  1. **El feed de la sección Editorial** (`/seccion/editorial/feed/`, páginas 1-2): 50 piezas en la ventana. La sección está **incompleta**: no recoge la mayoría de los «[EDITORIAL]» de 2026, por ejemplo los del 06, 10 y 12-09.
  2. **El feed del buscador del sitio para «editorial»** (`/?s=editorial&feed=rss2`, páginas 1-7, hasta pasar del 09-10-2025): 316 piezas en la ventana, de las que **181 llevan «editorial» en el título o en la URL**.
  - Unión de las dos, deduplicada por URL: **213 piezas**. Se quitaron 2 que solo usan la palabra en otro sentido (la editorial Punto y Coma en la FILBO; la «colección editorial» de Petro en una noticia sobre Cabal). **Quedan 211, y se descargaron las 211.**
- **Voz de la casa.** Los editoriales se titulan «[EDITORIAL] …» o «Editorial | …», se publican con cuentas de redacción (Redacción1 hasta el 29-04-2026; Redacción4 desde el 05-05; Redacción2 y Redacción3 en algunos) y hablan como la casa: «Consideramos en LA LIBERTAD», «en este espacio editorial», «lo apoyaremos como voceros de la comunidad que siempre hemos sido en LA LIBERTAD». Las piezas sin «[EDITORIAL]» pero colgadas en la sección Editorial, sin firma y en la misma voz («A gobernar, señor Presidente», «La paz también necesita autoridad»…) también se cuentan como voz de la casa.
- **Excluidas de las 211 (13)**, porque no son voz de la casa:
  - **Columnas firmadas o de tercero (10):**
    - María Fernanda Cabal, «La hora de la patria MILAGRO» (22-06);
    - el 05-07, cinco piezas: Sofy Casas («Cepeda llama a incendiar el país…»), Indalecio Dangond («Empalme»), un columnista que se presenta como tal («Presidente De la Espriella: no repita el error de Petro con Roa»), «Mindset» y «Canacol estresa el mercado del gas»;
    - Isis Navarro, «Abelardo hereda otra gran crisis…» (05-08);
    - «¿Un “Supermetro” por un ojo de la cara?» (02-10, primera persona: «Atónito quedé…»);
    - «La pelotera & jab de derecha, jab de izquierda» (17-06): sin firma, pero es una serie con nombre propio, escrita en primera persona del plural de un autor («Así explicábamos…»). Probable columna; además no tiene postura clara;
    - «Grupo Banco Mundial» (08-12-2025): un comentario cerrado con «Barranquilla, diciembre 7 de 2025» y el comunicado del Banco Mundial pegado detrás. Parece una colaboración. **Dudosa:** si fuera de la casa, sumaría una pieza más a la derecha («Con esa política de endeudamiento del gobierno Petro…»).
  - **Reimpresión de otro medio (1):** «Bloqueo al control político… en Fundación» (15-05), firmada «Por: Editorial Sin tapujos Col.».
  - **Noticias (2):** USTDA y el centro de datos (30-09); el Carnaval en Madrid (02-10).
- **Quedan 198 piezas en voz de la casa**: 151 antes del 07-08-2026 y 47 desde ese día. Por mes: oct-2025 5 · nov 11 · dic 10 · ene-2026 12 · feb 13 · mar 21 · abr 17 · may 19 · jun 22 · jul 26 · ago 25 · sep 22 · oct 8 (cifras de las 211, antes de quitar las 13).
- **Filtro.**
  - Se extrajo el texto de las 211 y se buscaron estos términos: Petro, Gobierno nacional, «el Gobierno», gobierno del cambio, Pacto Histórico, De la Espriella/Abelardo, Cepeda, izquierda/derecha, presidente, ministr-, paz total, Ejecutivo, Uribe, Centro Democrático, Paloma, Fajardo, oposición, reforma, Constituyente, JEP, gabinete.
  - Salieron **131** piezas con algún término. Se leyeron por esas frases, y **las 45 que tenían postura o la rozaban se leyeron enteras**.
  - Las demás son locales (seguridad en Barranquilla, frentes de seguridad, alcaldes), de salud y Ley 100, de violencia contra la mujer, de canasta familiar o de energía en el Caribe, o bien efemérides. Muchas se republican casi idénticas varias veces: «Grandes expectativas para el 2026» ×3, «Expectativas por el nuevo Congreso» ×3, «La paz, anhelo histórico…» ×2, «Reacciones del país político» ×2, «Matrículas universitarias…» ×2.
- **La directora.** Ningún editorial de la ventana nombra a Luz Marina Esper, a Daniela Esper ni a Samuel Tcherassi: se buscó «Esper», «Luz Marina» y «Tcherassi» en las 211. **No hay cobertura editorial de la candidatura anunciada de la directora que separar.** Su anuncio (12-10-2025) es una pieza informativa y queda fuera de este barrido. Tampoco hay editoriales sobre la política del Atlántico que pudieran leerse como campaña propia.
- **Qué se clasificó.** Solo las piezas con postura sobre el Gobierno nacional, las candidaturas presidenciales o el presidente electo. La seguridad local, el alcalde Char y el gobernador se declaran y no se puntúan (polo fijo nacional, igual que en la ficha).
  - **D, dirección derecha:**
    - critica o fiscaliza al Gobierno Petro, al Pacto Histórico o a su política (se marca *fiscaliza a quien manda* para leerla con el polo fijo, §3);
    - favorece a De la Espriella o a su programa como candidato o presidente electo;
    - celebra, apoya o disculpa a su Gobierno.
  - **I, dirección izquierda:**
    - favorece o disculpa al Gobierno Petro o a su candidato;
    - critica un discurso de la derecha;
    - controla o fiscaliza al Gobierno De la Espriella.
  - **Fuerza:** *clara* (la postura es la tesis de la pieza), *moderada* o *leve* (una frase o un remate dentro de una pieza sobre otra cosa). El recuento se da con todas y solo con las claras y moderadas.

---

## 2. Tabla de piezas que cuentan (voz de la casa)

### Antes del cambio de gobierno (09-10-2025 → 06-08-2026)

| # | Fecha | Pieza | Lado | Clasificación | Fuerza |
|---|---|---|---|---|---|
| 1 | 2025-10-27 | [Consulta del Pacto Histórico](https://diariolalibertad.com/2025/10/27/editorial-consulta-del-pacto-historico/) | D | Fiscaliza a quien manda: «los discursos de superioridad que siempre han venido manteniendo algunos líderes del actual gobierno, incluyendo al presidente Petro»; «lo que no se conoce es el monto económico» | moderada |
| 2 | 2025-12-24 | [¡Feliz Navidad para nuestros lectores!](https://diariolalibertad.com/2025/12/24/editorial-feliz-navidad-para-nuestros-lectores/) | D | Fiscaliza a quien manda: el Gobierno «no ha encarado el problema [del reclutamiento] con la convicción que requiere» | leve |
| 3 | 2026-02-05 | [Trump y Petro en la Casa Blanca](https://diariolalibertad.com/2026/02/05/editorial-trump-y-petro-en-la-casa-blanca/) | **I** | Favorable a Petro: «regresó de Washington con imagen reforzada»; «eso es un buen comienzo» (con reparos: «más interrogantes que certezas») | leve |
| 4 | 2026-03-31 | [La farsa de la paz, negociar con quien nunca dejó de delinquir](https://diariolalibertad.com/2026/03/31/editorial-la-farsa-de-la-paz-negociar-con-quien-nunca-dejo-de-delinquir/) | D | Fiscaliza a quien manda: «La política de ‘paz total’ del presidente Gustavo Petro queda hoy profundamente cuestionada»; «un montaje político desconectado de la realidad» | clara |
| 5 | 2026-04-06 | [Entre la fe que transforma y la política que interpela](https://diariolalibertad.com/2026/04/06/entre-la-fe-que-transforma-y-la-politica-que-interpela/) | **I** | Critica un discurso de la derecha: «asociar “la derecha” con un mandato espiritual» simplifica la democracia; «La espiritualidad no debería ser un instrumento de presión ideológica» | leve |
| 6 | 2026-04-08 | [El Banco de la República, en el ojo del huracán](https://diariolalibertad.com/2026/04/08/editorial-el-banco-de-la-republica-en-el-ojo-del-huracan/) | D | Fiscaliza a quien manda: «una ruptura con el Banco de la República no es una diferencia técnica, es una señal riesgosa»; «la economía no se puede politizar» | clara |
| 7 | 2026-05-29 | [El sistema de salud en estado de coma](https://diariolalibertad.com/2026/05/29/editorial-el-sistema-de-salud-en-estado-de-coma/) | D | Fiscaliza a quien manda: «la opinión pública le está pasando una cuenta de cobro al Gobierno Nacional»; «Esperemos que el nuevo Presidente… le ponga punto final» | leve |
| 8 | 2026-07-01 | [La salud, un gran reto para el nuevo Presidente](https://diariolalibertad.com/2026/07/01/editorial-la-salud-un-gran-reto-para-el-nuevo-presidente/) | D | Favorable al electo y crítica al saliente: «En el pasado las intervenciones estatales resultaron fallidas»; expone sin reparos el plan de De la Espriella | leve |
| 9 | 2026-07-06 | [La Costa Caribe no puede seguir gobernada por el miedo](https://diariolalibertad.com/2026/07/06/editorial-la-costa-caribe-no-puede-seguir-gobernada-por-el-miedo/) | D | Favorable al electo: «cobra especial importancia la propuesta anunciada por el presidente electo… Bloque de Defensa para la Seguridad Urbana» | leve |
| 10 | 2026-07-09 | [La paz que fortaleció a los violentos](https://diariolalibertad.com/2026/07/09/editorial-la-paz-que-fortalecio-a-los-violentos/) | D | Fiscaliza al saliente y favorece al electo: la Paz Total, «una estrategia que confundió el diálogo con la renuncia al ejercicio legítimo de la autoridad»; el discurso de De la Espriella «resulta contundente y responde al clamor de millones» (con reparo: «la realidad será mucho más compleja») | clara |
| 11 | 2026-07-27 | [Sin excusas el Gobierno y los chats de Guerrero](https://diariolalibertad.com/2026/07/27/sin-excusas-el-gobierno-y-los-chats-de-guerrero/) | D | Fiscaliza a quien manda: «un golpe profundo para una administración que hizo de la ética pública su principal argumento electoral» (con contrapeso interno: elogia a Cepeda y a Bolívar y dice «Ni el uribismo puede reclamar indulgencia») | clara |
| 12 | 2026-08-05 | [La posesión de Abelardo De La Espriella en Cali](https://diariolalibertad.com/2026/08/05/editorial-la-posesion-de-abelardo-de-la-espriella-en-cali/) | D | Favorable al electo frente a sus adversarios: el fallo es «un hecho que fortalece el Estado Social de Derecho»; «pese a los señalamientos de aparente fraude electoral que aun se pregona… por parte de adversarios»; Cepeda «aún se niega a reconocer al Presidente» | moderada |

### Desde el cambio de gobierno (07-08-2026 → 09-10-2026)

| # | Fecha | Pieza | Lado | Clasificación | Fuerza |
|---|---|---|---|---|---|
| 13 | 2026-08-07 | [Un nuevo capítulo político en Colombia](https://diariolalibertad.com/2026/08/07/editorial-un-nuevo-capitulo-politico-en-colombia/) | **I** | Control del entrante: «el poder no se celebra, se ejerce con responsabilidad»; «apoyar no significa justificarlo todo» | moderada |
| 14 | 2026-08-08 | [Expectativas por el nuevo presidente](https://diariolalibertad.com/2026/08/08/editorial-expectativas-por-el-nuevo-presidente/) | **I** | Escepticismo frente al entrante: «siempre prometen mucho… pero por lo regular nunca cumplen»; lo «cuestionado por prometer hacer un gobierno con quienes nunca han estado al mando, pero contradictoriamente elegir…» | leve |
| 15 | 2026-08-10 | [A gobernar, señor Presidente](https://diariolalibertad.com/2026/08/10/a-gobernar-senor-presidente/) | D | Favorable al Gobierno: el discurso de posesión, «indiscutiblemente… un mensaje bienvenido y muy necesario»; da por sentado «el fracaso de la política de “paz total”» | leve |
| 16 | 2026-08-12 | [Medicamentos por las nubes](https://diariolalibertad.com/2026/08/12/editorial-medicamentos-por-las-nubes-2/) | D | Celebra al Gobierno: «una gran noticia del actual gobierno dirigido por Abelardo De la Espriella»; «existirán personas en el actual Gobierno, capaces de conducir la salud a buen puerto» | clara |
| 17 | 2026-08-12 | [Emergencia económica: gobernar la tragedia y preparar la reconstrucción](https://diariolalibertad.com/2026/08/12/editorial-emergencia-economica-gobernar-la-tragedia-y-preparar-la-reconstruccion/) | **I** | Control del Gobierno: «La excepcionalidad del momento no puede significar ausencia de controles»; «tampoco puede convertirse en un cheque en blanco»; «tiene que explicar… cuánto dinero requiere y de dónde pretende obtenerlo» | clara |
| 18 | 2026-08-18 | [La responsabilidad de un ministro](https://diariolalibertad.com/2026/08/18/editorial-la-responsabilidad-de-un-ministro/) | **I** | Control matizado: la moción contra el ministro Beltrán es «un escenario válido de control político». A la vez lo protege: «Una fotografía, por sí sola, no demuestra que un ministro haya incumplido sus funciones» | leve |
| 19 | 2026-08-20 | [Una medida para implementar en Colombia](https://diariolalibertad.com/2026/08/20/editorial-una-medida-para-implementar-en-colombia/) | D | Favorable al Presidente: su agenda de salud, «sin tener en cuenta las parcialidades políticas»; el control de precios, «una gran estrategia que… se defendería por sí sola» | moderada |
| 20 | 2026-08-24 | [Solidaridad con los afectados por el terremoto](https://diariolalibertad.com/2026/08/24/solidaridad-con-los-afectados-por-el-terremoto/) | D | Favorable al Gobierno: «hasta ahora se ha hecho lo que es menester»; «el anterior gobierno de izquierda» | leve |
| 21 | 2026-08-25 | [Una alianza perfecta](https://diariolalibertad.com/2026/08/25/editorial-una-alianza-perfecta/) | D | Favorable al Presidente: «la necesidad de implementar rápido las medidas que ha trazado el presidente Abelardo De la Espriella» | leve |
| 22 | 2026-09-06 | [Colombia no necesitaba más discursos: necesitaba autoridad](https://diariolalibertad.com/2026/09/06/editorial-colombia-no-necesitaba-mas-discursos-necesitaba-autoridad/) | D | Celebración y autoubicación: «una parte de la izquierda política consiguió instalar la idea de que hablar de seguridad era casi una declaración de guerra…»; «Ese debería ser el verdadero ADN de una derecha moderna» (con reparo: «no significa entregarle un cheque en blanco») | clara |
| 23 | 2026-09-10 | [De la Espriella comienza a demostrar que Colombia sí podía cambiar de rumbo](https://diariolalibertad.com/2026/09/10/editorial-de-la-espriella-comienza-a-demostrar-que-colombia-si-podia-cambiar-de-rumbo/) | D | Celebración y autoubicación: «Ahora la derecha tiene la responsabilidad histórica de demostrar que puede hacerlo mejor»; «La izquierda… debería preguntarse por qué una parte significativa de los colombianos está mirando ahora hacia la derecha» (con reparo: «No es un cheque en blanco») | clara |
| 24 | 2026-09-12 | [Se acabó la paz de rodillas: Colombia necesita autoridad](https://diariolalibertad.com/2026/09/12/editorial-se-acabo-la-paz-de-rodillas-colombia-necesita-autoridad/) | D | Celebración: cerrar los diálogos es «una decisión que era tal vez la única correcta para enderezar el camino»; «resulta razonable que el Gobierno cambie el lenguaje» (pide explicar los $7.000 millones en honorarios) | clara |
| 25 | 2026-09-16 | [Colombia necesita energía, inversión y un Estado que decida](https://diariolalibertad.com/2026/09/16/editorial-colombia-necesita-energia-inversion-y-un-estado-que-decida/) | D | Favorable al Gobierno: «el verdadero éxito de la actual política ambiental» (con reparos: «agilizar no significa flexibilizar irresponsablemente»; «sería un error convertir estas decisiones en una victoria política») | leve |
| 26 | 2026-09-24 | [Un grave perjuicio para Santa Marta](https://diariolalibertad.com/2026/09/24/editorial-un-grave-perjuicio-para-santa-marta/) | D | Favorable al Presidente: «La respuesta del Estado, con el presidente Abelardo De la Espriella a la cabeza, confirma la necesidad…» | leve |
| 27 | 2026-09-25 | [Colombia vuelve a hablarle al mundo desde la seguridad y la soberanía](https://diariolalibertad.com/2026/09/25/editorial-colombia-vuelve-a-hablarle-al-mundo-desde-la-seguridad-y-la-soberania/) | D | Celebración: la política exterior nueva, presentada con el marco del Gobierno («una discusión incómoda pero legítima») | clara |

### Con tema nacional y sin postura (no cuentan, se listan para recontar)

Hay muchas piezas descriptivas. Son de campaña: 17-10-2025, 05-11-2025, 26 y 27-02, 10, 11, 12, 13, 20 y 28-03, 14 y 28-04, 07, 15, 19, 23, 25 y 30-05, 01, 10, 20, 22 y 25-06, 21, 22, 23 y 28-07 de 2026. Son de política pública: 13-01, 30-01, 12-02, 14-03, 30-03, 03-06, 13-06, 30-06, 10-07, 15-07, 30-07, 10-08, 14-08, 02-09, 10-09 (PISA), 29-09 y 03-10. Y hay piezas mixtas o neutras de fondo:
- [La energía no admite improvisaciones](https://diariolalibertad.com/2026/06/30/editorial-la-energia-no-admite-improvisaciones/) (30-06): «El gobierno que concluye impulsó debates necesarios…» frente a «consideraciones ideológicas»;
- [Sin empalme presidencial](https://diariolalibertad.com/2026/07/10/editorial-sin-empalme-presidencial/) (10-07): narra las dos partes;
- [La paz también necesita autoridad](https://diariolalibertad.com/2026/09/21/la-paz-tambien-necesita-autoridad/) (21-09): apoya el enfoque, pero «La paz no puede ser patrimonio de la izquierda ni de la derecha»;
- [El presidente De la Espriella y la JEP](https://diariolalibertad.com/2026/09/22/editorial-el-presidente-de-la-espriella-y-la-jep/) (22-09): descriptivo;
- [Votemos por el bien de la democracia](https://diariolalibertad.com/2026/06/20/editorial-votemos-por-el-bien-de-la-democracia/) (20-06): no nombra candidato;
- [Candidatos por la presidencia](https://diariolalibertad.com/2026/05/25/candidatos-por-la-presidencia/) (25-05): llama a De la Espriella «considerado por la opinión pública como de extrema derecha», sin tomar partido.

---

## 3. Recuento

| | D | I | Total con postura |
|---|---|---|---|
| Antes del 07-08-2026 | 10 | 2 | 12 |
| Desde el 07-08-2026 | 11 | 4 | 15 |
| **Total** | **21** | **6** | **27** |
| Solo claras y moderadas | 12 (6 antes, 6 después) | 2 (ambas después) | 14 |

- **Proporción con todas las piezas: 21 : 6 = 3,5 : 1** hacia la derecha. **Con solo las claras y moderadas: 12 : 2 = 6 : 1.**
- **Lectura con polo fijo.** De las 10 D de antes del cambio, 7 son *fiscalizar a quien manda* (n.º 1, 2, 4, 6, 7, 10 y 11), y eso solo no cuenta. La prueba es qué hace la casa cuando cambia quien manda:
  - **Con Petro en el poder:** 7 piezas de control y 1 favorable (leve, la de Trump).
  - **Con De la Espriella**, contando también sus semanas de presidente electo (n.º 8, 9, 10 y 12): **15 piezas favorables o de celebración** (4 de electo y 11 de presidente) y **4 de control** (1 clara, 1 moderada y 2 leves).
  - **Esa es la asimetría:** al Gobierno saliente lo fiscaliza casi sin elogio; al entrante lo celebra casi cuatro veces más de lo que lo controla, y dos veces se ubica a sí misma en «la derecha».
- **Proporción sin el control de quien manda** (solo celebración, disculpa y autoubicación): **15 favorables a De la Espriella** (4 antes y 11 después del 07-08) **frente a 2 de dirección contraria** (Trump y Petro; Semana Santa). Son 7,5 : 1.
- **El punto débil.** Contando solo lo publicado desde el 07-08, la proporción es **11 : 4 = 2,75 : 1**, por debajo de 3 : 1. El mínimo de la regla se cumple con el barrido entero (3,5 : 1) y con cualquier lectura que quite la fiscalización (7,5 : 1), **no con la ventana posterior sola**. Se declara.
- **Densidad.** 27 de 198 piezas en voz de la casa (14 %) tienen postura nacional. El resto es local, de salud, de seguridad o de efemérides.
- **Concentración.** 9 de las 12 claras y moderadas de dirección D caen entre el 09-07 y el 25-09-2026, y las dos autoubicaciones en «la derecha» son del 06 y el 10-09. De octubre de 2025 a junio de 2026 hay 7 piezas con postura en nueve meses (5 D y 2 I).

---

## 4. Contrapesos (lo que contradice la dirección, y cuánto pesa)

1. **Control escrito del Gobierno entrante (4 piezas: n.º 13, 14, 17 y 18).**
   - El 07-08 y el 12-08 son controles reales y bien argumentados: «el poder no se celebra», «no puede convertirse en un cheque en blanco».
   - **Pesan, pero no igualan:** son 4 frente a 11 favorables en el mismo periodo, y el último es del 18-08. Del 19-08 al 09-10 no hay ningún editorial cuya tesis sea el control de De la Espriella.
2. **Reparos internos en los editoriales de celebración.** Por ejemplo: «no es un cheque en blanco» (06 y 10-09); «Una derecha democrática debe defender también la libertad de prensa» (06-09); «agilizar no significa flexibilizar irresponsablemente» (16-09); que el Gobierno explique los $7.000 millones de honorarios (12-09).
   - Atemperan el tono. **No cambian la tesis de ninguna de esas piezas.**
3. **Piezas de dirección contraria antes del cambio (2, leves).**
   - Una reconoce a Petro una «imagen reforzada» tras la Casa Blanca (05-02).
   - Otra critica que se asocie «la derecha» con un mandato espiritual (06-04).
   - Pesan poco: una frase cada una.
4. **Equilibrio en la campaña.** Los editoriales de campaña (unas 25 piezas de marzo a junio) son descriptivos.
   - El de la víspera de la segunda vuelta no nombra candidato (20-06), y no hay endoso.
   - El 25-05 la casa recoge que a De la Espriella se le considera «de extrema derecha».
   - **Pesa:** la orientación no aparece en campaña, aparece con el Gobierno.
5. **«Sin excusas el Gobierno y los chats de Guerrero» (27-07)** fiscaliza a Petro, pero elogia la reacción de Cepeda y de Bolívar y pide «el mismo rasero» para el uribismo. Es control de quien manda con vocación simétrica.
6. **Fuera del barrido, y sin contar:**
   - el 01-09 la casa publica, con firma de redacción, que el Gobierno De la Espriella «endurece su relación con los medios». Está atribuido a un acta conocida por Caracol Radio: es una noticia reescrita y no cuenta, pero es cobertura crítica del Gobierno;
   - las columnas de terceros con postura (Cabal 22-06; Sofy Casas, Dangond y el columnista del caso Roa el 05-07) se inclinan también a la derecha. **Se declaran y no cuentan.**
7. **Posible cambio de redactor de los editoriales** (tensión 2 de la ficha). El barrido la refuerza sin confirmarla:
   - la cuenta pasa de Redacción1 a Redacción4 el 05-05-2026;
   - desde finales de junio aparecen editoriales largos de registro ensayístico (30-06, 06-07, 09-07, 27-07, 12-08, 18-08, 06-09, 10-09, 12-09, 16-09, 21-09 y 25-09), muy distintos de los formularios de antes («Indiscutiblemente…», «Como se recordará…»);
   - 09-02 y 09-06 salen con Redacción3.
   - **Pesa en la lectura:** si la voz es nueva, la orientación medida es la de los últimos cuatro meses, no la de doce. Sigue siendo voz de la casa (la regla no pide más), pero es una razón para no subir al techo.
8. **Cobertura del barrido.**
   - Entre octubre y diciembre de 2025 aparecen solo 26 piezas (unas dos por semana), frente a casi una diaria desde mayo. Pueden faltar editoriales de esos meses que no lleven la palabra «editorial» y no estén en la sección. La ventana antes del cambio podría estar infrarrepresentada.
   - No se barrieron los titulares informativos (unas 70 piezas al día).

---

## 5. Veredicto por condición

| Condición | Veredicto | Por qué |
|---|---|---|
| 1. Voz de la casa | **Se cumple** | Las 27 son editoriales sin firma personal, de cuenta de redacción, en la sección o con «[EDITORIAL]», y en primera persona de la casa. Se excluyeron 13 piezas: 10 columnas o probables columnas, 1 reimpresión y 2 noticias. **Matiz:** puede haber cambiado el redactor (§4.7) |
| 2. A los dos lados del cambio, en 12 meses | **Se cumple** | 12 piezas con postura antes del 07-08 y 15 después. La asimetría aparece con el cambio: control al saliente (7 de 8 piezas sobre él) y celebración al entrante (15 favorables frente a 4 de control) |
| 3a. ≥10 piezas con postura | **Se cumple** | 27 (14 claras o moderadas) |
| 3b. ≥3 a cada lado del cambio | **Se cumple** | 12 antes y 15 después. Solo claras y moderadas: 6 y 8 |
| 3c. ≥3 : 1 en la misma dirección | **Se cumple, con un punto débil** | 3,5 : 1 con todas; 6 : 1 con claras y moderadas; 7,5 : 1 sin la fiscalización. **Solo la ventana posterior da 2,75 : 1** |
| 4. Contrapesos escritos | **Se cumple** | §4: 4 controles del entrante, reparos internos, 2 piezas contrarias, campaña sin endoso, posible cambio de redactor y huecos de cobertura |
| 5. Reproducible | **Se cumple** | §1 (fuentes y filtros) y §2 (las 27 piezas con URL, fecha, lado y fuerza, más la lista de las piezas sin postura) |

**Las cinco condiciones se cumplen.** La dirección es **derecha**.

---

## 6. PROPUESTA (pendiente de la firma del responsable editorial)

**Pasar de 0,00 a +0,20** («Derecha moderada», en su borde inferior), como **juicio declarado** bajo la regla «Evidencia editorial histórica».

**El tope.** Es **±0,30**:
- **no hay propiedad con posición acreditada.** La compra por Samuel Tcherassi sigue siendo una versión del comprador, sin registro; el medio se describe como propiedad de los Esper;
- **no hay endoso.** El 20-06 no nombra candidato;
- y la directora no fue candidata inscrita: el aviso se cerró con `hasta` 2026-06-21.

**Por qué +0,20 y no más:**
1. **Frente a los vecinos:**
   - **El Heraldo (+0,20)**, en la misma ciudad y el mismo departamento, es la referencia natural;
   - **El Pilón (+0,20)**, otro diario del Caribe con apoyo editorial al Gobierno De la Espriella;
   - **Vive el Meta (+0,25, propuesto).** La Libertad no muestra más que ellos:
     - la autoubicación explícita en «la derecha» se reduce a dos editoriales de septiembre;
     - y su control del entrante (4 piezas) es comparable o mayor.
2. **El punto débil del §3:** la ventana posterior sola da 2,75 : 1. El mínimo se cumple con el año, pero no sobra margen.
3. **La sospecha de cambio de redactor (§4.7).** Si la voz es nueva, la orientación tiene cuatro meses, no doce.
4. **Regla 2.** Ante la duda entre +0,20 y +0,25, que están en la misma banda, se queda el valor más cercano a la mixta.

**Opciones descartadas:**
- **+0,25.** Era el borde alto de lo que proponía la condición de refutación de la tanda 1 («+0,20/+0,25»). Pondría a La Libertad por encima de El Heraldo y El Pilón con menos densidad editorial y una ventana posterior por debajo de 3 : 1.
- **Mantener 0,00.** Ya no se sostiene: las cinco condiciones se cumplen y la asimetría está contada, no solo citada.
- **+0,30.** No hay nivel 1 ni endoso que lo justifiquen, y los controles del entrante existen.

**Qué cambiaría si el responsable editorial lo firma** (no se aplica aquí: este archivo no toca la ficha ni el código):
- `fichas/diario-la-libertad.md`:
  - el valor pasa a +0,20, apoyado en este barrido;
  - el apartado «Lo que falta para firmar» queda resuelto por la regla nueva: el recuento de tres meses que pedía la tanda 1 lo sustituye este barrido de doce;
  - y la tensión 1 («Editoriales de septiembre frente al 0,00») se reescribe.
- El texto público (`biasRationale`) debería decir que la orientación sale de la voz editorial de la casa y que hay control escrito del Gobierno entrante.
- **Mover el valor no hace firmable la ficha:** sigue pendiente el certificado de la Cámara de Comercio de Barranquilla, que decide si hay aviso por Tcherassi.

**Condición de revisión propuesta.** Repetir el barrido el 07-02-2027, a los seis meses del Gobierno.
- Si el control del entrante pasa a igualar a la celebración (proporción posterior ≤ 2 : 1), vuelve a 0,00 con evidencia.
- Si la autoubicación en «la derecha» se hace sostenida (≥ 6 editoriales en el semestre), se discute +0,25.

---

## 7. Avisos

- **No se copió ningún dato personal.** No hay cédulas, teléfonos ni direcciones. Se nombra a personas públicas y su papel: la directora, columnistas, ministros, candidatos.
- **El sitemap está congelado desde el 16-07-2026.** Cualquier barrido futuro de este medio tiene que ir por los feeds de sección o del buscador, no por el sitemap.
- **La sección Editorial del sitio está incompleta.** Tiene 50 piezas en un año, frente a unas 200 «[EDITORIAL]». Quien recuente debe usar el feed del buscador.
- **Fechas.** Se usa la fecha de la URL. Varias piezas aparecen en el feed con el día siguiente por la hora UTC (por ejemplo, la del 06-09 sale el 07-09). Las tablas usan la fecha de la URL, igual que la ficha.
- **Duplicados.** La casa republica editoriales casi idénticos con sufijos `-2`, `-3`. Ninguno de los 27 con postura es duplicado de otro.
- **Mismo autor, misma casa.** Este barrido lo hace el mismo modelo que escribió la ficha y la resolución del ciclo 2. La clasificación de las piezas *leves* es la parte más discutible: con solo las claras y moderadas, el resultado se mantiene (12 : 2).
- **La copia local del barrido** (HTML de las 211 piezas, feeds y extractos) está en la carpeta temporal de la sesión, no en el repositorio.
