# Barrido editorial: CasaMacondo

| | |
|---|---|
| **Medio** | CasaMacondo (`casa-macondo`), en el catálogo desde el 2026-08-08. **No noticioso** desde el 2026-09-16: fuera del mapa, sigue en la ingesta y en las historias |
| **Valor vigente** | **−0,35**, sin firmar, apoyado solo en nivel 4 (`fichas/casa-macondo.md`) |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus dos precisiones |
| **Ventana** | 2025-10-10 → 2026-10-10 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Resolución de origen** | `revision-externa/respuestas/opus-5-5-casa-macondo.md` (revisor: 6 piezas con postura, todas a la izquierda, 4 antes y 2 después, y 2 contrapesos) |
| **Quién lo hizo** | Claude Opus 5.5 (`claude-opus-5-5`), verificador del ciclo 2, tanda 8, a petición del responsable editorial, el 2026-10-10. Es de la misma casa que el autor de la ficha y que el revisor: su acuerdo no es aval |
| **Estado** | **DECIDIDO el 2026-10-10: 0,00 con evidencia** (antes −0,35), por el responsable editorial; firmado en bloque el mismo día (`DECISIONES.md`, «2026-10-10 · Tandas 8 y 9 del ciclo 2: el barrido manda sobre los números sin evidencia»). Lo que más abajo dice «propuesta», «recomendada» o «pendiente» es el estado anterior a la decisión y se conserva como historia |
| **Resultado** | **No se cumplen las condiciones.** En la lectura estricta (cuenta de la casa y director) hay **0 piezas con postura**. En la lectura amplia (más el editor general, los demás cofundadores y la plantilla) hay **5** (una leve), todas a la izquierda y **todas anteriores al 07-08-2026**, frente a 2 contrapesos. Después del cambio, **0**: las dos que el revisor contó después son una columna de noviembre de 2024 publicada con fecha nueva y una pieza internacional. Mínimos: 10 piezas, 3 a cada lado, 3 a 1. **El número no puede moverse por esta vía** |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas, el
> fragmento y el método están aquí para eso. **La clasificación de cada pieza
> es juicio de un solo lector**, de la misma casa que el autor de la ficha y
> que el revisor.

---

## 1. Método

- **robots.txt** de `casamacondo.co`, leído el 2026-10-10 antes de descargar nada:
  `User-agent: *` con `Disallow` de `/wp-admin/`, `/?s=`, `/feed/`, `/*/feed/` y `/*/embed/`; `Sitemap:` `sitemap_index.xml` y `monopolitica-sitemap.xml`. **No excluye `/wp-json/`**, que es la vía usada. **No se leyó `/feed/` ni ninguna ruta `/*/feed/`.**
- **Descarga:** `curl -sL --ssl-no-revoke` con User-Agent de navegador (Chrome 126), con un segundo entre peticiones.
- **Universo, sin muestreo**, desde la API pública de WordPress del medio:
  ```
  https://casamacondo.co/wp-json/wp/v2/posts?after=2025-10-10T00:00:00&per_page=100&page=1…3
    &_fields=id,date,link,title,categories,author
  X-WP-Total: 208
  ```
  y el cuerpo de las 208 con `&_fields=id,date,modified,link,content` (9 páginas de 25). Autores: `/wp-json/wp/v2/users?per_page=100`. Categorías: `/wp-json/wp/v2/categories?per_page=100`. Tipos públicos (`/wp-json/wp/v2/types`): las piezas son `post`; no hay otro tipo de contenido editorial.
- **Lo que hay:** 208 entradas del 2025-10-11 al 2026-10-10. **70 caricaturas** (categoría Caricatura, todas de Leo Parra, director de arte de plantilla) y **138 piezas de texto**. 169 antes del 07-08-2026 y 39 desde ese día (25 de texto).
- **Fechas:** el campo `date` de la API, en hora de Colombia.
- **Lectura:** se buscaron en el cuerpo de las 138 piezas de texto los términos `petro|espriella|abelardo|cepeda|uribe|izquierd|derech|paloma|pacto hist|centro democr|comunis|progresis|fascis|ultraderech|tigre|gobierno del cambio|fajardo|milei|trump|bukele`; 95 tienen alguno. Se leyeron por fragmentos alrededor de cada término todas las de autores de la casa, y enteras las de Opinión con contenido político.

