# Barrido editorial: La Patria

| | |
|---|---|
| **Medio** | La Patria (`la-patria`), diario de Manizales, lapatria.com. De la familia Restrepo desde 1940 (`shared/mediaOwnership.js`). No tenía ficha técnica: la crea este mismo encargo, mínima, en `fichas/la-patria.md` |
| **Valor vigente** | **+0,25**, derecha moderada, `reviewedAt: '2026-10-10'` (firma en bloque). Su razón en el registro es una frase: «Diario del Eje Cafetero; línea tradicional con agenda regional agroindustrial». Sus dos fuentes son crónicas de Las2Orillas sobre los dueños de periódicos regionales. **No hay lectura de piezas detrás: se apoya solo en los niveles 4 y 5.** El texto público ya lo dice (`shared/resumenesPublicos/la-patria.js`) |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con la regla del polo fijo y la precisión del 2026-10-10 |
| **Ventana** | 2025-10-12 → 2026-10-12 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Quién lo hizo** | Claude Opus 5.5, a petición del responsable editorial, 2026-10-12. Es de la misma casa que quien escribió otras fichas y barridos del catálogo: su acuerdo con ellos no es aval |
| **Estado** | **FIRMADO el 2026-10-12: +0,10** (antes +0,25), como se propuso; se descarta la alternativa de 0,00. Aplicado en el registro, la ficha y el texto público el 2026-10-12 (`DECISIONES.md`, «Veinte medios: barridos firmados, sin medir permanente para quien no autoriza la IA, y feeds que se mantienen») |
| **Resultado** | **Cumple las cinco condiciones, pero solo contando las piezas leves.** En los editoriales de la ventana (360 distintos, todos leídos) hay **14 con dirección derecha y 4 con dirección izquierda: 3,5 a 1.** Son 9 a la derecha antes del cambio y 5 después. **Sin las leves no se llega**: quedan 3 claras a la derecha y 0 a la izquierda. Y el contrapeso es fuerte: **el diario fiscaliza al Gobierno De la Espriella con la misma dureza con que fiscalizó al de Petro** (12 editoriales críticos en 9 semanas, frente a unos 80 en 43). Sin endoso. Rama 1 de la precisión: valor del barrido, con tope ±0,30. **Valor propuesto: +0,10**, dentro de la banda mixta. Alternativa: 0,00 con evidencia |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas, los
> fragmentos y el método están aquí para eso. **La clasificación de cada
> pieza es el juicio de un solo lector.** Las 15 piezas «leves» son las más
> discutibles, y de ellas depende que se cumplan los mínimos (§5).

---

## 1. Método

- **robots.txt** de `www.lapatria.com`, descargado el 2026-10-12 antes de cualquier otra petición (HTTP 200). Es el de serie de Drupal: un solo bloque `User-agent: *` con `Disallow` en `/core/`, `/profiles/`, ficheros README, `/admin/`, `/comment/reply/`, `/filter/tips`, `/node/add/`, `/search/`, `/search?`, `/user/register`, `/user/password`, `/user/login`, `/user/logout` y `/media/oembed` (también con el prefijo `/index.php/`). **No nombra a ningún agente**, ni a `ClaudeBot`, `Claude-Web` o `anthropic-ai`, y **no excluye `/opinion/`**. No se usó el buscador.
- **User-Agent honesto en todas las peticiones:** `DobleFocoBot/1.0 (+https://doblefoco.co; doblefoco.co@gmail.com)`. Nunca el de un navegador. Cliente `curl -s --ssl-no-revoke`, una petición tras otra, **2 s de pausa** después de cada una. Una sola descarga a la vez en el dominio.
- **Fuente del propio medio.** El `sitemap.xml` solo lista secciones (25 URL), no piezas. Se usó la sección **`/opinion/editoriales`**, paginada (`?page=N`, 20 por página), de la página 0 a la 19, hasta que todas las piezas de una página fueron anteriores a la ventana.
- **Peticiones:** robots.txt (1), portada (1), sitemap (1), páginas de la sección (20), editoriales (400, de ellos 3 con un 502 del servidor que se repitieron una vez y respondieron 200). **Unas 426.**
- **Fecha y título:** `article:published_time` y `og:title` de cada pieza. La pieza se marca como «EDITORIAL» en su descripción y no lleva firma.
- **No se tocaron** eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. Ni buscadores ni Internet Archive. Ningún muro: los editoriales se sirven abiertos. Descargas en una carpeta temporal fuera del repositorio; no se ejecutó nada desde ella.

### Voz de la casa

