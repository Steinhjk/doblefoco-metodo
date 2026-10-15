# Barrido editorial: Euronews Español

| | |
|---|---|
| **Medio** | Euronews Español (`euronews-es`), edición en español de la cadena paneuropea Euronews, es.euronews.com. Sin ficha técnica hasta este barrido: se crea, mínima, en `fichas/euronews-es.md` |
| **Valor vigente** | **+0,05**, firmado en bloque el 2026-10-10 (`reviewedAt: '2026-10-10'`). Su razón en el registro: «Cadena paneuropea; agenda centrada en instituciones de la Unión Europea». Habla de la agenda, no de la línea, y no tiene piezas detrás; sus fuentes tratan de la propiedad (Alpac Capital). Se apoya solo en los niveles 4 y 5 |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con la regla del polo fijo y la precisión del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente). Por ser un medio internacional, solo sus piezas sobre Colombia |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12. Es de la misma casa que quien escribió otras fichas y barridos del catálogo: su acuerdo con ellos no es aval |
| **Estado** | **FIRMADO el 2026-10-12: −0,10** (antes +0,05), como se propuso. **Decisión del responsable editorial sobre la pregunta del §5:** «ultraderechista» en voz de la casa cuenta como rótulo, igual que en Revista RAYA, Noticias RCN y Cuestión Pública. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **Cumple las cinco condiciones, pero solo contando las piezas leves.** 113 piezas sobre Colombia en la ventana, leídas enteras (titular, entradilla y cuerpo). Con postura en voz de la casa: **22. 20 hacia la izquierda (I), 1 hacia la derecha (D) y 1 mixta.** Antes del cambio, 13 I, 1 D y 1 M; desde el cambio, 7 I. **De las 20 I, 19 son leves y consisten sobre todo en un rótulo:** la casa llama «ultraderechista» o «de extrema derecha» a De la Espriella, antes y después de que gobierne, mientras a Petro y a Cepeda los llama «izquierdistas», nunca «de extrema izquierda». Sin las leves queda 1 a 0 y no llega. La fiscalización es pareja: 4 piezas al Gobierno Petro y 6 al de De la Espriella (3 solas y 3 dentro de piezas I). Rama de la precisión: **cumple mínimos → valor del barrido, con tope ±0,30.** **Valor propuesto: −0,10.** Alternativa: 0,00 con evidencia |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas, los
> títulos literales, el fragmento y el método están aquí para eso. **La
> clasificación de cada pieza es el juicio de un solo lector.** Lo que decide
> el resultado es una sola pregunta, y se declara en §5: si «ultraderechista»
> en voz de la casa es un rótulo o una clasificación descriptiva.

---

## 1. Método

- **robots.txt** de `es.euronews.com`, descargado el 2026-10-12 con el User-Agent de abajo (HTTP 200). El bloque `User-agent: *` veta `/api/`, `/login`, `/register`, rutas técnicas (`/modules`, `/plugin`, `/src`, `/lib`…) y la paginación del tiempo; un bloque titulado `# ai bots allowed` repite esas reglas con `Allow: /` para OAI-SearchBot, ChatGPT-User, PerplexityBot y otros; y otro titulado `# ai bots disallowed` dice, literal:

  ```
  User-agent: GPTBot
  User-agent: CCBot
  Disallow: /
  ```

  **No nombra a ClaudeBot, Claude-Web ni anthropic-ai**, así que les rige `User-agent: *`. Las rutas usadas (`/sitemap/…` y las páginas de artículo `/AAAA/MM/DD/…`) no están vetadas. Anuncia trece sitemaps, entre ellos `/sitemap/articles.xml` y `/sitemap/ai-translated.xml`.