**Quién es «la casa».** CasaMacondo no publica editoriales sin firma. Por eso se hacen dos lecturas:

- **Estricta**, la del protocolo: piezas sin firma o firmadas por la cuenta institucional «CasaMacondo» (autor 12, 16 piezas) o por el director general, Christopher Tibble (autor 15, 4 piezas).
- **Amplia**, la del revisor: además, el editor general y cofundador José Alejandro Castaño (autor 9, 41 piezas), los demás cofundadores con firma en la ventana (Juan Pablo Barrientos, 23; Ricardo Mendivil, 1) y la plantilla de /somos/ (Santiago Wills, 8; Pacho Escobar, 6; Alejandra Torrijos, 2). **El protocolo no dice si una columna del editor general es voz de la casa.** Se declara la duda y se cuenta aparte.

**No cuentan, y se declaran:** las columnas de terceros (Daniella Sánchez Russo, Luis Tejada, Manuela Lopera, Marcos Colón, Andrea Mejía…), las reimpresiones (Cerosetenta, 18-07-2026; la columna de Luis Tejada de los años veinte, 06-06-2026), las 70 caricaturas (ver §5), y las piezas internacionales.

**Clases.**
- **I, postura hacia la izquierda** (cuenta): rótulo ideológico en voz propia contra la derecha o sus candidatos fuera del poder; elogio o disculpa de la izquierda o de su gobierno.
- **D, postura hacia la derecha** (cuenta): lo simétrico.
- **C, contrapeso:** pieza de la casa que reparte el reproche a los dos lados, o que matiza la dirección dominante.
- **F, solo fiscaliza** (no cuenta, se declara): investigación o crítica a quien ejerce poder público, de cualquier signo. Por la precisión del 2026-10-09, no suma para el mínimo por lado.
- **Fuera:** internacionales, culturales, ambientales sin destinatario político nacional, testimonios, perfiles biográficos, crónicas del terremoto.

---

## 2. Piezas con postura (lectura amplia)

Todas son de Opinión, firmadas por el editor general o por un cofundador. **En la lectura estricta no hay ninguna.**

### 2.1 Antes del cambio: 2025-10-10 → 2026-08-06