**Los editoriales de La Patria son la voz de la casa por definición**: sin firma, marcados «EDITORIAL», en primera persona del plural («Coincidimos con los tributaristas…», «Invitamos al presidente…»). El 20-06-2026 el diario se presenta a sí mismo en uno («LA PATRIA, la historia y el futuro»). **No se barrieron** las columnas de opinión (firmadas por terceros), las caricaturas ni los titulares de las secciones de noticias (§7).

### Lectura y clases

- De los 365 editoriales de la ventana (**360 distintos**: cinco se publicaron dos veces con otra URL), se sacó el texto completo del cuerpo y **se leyeron las frases que tocan al Gobierno nacional, al presidente, a las candidaturas o a los partidos** (filtro por términos: Petro, De la Espriella, Abelardo, Gobierno, presidente, Cepeda, Paloma, Fajardo, izquierda, derecha, Pacto, candidato, uribismo, petrismo). Los que no tocan esos temas (la mayoría son de Manizales y Caldas) se clasificaron por el título y el arranque.
- **Clases** (las de los barridos de KienyKe y NTN24):
  - **D**, dirección derecha (cuenta): elogio o disculpa del candidato o del Gobierno De la Espriella; rótulo descalificador contra Petro, la izquierda o sus candidatos que va más allá de fiscalizar un acto (alineamiento con dictaduras, juicio sobre la persona); crítica a un candidato de la izquierda. Después del 07-08, el rótulo contra el gobierno saliente ya no fiscaliza a quien manda y cuenta. **D (leve)**: lo mismo con menos carga o con matiz. **D (encuadre)**: hace suyo, sin contraste, el relato del Gobierno sobre su antecesor.
  - **I**, dirección izquierda (cuenta): lo simétrico, incluida la crítica al candidato o al presidente electo de la derecha antes de que gobierne.
  - **M**, mixta: postura repartida en la misma pieza. No suma.
  - **F**, fiscaliza a quien gobierna, aunque el tono sea duro. No suma (polo fijo; precisión del 2026-10-09).
  - **X**, sin postura en el eje.

---

## 2. Cobertura y huecos

| Universo | En la ventana | Leídos | Cuentan |
|---|---:|---:|---|
| Editoriales (voz de la casa) | 360 distintos (365 URL) | Todos: las frases sobre Gobierno y candidaturas; el resto, título y arranque | Sí |
| Columnas de opinión firmadas | sin contar | 0 | No |
| Titulares de las secciones de noticias | cientos | 0 | Hueco |

Por periodo: **297 URL antes del cambio y 68 después.** El diario publica un editorial al día, a veces dos.

**Huecos que se declaran:**

- **La lectura es por frases.** Se leyeron enteras las frases que nombran al Gobierno o a las candidaturas, no cada editorial de principio a fin. Un editorial con postura expresada sin esos términos pudo quedar como X.
- **La mayor parte del corpus es regional.** Aerocafé, Autopistas del Café, la salud en Caldas, la Federación de Cafeteros, el terremoto del 10 de agosto. Cuando el diario critica al Gobierno nacional lo hace casi siempre desde un asunto de la región; eso se clasificó F, no D.
- **No se barrieron** las columnas ni los titulares de noticias.

---

## 3. Las piezas con dirección o mixtas

Todas en `https://www.lapatria.com/opinion/editoriales/<slug>`. Fragmentos literales del texto descargado.

### 3.1 Antes del cambio: 2025-10-12 → 2026-08-06 (gobierna Petro)

