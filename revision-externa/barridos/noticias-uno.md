# Barrido editorial: Noticias Uno

| | |
|---|---|
| **Medio** | Noticias Uno (`noticias-uno`), noticiero de televisión de NTC Televisión, por Cablenoticias. Publica en ráfagas los fines de semana |
| **Valor vigente** | **−0,40** (`shared/mediaRegistry.js`, `reviewedAt: '2026-10-10'`, firma en bloque). La razón escrita es «treinta años de fiscalización a gobiernos sucesivos —Uribe, Santos, Duque—… esa vigilancia al establecimiento lo sitúa a la izquierda». La ficha dice que eso es historia y un razonamiento que el polo fijo descarta, y que «la evidencia disponible apunta a 0,00». Su nivel 2 está vacío y la propiedad no está documentada: **el valor solo se apoya en los niveles 4 y 5** |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus precisiones y la del 2026-10-10. Se lee junto con la regla del polo fijo |
| **Ventana** | 2025-10-11 → 2026-10-11 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-11. Es de la misma casa que el autor de la ficha: su acuerdo no es aval |
| **Estado** | **FIRMADO el 2026-10-12: −0,30** (antes −0,40). **No es el valor que proponía este barrido** («sin medir», con la tensión hacia la izquierda), sino la lectura alternativa de su §6 y §8.3. Aplicado en el registro, la ficha y el texto público (`DECISIONES.md`, 2026-10-12). Lo que más abajo dice «propuesta» o «pendiente de firma» es el estado anterior a la firma y se conserva como historia |
| **Decisión del responsable editorial** | −0,30, el máximo que sostiene la lectura alternativa que cuenta las piezas leves posteriores al cambio (la fiscalización «con tono» del §6, sensibilidad), por su conocimiento del contexto mediático. **Queda declarada la fragilidad:** 0 piezas con postura clara después del 07-08-2026. El recuento de diciembre de 2026 y febrero de 2027 del §8.5 sigue en pie |
| **Resultado** | **No cumple los mínimos, y la dirección es clara.** Antes del cambio hay 40 piezas con postura: 31 a la izquierda (19 claras y 12 leves), 2 leves a la derecha y 7 mixtas, todas en la campaña presidencial. Después del cambio hay **0 piezas con postura que cuenten**: 17 fiscalizan al gobierno De la Espriella y 3 a la izquierda que salió o pasó a la oposición. **Rama de la precisión del 2026-10-10: «dirección clara sin mínimos» → «sin medir» (`bias: null`), con la tensión hacia la izquierda declarada.** Ninguna lectura del barrido sostiene el −0,40 |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas, los títulos
> y el criterio están aquí para eso. **La clasificación de cada pieza es el
> juicio de un solo lector**, y ese lector solo leyó texto: títulos y
> entradillas. **No vio ningún vídeo** (ver §3).

---

## 1. Método

- **robots.txt** de `www.noticiasuno.com`, descargado el 2026-10-11 antes de cualquier otra petición. Es el bloque de Yoast: `User-agent: *`, `Disallow:` vacío y `Sitemap: https://www.noticiasuno.com/sitemap_index.xml`. No excluye a ningún agente ni ninguna ruta.
- **User-Agent honesto** en todas las peticiones: `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. No se suplantó a ningún navegador. Ningún servidor rechazó una petición: todas respondieron `200`.
- **Ritmo:** 2 s de pausa entre peticiones. En total fueron 31: robots.txt, el índice de sitemaps, seis sitemaps (`post-sitemap11` a `14`, `post-sitemap` y `category-sitemap`), la lista de categorías, una prueba y 21 páginas de la API.
- **Fuente:** solo el propio medio. Se usaron los sitemaps para delimitar el archivo y la API pública de WordPress del sitio para el texto: `/wp-json/wp/v2/posts?after=2025-10-11T00:00:00&before=2026-10-12T00:00:00&per_page=100&orderby=date&order=asc`, con `_fields=id,date,link,title,categories,tags,content,excerpt,author`. La API da **2.056 piezas** en la ventana (cabecera `X-WP-Total`), de la primera, del 2025-10-11, a la última, del 2026-10-10. La fecha es el campo `date` de WordPress.
- **No se tocaron** eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. No se usó ningún buscador.
- **Copia local:** fuera del repositorio, en una carpeta de descargas de la sesión. No se ejecutó nada desde ella.
- **Qué se leyó.** Título y entradilla (el campo `content`, que en este medio es un párrafo de presentación del vídeo) de **813 piezas**: todas las que en el título o la entradilla nombran a Petro, De la Espriella, Cepeda, el Gobierno, el presidente, los ministros, la Casa de Nariño, el Pacto Histórico o «el tigre» (450); todas las que nombran a otros candidatos, partidos o «la derecha»/«la izquierda» (106); todas las de las secciones de voz propia del noticiero (Qué Tal Esto, Top Secret, Noticias Uno al Aire, Reporte Coronell, Elecciones 2026 y Primicia), y **todas** las publicadas después del cambio fuera de Emisiones, Internacional y Deportes. Las 1.243 restantes son internacionales, de deportes, de economía de servicio, crónica local o las 120 «Emisiones» (el programa entero, en vídeo), y no se leyeron una a una.
- **Voz de la casa.** El noticiero no publica editoriales. Lo que aquí cuenta como voz de la casa:
  1. **los títulos y entradillas que no atribuyen la tesis a una fuente**;
  2. **las secciones de comentario propio:** «Qué Tal Esto», la denuncia irónica de cierre, y «Top Secret, la vida secreta de los famosos», la sátira política del domingo. Son de la casa y no van firmadas. Top Secret es sátira, así que se cuenta aparte y el recuento se da también sin ella (§4).
- **Lo que no es voz de la casa y no cuenta:** lo atribuido («dice», «según», «denuncian»), las piezas que solo retoman la columna de Daniel Coronell en otro medio y el «Reporte Coronell» (3 piezas, julio de 2026); los formatos de tiempo igual, «Proyecto Uno» (un minuto para cada candidato, 11 piezas) y «De lado y lado» (dos voces enfrentadas, 14 piezas); los segmentos con marca de Bancolombia (96 piezas), y las piezas de la Procuraduría y de la Gobernación de Cundinamarca con tono de comunicado (§3).
- **Clases** (las mismas que en los barridos de Razón Pública y Vorágine):
  - **I**, dirección izquierda (cuenta): un rótulo descalificador en voz propia contra la derecha o sus candidatos, o un elogio, una disculpa o una defensa de la izquierda, sus candidatos o el gobierno Petro. **I-leve:** lo mismo, pero solo por encuadre (la elección del título o el contraste), sin rótulo explícito.
  - **D / D-leve**, dirección derecha (cuenta): lo simétrico.
  - **M**, mixta: postura repartida entre los dos lados en la misma pieza. No suma a ninguna dirección.
  - **F**, solo fiscaliza a quien manda: a Petro hasta el 06-08 y a De la Espriella desde el 07-08. Se declara y no suma (polo fijo; primera precisión del 2026-10-09). «Con tono» marca la fiscalización con un adjetivo propio («empecinado», «presupuesto milagro»): sigue siendo F, pero se mide en la sensibilidad del §6.
  - **Fo**, fiscaliza a la oposición o al gobierno que ya salió. No suma, pero es contrapeso.
  - **Fc**, fiscaliza a un candidato (antes del cambio). No suma pieza a pieza. Se cuenta por destinatario, porque la asimetría entre candidatos es justo lo que el polo fijo deja ver.
  - **X**, fuera: atribuido, sin postura en el eje, internacional o local.

---

## 2. Cobertura

| | Antes del cambio (2025-10-11 → 2026-08-06) | Después (2026-08-07 → 2026-10-11) |
|---|---:|---:|
| Piezas en la ventana (API) | 1.812 | 244 |
| Leídas con entradilla | 592 | 221 |
| Qué Tal Esto | 54 | 5 |
| Top Secret | 40 | **0** (la última es del 2026-08-02) |
| Proyecto Uno / De lado y lado | 11 / 14 | 0 / 0 |
| Piezas de la Procuraduría (título o entradilla) | 13 | 11 |

**783 de las 2.056 piezas no traen texto**: el campo `content` llega vacío y solo está el vídeo. Entre las 813 leídas, son 258. En esas solo queda el título, y así se marca en la tabla («Sin texto: solo vídeo»).

---

## 3. Huecos y limitaciones

1. **No se vio ningún vídeo.** Noticias Uno es televisión: la voz del medio está en la locución, el montaje y el tono, y el sitio solo publica un título y una entradilla de dos o tres frases. Este barrido mide **la voz escrita de la casa**, que es una parte de su voz. Las 120 «Emisiones» (los programas enteros) no se abrieron.
2. **Después del cambio el material es corto y distinto.** Son dos meses (244 piezas, frente a 1.812 en diez meses). **Top Secret, la sección que más postura daba antes del cambio, no publica nada después del 2026-08-02**, y Qué Tal Esto pasa de 54 piezas a 5. No se sabe si el noticiero dejó de emitirlas o si solo dejó de subirlas al sitio. Con eso, «0 piezas con postura después» es un hecho del archivo, pero no prueba que el noticiero haya cambiado de tono.
3. **Hay un terremoto en la mitad del «después».** Desde el 10 de agosto una parte grande de la agenda es la emergencia. Eso desplaza la cobertura política.
4. **Hay conflictos en los que el medio es parte.** «Por decirle que tenía polvo, De la Espriella sacó casas de Ignacios Gómez del registro» (Qué Tal Esto, 2026-05-30) enfrenta al candidato con el director del noticiero. «Juan Daniel Oviedo redactó proyecto que sacaba a Noticias Uno de la industria de la televisión» (2026-03-15) enfrenta a otro candidato con el medio. Las dos están como Fc y no suman, pero explican parte de la temperatura.
5. **Daniel Coronell.** Varias piezas retoman su columna, y en julio de 2026 aparece la sección «Reporte Coronell por Noticias Uno». No cuentan como voz de la casa. Queda sin resolver si es accionista de NTC: la ficha dice que «no consta verificada», pero `shared/centinela.js` dice «tiene el 60,5 % de NTC Televisión», y `shared/mediaOwnership.js` todavía dice que «hoy es accionista de la revista Cambio (22 % en 2024)», cuando la ficha retiró ese vínculo el 2026-10-07. **Es una incoherencia del repositorio y no se toca aquí.** Si llegara a constar que el dueño mayoritario firma una sección propia, la pregunta de qué es voz de la casa cambiaría.
6. **Contenido de marca.** Los segmentos «– Bancolombia» (88 antes y 8 después) son contenido con marca, y no se leen como voz del noticiero. Las piezas de la Procuraduría después del cambio («Gracias a la intervención de la Procuraduría…», «Andesco reconoció labor del procurador…») tienen tono de comunicado. Son 11 en dos meses, frente a 13 en los diez anteriores. El Procurador no es el Gobierno nacional y estas piezas no entran en el eje, pero el patrón se deja anotado.
7. **El recorte por términos puede dejar fuera alguna pieza** que trate del Gobierno sin nombrarlo. Para reducir el riesgo, después del cambio se leyeron todas las piezas de las secciones nacionales.

---

## 4. Piezas clasificadas

Todas las URL son de `https://www.noticiasuno.com/`. El título es el literal de la API, sin el sufijo «| Noticias UNO». El «por qué» cita la entradilla cuando la hay.