- **User-Agent honesto en todas las peticiones:** `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. Nunca el de un navegador. Cliente: `curl -sS --ssl-no-revoke`, una petición a la vez, 1,6 s de pausa después de cada una. 139 peticiones en total.
- **Solo fuentes del propio medio.** Ningún buscador, ningún archivo de terceros. No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. No hay muro de pago.
- **Cómo se armó el universo.**
  1. `/sitemap/articles.xml` es un índice de sitemaps mensuales. Se bajaron los 13 de octubre de 2025 a octubre de 2026 (`articles-AAAA-MM.xml`): **17.895 URL únicas, 17.439 dentro de la ventana.**
  2. Filtro por la URL (el *slug* resume el titular): `colombi`, `petro` (sin `petroleo`/`petrol`), `espriella`, `cepeda`, `bogota`, `farc`, `eln`, `paloma-valencia`, `fajardo`, `uribe`, `medellin`, `cali-`, `cartagena`. Quedaron **130 URL**.
  3. Se quitaron a mano 17 que no tratan de Colombia ni de su política (una de petroquímicas rusas; crónicas de sucesos en España con víctimas o detenidos colombianos; turismo; cine; arte; mercenarios en Ucrania). Quedaron **113**, que se bajaron todas (HTTP 200).
  4. De cada página se sacó el título (`og:title`), la entradilla (`og:description`), la fecha (`datePublished`), el autor y el **cuerpo completo** (`articleBody` del JSON-LD). Todas traían cuerpo.
- **Traducciones automáticas.** El sitio publica un sitemap de piezas «ai-translated»: **11.041 de las 17.439 piezas de la ventana son traducciones automáticas** de otras ediciones de Euronews. Todas están también en los sitemaps de artículos. Entre las 113 de Colombia hay 12; de las clasificadas con postura, 2 (se marcan en la tabla). El resultado no depende de ellas.
- **Voz de la casa.** Euronews no publica editoriales sobre Colombia. Casi todas las piezas van firmadas por periodistas de la cadena (en 4 no consta autor); no hay columnas de terceros entre las 113. Por eso cuentan **el titular, la entradilla y el cuerpo en lo que no se atribuye a una fuente**. Lo que va entre comillas o se atribuye («según…», «afirmó…», los analistas consultados) no es voz de la casa.
- **Clases** (las de los barridos de NTN24 y KienyKe):
  - **I, dirección izquierda (cuenta):** en voz propia, encuadre desfavorable o rótulo descalificador del candidato, presidente electo o presidente De la Espriella, o de la derecha que lo apoya, que va más allá de fiscalizar un acto; o elogio de Petro, Cepeda o su campo. **I leve:** lo mismo con menos carga, en particular el **rótulo ideológico asimétrico** («ultraderechista», «extrema derecha», «derecha populista») cuando el campo contrario recibe solo «izquierdista». Es el criterio con el que se contó «ultraderecha» como rótulo en los barridos de Revista RAYA, Noticias RCN y Cuestión Pública.
  - **D, dirección derecha (cuenta):** lo simétrico. **D leve**, con menos carga.
  - **M, mixta:** postura repartida. No suma.
  - **F, fiscalización de quien gobierna:** crítica en voz propia a un acto del gobierno vigente. Se declara y **no cuenta** (polo fijo y precisión del 2026-10-09). Si una pieza fiscaliza y además rotula, cuenta por el rótulo y se dice.
  - **X, sin postura en voz propia:** informativa, o con la postura atribuida. Se cuenta, no se lista.
- **Descargas y scripts** en la carpeta temporal de la sesión, fuera del repositorio. No se publica el texto de ninguna pieza: solo títulos y fragmentos breves como evidencia.

---

## 2. Cobertura y huecos

| | Piezas sobre Colombia | Con postura (I, D, M) | Fiscalización (F) | X |
|---|---:|---:|---:|---:|
| Antes del 07-08-2026 | 71 | 15 | 4 | 52 |
| Desde el 07-08-2026 | 42 | 7 | 3 | 32 |
| **Total** | **113** | **22** | **7** | **84** |

Por mes: oct-2025 3 (desde el 12), nov 7, dic 4, ene-2026 8, feb 2, mar 10, abr 11, may 6, jun 14, jul 5, ago 29 (el terremoto del 10-08 se lleva 16), sep 14, oct-2026 0 (hasta el 12).

**Huecos que se declaran:**
- **El filtro es por URL, y los *slugs* de Euronews se cortan hacia los 90 caracteres.** Una pieza sobre Colombia cuyo *slug* no nombre el país ni a ninguno de los términos se quedó fuera. Las piezas regionales que mencionan a Colombia de pasada (Venezuela, Ecuador, la política de Trump en el Caribe) solo entraron si el *slug* lo decía.
- **No se barrieron los vídeos, la emisión de televisión ni los boletines «Euronews Hoy»** más allá de los dos que entraron por el filtro (ninguno con postura).
- **Cobertura escasa.** 113 piezas en un año, y la mitad de las de agosto son del terremoto. El número lo deciden pocas piezas: es el coste que la ficha de CNN en Español anticipaba para los internacionales (refutación 3 de `fichas/cnn-es.md`).

---

## 3. Piezas clasificadas

Todas las URL son del sitio vivo, comprobadas el 2026-10-12. El título es el `og:title` de la página. «Cuerpo» quiere decir que el fragmento está en el texto de la pieza, no en el titular ni en la entradilla.

### 3.1 Antes del cambio, con postura (gobierna Petro)

| # | Fecha | Título literal | Fragmento en voz de la casa | Clase |
|---|---|---|---|---|
| 1 | 2026-04-27 | [26 atentados en 2 días: un nuevo ataque deja 20 muertos en Colombia](https://es.euronews.com/2026/04/27/un-atentado-en-la-carretera-panamericana-deja-20-muertos-en-colombia-farc-petro) | «el senador izquierdista Iván Cepeda, artífice de la controvertida política de Petro de negociar con grupos armados» (cuerpo) | D leve |
| 2 | 2026-05-25 | [Colombia: Comienzan las elecciones presidenciales en el exterior](https://es.euronews.com/2026/05/25/comienzan-elecciones-presidenciales-colombianas-voto-exterior) | «un abogado millonario de extrema derecha», «el movimiento de ultraderecha Defensores de la Patria», «El opositor ultra»; el perfil de Cepeda, en cambio, es elogioso («una trayectoria política marcada por la defensa de las víctimas») | I leve |
| 3 | 2026-05-26 | [Elecciones presidenciales en Colombia: los expatriados ya pueden votar](https://es.euronews.com/2026/05/26/comienzan-las-presidenciales-en-colombia-los-expatriados-ya-pueden-votar) | Entradilla: «dos candidatos de la derecha y la extrema derecha»; cuerpo: «el ultraderechista Abelardo de la Espriella» frente a «el izquierdista Iván Cepeda» (traducción automática de otra edición) | I leve |
| 4 | 2026-05-28 | [Elecciones en Colombia: ¿Quienes son los candidatos a la presidencia?](https://es.euronews.com/2026/05/28/elecciones-en-colombia-quienes-son-los-principales-candidatos-a-la-presidencia) | Entradilla: «el candidato ultraderechista»; perfil de Cepeda en tono favorable («el huérfano del militante asesinado que ha sacudido las encuestas») | I leve |
| 5 | 2026-05-29 | [Elecciones en Colombia: 5 claves de la campaña](https://es.euronews.com/2026/05/29/elecciones-en-colombia-5-claves-de-unas-elecciones-decisivas-para-la-region) | Entradilla: «el auge de nuevos discursos populistas»; cuerpo, en voz propia: «el discurso de la nueva derecha populista» | I leve |
| 6 | 2026-06-01 | [El aliado de Trump toma ventaja en Colombia: habrá segunda vuelta](https://es.euronews.com/2026/06/01/elecciones-colombia-de-la-espriella-desafia-cepeda-proyecto-petro) | De la Espriella, «derechista», «admirador de Donald Trump», «se hace llamar 'El Tigre'»; Cepeda, con «un complicado plan para lograr la "paz total"» (traducción automática de otra edición) | M |
| 7 | 2026-06-11 | [Cepeda denunciará a De la Espriella por vínculos con paramilitares](https://es.euronews.com/2026/06/11/cepeda-denunciara-a-de-la-espriella-por-presuntos-vinculos-con-paramilitares-en-colombia) | Cuerpo: «su rival, el ultraderechista Abelardo de la Espriella» | I leve |
| 8 | 2026-06-21 | [Petro descarta volver a presentarse a las elecciones presidenciales](https://es.euronews.com/2026/06/21/petro-descarta-volver-a-presentarse-a-unas-elecciones-presidenciales-en-colombia) | Entradilla: «entre el ultraderechista De la Espriella y el izquierdista Cepeda» | I leve |
| 9 | 2026-06-22 | [La derecha recupera Colombia: De la Espriella gana las elecciones](https://es.euronews.com/2026/06/22/de-la-espriella-se-hace-con-la-presidencia-de-colombia-por-el-margen-mas-estrecho-de-la-hi) | Entradilla: «El abogado ultraderechista derrota a Iván Cepeda» | I leve |
| 10 | 2026-06-22 | [Quién es Abelardo de la Espriella, el nuevo presidente de Colombia](https://es.euronews.com/2026/06/22/abelardo-de-la-espriella-de-abogado-de-clientes-incomodos-a-presidente-de-colombia) | Entradilla: «discurso patriótico, mano dura contra el crimen y desprecio a la política tradicional»; cuerpo: «clientes tan controvertidos», «bebe del mismo manual que Nayib Bukele […] o Donald Trump […], a quien admira sin disimulo» | I leve |
| 11 | 2026-06-23 | [El efecto Trump conquista América: por qué la derecha no para de ganar](https://es.euronews.com/2026/06/23/bolsonaro-bukele-fujimori-espriella-trump-auge-derecha-america-latina) | Cuerpo: «un discurso nacionalista, un populismo sin complejos y, sobre todo, un claro modelo a seguir: Donald Trump»; subtítulo «¿Doctrina 'Donroe' o simple injerencia política?» | I leve |
| 12 | 2026-06-24 | [Cepeda reconoce la victoria de De la Espriella en Colombia](https://es.euronews.com/2026/06/24/cepeda-reconoce-la-victoria-de-de-la-espriella-en-colombia-es-el-nuevo-presidente) | Cuerpo: «aplicar un programa de corte conservador y ultraderechista» | I leve |
| 13 | 2026-06-24 | [Petro pide invalidar las elecciones en Colombia por el apoyo de Trump](https://es.euronews.com/2026/06/24/petro-pide-anular-las-elecciones-de-colombia-por-la-injerencia-de-trump-a-favor-de-de-la-e) | Entradilla: «las elecciones ganadas por la ultraderecha» | I leve |
| 14 | 2026-07-06 | [De la Espriella amenaza a Petro con denuncias por presunta corrupción](https://es.euronews.com/2026/07/06/de-la-espriella-anuncia-querellas-sin-pruebas-contra-petro-por-presunta-corrupcion) | Titular: «amenaza»; entradilla: «El político de ultraderecha»; cuerpo: «Trump, en una nueva injerencia durante un proceso electoral extranjero», «Su valido en Colombia». La URL (`querellas-sin-pruebas`) muestra un titular anterior más duro | I |
| 15 | 2026-07-14 | [Secuestro masivo en Colombia: el ELN captura a 39 personas](https://es.euronews.com/2026/07/14/el-eln-secuestra-dos-autobuses-con-unos-39-pasajeros-en-el-choco-colombiano) | Cuerpo: «la victoria del ultraderechista Abelardo de la Espriella» | I leve |

### 3.2 Desde el cambio, con postura (gobierna De la Espriella)

| # | Fecha | Título literal | Fragmento en voz de la casa | Clase |
|---|---|---|---|---|
| 1 | 2026-08-12 | [Colombia recibirá ayuda foránea tras la inacción inicial del Gobierno](https://es.euronews.com/2026/08/12/de-la-espriella-rectifica-colombia-recibira-ayuda-internacional) | Entradilla: «el nuevo Gobierno de extrema derecha»; cuerpo: «la entente de la derecha populista que protagonizan Bukele o De la Espriella». La crítica a la respuesta al terremoto («inacción inicial») es fiscalización y no cuenta; cuenta el rótulo | I leve |
| 2 | 2026-08-13 | [Colombia autoriza a EE.UU. a operar militarmente en su territorio](https://es.euronews.com/2026/08/13/colombia-autoriza-a-eeuu-a-operar-militarmente-en-su-territorio-contra-el-narcoterrorismo) | Cuerpo: «el abogado ultraderechista Abelardo de la Espriella» | I leve |
| 3 | 2026-08-14 | [72 horas tras el terremoto colombiano: 379 desaparecidos y 281 muertos](https://es.euronews.com/2026/08/14/72-horas-tras-el-terremoto-de-colombia-379-personas-continuan-desaparecidas) | Cuerpo: «El recién estrenado ejecutivo del abogado ultraderechista» | I leve |
| 4 | 2026-08-19 | [Colombia cifra en 8.264 millones el daño provocado por el terremoto](https://es.euronews.com/2026/08/19/de-la-espriella-cifra-en-8264-millones-de-euros-el-dano-provocado-por-el-terremoto) | Cuerpo: «El presidente ultraderechista aseguró haber utilizado una empresa privada […] pero no reveló sus fuentes» (lo segundo es fiscalización) | I leve |
| 5 | 2026-08-20 | [Colombia declara el estado de emergencia en 15 departamentos](https://es.euronews.com/2026/08/20/de-la-espriella-declara-el-estado-de-emergencia-en-colombia) | Cuerpo: «La medida permite al presidente ultraderechista sortear que el Congreso […] vote» (lo segundo es fiscalización) | I leve |
| 6 | 2026-08-31 | [Colombia lanza una operación en Guaviare para capturar a Iván Mordisco](https://es.euronews.com/2026/08/31/espriella-lanza-operacion-disidencias-de-las-farc-colombia) | Cuerpo: «El presidente ultraderechista, cuyo Gobierno…» | I leve |
| 7 | 2026-09-08 | [Rubio comienza en Colombia su gira sudamericana por países afines](https://es.euronews.com/2026/09/08/marco-rubio-comienza-en-colombia-su-gira-sudamericana-por-paises-ideologicamente-afines) | Entradilla: «la victoria del ultraderechista Abelardo de la Espriella»; cuerpo: «mandatarios de ultraderecha sudamericanos» | I leve |

### 3.3 Fiscalización de quien gobierna (se declara, no cuenta)

| # | Fecha | Título literal | Fragmento en voz de la casa | Clase |
|---|---|---|---|---|
| 1 | 2025-11-20 | [Petro responde al escándalo por su visita a un prostíbulo en Lisboa](https://es.euronews.com/2025/11/20/gustavo-petro-responde-al-escandalo-por-su-visita-a-un-burdel-en-lisboa-aprendi-a-no-compr) | Petro gobierna. Titular: «Petro responde al escándalo por su visita a un prostíbulo en Lisboa» | F |
| 2 | 2026-04-24 | [Petro protagoniza la primera visita de un jefe de Gobierno a Delcy](https://es.euronews.com/2026/04/24/gustavo-petro-protagoniza-la-primera-visita-de-un-jefe-de-gobierno-a-delcy-rodriguez) | Petro gobierna. Entradilla: «otorga legitimidad a la presidenta venezolana no electa» | F |
| 3 | 2026-06-21 | [Colombia elige presidente entre la mano dura y la apuesta por la paz](https://es.euronews.com/2026/06/21/segunda-vuelta-elecciones-colombia-de-la-espriella-cepeda) | Petro gobierna. Cuerpo: «El presidente Gustavo Petro puso en duda esos resultados sin aportar pruebas». El titular («entre la mano dura y la apuesta por la paz») no toma partido | F |
| 4 | 2026-07-07 | [Abelardo de la Espriella acusa a Petro de orquestar un golpe de Estado](https://es.euronews.com/2026/07/07/presidente-electo-colombia-acusa-petro-impulsar-golpe-de-estado) | Petro gobierna. Cuerpo: «aunque no presentó pruebas que respalden sus afirmaciones» | F |
| 5 | 2026-09-04 | [De la Espriella posa con los cuerpos de 4 presuntos narcoterroristas](https://es.euronews.com/2026/09/04/espriella-cadaveres-de-presuntos-narcoterroristas-abatidos) | De la Espriella gobierna. Titular: «De la Espriella posa con los cuerpos de 4 presuntos narcoterroristas» | F |
| 6 | 2026-09-24 | [Colombia: Controvertida presencia de tropas de EE.UU. en Tumaco](https://es.euronews.com/2026/09/24/colombia-justicia-pide-explicaciones-ministro-defensa-presencia-tropas-eeuu-tumaco) | De la Espriella gobierna. Titular: «Controvertida presencia de tropas de EE.UU. en Tumaco» | F |
| 7 | 2026-09-30 | [El Gobierno de Colombia cambia las reglas de las protestas: qué cambia](https://es.euronews.com/2026/09/30/colombia-nuevas-reglas-protestas-policia-decreto) | De la Espriella gobierna. Subtítulo: «¿Por qué es controvertido?» (las nuevas reglas de protesta) | F |

Además, tres piezas I de §3.2 (n.º 1, 4 y 5) fiscalizan al Gobierno De la Espriella en lo que no es rótulo: la «inacción inicial» ante la ayuda internacional, la cifra de daños sin fuentes y el estado de emergencia que «permite sortear» al Congreso.

---

## 4. Números

| | I | I leve | D | D leve | M | Con postura | F (no cuenta) |
|---|---:|---:|---:|---:|---:|---:|---:|
| Antes del 07-08-2026 | 1 | 12 | 0 | 1 | 1 | 15 | 4 |
| Desde el 07-08-2026 | 0 | 7 | 0 | 0 | 0 | 7 | 3 |
| **Total** | **1** | **19** | **0** | **1** | **1** | **22** | **7** |

- **Proporción I:D = 20 a 1.** **Sin las leves, 1 a 0**: no llega a 10 piezas ni a 3 por lado.
- **Sin las 2 traducciones automáticas** (n.º 3 y 6 de §3.1): 19 a 1. No cambia nada.
- **Con el polo fijo:**
  - **Con Petro en el poder**, la casa lo fiscaliza en voz propia 4 veces («el escándalo» de Lisboa, la visita a Delcy Rodríguez que «otorga legitimidad a la presidenta venezolana no electa», sus acusaciones de fraude «sin aportar pruebas» y «aunque no presentó pruebas»). Lo llama «izquierdista» y «el primer presidente de izquierdas del país», nunca con un rótulo de extremo.
  - **Con De la Espriella en el poder**, lo fiscaliza en voz propia 6 veces (las 3 de §3.3 y las 3 que van dentro de piezas I). Es la misma conducta que con Petro, algo más frecuente. **No lo celebra ni lo disculpa en ninguna pieza**, y tampoco rotula al gobierno anterior.
  - **Lo asimétrico es el rótulo.** Desde la campaña, la casa llama a De la Espriella «ultraderechista», «de extrema derecha», «opositor ultra», y sitúa su movimiento en «la nueva derecha populista»; a Paloma Valencia la llama «derechista» (distingue grados en la derecha); a Petro y a Cepeda, «izquierdistas» o «progresistas». **El rótulo sigue igual cuando De la Espriella gobierna** («el presidente ultraderechista», 19-08, 20-08 y 31-08). Los perfiles de campaña tratan a Cepeda con simpatía («el huérfano del militante asesinado que ha sacudido las encuestas») y a De la Espriella con distancia («desprecio a la política tradicional», «clientes tan controvertidos», «admira sin disimulo» a Trump).
  - **La prueba del protocolo:** si el gobierno cambiara y el medio mantuviera la misma conducta, ¿cambiaría la clasificación? En la fiscalización, no: la conducta se mantuvo. En el léxico, sí: el rótulo de extremo va siempre al mismo lado.

---

## 5. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | Sí | Piezas firmadas por la redacción de la cadena; se cuenta solo lo no atribuido |
| 2. A los dos lados del cambio, en 12 meses | Sí, solo por el rótulo | La fiscalización es pareja; el rótulo asimétrico está a los dos lados (13 piezas antes, 7 después) |
| 3a. ≥10 piezas con postura | Sí, con las leves | 22 (2 sin las leves) |
| 3b. ≥3 a cada lado, sin contar la fiscalización | Sí, con las leves | Antes 15, después 7 (sin las leves: 2 y 0) |
| 3c. Proporción ≥3:1 | Sí | 20:1 (1:0 sin las leves) |
| 4. Contrapesos escritos | Sí | §7, con su peso |
| 5. Reproducible | Sí | §3: fecha, título literal, URL, fragmento y clase de cada pieza |

**La pregunta que decide el resultado.** Si «ultraderechista» en voz de la casa es un **rótulo** (como se contó en Revista RAYA, Noticias RCN y Cuestión Pública), el barrido cumple las cinco condiciones. Si es una **clasificación descriptiva** —es una etiqueta corriente en la prensa europea para De la Espriella, y Euronews distingue grados: llama «derechista» a Valencia y no a todo el campo—, las piezas I leves bajan a X, la postura no llega a los mínimos y lo que queda es la misma fiscalización con los dos gobiernos: **0,00 con evidencia**. Este barrido aplica el criterio de los barridos anteriores, para que no haya una regla para los medios colombianos y otra para los extranjeros, y deja la alternativa escrita.

**Rama de la precisión del 2026-10-10:** el +0,05 vigente se apoya solo en los niveles 4 y 5, así que el barrido manda. Con el criterio de los barridos anteriores **cumple mínimos → valor del barrido, con el tope de ±0,30**. No se levanta el tope:
- **No hay endoso explícito.** Euronews no pidió el voto por nadie ni declaró apoyo en su voz.
- **No hay nivel 1 con posición conocida.** El dueño (Alpac Capital) está documentado como fondo de inversión; el vínculo con un asesor de Orbán que señaló RFE/RL se consigna como señalamiento, no como posición, y en todo caso apuntaría al lado contrario de lo que muestran las piezas.

## 6. Lo que se declara y no cuenta

- **La selección de fuentes y de temas.** Los analistas consultados en las piezas de campaña (Pares y otros) y la elección de temas (el terremoto, la violencia, la relación con EE. UU.) no se midieron.
- **Lo que no es Gobierno nacional colombiano:** el «autoritario Daniel Noboa» (08-09), el «ultraderechista» Kast (28-05), la política antidrogas de Trump («fuerza letal», 15-09). Se ven en las mismas piezas y apuntan en la misma dirección, pero quedan fuera del eje que mide este barrido.
- **Las traducciones automáticas** (§1): voz de la casa, porque la cadena las publica como suyas, pero escritas en otra edición.

## 7. Contrapesos y su peso

- **Fiscalización simétrica.** La casa fiscaliza a Petro mientras gobierna (4 piezas) y a De la Espriella cuando gobierna (6). **Peso alto sobre la magnitud:** es la conducta que el polo fijo pide y la que sostendría un 0,00.
- **Euronews gradúa el rótulo.** Valencia es «derechista»; el Centro Democrático, «el principal partido de la oposición»; De la Espriella, «ultraderechista». Es una etiqueta corriente en la prensa europea y española para De la Espriella (no se comprobó en este barrido, que no leyó otros medios). **Peso medio:** explica el rótulo, pero no lo hace simétrico, porque nadie de la izquierda recibe el grado equivalente.
- **Una pieza D leve y una M** contra el campo de Petro («la controvertida política de Petro de negociar con grupos armados», 27-04; «un complicado plan para lograr la "paz total"», 01-06). **Peso bajo.**
- **Coberturas factuales sin carga** de los dos gobiernos: la reunión Petro-Trump («el tono interno del encuentro fue sorprendentemente positivo», 03-02), la investidura (07-08), las operaciones contra las disidencias (10-08, 27-08, 31-08), el levantamiento de la suspensión del porte de armas (08-09). **Peso bajo:** muestran que la casa no rotula todo.
- **Lo que el barrido no ve:** las piezas que el filtro dejó fuera, los vídeos y la emisión.

## 8. Valor propuesto

**−0,10**, orientación mixta con leve inclinación a la izquierda, como **juicio declarado**:
- **La dirección existe pero es tenue.** 20 a 1 con las leves; 1 a 0 sin ellas. La magnitud no puede ir al tope (±0,30), que es para direcciones que se sostienen sin las leves (NTN24, 32 a 0 sin ellas). Tampoco a −0,25, donde quedaron Volcánicas (cumplía solo con las leves, pero sus leves eran encuadres de fondo y no una etiqueta) y El País de España.
- **Frente a los internacionales vecinos:** DW y BBC Mundo (−0,05), France 24 y EFE (0,00), El País y The New York Times (−0,25), todos firmados el 2026-10-10 sin barrido. Euronews quedaría entre DW/BBC y El País, más cerca de los primeros, que es donde lo pone una asimetría que es sobre todo léxica.
- **Ante la duda entre bandas, la más cercana a la mixta:** −0,10 sigue dentro de la banda mixta (−0,20 a +0,20).
- **Antes y después:** de **+0,05** (sin piezas) a **−0,10** (con 22 piezas con postura). Cambia de signo.
- **Alternativa: 0,00 con evidencia**, si la dirección editorial decide que «ultraderechista», en un medio que gradúa los rótulos de la derecha, es una clasificación y no un rótulo. Entonces la postura no llega a los mínimos y la fiscalización es pareja (4 y 6 piezas, ≥3 a cada lado): la misma conducta con los dos gobiernos. Si se elige esta vía, conviene revisar con el mismo criterio los barridos que contaron «ultraderecha» como rótulo.
- **Qué lo movería:** que la casa siga llamando «ultraderechista» al presidente en piezas sin relación con su ideología (como el 31-08) o que aparezcan encuadres de fondo y no solo el rótulo lo acercaría a −0,20; que el rótulo se gradúe también a la izquierda, o desaparezca con el ejercicio del gobierno, lo devolvería al 0,00.
- **Ficha técnica:** se crea, mínima, en `fichas/euronews-es.md`, sin valor nuevo. **No se toca el registro (`shared/mediaRegistry.js`), ni el perfil de propiedad, ni el texto público** (`shared/resumenesPublicos/euronews-es.js`): eso queda para después de la firma.