| # | Fecha | Título literal (enlace) | Clase | Fragmento literal o nota |
|---|---|---|---|---|
| 1 | 2025-10-27 | [Consulta de una izquierda menguada](https://www.lapatria.com/opinion/editoriales/consulta-de-una-izquierda-menguada) | **D (leve)** | «Son cifras que muestran unos partidos de izquierda menguados»; «fue una consulta que efectivamente contó con la maquinaria del Estado» |
| 2 | 2026-02-02 | [Tiempo para limar asperezas](https://www.lapatria.com/opinion/editoriales/tiempo-para-limar-asperezas) | **D (leve)** | Contra el candidato de la izquierda: «Rechazable desde todo punto de vista que el precandidato presidencial Iván Cepeda […] se haya tomado atribuciones de convocar a marchas» |
| 3 | 2026-02-05 | [Fue un encuentro positivo](https://www.lapatria.com/opinion/editoriales/fue-un-encuentro-positivo) | M | Elogia el resultado de la reunión Petro–Trump («terminó de manera positiva») y lo usa contra él: «Cuánto nos habríamos evitado como país si el presidente Petro hubiese escogido desde sus inicios la estrategia del diálogo» |
| 4 | 2026-02-13 | [La suspensión no es solo retórica](https://www.lapatria.com/opinion/editoriales/la-suspension-no-es-solo-retorica) | M | Reparte: un país «gobernado por ideólogos y no por técnicos, mientras la oposición se parapeta en que todos los males actuales del país son únicamente propiciados por este Gobierno» |
| 5 | 2026-03-08 | [Después de las consultas](https://www.lapatria.com/opinion/editoriales/despues-de-las-consultas) | **D (leve)** | Elogio a la consulta de la centroderecha: «la contundencia con que se impuso Paloma Valencia», «un mensaje de trabajo en equipo, de respeto» |
| 6 | 2026-04-16 | [Ni un candidato más asesinado](https://www.lapatria.com/opinion/editoriales/ni-un-candidato-mas-asesinado) | **I (leve)** | Rótulo contra el candidato de la derecha: «el candidato presidencial de ultraderecha y cercano al uribismo Abelardo de la Espriella» |
| 7 | 2026-05-18 | [Crear una crisis para salirse con la suya](https://www.lapatria.com/opinion/editoriales/crear-una-crisis-para-salirse-con-la-suya) | **D** | Alineamiento con una dictadura y proyección electoral: «Al mejor estilo del “exprópiese” de Hugo Chávez en Venezuela […] ahora el presidente, Gustavo Petro […]»; «La pregunta es si ese será el mismo actuar de un potencial siguiente Gobierno de la izquierda» |
| 8 | 2026-06-01 | [Hora de decir cómo y dejar los ataques personales](https://www.lapatria.com/opinion/editoriales/hora-de-decir-como-y-dejar-los-ataques-personales) | **D (leve)** | Pide a los dos «los cómo», pero lee el voto así: «Los más de 10 millones de votos de Abelardo de la Espriella expresan un país cansado con un Gobierno que ideologizó todo»; y de Cepeda: «su campaña en plaza pública, y a escondidas de los medios» |
| 9 | 2026-06-22 | [Debe venir la calma](https://www.lapatria.com/opinion/editoriales/debe-venir-la-calma) | M | Al ganador: «celebrar sin excederse en triunfalismos innecesarios ni provocadores»; del saliente: «recibirá un país descuadernado» |
| 10 | 2026-07-04 | [EE. UU. 250 años después](https://www.lapatria.com/opinion/editoriales/ee-uu-250-anos-despues) | **I (leve)** | Del presidente electo: entrará en el grupo que «seguirá el ideario Trumpista, […] tan alejado del comercio internacional, del respeto por los derechos humanos» |
| 11 | 2026-07-05 | [De la resistencia civil al capricho ideológico](https://www.lapatria.com/opinion/editoriales/de-la-resistencia-civil-al-capricho-ideologico) | **D (leve)** | Contra el candidato derrotado: «lo que terminó por hacer el senador Cepeda fue estigmatizar un derecho»; con matiz: «Cepeda mostró altura y que es un demócrata» |
| 12 | 2026-07-08 | [A ponerse serios, presidentes](https://www.lapatria.com/opinion/editoriales/ponerse-serios-presidentes) | M | A Petro: «¿Acaso prolongar su mandato?»; al electo: «una reacción vociferante» |
| 13 | 2026-07-13 | [La legitimidad es la institucionalidad](https://www.lapatria.com/opinion/editoriales/la-legitimidad-es-la-institucionalidad) | **D (leve)** | Contra el jefe de la oposición: «Resulta un pésimo mensaje de la oposición señalar que ellos son los validadores de quién es el presidente legítimo […] por arte de birlibirloque»; reparte el rótulo de populistas «de derecha o de izquierda» |
| 14 | 2026-07-22 | [La necesidad de los consensos](https://www.lapatria.com/opinion/editoriales/la-necesidad-de-los-consensos) | M | Critica a Petro y a Cepeda y advierte al electo: «la política se hace con diálogo […] y debe tener en cuenta a los otros» |
| 15 | 2026-07-27 | [¿Si será una apuesta descentralizadora?](https://www.lapatria.com/opinion/editoriales/si-sera-una-apuesta-descentralizadora) | **I (leve)** | Del electo: su idea «pareciera no ser muy novedosa»; «que no se entienda como un deseo de fortalecer la Costa Atlántica, que es su tierra natal» |
| 16 | 2026-07-28 | [Seguridad, con límites legales](https://www.lapatria.com/opinion/editoriales/seguridad-con-limites-legales) | **I (leve)** | «asusta la propuesta del presidente electo, Abelardo de la Espriella» (lo compara con las Convivir) |
| 17 | 2026-08-05 | [Respeto por la posesión presidencial](https://www.lapatria.com/opinion/editoriales/respeto-por-la-posesion-presidencial) | **D** | Juicio sobre la persona: «Petro pareciera no salir de la enajenación mental que lo persiguió estos cuatro años». Contrapeso menor en la misma pieza: «también se han criticado ideas del presidente electo […] esperamos que sea una ligereza» |
| 18 | 2026-08-06 | [Un equipo para retomar el rumbo](https://www.lapatria.com/opinion/editoriales/un-equipo-para-retomar-el-rumbo) | **D (leve)** | Del vicepresidente electo: «profesional de las más altas calidades, formación, experiencia y conocimientos»; el título da por perdido el rumbo |

### 3.2 Después del cambio: 2026-08-07 → 2026-10-12 (gobierna De la Espriella)

| # | Fecha | Título literal (enlace) | Clase | Fragmento literal o nota |
|---|---|---|---|---|
| 19 | 2026-08-07 | [No podemos quedarnos en la polarización](https://www.lapatria.com/opinion/editoriales/no-podemos-quedarnos-en-la-polarizacion) | **D (leve)** | Contra el partido del gobierno saliente: «la peligrosa posición que están asumiendo miembros del Pacto Histórico, que entraña en sí mismo una irresponsabilidad enorme, la misma con la que se gobernó durante este cuatrienio»; al entrante le pone condiciones |
| 20 | 2026-08-09 | [“El presidente de todos los colombianos”](https://www.lapatria.com/opinion/editoriales/el-presidente-de-todos-los-colombianos) | M | «Abre una esperanza su compromiso contra la corrupción, aunque sabemos que cada presidente llega con anuncios similares»; «Confiamos en que Abelardo de la Espriella mantenga el talante de lo dicho» |
| 21 | 2026-08-21 | [Que sirva para llegar a la verdad](https://www.lapatria.com/opinion/editoriales/que-sirva-para-llegar-la-verdad) | **D (encuadre)** | Hace suyo el Libro de la Verdad: «¿Ocultaba algo el Gobierno de Gustavo Petro?»; matiza: «A cada uno de los implicados se les debe dar garantía de derechos» |
| 22 | 2026-08-25 | [¿Mano negra en los incendios?](https://www.lapatria.com/opinion/editoriales/mano-negra-en-los-incendios) | **D (leve)** | «el gobierno anterior no quiso escuchar a los expertos y más bien se dedicó a hacer demagogia con el tema ambiental y climático» |
| 23 | 2026-09-06 | [De paz total, bombardeos y exhibicionismo](https://www.lapatria.com/opinion/editoriales/de-paz-total-bombardeos-y-exhibicionismo-0) | M | «El presidente de la República hace bien en pasar a la ofensiva […] pero no son necesarios exhibicionismos»; del saliente: «ese mal llamado proceso». Publicado dos veces (06-09 y 07-09); se cuenta una |
| 24 | 2026-09-21 | [Más que nunca, Creer en Caldas](https://www.lapatria.com/opinion/editoriales/mas-que-nunca-creer-en-caldas) | **D (leve)** | «hay oportunidades con la llegada del nuevo Gobierno, con un discurso muy distinto al de desconfianza en la inversión privada que mostraba el anterior» |
| 25 | 2026-09-24 | [A los toros, por los cachos](https://www.lapatria.com/opinion/editoriales/los-toros-por-los-cachos) | **D** | «El anterior Gobierno, tan dado a producir normas populistas sin reflexión económica»; «el Gobierno de Abelardo de la Espriella que poco a poco ha ido desmontando exabruptos del anterior cuatrienio» |

---

## 4. La fiscalización (F), que no suma y es el contrapeso

### 4.1 Al Gobierno Petro, antes del cambio: unos 80 editoriales

Críticas en voz propia al Gobierno nacional, casi todas desde un asunto concreto (salud, Nueva EPS, peajes de Autopistas del Café, Aerocafé, vivienda, salario mínimo, emergencia económica, paz total, relación con EE. UU., seguridad). Muchas con tono duro («Perverso que el presidente Petro…», 12-03; «Enceguecido, como acostumbra…», 02-06; «Este Gobierno improvisador», 16-06; «Es un fin populista», 30-12), que se clasificaron F porque juzgan un acto del gobierno vigente. Lista, por fecha:

[2025-10-12](https://www.lapatria.com/opinion/editoriales/la-seriedad-de-las-alertas-electorales) · [10-13](https://www.lapatria.com/opinion/editoriales/mas-riesgos-que-someten-la-seguridad-nacional) · [10-16](https://www.lapatria.com/opinion/editoriales/no-hay-que-forzar-los-dialogos-de-paz) · [10-20](https://www.lapatria.com/opinion/editoriales/de-las-acusaciones-las-afectaciones) · [10-22](https://www.lapatria.com/opinion/editoriales/politica-sin-penalidad) · [10-24](https://www.lapatria.com/opinion/editoriales/una-semana-de-tension) · [10-30](https://www.lapatria.com/opinion/editoriales/decisiones-responsables) · [11-05](https://www.lapatria.com/opinion/editoriales/que-no-se-vuelva-repetir) · [11-08](https://www.lapatria.com/opinion/editoriales/avances-y-retos-regionales) · [11-15](https://www.lapatria.com/opinion/editoriales/el-mal-momento-del-multilateralismo-0) · [11-16](https://www.lapatria.com/opinion/editoriales/esperan-que-sea-la-hora-del-macroproyecto-san-jose) · [11-19](https://www.lapatria.com/opinion/editoriales/los-bombardeos-y-los-menores) · [11-20](https://www.lapatria.com/opinion/editoriales/la-necesaria-desclasificacion-de-archivos-de-inteligencia) · [11-30](https://www.lapatria.com/opinion/editoriales/sin-sesgos-por-la-inteligencia-0) · [12-07](https://www.lapatria.com/opinion/editoriales/inevitables-alzas-del-gas) · [12-13](https://www.lapatria.com/opinion/editoriales/gobierno-en-dificultades) · [12-18](https://www.lapatria.com/opinion/editoriales/segundo-fracaso-de-reforma) · [12-30](https://www.lapatria.com/opinion/editoriales/alarmante-237) · [12-30](https://www.lapatria.com/opinion/editoriales/bienvenido-2026) · [2026-01-02](https://www.lapatria.com/opinion/editoriales/dignidad-para-las-familias-buscadoras) · [01-06](https://www.lapatria.com/opinion/editoriales/no-es-momento-de-acrecentar-conflictos) · [01-07](https://www.lapatria.com/opinion/editoriales/escalada-de-precios-0) · [01-10](https://www.lapatria.com/opinion/editoriales/otra-arremetida-contra-la-construccion) · [01-10](https://www.lapatria.com/opinion/editoriales/se-mantiene-la-incertidumbre-economica) · [01-14](https://www.lapatria.com/opinion/editoriales/emergencia-economica-sin-sustento) · [01-16](https://www.lapatria.com/opinion/editoriales/la-indiferencia-del-gobierno-petro) · [01-19](https://www.lapatria.com/opinion/editoriales/un-ano-de-crisis-humanitaria) · [01-23](https://www.lapatria.com/opinion/editoriales/aranceles-la-nueva-arma-de-presion) · [01-23](https://www.lapatria.com/opinion/editoriales/buscar-salvavidas-para-el-empleo) · [02-09](https://www.lapatria.com/opinion/editoriales/medicamentos-que-estan-costando-vidas) · [02-13](https://www.lapatria.com/opinion/editoriales/cerrarle-espacios-la-corrupcion) · [02-24](https://www.lapatria.com/opinion/editoriales/de-mexico-colombia) · [02-26](https://www.lapatria.com/opinion/editoriales/vigilar-la-eleccion-con-rigor-tecnico) · [02-27](https://www.lapatria.com/opinion/editoriales/cortinas-constituyentes) · [03-06](https://www.lapatria.com/opinion/editoriales/lineas-ferreas-mas-que-una-promesa) · [03-06](https://www.lapatria.com/opinion/editoriales/por-un-voto-etico-y-responsable) · [03-12](https://www.lapatria.com/opinion/editoriales/no-mas-contra-la-salud-de-los-colombianos) · [03-13](https://www.lapatria.com/opinion/editoriales/llego-la-hora-de-reducir-el-abanico-politico) · [03-17](https://www.lapatria.com/opinion/editoriales/una-positiva-reconexion-con-africa) · [03-20](https://www.lapatria.com/opinion/editoriales/cuatro-anos-y-la-vivienda-frenada) · [03-20](https://www.lapatria.com/opinion/editoriales/mas-bien-reducir-el-gasto) · [03-26](https://www.lapatria.com/opinion/editoriales/se-desequilibra-la-red-de-salud) · [03-27](https://www.lapatria.com/opinion/editoriales/confa-una-fortaleza-regional) · [03-27](https://www.lapatria.com/opinion/editoriales/hechos-que-causan-repudio-nacional) · [03-27](https://www.lapatria.com/opinion/editoriales/para-que-cambiar-el-regimen-sindical) · [04-01](https://www.lapatria.com/opinion/editoriales/la-independencia-del-banco-de-la-republica-inquebrantable) · [04-08](https://www.lapatria.com/opinion/editoriales/ministro-jaramillo-ojala-llegue-anunciar-soluciones) · [04-10](https://www.lapatria.com/opinion/editoriales/de-la-paz-total-solo-cenizas-quedan) · [04-10](https://www.lapatria.com/opinion/editoriales/el-pasaporte-como-derecho) · [04-15](https://www.lapatria.com/opinion/editoriales/reflexiones-tras-las-protestas) · [04-16](https://www.lapatria.com/opinion/editoriales/el-mal-momento-con-ecuador) · [04-17](https://www.lapatria.com/opinion/editoriales/actualizacion-catastral-una-responsabilidad-compartida) · [04-17](https://www.lapatria.com/opinion/editoriales/exigir-sin-parar-clases) · [04-21](https://www.lapatria.com/opinion/editoriales/ni-quintero-ni-ospina) · [04-22](https://www.lapatria.com/opinion/editoriales/ligerezas-del-ministro-de-trabajo) · [04-25](https://www.lapatria.com/opinion/editoriales/democracia-en-riesgo) · [04-28](https://www.lapatria.com/opinion/editoriales/no-mas-tolerancia-con-el-terrorismo) · [04-30](https://www.lapatria.com/opinion/editoriales/empleo-en-medio-de-fuertes-presiones) · [05-07](https://www.lapatria.com/opinion/editoriales/evitar-la-especulacion) · [05-08](https://www.lapatria.com/opinion/editoriales/ley-que-no-se-puede-quedar-en-el-papel) · [05-11](https://www.lapatria.com/opinion/editoriales/mas-premios-para-los-delincuentes) · [05-15](https://www.lapatria.com/opinion/editoriales/asumir-los-compromisos) · [05-19](https://www.lapatria.com/opinion/editoriales/nadie-asume-el-doble-gasto-en-salud) · [05-21](https://www.lapatria.com/opinion/editoriales/voto-libre) · [05-23](https://www.lapatria.com/opinion/editoriales/deberia-volver-el-pico-y-placa-ambiental) · [05-25](https://www.lapatria.com/opinion/editoriales/la-voz-de-la-region-sobre-las-concesiones) · [05-27](https://www.lapatria.com/opinion/editoriales/el-compromiso-de-la-registraduria) · [06-02](https://www.lapatria.com/opinion/editoriales/fue-una-eleccion-con-garantias) · [06-09](https://www.lapatria.com/opinion/editoriales/por-10-anos-mas) · [06-15](https://www.lapatria.com/opinion/editoriales/mineria-e-hidrocarburos-no-son-los-enemigos) · [06-16](https://www.lapatria.com/opinion/editoriales/que-si-que-no-los-peajes-700) · [06-25](https://www.lapatria.com/opinion/editoriales/convenir-lo-mejor-para-los-cafeteros) · [06-26](https://www.lapatria.com/opinion/editoriales/otro-escandalo-del-gobierno-que-pide-claridades) · [07-03](https://www.lapatria.com/opinion/editoriales/responsabilidad-con-la-doble-calzada) · [07-12](https://www.lapatria.com/opinion/editoriales/la-constitucion-sigue-siendo-el-camino) · [07-21](https://www.lapatria.com/opinion/editoriales/imponen-el-prohibicionismo-en-los-toros) · [07-26](https://www.lapatria.com/opinion/editoriales/que-no-sea-otra-trapisonda-para-caldas) · [07-29](https://www.lapatria.com/opinion/editoriales/se-requiere-ministra-1a) · [08-01](https://www.lapatria.com/opinion/editoriales/transformar-la-percepcion-del-pais) · [08-04](https://www.lapatria.com/opinion/editoriales/lecciones-desde-nueva-york)

(80 editoriales; los publicados dos veces se cuentan una.)

### 4.2 Al Gobierno De la Espriella, después del cambio: 12 editoriales en 9 semanas

| Fecha | Título literal (enlace) | Fragmento literal |
|---|---|---|
| 2026-08-24 | [El camino correcto es el multilateralismo](https://www.lapatria.com/opinion/editoriales/el-camino-correcto-es-el-multilateralismo) | «Que el recientemente posesionado Gobierno busque estrechar lazos con Israel es importante, pero no puede hacerlo a costa de renunciar a la juridicidad internacional» |
| 2026-08-28 | [Contra el unanimismo](https://www.lapatria.com/opinion/editoriales/contra-el-unanimismo) | «invitamos al nuevo Gobierno nacional a dejar la actitud macartista que empieza a hacer ruido»; «El Gobierno no puede repetir la forma de actuar de su antecesor» |
| 2026-08-31 | [Del sueño bolivariano y la aporofobia](https://www.lapatria.com/opinion/editoriales/del-sueno-bolivariano-y-la-aporofobia) | «no es xenofobia lo que mueve a las naciones a tomar este tipo de decisiones que ahora promueve De la Espriella, sino aporofobia» |
| 2026-09-10 | [Sin parámetros no hay reconstrucción](https://www.lapatria.com/opinion/editoriales/sin-parametros-no-hay-reconstruccion) | «ya se requiere pasar a los hechos, porque las necesidades de los damnificados no dan espera» |
| 2026-09-25 | [45 días después](https://www.lapatria.com/opinion/editoriales/45-dias-despues) | «no ha logrado que el Gobierno nacional trascienda del compromiso de que apoyará en todo». Publicado dos veces; se cuenta uno |
| 2026-09-26 | [10 años, y el conflicto ahí](https://www.lapatria.com/opinion/editoriales/10-anos-y-el-conflicto-ahi) | «Esa miopía es la misma en la que incurrió Gustavo Petro y en la que parece caer el actual Gobierno»; la institucionalidad del acuerdo «ahora está amenazada por el presidente Abelardo de la Espriella» |
| 2026-09-28 | [Los tales paros armados sí existen](https://www.lapatria.com/opinion/editoriales/los-tales-paros-armados-si-existen) | «el reto del Gobierno de AdlE es justamente no incurrir en este error» |
| 2026-10-04 | [De la independencia de los gremios](https://www.lapatria.com/opinion/editoriales/de-la-independencia-de-los-gremios) | «No puede ser que fuera malo tal intervencionismo del Estado en los gremios cuando se trataba de un gobierno de izquierda y está bien si se trata de uno de derecha»; «en este Gobierno, parece pensar más con ánimo sectario» |
| 2026-10-09 | [Riesgosa “encarguitis” en el Sena](https://www.lapatria.com/opinion/editoriales/riesgosa-encarguitis-en-el-sena) | «Bastante inquietante que el Gobierno nacional, antes de nombrar personas en interinidad, no haya procedido de una vez a reactivar el concurso de méritos» |
| 2026-10-10 | [Un Fondo del que se esperan más que milagros](https://www.lapatria.com/opinion/editoriales/un-fondo-del-que-se-esperan-mas-que-milagros) | Exige transparencia: «se debe dar a conocer la cantidad desglosada de dineros recibidos, su procedencia y su distribución» |
| 2026-10-11 | [Increíble: falta de certezas con Aerocafé](https://www.lapatria.com/opinion/editoriales/increible-falta-de-certezas-con-aerocafe) | «pasaron ya dos meses del nuevo Gobierno y las esperadas determinaciones no llegan»; también: «un coletazo de las malas decisiones del Gobierno anterior» |
| 2026-10-12 | [Los taurinos esperan apoyo presidencial](https://www.lapatria.com/opinion/editoriales/los-taurinos-esperan-apoyo-presidencial) | Reclama al Gobierno que derogue el decreto de Petro: «aún no hay decisiones tomadas» |

Más cuatro exigencias suaves al nuevo Gobierno sobre la reconstrucción, los cafeteros y las pensiones (11-08, 20-08, 01-09, 04-09), que no se suman aquí.

---

## 5. Recuento y veredicto

| | D | I | M | F (a quien gobierna) |
|---|---:|---:|---:|---:|
| Antes del 07-08-2026 | 9 (2 claras y 7 leves) | 4 (leves) | 5 | ~80 |
| Desde el 07-08-2026 | 5 (1 clara, 3 leves y 1 de encuadre) | 0 | 2 | 12 |
| **Total** | **14** | **4** | **7** | **~92** |

**Piezas con dirección: 18. En la misma dirección: 14 a la derecha frente a 4 a la izquierda, 3,5 a 1.** Sin las leves y la de encuadre: **3 a 0.**

**La prueba del polo fijo.**

- **La fiscalización no cambia con el gobierno.** Unos 80 editoriales críticos con Petro en 43 semanas (casi 2 por semana) y 12 con De la Espriella en 9 (1,3 por semana), con la misma dureza: «actitud macartista», «aporofobia», «ánimo sectario», la institucionalidad de la paz «amenazada por el presidente». El editorial del 04-10 enuncia la regla del polo fijo con sus palabras: «No puede ser que fuera malo tal intervencionismo […] cuando se trataba de un gobierno de izquierda y está bien si se trata de uno de derecha».
- **La dirección está en otra parte**: en el trato a las candidaturas durante la campaña (críticas a Cepeda y a la izquierda, elogio a la consulta de Paloma Valencia, frente a cuatro críticas leves al candidato y presidente electo de la derecha), y, ya con el nuevo gobierno, en los rótulos contra el saliente («normas populistas», «demagogia», «exabruptos del anterior cuatrienio»).

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | Sí | Editoriales sin firma |
| 2. A los dos lados del cambio | Sí | 9 D antes del 07-08 y 5 después |
| 3a. ≥10 piezas con postura | Sí, con las leves | 18 con dirección; 3 sin las leves |
| 3b. ≥3 a cada lado (solo elogios, disculpas y rótulos) | Sí, con las leves | 9 y 5; sin las leves, 2 y 1 |
| 3c. Proporción ≥3 a 1 | Sí, por poco | 14 a 4 (3,5 a 1). Con tres D leves recalificadas como M se baja de 3 a 1 (11 a 4 = 2,75) |
| 4. Contrapesos escritos | Sí | §6 |
| 5. Reproducible | Sí | Tablas del §3 y listas del §4 |

**Rama de la precisión del 2026-10-10: la primera** («cumple las cinco condiciones → el valor del barrido, con el tope de ±0,30»), porque el valor vigente se apoya solo en los niveles 4 y 5. **Sin endoso explícito**: ningún editorial pide el voto; el del día de la segunda vuelta («El día de las decisiones», 21-06) no toma partido. Tope ±0,30. El valor exacto es un juicio declarado (§7).

**La rama alternativa, que hay que dejar escrita.** Si se descuentan las leves, como propone la regla 2 ante la duda, el barrido no llega a los mínimos y documenta **la misma conducta con los dos gobiernos** (≥3 F a cada lado; postura 3 a 0 con piezas claras, que con tres piezas no es una dirección): **rama 2, 0,00 con evidencia.**

---

## 6. Contrapesos

- **Fiscaliza al nuevo gobierno, y fuerte.** Es el contrapeso principal, y pesa: en 9 semanas, 12 editoriales críticos con De la Espriella, varios por asuntos de principio (justicia internacional, migración, independencia de los gremios, la JEP), no solo regionales. Un medio que acompaña al ganador no escribe «actitud macartista» al mes de la posesión. **Peso alto.**
- **Cuatro críticas al candidato y presidente electo de la derecha** durante la transición (ultraderecha, ideario trumpista, descentralización, Convivir). Son leves, pero existen. **Peso medio.**
- **Siete piezas mixtas** que reparten entre los dos lados (§3). **Peso medio.**
- **La dureza con Petro es fiscalización**, y es la mayoría del corpus: casi siempre por un asunto concreto de la región o de la política pública. No se contó como dirección, salvo dos piezas que pasan del acto a la persona o al régimen («enajenación mental», el «exprópiese» chavista).
- **El valor vigente (+0,25) no tenía lectura detrás.** Este barrido es la primera evidencia.

---

## 7. PROPUESTA (pendiente de firma)

- **Valor: +0,10**, dentro de la banda mixta. Rama 1 de la precisión: cumple los mínimos, pero solo con las leves, por poco en la proporción (3,5 a 1), y con un contrapeso de peso alto. Juicio declarado frente a los vecinos:
  - **KienyKe, +0,30:** 9 a 1, y casi nada de fiscalización al nuevo gobierno (1 pieza). La Patria fiscaliza al nuevo gobierno 12 veces: no puede estar a su altura.
  - **Noticias RCN, +0,15:** 5,5 a 1, con la mayoría leves, y 2 fiscalizaciones a De la Espriella. La Patria tiene menos proporción (3,5 a 1) y mucha más fiscalización del entrante: por debajo.
  - **El Pilón, +0,20:** no llega a 3 a 1 y conserva su valor por otra vía. La Patria sí llega, pero no con piezas claras.
  - **Las2Orillas, 0,00 con evidencia:** misma conducta con los dos gobiernos y sin dirección. La Patria tiene dirección en las candidaturas y en el trato al saliente, aunque leve.
  - Ante la duda entre +0,10 y +0,15, se elige el más cercano a la mixta (regla 2).
- **Alternativa: 0,00 con evidencia** (rama 2), si el responsable editorial no da por buenas las leves. Es la lectura más estricta, y la que se sostiene con solo las piezas claras.
- **No se propone mantener +0,25**: no hay piezas que lo sostengan y la fiscalización del nuevo gobierno lo contradice.
- **Ficha técnica:** se crea, mínima, en `fichas/la-patria.md`. **No se toca el registro, el perfil de propiedad ni el texto público.**
- **Revisión:** recontar en enero de 2027 si la fiscalización del nuevo Gobierno se sostiene (hoy, 12 piezas) y si los rótulos contra el saliente crecen o se apagan.