| # | Fecha | Id | Firma | Pieza | Clase | Fragmento literal |
|---|---|---|---|---|---|---|
| 1 | 2025-11-08 | 13808 | Castaño (editor general) | [Miguel Polo Polo, el rico más pobre en su álbum de fotografías](https://casamacondo.co/opinion/miguel-polo-polo-el-rico-mas-pobre-en-su-album-de-fotografias/) | I, con matiz dentro | «los vínculos con el paramilitarismo y el narcotráfico de Álvaro Uribe Vélez, su tutor e inspirador ideológico»; y dentro: «La crueldad de la extrema izquierda no justifica la crueldad de la extrema derecha» |
| 2 | 2026-06-06 | 17950 | Castaño | [Una gallina no es un tigre](https://casamacondo.co/opinion/abelardo-de-la-espriella/) | I | «Hay algo profundamente aciago en que una parte del país vea en Abelardo de la Espriella un presidente posible»; «El candidato de la extrema derecha colombiana parece construido para esa mutación cultural» |
| 3 | 2026-06-18 | 18071 | Castaño | [La Virgen del Cobre y el arroz que desarmó el fortín de las AUC](https://casamacondo.co/opinion/economia-campesina-victimas-conflicto-uraba/) | I (leve) | Crónica de restitución de tierras en Opinión. Encuadra el programa del candidato: «propone desmontar una parte de la arquitectura institucional que hizo posibles procesos como este y reemplazarla por una visión centrada en la propiedad privada». El revisor no la cuenta; aquí se cuenta como leve para no quedarse corto |
| 4 | 2026-06-24 | 18129 | Castaño («como enviado especial de CasaMacondo») | [No tenemos miedo. Venimos de peores noches](https://casamacondo.co/opinion/no-tenemos-miedo-cronica-eleccion-colombia/) | I | «por suerte, el ciclo reciente de reformas sociales no desaparecerá»; «la sorprendente votación de algunos sectores populares en favor del modelo económico que más los ha explotado y envilecido» |
| 5 | 2026-07-18 | 18605 | Castaño | [Ignorantes y desvergonzados](https://casamacondo.co/opinion/ignorantes-desvergonzados-jose-castano/) | I | «el legado del sátrapa» (Álvaro Uribe); Viviane Morales, «una negacionista de derechos civiles»; «Abelardo de la Espriella resulta minúsculo». De la Espriella era presidente electo, no gobernante |

**Contrapesos antes del cambio:**

| # | Fecha | Id | Firma | Pieza | Clase | Fragmento literal |
|---|---|---|---|---|---|---|
| C1 | 2025-11-22 | 13958 | Castaño | [Las mentiras de la verdad absoluta](https://casamacondo.co/opinion/las-mentiras-de-la-verdad-absoluta-opinion/) | C pleno | Reparte a los dos lados: «que Gustavo Petro es un capo del narcotráfico internacional» y, del otro, «que las sanciones de Donald Trump a Gustavo Petro por narcotráfico fueron un complot uribista», «sabotajes directos de gremios y paramilitares para derrocar al gobierno del cambio» |
| C2 | 2026-07-04 | 18413 | Ricardo Mendivil (cofundador) | [La independencia incómoda](https://casamacondo.co/opinion/importancia-periodismo-independiente/) | C parcial | «los seguidores de Abelardo de la Espriella hicieron señalamientos por nuestra labor»; «muchos de los que nos defendían comenzaron a atacarnos por confrontar también al poder de turno: el de Gustavo Petro» |

### 2.2 Después del cambio: 2026-08-07 → 2026-10-10

**Ninguna pieza con postura nacional.** Las dos que contó el revisor no entran:

| Fecha | Id | Pieza | Por qué no cuenta |
|---|---|---|---|
| 2026-08-22 | **5953** | [Donald Trump](https://casamacondo.co/opinion/donald-trump/) | **Es una columna de noviembre de 2024 con fecha nueva.** Su id (5953) está entre el 5948 (caricatura del 2024-11-07) y el 5974 (2024-11-10) de la propia API; las piezas de octubre de 2025 ya van por el 13500. El texto habla de Trump «transfigurado por segunda vez en presidente electo», que es noviembre de 2024. La API la data el 2026-08-22, con `modified` del 2026-07-22, anterior a su publicación. Además es política extranjera. **Fuera** |
| 2026-10-03 | 20002 | [Milei y De la Espriella son felinos forasteros, y asustados](https://casamacondo.co/opinion/milei-y-de-la-espriella-felinos-asustados/) | La parte de Milei («El león es manso con los poderosos y fiero con los débiles») es internacional: **fuera**. La de De la Espriella («El tigre que gobierna Colombia aparenta otra presencia»; «una parte de su fortuna proviene de representar corruptos y asesinos en serie») es burla y crítica del presidente en ejercicio: **F, no suma** |

---

## 3. Lo que solo fiscaliza (F), a los dos lados, y no suma

| Fecha | Id | Firma | Pieza | A quién |
|---|---|---|---|---|
| 2025-10-11 a 2026-05-28 | 13522, 13610, 13691, 17860 | Barrientos | Serie sobre el presidente de la Corte Constitucional | Poder judicial |
| 2026-01-17 · 2026-02-07 · 2026-02-21 | 15819, 15992, 16266 | Barrientos | Alirio Barrera y los baldíos | Senador; su prima, según la pieza, fue «exsenadora del Centro Democrático» |
| 2026-01-24 | 15890 | Barrientos | Aníbal Gaviria y los baldíos | Gobernador |
| 2026-02-28 | 16313 | Barrientos | [Juan Diego Gómez: el candidato imputado por estafa que quiere volver al Senado](https://casamacondo.co/denuncias/juan-diego-gomez-expediente-de-corrupcion/) | «el exsenador conservador» |
| 2026-03-21 | 16473 | Barrientos | Una vaca de El Ubérrimo… y los Uribe dejaron de responder | Familia del expresidente |
| 2026-05-16 | 17638 | Castaño | [Carlos Caicedo, el candidato embargado](https://casamacondo.co/casamacondo/carlos-caicedo-candidato-embargado/) | Candidato presidencial |
| 2026-05-22 | 17783 | Castaño | Santiago Botero, el candidato antiestafas que negoció con un estafador | Candidato presidencial |
| 2026-06-13 | 18026 | Barrientos | [El proceso contra Abelardo de la Espriella que fue archivado…](https://casamacondo.co/investigacion/abelardo-de-la-espriella-fiscalia/) | Candidato presidencial |
| 2026-06-27 | 18168 | Barrientos | [El gobierno que prometió no matar niños asesinó más que el anterior](https://casamacondo.co/investigacion/ninos-muertos-en-bombardeos-durante-gobierno-petro/) | **Gobierno Petro, en ejercicio**: «Durante el de Gustavo Petro, 57, a un ritmo de 15,2 por año, un 41 por ciento más» |
| 2026-08-01 | 19231 | Barrientos | Tres candidatos impresentables a la Contraloría | Candidatos a contralor |
| 2026-08-15 | 19464 | Barrientos | La denuncia por enriquecimiento ilícito contra Jorge Eliécer Laverde, nuevo contralor general | Contralor |
| **2026-08-28** | **19769** | **CasaMacondo (cuenta institucional, Opinión)** | [Viviane Morales y el credo de los curas en los colegios públicos](https://casamacondo.co/opinion/viviane-morales-curas-colegios-publicos/) | **Gobierno De la Espriella**: «que la misma institución que ha encubierto sistemáticamente a abusadores de menores ahora contemple, con el beneplácito del nuevo gobierno, administrar colegios públicos». El revisor no la cita |
| 2026-09-19 | 19915 | CasaMacondo | [Gobierno de Petro entregó tierras a Pablo Catatumbo cuando era senador](https://casamacondo.co/noticia/petro-entrego-tierras-pablo-catatumbo/) | Gobierno saliente y Comunes |
| 2026-09-24 | 19942 | CasaMacondo | [Viceministro de Vivienda se presenta con una maestría que no ha completado](https://casamacondo.co/investigacion/reynaldo-dsilva-uribe-maestria-externado/) | Gobierno De la Espriella |
| 2026-10-03 | 20011 | Castaño | [La ANT le tituló tierras a Germán Gómez cuando era representante a la Cámara](https://casamacondo.co/noticia/tierra-firmantes-catatumbo-gomez-ant/) | Gobierno saliente; «el excongresista del partido Comunes» |
| 2026-10-10 | 20051 | Castaño | [Otro viceministro del Tigre presume de un título que no tiene](https://casamacondo.co/investigacion/viceministro-ambiente-gustavo-guerrero/) | Gobierno De la Espriella |

**Lectura del polo fijo.** Antes del cambio fiscalizó al Gobierno Petro en ejercicio (18168). Después, fiscaliza al Gobierno De la Espriella (19769, 19942, 20051) **y** sigue investigando actos del Gobierno Petro y de congresistas de Comunes (19915, 20011). No hay celebración del gobierno entrante ni disculpa del saliente después del 07-08. Es la conducta que el protocolo describe como periodismo, no como orientación.

**El objetivo más constante de la unidad investigativa no está en el eje:** la Iglesia católica (Archivo Secreto: 15964, 16422, 16458, 16569, 16790, 16831, 18415, 18601, 19960, 20045).

---

## 4. Recuento

| Lectura | Antes del 07-08 (I / D) | Desde el 07-08 (I / D) | Contrapesos | ¿Cumple? |
|---|---|---|---|---|
| **Estricta** (cuenta de la casa + director) | 0 / 0 | 0 / 0 | — | **No.** 0 de 10 |
| **Amplia** (+ editor general, cofundadores, plantilla) | **5** (4 + 1 leve) / 0 | **0** / 0 | 2 (1 pleno, 1 parcial), los dos antes | **No.** 5 de 10; 0 después del cambio (pide 3); 5:2 = 2,5:1 (pide 3:1) |
| **La del revisor** | 4 / 0 | 2 / 0 | 2 | No (él mismo lo dice) |

**Diferencia con el revisor:** aquí se añade una leve antes (18071), y él cuenta 2 después del cambio, y las dos son extranjeras (él mismo lo anota). Aquí no entran: «Donald Trump» es de noviembre de 2024 y la parte de Milei es internacional. **Con cualquiera de las tres lecturas, la condición 2 (a los dos lados del cambio) falla.**

---

## 5. Lo que no se cuenta, y se declara

- **Caricaturas (70, Leo Parra).** Firmadas por el director de arte, no son editorial. Por título, apuntan a los dos lados. Antes del cambio, contra el Gobierno Petro: «Personaje del (d)año» (Benedetti, 14-12-2025), «Excusa "médica"» (ministro de Salud, 25-02-2026), «Ni paz, ni total» (21-01-2026), «Parranda total» (15-04-2026), «Bombardeos» (17-11-2025), «El discurso» y «La graduada» (Juliana Guerrero, 29-07 y 17-09-2026); contra la derecha: «Centro dedocrático» (21-11-2025), «Apóstol condenado» (28-11-2025), «Estrategia uribista» (12-03-2026), «Postura de Centro… Democrático» (19-03-2026), «El tigre de papel» (13-02-2026), «"El tigre" al desnudo» (15-05-2026). Después del cambio, contra el gobierno entrante: «"Administración milagro"» (08-08), «La patria espectáculo» (20-08), «Ministro de Vivienda» (21-08), «"Batalla cultural" en el ICBF» (26-08), «Por las nubes» (30-09), «"Interlocución milagro"» (08-10). No se leyó la imagen.
- **Perfil de Iván Cepeda** (17013, 2026-04-30, Pacho Escobar, plantilla). [El dedo acusador de Iván Cepeda](https://casamacondo.co/perfiles/el-dedo-acusador-de-ivan-cepeda/). Biográfico, recoge a sus críticos: «Algunas etapas de esa defensa son su talón de Aquiles. Sus opositores lo presentan como un político cuya figura se entrelaza con viejos fantasmas de la guerra». No se cuenta.
- **Testimonio sobre Milei** (18003, 2026-06-12, Alejandra Torrijos, correctora). Internacional.
- **«Los bombardeados»** (8 piezas del 15-05-2026). Ataques de Estados Unidos a lanchas: internacional.
- **Opinión sin postura en el eje**: 13728 «Miss Antioquia» (reprocha a una reina que preguntara a quién dispararía, si a Quintero o a Petro: es contra la incitación, no a favor de nadie), 14041, 16776, 17038 y la del 18-06 de Santiago Wills (18060), que propone reglas para elegir líderes sin nombrar a nadie.

---

## 6. Tensión que se declara (no mueve el número)

**Las columnas del editor general atacan al candidato de la derecha y no al de la izquierda.** Entre el 06-06 y el 18-07-2026, Castaño publicó tres columnas contra De la Espriella (17950, 18129, 18605), más el encuadre leve de 18071, y ninguna contra Iván Cepeda. Las investigaciones de campaña fueron contra Caicedo, Botero, De la Espriella y un exsenador conservador; de Cepeda hubo un perfil biográfico. **Es encuadre asimétrico entre candidatos**, que la regla del polo fijo no excluye, pero en una firma, no sin firma, y por debajo de todos los mínimos. Si el editor general siguiera con esa asimetría frente a la derecha en el poder y no frente a la izquierda en la oposición, la pregunta cambiaría; hoy no se ve: después del 07-08 la casa fiscaliza a los dos.

---

## 7. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | **Dudosa** | No hay editoriales sin firma. La cuenta institucional y el director no toman postura; quien la toma es el editor general en columnas firmadas |
| 2. A los dos lados del cambio | **No** | 5 antes y 0 después (lectura amplia) |
| 3a. ≥10 piezas con postura | **No** | 5 (amplia) o 0 (estricta) |
| 3b. ≥3 a cada lado | **No** | 0 después |
| 3c. ≥3:1 | **No** | 5:2 |
| 4. Contrapesos escritos | Sí | §2 y §3 |
| 5. Reproducible | Sí | §1 da la consulta; §2 y §3, id, URL, fecha, firma y fragmento |

**La regla no se cumple.** Por la segunda precisión del responsable editorial («un barrido que no llega a los mínimos no deshace nada»), este barrido tampoco retira por sí solo el −0,35. Lo que lo deja sin apoyo es otra cosa: la evidencia de nivel 1 que ahora consta y la declaración de nivel 4 completa. Eso se razona en la resolución.

**Qué lo reabriría:** que en los próximos meses la voz de la casa (cuenta institucional, dirección o, si el responsable editorial lo admite como tal, el editor general) tome postura con nombre a favor o en contra de un lado **después** del 07-08, o que deje de fiscalizar a uno de los dos gobiernos. Recuento propuesto: enero de 2027, con la misma consulta.