### 4.1 Antes del cambio: piezas con postura (I, I-leve, D-leve, M)

| # | Fecha | Título literal | Sección | Clase | Por qué |
|---|---|---|---|---|---|
| 1 | 2025-11-15 | [Centro Democrático emprende campaña anticomunista](https://www.noticiasuno.com/politica/centro-democratico-emprende-campana-anticomunista-noticias-uno/) | politica | **I** | Encuadre propio: «los tradicionales voceros de la derecha comenzaron a adoptar un discurso de miedo al comunismo» |
| 2 | 2025-11-16 | [Marelvis en video de Petro// El aguardiente y la rata// Clase de masajes para pollo](https://www.noticiasuno.com/top-secret/marelvis-en-video-de-petro-el-aguardiente-y-la-rata-clase-de-masajes-para-pollo/) | top-secret | **M** | Sátira (Top Secret): Petro y el candidato Juan Manuel Galán |
| 3 | 2025-11-23 | [Champeta de bogotano// ¿dónde está el policía?// Ojos que no ven](https://www.noticiasuno.com/top-secret/champeta-de-bogotano-donde-esta-el-policia-ojos-que-no-ven-noticias-uno/) | top-secret | **M** | Sátira (Top Secret): el precandidato Mauricio Cárdenas y Petro |
| 4 | 2025-12-13 | [Colombia es la cuarta economía con mejor desempeño en 2025 según The Economist](https://www.noticiasuno.com/economia/colombia-es-la-cuarta-economia-con-mejor-desempeno-en-2025-segun-the-economist-noticias-uno/) | economia | **I-leve** | Elogio por encuadre: «The Economist que ha publicado duras críticas al gobierno Petro» |
| 5 | 2026-01-18 | [Ojo por ojo// Cepeda rezado// Las SS de Oviedo](https://www.noticiasuno.com/top-secret/ojo-por-ojo-cepeda-rezado-las-ss-de-oviedo-noticias-uno/) | top-secret | **M** | Sátira (Top Secret): «las aseguranzas indígenas para Iván Cepeda y las insignias por casualidad nazis en el outfit del candidato Juan Daniel Oviedo» |
| 6 | 2026-01-25 | [Espriella, de Tigre a oveja perdida// Autocrítica de Peñalosa// El pésame equivocado](https://www.noticiasuno.com/top-secret/espriella-de-tigre-a-oveja-perdida-autocritica-de-penalosa-el-pesame-equivocado-noticias-uno/) | top-secret | **I** | Sátira (Top Secret): «El excantante, ronero y candidato Espriella que se había declarado ateo» |
| 7 | 2026-02-01 | [Top Secret: Cacería humana en Colombia/ La copialina robada/ Los outfits del Pacto](https://www.noticiasuno.com/top-secret/top-secret-caceria-humana-en-colombia-la-copialina-robada-los-outfits-del-pacto-noticias-uno/) | top-secret | **D-leve** | Sátira (Top Secret): «el desfile de modas de los candidatos del Pacto Histórico» |
| 8 | 2026-02-07 | [Magistrados desorganizan las listas del Pacto Histórico](https://www.noticiasuno.com/politica/magistrados-desorganizan-las-listas-del-pacto-historico-noticias-uno/) | politica | **I** | Defensa del Pacto en voz propia: «las jugaditas de la posición mayoritaria de sus consejeros en un intento por invalidar sus candidaturas» |
| 9 | 2026-02-08 | [Cambio de Plan// El estartazo// Ayuda sobrenatural// La falsa víctima de Rodríguez](https://www.noticiasuno.com/top-secret/cambio-de-plan-el-estartazo-ayuda-sobrenatural-la-falsa-victima-de-rodriguez-noticias-uno/) | top-secret | **I-leve** | Sátira (Top Secret): «la ayuda sobrenatural que pide Uribe en la campaña» |
| 10 | 2026-02-21 | [Convocados a la marcha de defensa del salario mínimo se quedaron sin contradictores](https://www.noticiasuno.com/nacional/convocados-a-la-marcha-de-defensa-del-salario-minimo-se-quedaron-sin-contradictores-noticias-uno/) | nacional | **M** | Ironía repartida: la marcha de Petro «perdió a todos sus detractores» |
| 11 | 2026-03-07 | [Candidatura homófaba // alcalde con novia y esposa // candidato sin voto // tigre de contratación](https://www.noticiasuno.com/nacional/candidatura-homofaba-alcalde-con-novia-y-esposa-candidato-sin-voto-tigre-de-contratacion/) | nacional | **I** | Sátira (Top Secret): «Un tigre para contratar… y un cierre homofóbico de campaña» |
| 12 | 2026-03-14 | [Centro Democrático le deja la bandera antiderechos LGBTIQ+ a Abelardo de la Espriella](https://www.noticiasuno.com/politica/centro-democratico-le-deja-la-bandera-antiderechos-lgbtiq-a-abelardo-de-la-espriella-noticias-uno/) | politica | **I** | Rótulo en el título: «bandera antiderechos» |
| 13 | 2026-03-21 | [Paloma Valencia fue promotora de la adopción gay que ahora pide negar como derecho](https://www.noticiasuno.com/politica/paloma-valencia-fue-promotora-de-la-adopcion-gay-que-ahora-pide-negar-como-derecho-noticias-uno/) | politica | **I** | En voz propia: «La búsqueda de adhesiones políticas a la causa de negación de los derechos ya adquiridos» |
| 14 | 2026-03-22 | [Vice-Therian// Los verdes quemados// “mi guerra es otra”// Cumpleaños extenuante](https://www.noticiasuno.com/top-secret/vice-therian-los-verdes-quemados-mi-guerra-es-otra-cumpleanos-extenuante-noticias-uno/) | top-secret | **M** | Sátira (Top Secret): «El baile del vice therian, la selfie de los quemados» |
| 15 | 2026-03-29 | [A lo James// Cuentas de la lechera// Energúmeno// Las barbies de Angélica Lozano](https://www.noticiasuno.com/top-secret/a-lo-james-cuentas-de-la-lechera-energumeno-las-barbies-de-angelica-lozano-noticias-uno/) | top-secret | **M** | Sátira (Top Secret): el ministro de Hacienda y el presidente de Ecopetrol; «Angélica Lozano y sus barbies» |
| 16 | 2026-04-02 | [Uribe abrió en redes El minuto de Cepeda para acusarlo de terrorismo sin pruebas](https://www.noticiasuno.com/politica/uribe-abrio-en-redes-el-minuto-de-cepeda-para-acusarlo-de-terrorismo-sin-pruebas-noticias-uno/) | politica | **I** | Disculpa del candidato en voz propia: «acusarlo de terrorismo sin pruebas»; «no sustentado en fechas, personajes ni documentos» |
| 17 | 2026-04-03 | [Políticos del Pacto piden frenar la estigmatización de su dirigencia y militancia](https://www.noticiasuno.com/politica/politicos-del-pacto-piden-frenar-la-estigmatizacion-de-su-dirigencia-y-militancia/) | politica | **I** | La entradilla lo afirma por su cuenta: «señalar, sin fundamentos fácticos, a Iván Cepeda» |
| 18 | 2026-04-03 | [Top Secret: Sin neón chino// Infundio aplazado// Saludo aeroespacial](https://www.noticiasuno.com/top-secret/top-secret-sin-neon-chino-infundio-aplazado-saludo-aeroespacial/) | top-secret | **I** | Sátira (Top Secret): «Infundio aplazado»; «Álvaro Uribe tenía programada una seguidilla diaria de ataques a Iván Cepeda» |
| 19 | 2026-04-12 | [Cartel de la copialina// Therian en rifa no registrada// No comen M* sino manjares del Pacífico](https://www.noticiasuno.com/top-secret/cartel-de-la-copialina-therian-en-rifa-no-registrada-no-comen-m-sino-manjares-del-pacifico/) | top-secret | **I** | Sátira (Top Secret): «La rifa no autorizada del candidato therian»; «la IA en la fabricación de la amenaza a Paloma Valencia» |
| 20 | 2026-04-26 | [El tatuaje, la mona y las fotos, Therian en Centro Democrático, El sueño presidencial de Fajardo](https://www.noticiasuno.com/top-secret/el-tatuaje-la-mona-y-las-fotos-therian-en-centro-democratico-el-sueno-presidencial-de-fajardo/) | top-secret | **I-leve** | Sátira (Top Secret): las fotos de Uribe con Noboa, «otro therian en la campaña presidencial», «La lucha de Sergio Fajardo contra el sueño» |
| 21 | 2026-05-02 | [Firmantes de paz comienzan a ser dueños de sus parcelas](https://www.noticiasuno.com/nacional/firmantes-de-paz-comienzan-a-ser-duenos-de-sus-parcelas-noticias-uno/) | nacional | **I-leve** | Elogio por contraste: «Aunque en el gobierno de Iván Duque se establecieron los ETCR… sólo ahora» |
| 22 | 2026-05-17 | [Firme por la plata// El cliente del tigre// En casa de herrero](https://www.noticiasuno.com/top-secret/firme-por-la-plata-el-cliente-del-tigre-en-casa-de-herrero-noticias-uno/) | top-secret | **I** | Sátira (Top Secret): «Un militante abelardista que se declara Firme por la Plata, las recomendaciones de Paloma Valencia a Alex Saab» |
| 23 | 2026-05-23 | [Madre de las Falsos Positivos de Soacha fue la primera impulsora de la candidatura de Cepeda](https://www.noticiasuno.com/nacional/madre-de-las-falsos-positivos-de-soacha-fue-la-primera-impulsora-de-la-candidatura-de-cepeda/) | nacional | **I-leve** | Perfil favorable: «la primera persona que le pidió lanzarse a la presidencia» |
| 24 | 2026-05-24 | [Aclaración// Andrés Cepeda en primera// Rechazo de Frontino// Llamada en espera](https://www.noticiasuno.com/top-secret/aclaracion-andres-cepeda-en-primera-rechazo-de-frontino-llamada-en-espera-noticias-uno/) | top-secret | **I-leve** | Sátira (Top Secret): «La fallida visita de Álvaro Uribe a Segovia… y la espera de Paloma Valencia a Sergio Fajardo en el teléfono» |
| 25 | 2026-06-06 | [Retiro de la Constituyente, coqueteo a Fajardo desde sectores pro-Cepeda](https://www.noticiasuno.com/politica/retiro-de-la-constituyente-coqueteo-a-fajardo-desde-sectores-pro-cepeda-noticias-uno/) | politica | **D-leve** | «A pesar de su invisibilidad el comité de campaña de Iván Cepeda…» |
| 26 | 2026-06-07 | [Víctima y victimario en campaña// Cuentahuesos en la Casa Blanca// Firmes por la plata](https://www.noticiasuno.com/top-secret/victima-y-victimario-en-campana-cuentahuesos-en-la-casa-blanca-firmes-por-la-plata/) | top-secret | **I** | Sátira (Top Secret): «La adhesión de Carlos Ledher a la campaña therian» |
| 27 | 2026-06-13 | [Las maniobras golpistas de Gloria Arizabaleta](https://www.noticiasuno.com/politica/las-maniobras-golpistas-de-gloria-arizabaleta-noticias-uno/) | politica | **I** | Rótulo en el título, a favor del presidente de turno: «maniobras golpistas» |
| 28 | 2026-06-13 | [Arizabaleta, la oveja descarriada que traicionó a la bancada del Pacto](https://www.noticiasuno.com/politica/arizabaleta-la-oveja-descarriada-que-traiciono-a-la-bancada-del-pacto-noticias-uno/) | politica | **I-leve** | «traicionó» en el título; «oveja negra» va atribuido al Pacto |
| 29 | 2026-06-14 | [Debate imposible// Al águila y el tigre// El tigre de feria// Yo me llamo Cepeda](https://www.noticiasuno.com/top-secret/debate-imposible-al-aguila-y-el-tigre-el-tigre-de-feria-yo-me-llamo-cepeda-noticias-uno/) | top-secret | **I** | Sátira (Top Secret): «él águila americana montando al tigre de bengala» |
| 30 | 2026-06-15 | [Campaña de De la Espriella ya recibió la adhesión de “todos los de siempre”](https://www.noticiasuno.com/politica/campana-de-de-la-espriella-ya-recibio-la-adhesion-de-todos-los-de-siempre-noticias-uno/) | politica | **I** | Rótulo en el título: «todos los de siempre». Sin texto: solo vídeo |
| 31 | 2026-06-15 | [Al menos $18 mil millones de la “teta del Estado” en los bolsillos de De la Espriella](https://www.noticiasuno.com/politica/al-menos-18-mil-millones-de-la-teta-del-estado-en-los-bolsillos-de-de-la-espriella-noticias-uno/) | politica | **I** | Rótulo en el título: «la "teta del Estado" en los bolsillos de De la Espriella». Sin texto: solo vídeo |
| 32 | 2026-06-15 | [Ataque a impuestos saludables es síntoma del acercamiento de Gillinski a campaña de De la Espriella](https://www.noticiasuno.com/economia/ataque-a-impuestos-saludables-es-sintoma-del-acercamiento-de-gillinski-a-campana-de-de-la-espriella/) | economia | **I-leve** | Interpretación propia en el título: «es síntoma del acercamiento de Gillinski a campaña de De la Espriella» |
| 33 | 2026-06-20 | [De la Espriella Style comenzó en la política en 2002, en Ralito](https://www.noticiasuno.com/politica/de-la-espriella-style-comenzo-en-la-politica-en-2002-en-ralito-noticias-uno/) | politica | **I** | Rótulo burlón en el título, el mismo día que el perfil de Cepeda («la causa»). Sin texto: solo vídeo |
| 34 | 2026-06-20 | [El barrio en el que nació la causa de Iván Cepeda](https://www.noticiasuno.com/politica/el-barrio-en-el-que-nacio-la-causa-de-ivan-cepeda-noticias-uno/) | politica | **I-leve** | Encuadre del título («la causa»), el mismo día que «De la Espriella Style… en Ralito». Sin texto: solo vídeo |
| 35 | 2026-06-20 | [Iván Cepeda el filósofo que renegó del comunismo](https://www.noticiasuno.com/politica/ivan-cepeda-el-filosofo-que-renego-del-comunismo-noticias-uno/) | politica | **I-leve** | El título responde al rótulo de «comunista» que le ponía la derecha. Sin texto: solo vídeo |
| 36 | 2026-06-28 | [Cambio de Meme// Firme por la Corte// Roce de pueblo// los procesados con el tigre](https://www.noticiasuno.com/top-secret/cambio-de-meme-firme-por-la-corte-roce-de-pueblo-los-procesados-con-el-tigre-noticias-uno/) | top-secret | **I** | Sátira (Top Secret): «los magistrados procesados en la manada del tigre» |
| 37 | 2026-06-29 | [Las cifras desmienten la tesis del voto-fusil de la derecha](https://www.noticiasuno.com/politica/las-cifras-desmienten-la-tesis-del-voto-fusil-de-la-derecha-noticias-uno/) | politica | **I** | Refutación en voz propia de «la tesis del voto-fusil de la derecha». Sin texto: solo vídeo |
| 38 | 2026-07-12 | [Como a perros en feria/ Los nazis de Valledupar/ Entre Platón y Diomedes/ Primera baja en la manada](https://www.noticiasuno.com/top-secret/como-a-perros-en-feria-los-nazis-de-valledupar-entre-platon-y-diomedes-primera-baja-en-la-manada/) | top-secret | **I-leve** | Sátira (Top Secret): «La primera baja en la manada del tigre» |
| 39 | 2026-07-13 | [Lucio organizaba sus denuncias desde 2024](https://www.noticiasuno.com/nacional/lucio-organizaba-sus-denuncias-desde-2024-noticias-uno/) | nacional | **I-leve** | Disculpa del presidente de turno: las denuncias contra Petro, «estrategia» de «desestabilización», con apoyo en un informe de inteligencia policial |
| 40 | 2026-07-26 | [Zoológico en el capitolio// Primera censura// El cuadro de Petro// Rosa Manuela y la espada](https://www.noticiasuno.com/top-secret/zoologico-en-el-capitolio-primera-censura-el-cuadro-de-petro-rosa-manuela-y-la-espada/) | top-secret | **M** | Sátira (Top Secret): «El primer censurado por De la Espriella» y «el trasteo de la Casa de Nariño» |

### 4.2 Antes del cambio: fiscalización del gobierno Petro (F)

| # | Fecha | Título literal | Sección | Clase | Por qué |
|---|---|---|---|---|---|
| 1 | 2025-10-13 | [Demanda pide que Benedetti devuelva lo devengado como embajador en la FAO](https://www.noticiasuno.com/politica/demanda-pide-que-benedetti-devuelva-lo-devengado-como-embajador-en-la-fao/) | politica | F | El ministro de Interior y el cargo en la FAO |
| 2 | 2025-11-09 | [Jefe de Sistemas de la Presidencia dice que él sale a manifestarse con la bandera del M19](https://www.noticiasuno.com/nacional/jefe-de-sistemas-de-la-presidencia-dice-que-el-sale-a-manifestarse-con-la-bandera-del-m19/) | nacional | F | «Las víctimas civiles han expresado su indignación»; entrevista del subdirector del noticiero |
| 3 | 2025-11-15 | [Eljach investiga a Benedetti y también por qué sigue quieto expediente contra la magistrada Lombana](https://www.noticiasuno.com/sin-categoria/eljach-investiga-a-benedetti-y-tambien-por-que-sigue-quieto-expediente-contra-la-magistrada-lombana/) | sin-categoria | F | El ministro de Interior, investigado |
| 4 | 2025-11-15 | [Siete menores de edad murieron en bombardeo de la Fuerza Aeroespacial en Calamar, Guaviare](https://www.noticiasuno.com/nacional/siete-menores-de-edad-murieron-en-bombardeo-de-la-fuerza-aeroespacial-en-calamar-guaviare/) | nacional | F | «El ministro de Defensa admitió el error» |
| 5 | 2025-11-23 | [Padre de niña bombardeada dice que le pidió buscarla al Ejército](https://www.noticiasuno.com/nacional/padre-de-nina-bombardeada-dice-que-le-pidio-buscarla-al-ejercito-noticias-uno/) | nacional | F | «nunca recibió apoyo del gobierno» |
| 6 | 2025-11-23 | [Ejecución del 50% en el Catatumbo; Gobierno dice que compromisos van en 68%](https://www.noticiasuno.com/economia/ejecucion-del-50-en-el-catatumbo-gobierno-dice-que-compromisos-van-en-68-noticias-uno/) | economia | F | La Contraloría frente a las cifras del Gobierno |
| 7 | 2025-12-13 | [Veinticinco mil colombianos desistieron de comprar casa por falta de subsidios](https://www.noticiasuno.com/economia/veinticinco-mil-colombianos-desistieron-de-comprar-casa-por-falta-de-subsidios-noticias-uno/) | economia | F | Suspensión de los subsidios de vivienda |
| 8 | 2025-12-18 | [Exministros irán a la cárcel por corrupción](https://www.noticiasuno.com/noticias-uno-al-aire/exministros-iran-a-la-carcel-por-corrupcion-noticias-uno/) | noticias-uno-al-aire | F | Sección «Noticias Uno al aire». Sin texto: solo vídeo |
| 9 | 2026-01-10 | [Petro cambió el discurso por la soberanía y sacó a la canciller de la manifestación](https://www.noticiasuno.com/nacional/petro-cambio-el-discurso-por-la-soberania-y-saco-a-la-canciller-de-la-manifestacion-noticias-uno/) | nacional | F | «desde allí tuvo que salir la canciller para atenderla» |
| 10 | 2026-01-11 | [Petrico y Trumpito// que nos cojan persignados// Traducciones de HP](https://www.noticiasuno.com/top-secret/petrico-y-trumpito-que-nos-cojan-persignados-traducciones-de-hp-noticias-uno/) | top-secret | F | Sátira (Top Secret) del presidente de turno, a la par de Trump |
| 11 | 2026-02-01 | [Funcionaria del DAPRE habla de la incautación de su celular en la oficina](https://www.noticiasuno.com/nacional/funcionaria-del-dapre-habla-de-la-incautacion-de-su-celular-en-la-oficina-noticias-uno/) | nacional | F | «las luchas internas de poder dentro de la Casa de Nariño» |
| 12 | 2026-02-15 | [Top Secret: La chica de Gorgona// Los Uribe del colegio// Lista acéfala](https://www.noticiasuno.com/top-secret/top-secret-la-chica-de-gorgona-los-uribe-del-colegio-lista-acefala-noticias-uno/) | top-secret | F | Sátira (Top Secret): «la aún misteriosa pareja de Petro en Gorgona» |
| 13 | 2026-03-14 | [Tres exministros, tres alcaldes y otro congresista serán investigados por UNGRD](https://www.noticiasuno.com/justicia/tres-exministros-tres-alcaldes-y-otro-congresista-seran-investigados-por-ungrd-noticias-uno/) | justicia | F | UNGRD: «el actual gobierno y los miembros de la Comisión Interparlamentaria de Crédito Público intercambiaron favores burocráticos» |
| 14 | 2026-04-05 | [¿Quién le habría informado a “Mordisco” de los bombardeos?](https://www.noticiasuno.com/nacional/quien-le-habria-informado-a-mordisco-de-los-bombardeos-noticias-uno/) | nacional | F | «Antes que ordenarle a la inteligencia…, el Ministerio de Defensa ordenó publicar una lista de golpes» |
| 15 | 2026-05-09 | [Petro deberá disculparse con las mujeres antes del jueves](https://www.noticiasuno.com/justicia/petro-debera-disculparse-con-las-mujeres-antes-del-jueves-noticias-uno/) | justicia | F | Orden judicial al presidente |
| 16 | 2026-05-16 | [Dudas fiscales fracturaron respaldo del Congreso al Gobierno Petro](https://www.noticiasuno.com/sin-categoria/dudas-fiscales-fracturaron-respaldo-del-congreso-al-gobierno-petro/) | sin-categoria | F | Sin texto: solo vídeo |
| 17 | 2026-05-31 | [Última hora: Apertura de investigación al ministro de trabajo Antonio Sanguino](https://www.noticiasuno.com/politica/ultima-hora-apertura-de-investigacion-al-ministro-de-trabajo-antonio-sanguino-noticias-uno/) | politica | F | Sin texto: solo vídeo |
| 18 | 2026-07-19 | [Petro buscará encuentro con Trump para que lo saque de la lista OFAC](https://www.noticiasuno.com/nacional/petro-buscara-encuentro-con-trump-para-que-lo-saque-de-la-lista-ofac-noticias-uno/) | nacional | F | «en busca de salir de la lista OFAC, que rehabilitaría su vida financiera» |
| 19 | 2026-07-25 | [“Pagaron de pendejos”, dijo Petro sobre supuestas coimas de Juliana Guerrero](https://www.noticiasuno.com/politica/pagaron-de-pendejos-dijo-petro-sobre-supuestas-coimas-de-juliana-guerrero-noticias-uno/) | politica | F | Coimas en el Ministerio de Vivienda |
| 20 | 2026-07-25 | [Exvicemindefensa será imputado por contrato de helicópteros MI la próxima semana](https://www.noticiasuno.com/nacional/exvicemindefensa-sera-imputado-por-contrato-de-helicopteros-mi-la-proxima-semana-noticias-uno/) | nacional | F | Contrato de los helicópteros MI |

### 4.3 Antes del cambio: fiscalización de candidatos (Fc), que no suma

| # | Fecha | Título literal | Sección | Clase | Por qué |
|---|---|---|---|---|---|
| 1 | 2025-11-17 | [CNE investigará a Mauricio Cárdenas por propaganda electoral engañosa](https://www.noticiasuno.com/politica/cne-investigara-a-mauricio-cardenas-por-propaganda-electoral-enganosa-noticias-uno/) | politica | Fc | Precandidato Cárdenas: propaganda engañosa |
| 2 | 2025-12-14 | [Hijo de Cabal y Lafaurie obtuvo subsidios como “pequeño agricultor”](https://www.noticiasuno.com/politica/hijo-de-cabal-y-lafaurie-obtuvo-subsidios-como-pequeno-agricultor-noticias-uno/) | politica | Fc | Precandidata Cabal; «según denunció Daniel Coronell en su columna» |
| 3 | 2026-02-15 | [Tenemos las grabaciones sobre una petición de De la Espriella a DMG para “cuadrar” congresistas](https://www.noticiasuno.com/nacional/tenemos-las-grabaciones-sobre-una-peticion-de-de-la-espriella-a-dmg-para-cuadrar-congresistas/) | nacional | Fc | Candidato De la Espriella: grabaciones del caso DMG |
| 4 | 2026-03-15 | [Juan Daniel Oviedo redactó proyecto que sacaba a Noticias Uno de la industria de la televisión](https://www.noticiasuno.com/nacional/juan-daniel-oviedo-redacto-proyecto-que-sacaba-a-noticias-uno-de-la-industria-de-la-television/) | nacional | Fc | Candidato Oviedo frente al propio noticiero (el medio es parte); «Así lo documentó en su columna Daniel Coronell» |
| 5 | 2026-04-02 | [Abelardo choca con la prensa y ciudadanos contradictores](https://www.noticiasuno.com/politica/abelardo-choca-con-la-prensa-y-ciudadanos-contradictores-noticias-uno/) | politica | Fc | Candidato De la Espriella: «insultando personalmente a ciudadanos… y a periodistas» |
| 6 | 2026-04-11 | [Paloma Valencia admite contacto con agitadora contra predial en Bucaramanga](https://www.noticiasuno.com/politica/paloma-valencia-admite-contacto-con-agitadora-contra-predial-en-bucaramanga/) | politica | Fc | Candidata Valencia: la protesta del predial |
| 7 | 2026-05-02 | [Paloma Valencia defiende acumulación de baldíos que su primo ya reconoció](https://www.noticiasuno.com/politica/paloma-valencia-defiende-acumulacion-de-baldios-que-su-primo-ya-reconocio-noticias-uno/) | politica | Fc | Candidata Valencia: los baldíos de su primo |
| 8 | 2026-05-03 | [CNE estudia solicitud de revocatoria de la inscripción de Abelardo de la Espriella](https://www.noticiasuno.com/politica/cne-estudia-solicitud-de-revocatoria-de-la-inscripcion-de-abelardo-de-la-espriella-noticias-uno/) | politica | Fc | Candidato De la Espriella: las firmas; «El candidato reaccionó insultando al denunciante» |
| 9 | 2026-05-24 | [Hija y hermana de Rosa Elvira Cely desmienten a Abelardo De la Espriella](https://www.noticiasuno.com/sin-categoria/hija-y-hermana-de-rosa-elvira-cely-desmienten-a-abelardo-de-la-espriella-noticias-uno/) | sin-categoria | Fc | Candidato De la Espriella; atribuida a la familia de la víctima |
| 10 | 2026-05-30 | [Por decirle que tenía polvo, De la Espriella sacó casas de Ignacios Gómez del registro](https://www.noticiasuno.com/que-tal-esto/por-decirle-que-tenia-polvo-de-la-espriella-saco-casas-de-ignacios-gomez-del-registro/) | que-tal-esto | Fc | Candidato De la Espriella frente al director del noticiero (el medio es parte). Sin texto: solo vídeo |
| 11 | 2026-06-07 | [De la Espriella privatizaría 39 negocios de la Nación y eliminaría 23 entidades](https://www.noticiasuno.com/politica/de-la-espriella-privatizaria-39-negocios-de-la-nacion-y-eliminaria-23-entidades-noticias-uno/) | politica | Fc | Candidato De la Espriella: borrador del plan de campaña |
| 12 | 2026-06-13 | [Ratificación: Documento de Raisbeck fue adoptado como “hoja de ruta” de la campaña De la Espriella](https://www.noticiasuno.com/nacional/ratificacion-documento-de-raisbeck-fue-adoptado-como-hoja-de-ruta-de-la-campana-de-la-espriella/) | nacional | Fc | Candidato De la Espriella: el programa. Sin texto: solo vídeo |
| 13 | 2026-06-14 | [Coronas fúnebres de Paloma y Abelardo fueron copias digitales de otra amenaza ajena](https://www.noticiasuno.com/nacional/coronas-funebres-de-paloma-y-abelardo-fueron-copias-digitales-de-otra-amenaza-ajena-noticias-uno/) | nacional | Fc | Candidatos De la Espriella y Valencia: examen forense de las amenazas |
| 14 | 2026-06-14 | [Así fue la gestión de De la Espriella en Santafé de Ralito, sede de la parapolítica](https://www.noticiasuno.com/politica/asi-fue-la-gestion-de-de-la-espriella-en-santafe-de-ralito-sede-de-la-parapolitica-noticias-uno/) | politica | Fc | Candidato De la Espriella: Ralito, «sede de la parapolítica» |
| 15 | 2026-07-26 | [La compra de la mansión De La Espriella en Miami se registró por US $10](https://www.noticiasuno.com/nacional/la-compra-de-la-mansion-de-la-espriella-en-miami-se-registro-por-us-10-noticias-uno/) | nacional | Fc | Presidente electo: escritura por «diez dólares y otros bienes de valor» |
| 16 | 2026-08-01 | [El Himno Nacional que modificó De la Espriella no podrá ser utilizado en ceremonias públicas](https://www.noticiasuno.com/que-tal-esto/el-himno-nacional-que-modifico-de-la-espriella-no-podra-ser-utilizado-en-ceremonias-publicas/) | que-tal-esto | Fc | Presidente electo (Qué Tal Esto): «que también presume de sus habilidades en el canto lírico» |
| 17 | 2026-08-01 | [De la Espriella regaló biblias a su gabinete y dijo que él está “tocado por el espíritu santo”](https://www.noticiasuno.com/politica/de-la-espriella-regalo-biblias-a-su-gabinete-y-dijo-que-el-esta-tocado-por-el-espiritu-santo/) | politica | Fc | Presidente electo: «tocado por el espíritu santo» |

### 4.4 Después del cambio: fiscalización del gobierno De la Espriella (F) y de la oposición (Fo)

No hay ninguna pieza I, D ni M después del 07-08-2026.

| # | Fecha | Título literal | Sección | Clase | Por qué |
|---|---|---|---|---|---|
| 1 | 2026-08-08 | [Gobierno Petro expidió más de 40 decretos en su última semana de mandato](https://www.noticiasuno.com/nacional/gobierno-petro-expidio-mas-de-40-decretos-en-su-ultima-semana-de-mandato/) | nacional | Fo | Fiscaliza al gobierno saliente, ya fuera del poder. Sin texto: solo vídeo |
| 2 | 2026-08-15 | [Hijo de Jorge Pretelt llega al Ministerio de Agricultura](https://www.noticiasuno.com/nacional/hijo-de-jorge-pretelt-llega-al-ministerio-de-agricultura/) | nacional | F | Sin texto: solo vídeo |
| 3 | 2026-08-22 | [Ambientalistas señalan que decisión de Min Ambiente favorecía a Aris Mining en Santurbán](https://www.noticiasuno.com/nacional/ambientalistas-senalan-que-decision-de-min-ambiente-favorecia-a-aris-mining-en-santurban/) | nacional | F | Atribuida a ambientalistas: Santurbán y Aris Mining |
| 4 | 2026-08-22 | [Los vídeos de Resistencia Chiquita que desconoce la nueva directora del ICBF](https://www.noticiasuno.com/nacional/los-videos-de-resistencia-chiquita-que-desconoce-la-nueva-directora-del-icbf/) | nacional | F | «El archivo no perdona el desconocimiento de la nueva directora del Bienestar Familiar» |
| 5 | 2026-08-29 | [Gobierno busca revivir fumigación con glifosato](https://www.noticiasuno.com/nacional/gobierno-busca-revivir-fumigacion-con-glifosato/) | nacional | F | Con tono: «El gobierno De la Espriella está empecinado en revivir la fumigación aérea» |
| 6 | 2026-08-29 | [Los bienes ocultos de la SAE](https://www.noticiasuno.com/nacional/los-bienes-ocultos-de-la-sae/) | nacional | F | La propuesta del presidente frente a un informe previo de la Contraloría |
| 7 | 2026-08-29 | [Fundador de Colombia Humana denuncia presiones del Pacto Histórico por listas cremalleras](https://www.noticiasuno.com/politica/fundador-de-colombia-humana-denuncia-presiones-del-pacto-historico-por-listas-cremalleras/) | politica | Fo | Fiscaliza a la oposición de izquierda: presiones del Pacto por las listas cremallera |
| 8 | 2026-08-30 | [Gobierno presenta presupuesto más alto que el de Petro](https://www.noticiasuno.com/economia/gobierno-presenta-presupuesto-mas-alto-que-el-de-petro-noticias-uno/) | economia | F | Sin texto: solo vídeo |
| 9 | 2026-08-30 | [La nueva directora de la Unidad de Restitución de Tierras seguía órdenes de Uribe](https://www.noticiasuno.com/nacional/la-nueva-directora-de-la-unidad-de-restitucion-de-tierras-seguia-ordenes-de-uribe-noticias-uno/) | nacional | F | Sin texto: solo vídeo |
| 10 | 2026-09-05 | [Campesinos que recibieron predios de alias Barbie denuncian amenazas](https://www.noticiasuno.com/que-tal-esto/campesinos-que-recibieron-predios-de-alias-barbie-denuncian-amenazas/) | que-tal-esto | F | Qué Tal Esto: «en uno de los cuales es socio el presidente De la Espriella» |
| 11 | 2026-09-05 | [Critican al presidente por posar frente a cadáveres](https://www.noticiasuno.com/nacional/critican-al-presidente-por-posar-frente-a-cadaveres/) | nacional | F | Con tono: exhibir cadáveres es «una práctica que existió en las sociedades antiguas y que las modernas habían abolido» |
| 12 | 2026-09-05 | [El pasado de D’Mar Córdoba nuevo director del CNMH frente al Palacio de Justicia](https://www.noticiasuno.com/nacional/el-pasado-de-dmar-cordoba-nuevo-director-del-cnmh-frente-al-palacio-de-justicia/) | nacional | F | El nuevo director de Memoria Histórica y «su posición negaci[onista]» |
| 13 | 2026-09-05 | [Divisiones motivadas del Pacto Histórico](https://www.noticiasuno.com/politica/divisiones-motivadas-del-pacto-historico/) | politica | Fo | Fiscaliza a la oposición de izquierda: «el respaldo de petristas a la maniobra de su defensa para evitar la indagatoria» |
| 14 | 2026-09-06 | [QTE: Min Trabajo reduce multa a Charry Trading en un 80%](https://www.noticiasuno.com/que-tal-esto/qte-min-trabajo-reduce-multa-a-charry-trading-en-un-80-noticias-uno/) | que-tal-esto | F | Qué Tal Esto. Sin texto: solo vídeo |
| 15 | 2026-09-06 | [Sorpresas del presupuesto milagro](https://www.noticiasuno.com/nacional/sorpresas-del-presupuesto-milagro-noticias-uno/) | nacional | F | Con tono («presupuesto milagro», eco de la «Patria Milagro»). Sin texto: solo vídeo |
| 16 | 2026-09-12 | [Abogados del “Dream Team” de Carlos Mattos llegaron al poder](https://www.noticiasuno.com/politica/abogados-del-dream-team-de-carlos-mattos-llegaron-al-poder/) | politica | F | «llegaron al poder» |
| 17 | 2026-09-19 | [Prometieron bajar tarifas, pero podrían subir](https://www.noticiasuno.com/nacional/prometieron-bajar-tarifas-pero-podrian-subir/) | economia,nacional | F | La promesa de campaña frente a lo que anuncia la ministra de Minas |
| 18 | 2026-09-20 | [Con asfixia presupuestal quieren acabar la JEP](https://www.noticiasuno.com/justicia/con-asfixia-presupuestal-quieren-acabar-la-jep-noticias-uno/) | justicia | F | Con tono («quieren acabar»). Sin texto: solo vídeo |
| 19 | 2026-10-03 | [Presidente de Ecopetrol estuvo en Fipaz con Abelardo](https://www.noticiasuno.com/nacional/presidente-de-ecopetrol-estuvo-en-fipaz-con-abelardo-noticias-uno/) | nacional | F | Fipaz y sus foros con jefes paramilitares |
| 20 | 2026-10-10 | [Acusaciones contra expresidente Petro sobre Miguel Uribe](https://www.noticiasuno.com/nacional/acusaciones-contra-expresidente-petro-sobre-miguel-uribe-noticias-uno/) | nacional | F | Contrasta al presidente con la investigación: «a pesar de que la investigación judicial que ha adelantado la Fiscalía no tiene pistas al respecto». Admite una segunda lectura como disculpa del expresidente (ver §6) |

---

## 5. Números

### 5.1 Piezas con postura (I, D, M)

| | I | I-leve | D | D-leve | M | **Con postura** | F | Fo | Fc |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Antes del 07-08-2026 | 19 | 12 | 0 | 2 | 7 | **40** | 20 | 0 | 17 |
| Desde el 07-08-2026 | 0 | 0 | 0 | 0 | 0 | **0** | 17 | 3 | — |
| **Total** | **19** | **12** | **0** | **2** | **7** | **40** | **37** | **3** | **17** |

- **Dirección:** 31 a la izquierda (I + I-leve) frente a 2 a la derecha (D-leve): **15,5 a 1**. Contando solo las claras, 19 a 0.
- **Sin Top Secret** (la sátira): 19 a la izquierda (11 I y 8 I-leve), 1 D-leve y 1 M. La dirección no cambia: 19 a 1.
- **Fc por destinatario** (fiscalización de candidatos antes del cambio): De la Espriella 12, Paloma Valencia 3 (una compartida con De la Espriella), María Fernanda Cabal 1, Mauricio Cárdenas 1, Juan Daniel Oviedo 1 e **Iván Cepeda 0**. No hay en la ventana ni una pieza que fiscalice al candidato de la izquierda. Las piezas sobre él son perfiles favorables (n.º 23, 34 y 35 de la tabla 4.1), defensas frente a acusaciones (16 y 17) o crónica de campaña.
- **F a los dos lados:** 20 piezas fiscalizan al gobierno Petro mientras manda (bombardeo de Calamar, UNGRD, DAPRE, Benedetti, la lista OFAC) y 17 al gobierno De la Espriella desde que manda. **Con quien gobierna, la conducta es la misma.**

### 5.2 Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | Sí, en texto | Títulos y entradillas sin atribución, más Qué Tal Esto y Top Secret. Ni un vídeo visto (§3.1) |
| 2. A los dos lados del cambio | **No** | Después del 07-08 no hay ninguna pieza con elogio, disculpa ni rótulo. Hay 17 F y 3 Fo |
| 3a. ≥10 piezas con postura | Sí | 40 (31 en una dirección) |
| 3b. ≥3 a cada lado del cambio | **No** | 40 antes y 0 después |
| 3c. ≥3 a 1 en la misma dirección | Sí | 15,5 a 1 (19 a 0 contando solo las claras) |
| 4. Contrapesos escritos | Sí | §7 |
| 5. Reproducible | Sí | §1 y §4: consulta, URL, fecha y clase |

**No cumple los mínimos.** Le falta el lado posterior al cambio.

---

## 6. Rama de la precisión del 2026-10-10

El −0,40 **solo se apoya en los niveles 4 y 5**: una descripción de trayectoria («treinta años», «Uribe, Santos, Duque») y el razonamiento «vigilar al establecimiento sitúa a la izquierda», que el polo fijo descarta. No hay nivel 1 (la propiedad está abierta) ni nivel 2 (el corpus es cero). Por eso **el barrido manda**, y estas son sus cuatro ramas:

| Rama | ¿Se da? | Por qué |
|---|---|---|
| Cumple las cinco condiciones → valor del barrido, tope ±0,30 salvo endoso | **No** | Falta el lado posterior (3b). Tampoco hay endoso explícito: ninguna pieza en voz de la casa pide el voto por Cepeda ni declara apoyo |
| Misma conducta con los dos gobiernos (≥3 piezas de fiscalización o postura a cada lado, postura por debajo de 3:1) → 0,00 con evidencia | **No** | La primera mitad sí se da: 20 F antes y 17 después, con la misma vara a Petro y a De la Espriella. **La segunda no:** la postura va 15,5 a 1 hacia la izquierda |
| **Dirección clara sin mínimos → «sin medir», con la tensión declarada** | **SÍ** | Toda la postura medida va en un sentido (31 a 2), pero está toda antes del cambio y en la campaña |
| Sin piezas suficientes para juzgar → «sin medir» | No aplica | Hay piezas de sobra antes del cambio |

**Valor que resulta: «sin medir» (`bias: null`)**, con esta tensión escrita en la ficha:

> En la campaña presidencial de 2026, la voz escrita de la casa trató de forma
> asimétrica a los candidatos. Rotuló a De la Espriella y a la derecha («la
> "teta del Estado"», «todos los de siempre», «bandera antiderechos», «De la
> Espriella Style… en Ralito») y defendió a Cepeda frente a acusaciones que dio
> por infundadas («sin pruebas», «sin fundamentos fácticos»). No fiscalizó ni
> una vez al candidato de la izquierda. Con quien gobierna se comporta igual:
> fiscalizó a Petro mientras mandaba y fiscaliza a De la Espriella desde que
> manda. No hay piezas con postura después del cambio que permitan aplicar la
> regla.

### Sensibilidad: qué cambiaría el resultado

- **Si la fiscalización «con tono» del después contara como rótulo.** Son cuatro piezas: «empecinado» (08-29), los cadáveres como trofeo (09-05), el «presupuesto milagro» (09-06) y «quieren acabar la JEP» (09-20). Si además «Acusaciones contra expresidente Petro sobre Miguel Uribe» (10-10) se leyera como disculpa del expresidente y no como contraste del presidente con la investigación, saldrían 5 piezas I-leve después del cambio. **Se cumplirían los mínimos**, y el valor del barrido sería izquierda con el tope: **−0,30 como máximo**, y probablemente menos por la regla 2, porque son leves. **No se propone**, porque la precisión del 2026-10-09 dice que «una pieza que solo fiscaliza a quien manda se declara, pero no suma», y esas cinco critican a quien manda por lo que hace. Pero es la lectura alternativa, y quien firme tiene que poder elegirla.
- **Si se viera el vídeo.** La locución puede contener rótulos o elogios que el texto no tiene, en un sentido o en el otro. Es lo que más puede mover este barrido.
- **En ninguna lectura sale −0,40.** Sin endoso explícito ni propiedad de nivel 1 con posición conocida, el tope es ±0,30.

---

## 7. Contrapesos, con su peso

**Hacia la mixta (contra la dirección izquierda):**
- **La conducta con el poder es simétrica.** 20 piezas fiscalizan a Petro mientras manda: el bombardeo de Calamar con menores, la UNGRD y la cárcel de sus exministros, el acoso en el DAPRE, la lista OFAC, «Pagaron de pendejos». Y 17 fiscalizan a De la Espriella desde que manda. El noticiero no se volvió complaciente con Petro en su último año. **Peso alto:** es la mitad de la regla del 0,00.
- **Fiscaliza a la izquierda cuando deja el poder.** «Divisiones motivadas del Pacto Histórico» (09-05), las presiones del Pacto por las listas cremallera (08-29) y los 40 decretos de la última semana de Petro (08-08). **Peso medio:** son 3 piezas.
- **Los formatos de tiempo igual.** Proyecto Uno dio un minuto a cada candidato, De la Espriella incluido (2026-04-19), y De lado y lado enfrentó a dos voces en 14 emisiones. **Peso medio:** es equilibrio formal, no de encuadre.
- **Top Secret también se burla de la izquierda:** los «outfits del Pacto», «Cepeda rezado», «Petrico y Trumpito», «la misteriosa pareja de Petro en Gorgona». **Peso bajo:** en Top Secret son 1 D-leve, 2 F y 6 M, frente a 12 a la izquierda.

**Hacia la izquierda (a favor de la dirección):**
- **La asimetría entre candidatos.** 12 piezas fiscalizan a De la Espriella y 0 a Cepeda. Los perfiles del 20 de junio, a ocho días de la segunda vuelta, van en pareja: «De la Espriella Style comenzó en la política en 2002, en Ralito» y «El barrio en el que nació la causa de Iván Cepeda», más «el filósofo que renegó del comunismo». **Peso alto:** es el encuadre asimétrico que la regla cuenta.
- **La defensa del presidente de turno en 2026.** «Las maniobras golpistas de Gloria Arizabaleta» (06-13), «Lucio organizaba sus denuncias desde 2024» (07-13) y The Economist «que ha publicado duras críticas al gobierno Petro» (2025-12-13). **Peso medio:** son pocas, pero son respaldo y no fiscalización.
- **Dos conflictos en los que el medio es parte** (§3.4). **Peso bajo** en la dirección: explican la temperatura con De la Espriella y con Oviedo, pero no la crean.

---

## 8. PROPUESTA (pendiente de firma)

1. **Valor: de −0,40 a «sin medir» (`bias: null`)**, por la rama «dirección clara sin mínimos» de la precisión del 2026-10-10. Con esa rama el −0,40 no se conserva: solo se apoyaba en los niveles 4 y 5, y el barrido manda.
2. **Tensión escrita en la ficha:** el texto del §6, con las piezas n.º 16, 17, 27, 30, 31, 33, 34 y 35 de la tabla 4.1 como ejemplos. También hay que corregir la frase de la ficha «la evidencia disponible apunta a 0,00». Lo que el barrido encontró es la mitad de eso: misma vara con quien gobierna, y otra vara con los candidatos.
3. **Alternativa declarada:** −0,30 «izquierda moderada» o menos, solo si quien firma decide que la fiscalización con adjetivo propio cuenta como rótulo (§6, sensibilidad). Este barrido no la recomienda.
4. **Fuera del alcance de este barrido, pero anotado:** la incoherencia sobre Daniel Coronell entre `centinela.js`, `mediaOwnership.js` y la ficha (§3.5), y el patrón de piezas de la Procuraduría con tono de comunicado (§3.6).
5. **Revisión:** recontar en diciembre de 2026 y en febrero de 2027 las piezas posteriores al cambio, y comprobar si Top Secret volvió. Si aparecen 3 o más piezas con rótulo, elogio o disculpa después del 07-08, el barrido se rehace con la regla completa. Si es posible, conviene ver una muestra de emisiones de cada lado del cambio para medir la locución, que este barrido no midió.
