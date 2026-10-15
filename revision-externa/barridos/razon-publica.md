# Barrido editorial: Razón Pública

| | |
|---|---|
| **Medio** | Razón Pública (`razon-publica`), Fundación Razón Pública. No noticioso desde el 2026-09-16: fuera del mapa, dentro del agrupamiento |
| **Valor vigente** | **−0,40**, sin firmar (`reviewedAt: null`). Viene del alta del catálogo (commit `75019ce`, 2026-07-27) con la razón «Análisis académico con énfasis en política social y crítica al modelo económico vigente». No consta en `DECISIONES.md` ninguna decisión que lo fije ni evidencia que lo sostenga |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus dos precisiones |
| **Ventana** | 2025-10-10 → 2026-10-10 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Resolución de origen** | `revision-externa/respuestas/opus-5-5-razon-publica.md` (el revisor leyó las 31 piezas del director y propuso «mixta o izquierda moderada muy leve») |
| **Quién lo hizo** | Claude Opus 5.5 (`claude-opus-5-5`), verificador del ciclo 2, tanda 8, a petición del responsable editorial, el 2026-10-10. Es de la misma casa que el autor de la ficha y que el revisor, así que su acuerdo no es aval |
| **Estado** | **DECIDIDO el 2026-10-10: sin medir** (antes −0,40), por el responsable editorial (`DECISIONES.md`, «2026-10-10 · Tandas 8 y 9 del ciclo 2: el barrido manda sobre los números sin evidencia»). Lo que más abajo dice «propuesta», «recomendada» o «pendiente» es el estado anterior a la decisión y se conserva como historia |
| **Resultado** | **No cumple las condiciones de la regla.** Las 31 piezas del director, leídas enteras, dan 2 con dirección (izquierda leve), 0 con dirección derecha, 6 de recomendación o defensa del centro, 10 mixtas, 3 que solo fiscalizan a quien manda y 10 fuera del eje. **Después del 07-08 no hay ninguna pieza con postura que cuente:** 2 fiscalizan, 1 es mixta y 1 no tiene postura. Los 42 boletines y las 8 síntesis firmadas por «Equipo Razón Pública» no tienen postura propia: todo lo que dicen va atribuido a un autor o a un panel |

> Quien lo rehaga puede llegar a otro número. Las URL, las fechas, el
> fragmento y el método están aquí para eso. **La clasificación de cada pieza
> es el juicio de un solo lector**, de la misma casa que el autor de la ficha y
> que el revisor.

---

## 1. Método

- **robots.txt** de `razonpublica.com` (descargado el 2026-10-10): `User-agent: *` con `Disallow` solo en rutas de WooCommerce (`/wp-content/uploads/wc-logs/`, `woocommerce_*`, `?add-to-cart=`) y `/wp-admin/`. El bloque de Yoast deja `Disallow:` vacío. No nombra a ClaudeBot, Claude-Web ni anthropic-ai.
- **Descarga:** `curl -sL --ssl-no-revoke` con User-Agent de navegador, con pausas de 4 a 8 s. **El cortafuegos del sitio (nginx) devolvió 403** a `/wp-json/wp/v2/posts`, a `?rest_route=`, a `/feed/?paged=2`, a los `post-sitemap*.xml` y a los feeds de categoría durante toda la sesión. A ráfagas también lo devolvió a páginas sueltas; al reintentar más despacio, o con otro User-Agent, respondieron 200. `/wp-json/wp/v2/categories` sí respondió. **Por eso este barrido no rehace el recuento de 845 entradas que el revisor sacó de la API**, y usa el archivo de cada autor, que es HTML público.
- **Quién es «voz de la casa» aquí.** Razón Pública no publica editoriales sin firma. Lo que el protocolo cuenta como voz de la casa son los textos «firmados por la casa o su director» y los «análisis propios no atribuidos a una fuente». Eso da tres universos, y se barrieron completos:
  1. **El director y editor general**, Hernando Gómez Buendía (`/author/hernandogb/`, páginas 1 a 4). Son 31 piezas en la ventana, del 2025-10-20 al 2026-10-05. **Se leyó el cuerpo entero de las 31.** La fecha es el `datePublished` del JSON-LD, en UTC. Coincide con la del revisor en las 31; el archivo del autor muestra a veces el día anterior, por la zona horaria.
  2. **«Equipo Razón Pública»** (`/author/razonpublica/`, páginas 1 a 7). Son 50 piezas en la ventana: 42 boletines semanales («EDICIÓN DEL…», categoría Boletín) y 8 síntesis de conversatorios. **Se leyeron las 50 enteras.**
  3. **Las caricaturas de B&B** (`/author/b-b/`, páginas 1 a 7), que la casa lista en «Nuestro equipo» («BYB — Caricaturas»). Son 40 en la ventana. **Solo se leyeron los títulos**: la postura de una caricatura está en la imagen, y las imágenes no se abrieron.
- **Lo que no es voz de la casa y no se barrió:** las columnas y análisis firmados por terceros, que son casi todo el sitio. Entre ellos están los miembros del Consejo Directivo de la fundación que firman con su nombre (ver §6).
- **Clases** (la misma lógica que los barridos de El Diario y El Informador, adaptada a una casa que no endosa):
  - **I**, dirección izquierda (cuenta): rótulo descalificador en voz propia contra la derecha o sus candidatos, sin contrapartida en la misma pieza; elogio, disculpa o recomendación para la izquierda.
  - **D**, dirección derecha (cuenta): lo simétrico.
  - **C**, centro: recomienda o defiende a candidatos o posiciones de centro y rechaza en la misma pieza a los dos polos. **No suma a ninguna dirección.**
  - **M**, mixta: postura sobre el eje repartida entre los dos lados, institucional o descriptiva. No suma.
  - **F**, solo fiscaliza a quien manda. No suma, por la precisión del responsable editorial del 2026-10-09.
  - **X**, fuera: internacional, promoción del libro del director, crónica en tercera persona o sin postura en el eje.

---

## 2. Las 31 piezas del director

Todas en `https://razonpublica.com/<slug>/`. La sección es el `articleSection` del JSON-LD. Los fragmentos se comprobaron contra el HTML crudo el 2026-10-10.

### 2.1 Antes del cambio: 2025-10-10 → 2026-08-06 (gobierna Petro)

| # | Fecha | Pieza | Sección | Clase | Fragmento literal |
|---|---|---|---|---|---|
| 1 | 2025-10-20 | [machado-trump-petro](https://razonpublica.com/machado-trump-petro/) | Columna | X | Internacional (Nobel a Machado). De paso fiscaliza a Petro: «Petro habla desde el idealismo del militante, pero olvida que su único papel es el de ser presidente de Colombia» |
| 2 | 2025-11-04 | [el-elefante-indigestado](https://razonpublica.com/el-elefante-indigestado/) | Columna | X | Internacional: «la "América profunda", blanca, rural, evangélica, racista» |
| 3 | 2025-11-18 | [las-elecciones-vienen-tres-matrimonios-forzados](https://razonpublica.com/las-elecciones-vienen-tres-matrimonios-forzados/) | Columna | M | De Cepeda: «al resto del país lo asusta demasiado». De Abelardo: «la pasión, la bandera, la arenga y la plata rara» |
| 4 | 2025-12-01 | [incendio-en-el-vecindario](https://razonpublica.com/incendio-en-el-vecindario/) | Columna | X | Internacional (Trump y Venezuela) |
| 5 | 2025-12-15 | [el-imperio-como-victima](https://razonpublica.com/el-imperio-como-victima/) | Columna | X | Internacional. Su párrafo colombiano critica a los dos lados: «Los gremios y la "gente de bien" se rasga las vestiduras…» y «Petro, por su parte, culpa a los gringos…» |
| 6 | 2026-01-12 | [despues-maduro-vacio](https://razonpublica.com/despues-maduro-vacio/) | Internacional | X | Internacional |
| 7 | 2026-01-12 | [venezuela-nadie-manda](https://razonpublica.com/venezuela-nadie-manda/) | Columna | X | Internacional |
| 8 | 2026-01-26 | [colombia-despues-petro-lecciones-del-gobierno-del-cambio](https://razonpublica.com/colombia-despues-petro-lecciones-del-gobierno-del-cambio/) | Política | X | Presentación de su libro, con nota de la casa: «No busca adhesiones ni aplausos» |
| 9 | 2026-02-09 | [las-consultas-del-8-marzo-una-equivocacion](https://razonpublica.com/las-consultas-del-8-marzo-una-equivocacion/) | Política, Voto Informado | **I (leve)** | «Paloma Valencia es la caverna con buenos modales». De Abelardo: «personalista, punitivo y moralizante». Sin rótulo equivalente para la izquierda; a Barreras y Quintero los llama los más versados «en el arte de las componendas» |
| 10 | 2026-02-09 | [problema-no-petro](https://razonpublica.com/problema-no-petro/) | Columna | M | «Petro hizo más de lo que dicen sus críticos y menos de lo que pudo haber hecho» |
| 11 | 2026-02-23 | [los-dos-petros](https://razonpublica.com/los-dos-petros/) | Columna | F | «el Petro agresivo, dogmático y autoritario». Critica también a la oposición: «La oposición ha respondido mal» |
| 12 | 2026-03-02 | [colombia-despues-petro-viaje-incomodo-al-corazon-del-pais](https://razonpublica.com/colombia-despues-petro-viaje-incomodo-al-corazon-del-pais/) | Política | X | Crónica en tercera persona de la presentación del libro («Hernando Gómez Buendía presentó…»). No es su voz |
| 13 | 2026-03-02 | [tres-consultas-suicidas](https://razonpublica.com/tres-consultas-suicidas/) | Política, Voto Informado | M | «la muy uribista Paloma Valencia»; de Abelardo, «una platica (no sé yo de dónde)»; de Quintero, «maquinaria-demagogia» |
| 14 | 2026-03-07 | [quien-elegimos-hoy](https://razonpublica.com/quien-elegimos-hoy/) | Columna | **C** | Recomienda a López en las consultas: «Si a usted le preocupa Cepeda, López es el dique más eficaz […] Si le preocupa de la Espriella, Claudia es el dique más eficaz». La describe como «una progresista institucionalista» |
| 15 | 2026-03-09 | [la-paz-los-mercaderes](https://razonpublica.com/la-paz-los-mercaderes/) | Internacional | X | Internacional: «dictadores de extrema derecha» |
| 16 | 2026-03-23 | [anatomia-las-candidaturas-presidenciales](https://razonpublica.com/anatomia-las-candidaturas-presidenciales/) | Política, Voto Informado | **C** | «Cepeda entiende todo de derechos y reclamos sociales, pero en cambio entiende nada de crecimiento económico o clima de inversión». De Abelardo: «la versión más radical de la derecha colombiana». Fajardo y su fórmula son «dos educadores de probados quilates que el país necesita» |
| 17 | 2026-03-23 | [elecciones-lo-siempre](https://razonpublica.com/elecciones-lo-siempre/) | Columna | **I (leve)** | «la derecha cerril de Abelardo de la Espriella o el uribismo disfrazado de centro de Paloma Valencia». Cierra simétrico: «Nadie que condene a los unos y a los otros…» |
| 18 | 2026-04-06 | [lo-malo-lo-peor](https://razonpublica.com/lo-malo-lo-peor/) | Columna | **C** | Petro y Cepeda «están completamente equivocados en materias de paz, economía, políticas sociales y política internacional»; Abelardo, «un fascismo estridente y ramplón», «un patán exitoso»; «López y Fajardo, la centroizquierda y la centroderecha verdaderas» |
| 19 | 2026-04-20 | [suicidio-del-centro](https://razonpublica.com/suicidio-del-centro/) | Columna | **C** | «Sergio Fajardo representa la centroderecha moderna […] Y tiene razón»; «La izquierda lo llama neoliberalismo. La derecha lo llama tibieza. Yo lo llamo civilización.» |
| 20 | 2026-05-18 | [defensa-del-centro](https://razonpublica.com/defensa-del-centro/) | Columna | **C** | «Cepeda y Paloma son personas decentes. […] Abelardo no pertenece a esa categoría»; «Los extremos ofrecen identidad. El centro ofrece realidad.» |
| 21 | 2026-05-31 | [que-elegimos-hoy](https://razonpublica.com/que-elegimos-hoy/) | Columna | **C** | Día de la primera vuelta. De Fajardo: «Es la opción racional»; de López: «la candidata que mejor podría recoger las dos mitades rotas de Colombia». De Abelardo: «su visión del poder es la del dictador». Y de Cepeda: «reformas sociales financiadas con un déficit fiscal y una deuda externa insostenibles» |
| 22 | 2026-06-01 | [primera-vuelta-las-ocho-cosas-no-se-dijeron](https://razonpublica.com/primera-vuelta-las-ocho-cosas-no-se-dijeron/) | Política, Voto Informado | M | De Cepeda: «ese también es el peligro que representa para Colombia». Pero también: «el verdadero riesgo autoritario no se llama Cepeda»; el líder de la nueva derecha es «un hombre narcisista, machista y homófobo». Y Petro, «el presidente irresponsable», «anunció un fraude» |
| 23 | 2026-06-15 | [la-otra-mitad-del-pais](https://razonpublica.com/la-otra-mitad-del-pais/) | Columna | M | No endosa a nadie en la segunda vuelta: «Esta es una elección entre dos gobiernos desastrosos.» |
| 24 | 2026-06-29 | [nuestra-arma-secreta](https://razonpublica.com/nuestra-arma-secreta/) | Columna | M | «Los seguidores de Abelardo consideran que esos controles son un obstáculo. Los seguidores de Petro pensaban exactamente lo mismo.» |
| 25 | 2026-07-13 | [la-verdadera-herencia-de-1991](https://razonpublica.com/la-verdadera-herencia-de-1991/) | Política | M | «Gustavo Petro quiere cambiar la Constitución. Abelardo de la Espriella promete defenderla.» Examina a los dos |
| 26 | 2026-07-14 | [del-empalme-a-la-pelea](https://razonpublica.com/del-empalme-a-la-pelea/) | Columna | M | Critica la auditoría del presidente electo, pero añade que la falta de información «beneficia a los funcionarios salientes»: «Unos ganan con el silencio, los otros ganan con el ruido.» |
| 27 | 2026-07-27 | [la-posesion-de-abelardo](https://razonpublica.com/la-posesion-de-abelardo/) | Columna | M | Institucional: «Ese principio no protege a Gustavo Petro. Tampoco protegerá a Abelardo de la Espriella» |

### 2.2 Después del cambio: 2026-08-07 → 2026-10-10 (gobierna De la Espriella)

| # | Fecha | Pieza | Sección | Clase | Fragmento literal |
|---|---|---|---|---|---|
| 28 | 2026-08-10 | [estado-laico](https://razonpublica.com/estado-laico/) | Columna | M | Exculpa en lo jurídico: «Abelardo de la Espriella no violó la Constitución». Critica el modelo de la Ley 133 y se burla del gabinete: «el sincretismo entre la Biblia y las abelardadas» |
| 29 | 2026-08-24 | [volvimos-a-ser-colombianos](https://razonpublica.com/volvimos-a-ser-colombianos/) | Columna | X | Sobre el terremoto; sin postura en el eje |
| 30 | 2026-09-20 | [la-insana-doctrina-de-abelardo](https://razonpublica.com/la-insana-doctrina-de-abelardo/) | Columna | F | «ser presidente no lo convierte en autoridad religiosa» |
| 31 | 2026-10-05 | [el-tigre-y-los-militares](https://razonpublica.com/el-tigre-y-los-militares/) | Columna | F | «No, señor presidente. Usted no es un soldado. Afortunadamente.» |

---

## 3. «Equipo Razón Pública»: boletines y síntesis

### 3.1 Los 42 boletines (37 antes del cambio y 5 después)

Son la presentación semanal de la edición. **Se leyeron los 42.** Cada boletín es una lista de entradillas, y cada entradilla termina atribuyendo la tesis a su autor («Analiza…», «Explica…», «Expone…», «Responde…»). Se comprobó por programa: de 523 párrafos largos, 452 terminan en una atribución. Los 71 restantes son títulos, el aviso fijo de la sección de poesía o atribuciones sin verbo («… Álvaro Duque Soto»). **Ninguno dice nada en voz propia**, así que no cuentan como voz de la casa. Ejemplo, 2026-10-05: «La crisis sigue, los 10 billones no aparecen y el discurso cambió. Petro y De la Espriella acabaron en las mismas confusiones. Expone Isabel Arroyo.»

[2025-10-14](https://razonpublica.com/edicion-del-lunes-13-octubre-al-19-octubre-2025/) · [2025-10-28](https://razonpublica.com/edicion-del-lunes-27-octubre-al-02-noviembre-2025/) · [2025-11-04](https://razonpublica.com/edicion-del-lunes-03-noviembre-al-09-noviembre-2025/) · [2025-11-11](https://razonpublica.com/edicion-del-lunes-10-noviembre-al-16-noviembre-2025/) · [2025-11-18](https://razonpublica.com/edicion-del-lunes-17-noviembre-al-23-noviembre-2025/) · [2025-11-25](https://razonpublica.com/edicion-del-lunes-24-noviembre-al-30-noviembre-2025/) · [2025-12-01](https://razonpublica.com/edicion-del-lunes-01-diciembre-al-07-diciembre-2025/) · [2025-12-09](https://razonpublica.com/edicion-del-lunes-08-diciembre-al-14-diciembre-2025/) · [2025-12-23](https://razonpublica.com/edicion-del-lunes-22-diciembre-al-11-enero-2026/) · [2026-01-15](https://razonpublica.com/edicion-del-lunes-12-de-enero-al-18-de-enero-2026/) · [2026-01-19](https://razonpublica.com/edicion-del-lunes-19-enero-al-25-enero-2026/) · [2026-01-30](https://razonpublica.com/edicion-del-26-enero-al-01-febrero-del-2026/) · [2026-02-04](https://razonpublica.com/edicion-del-02-febrero-al-08-febrero-del-2026/) · [2026-02-10](https://razonpublica.com/edicion-del-09-febrero-al-15-febrero-del-2026/) · [2026-02-18](https://razonpublica.com/edicion-del-16-febrero-al-22-febrero-del-2026/) · [2026-02-23](https://razonpublica.com/edicion-del-23-de-febrero-al-01-de-marzo-del-2026/) · [2026-03-04](https://razonpublica.com/edicion-del-02-marzo-al-08-marzo-del-2026/) · [2026-03-12](https://razonpublica.com/edicion-del-09-marzo-al-15-marzo-del-2026/) · [2026-03-16](https://razonpublica.com/edicion-del-16-marzo-al-22-marzo-del-2026/) · [2026-03-25](https://razonpublica.com/edicion-del-26-marzo-al-29-marzo-del-2026/) · [2026-04-01](https://razonpublica.com/edicion-del-30-marzo-al-05-abril-del-2026/) · [2026-04-08](https://razonpublica.com/edicion-del-06-abril-al-12-abril-del-2026/) · [2026-04-13](https://razonpublica.com/edicion-del-13-abril-al-19-abril-del-2026/) · [2026-04-21](https://razonpublica.com/edicion-del-20-abril-al-26-abril-del-2026/) · [2026-04-28](https://razonpublica.com/edicion-del-27-abril-al-03-mayo-del-2026/) · [2026-05-14](https://razonpublica.com/edicion-del-11-mayo-al-17-mayo-del-2026/) · [2026-05-19](https://razonpublica.com/edicion-del-18-de-mayo-al-24-de-mayo-del-2026/) · [2026-05-27](https://razonpublica.com/edicion-del-25-mayo-al-31-mayo-del-2026/) · [2026-06-02](https://razonpublica.com/edicion-del-01-junio-al-07-junio-del-2026/) · [2026-06-10](https://razonpublica.com/edicion-del-08-junio-al-14-junio-del-2026/) · [2026-06-19](https://razonpublica.com/edicion-del-15-junio-al-21-junio-del-2026/) · [2026-06-24](https://razonpublica.com/edicion-del-22-junio-al-28-junio-del-2026/) · [2026-07-10](https://razonpublica.com/edicion-del-06-de-julio-al-12-de-julio-del-2026/) · [2026-07-15](https://razonpublica.com/edicion-del-13-de-julio-al-19-de-julio-del-2026/) · [2026-07-22](https://razonpublica.com/edicion-del-20-de-julio-al-26-de-julio-del-2026/) · [2026-07-29](https://razonpublica.com/edicion-del-29-de-julio-al-02-de-agosto-del-2026/) · [2026-08-04](https://razonpublica.com/edicion-del-03-de-agosto-al-09-de-agosto-del-2026/) · [2026-08-11](https://razonpublica.com/edicion-del-10-de-agosto-al-16-de-agosto-del-2026/) · [2026-08-24](https://razonpublica.com/edicion-del-24-de-agosto-al-30-de-agosto-del-2026/) · [2026-08-31](https://razonpublica.com/edicion-del-31-de-agosto-al-06-de-septiembre-del-2026/) · [2026-09-22](https://razonpublica.com/edicion-del-21-de-septiembre-al-27-de-septiembre-del-2026/) · [2026-10-05](https://razonpublica.com/edicion-del-05-de-octubre-al-11-de-octubre-del-2026/)

**Un dato de financiación que sale de aquí, y no mueve el eje.** El boletín del 2026-09-22 rotula una pieza: «Es un artículo del convenio con la U. Externado y analizan Jacobo Campos y Jose Gómez». La misma pareja de autores aparece en 9 boletines de la ventana, y solo ese lo rotula. La Universidad Externado es uno de los dos «aliados» del pie (ver la resolución, objeción 1). El mismo boletín marca otra pieza «En convenio con Contexto Media».

### 3.2 Las 8 síntesis de conversatorios

| Fecha | Lado | Pieza | Firma | Clase |
|---|---|---|---|---|
| 2025-11-17 | antes | [encuestas-colombia-historia-metodologia-una-ley-cambio-juego-politico](https://razonpublica.com/encuestas-colombia-historia-metodologia-una-ley-cambio-juego-politico/) | Equipo Razón Pública | X: metodología de encuestas, atribuida a dos analistas |
| 2026-01-27 | antes | [debate-la-gente-las-tensiones-la-deliberacion-politica-una-consulta-fragmentada](https://razonpublica.com/debate-la-gente-las-tensiones-la-deliberacion-politica-una-consulta-fragmentada/) | Equipo + 2 profesores | X: atribuida |
| 2026-02-05 | antes | [trump-petro-oxigeno-diplomatico-tablero-inestable](https://razonpublica.com/trump-petro-oxigeno-diplomatico-tablero-inestable/) | Equipo + 3 analistas | X: atribuida («Según el análisis de…») |
| 2026-03-09 | antes | [elecciones-legislativas-consultas-interpartidistas-…](https://razonpublica.com/elecciones-legislativas-consultas-interpartidistas-fragmentacion-partidista-reconfiguracion-del-campo-politico-colombiano/) | 4 politólogos + Equipo | X: atribuida a la mesa redonda |
| 2026-05-11 | antes | [elecciones-2026-analisis-comparativo-las-propuestas-los-candidatos-presidenciales](https://razonpublica.com/elecciones-2026-analisis-comparativo-las-propuestas-los-candidatos-presidenciales/) | Equipo Razón Pública | M: se declara «comparativa y neutral» y describe los cinco programas sin calificar |
| 2026-06-01 | antes | [colombia-entra-lleno-la-la-antipolitica](https://razonpublica.com/colombia-entra-lleno-la-la-antipolitica/) | 4 analistas + Equipo | X: atribuida («La principal conclusión del debate…») |
| 2026-06-22 | antes | [una-eleccion-al-limite-la-mitad-pais-le-gano-la-otra-mitad](https://razonpublica.com/una-eleccion-al-limite-la-mitad-pais-le-gano-la-otra-mitad/) | Equipo Razón Pública | X: atribuida a los panelistas («Los panelistas…», «según los analistas»), incluido «un gobierno de derecha radical» |
| 2026-08-10 | después | [la-posesion-como-programa-de-gobierno-…](https://razonpublica.com/la-posesion-como-programa-de-gobierno-fuerza-simbolos-y-limites-institucionales/) | 3 analistas + Equipo | X: «Síntesis analítica de la conversación…» |

Ninguna de las 8 cuenta. Siete atribuyen sus tesis a analistas con nombre, y la comparativa del 11-05 no toma partido.

---

## 4. Caricaturas de B&B (solo títulos, no cuentan)

Son 40 en la ventana: 32 antes del cambio y 8 después. **Las 12 que cita el revisor existen, con esos títulos y esas fechas.** Los títulos siguen a quien manda o a quien lidera:

- **Antes:** Petro aparece en el título 6 veces («Petro no Kings», «Petro le escribe a Petro», «Reunión Petro y Trump», «Therian Petro y Abelardo», «Petro desconoce resultado» y «Trino Karol G al presidente»), Cepeda 2 y la «Paz Total» 1. Del otro lado: «Paloma y Oviedo derechos» y, ya con presidente electo, «Gobierno los de siempre», «Tigre odia Bogotá» y «Casa Blanca Barranquilla».
- **Después:** «Balones defensores Abelardo», «presupuesto Abelardo austero», «Muertos en bolsas Abelardo», «Abelardo armado», «Ecopetrol corrupción» y «Directora del ICBF».

**No se clasifican**, porque no se abrieron las imágenes. Un título no es una postura. Lo que sí muestran, y lo dice también el revisor, es a quién mira la casa. Lista completa, con la fecha que muestra el archivo del autor:

| # | Fecha | Lado | Título |
|---|---|---|---|
| 1 | 2025-10-14 | antes | [Caricatura Maduro](https://razonpublica.com/caricatura-maduro/) |
| 2 | 2025-10-19 | antes | [Caricatura Petro no Kings](https://razonpublica.com/caricatura-petro-no-kings/) |
| 3 | 2025-11-10 | antes | [Caricatura Se quedó sin título](https://razonpublica.com/caricatura-se-quedo-sin-titulo/) |
| 4 | 2025-11-18 | antes | [Caricatura Petro le escribe a Petro](https://razonpublica.com/caricatura-petro-le-escribe-petro/) |
| 5 | 2025-11-23 | antes | [Caricatura Verónica Alcocer vuelve](https://razonpublica.com/caricatura-veronica-alcocer-vuelve/) |
| 6 | 2025-12-01 | antes | [Caricatura Precandidatos Encuesta Invamer](https://razonpublica.com/caricatura-precandidatos-encuesta-invamer/) |
| 7 | 2025-12-09 | antes | [Caricatura Diciembre](https://razonpublica.com/caricatura-diciembre/) |
| 8 | 2025-12-14 | antes | [Caricatura Salario Mínimo en Colombia](https://razonpublica.com/caricatura-salario-minimo-colombia/) |
| 9 | 2025-12-22 | antes | [Caricatura año viejo nuevo](https://razonpublica.com/caricatura-ano-viejo-nuevo/) |
| 10 | 2026-01-12 | antes | [Encuesta Semana inflados](https://razonpublica.com/encuesta-semana-inflados/) |
| 11 | 2026-01-18 | antes | [Rodriguez Carrillo Idarraga](https://razonpublica.com/rodriguez-carrillo-idarraga/) |
| 12 | 2026-01-26 | antes | [Caricatura Gregory Bovino](https://razonpublica.com/caricatura-gregory-bovino/) |
| 13 | 2026-02-02 | antes | [Caricatura Reunión Petro y Trump](https://razonpublica.com/caricatura-reunion-petro-trump/) |
| 14 | 2026-02-17 | antes | [Caricatura Salario Vital](https://razonpublica.com/caricatura-salario-vital/) |
| 15 | 2026-02-22 | antes | [Caricatura Therian Petro y Abelardo](https://razonpublica.com/caricatura-therian-petro-abelardo/) |
| 16 | 2026-03-10 | antes | [Caricatura Pabellón de quemados](https://razonpublica.com/caricatura-pabellon-quemados/) |
| 17 | 2026-03-15 | antes | [Caricatura Paloma y Oviedo derechos](https://razonpublica.com/caricatura-paloma-oviedo-derechos/) |
| 18 | 2026-03-24 | antes | [Caricatura Abuso Sexual en Caracol](https://razonpublica.com/abuso-sexual-caracol/) |
| 19 | 2026-04-06 | antes | [Caricatura Papá Pitufo habla](https://razonpublica.com/caricatura-papa-pitufo-habla/) |
| 20 | 2026-04-19 | antes | [Caricatura Colombia campeón Sub 17](https://razonpublica.com/caricatura-colombia-campeon-sub-17/) |
| 21 | 2026-04-27 | antes | [Caricatura Paz Total](https://razonpublica.com/caricatura-paz-total/) |
| 22 | 2026-05-04 | antes | [Caricatura Cepeda rima con constituyente](https://razonpublica.com/caricatura-cepeda-rima-constituyente/) |
| 23 | 2026-05-18 | antes | [Caricatura Ivan Cepeda primera vuelta](https://razonpublica.com/caricatura-ivan-cepeda-primera-vuelta/) |
| 24 | 2026-06-01 | antes | [Caricatura Elecciones 10 millones](https://razonpublica.com/caricatura-elecciones-10-millones/) |
| 25 | 2026-06-09 | antes | [Caricatura Petro desconoce resultado](https://razonpublica.com/caricatura-petro-desconoc/) |
| 26 | 2026-06-21 | antes | [Caricatura Unir a Colombia elecciones](https://razonpublica.com/caricatura-unir-colombia-elecciones/) |
| 27 | 2026-06-30 | antes | [Caricatura Trino Karol G al presidente](https://razonpublica.com/caricatura-trino-karol-g-al-presidente/) |
| 28 | 2026-07-10 | antes | [Tarjeta roja anulada](https://razonpublica.com/tarjeta-roja/) |
| 29 | 2026-07-14 | antes | [Caricatura Gobierno los de siempre](https://razonpublica.com/caricatura-gobierno-los-de-siempre/) |
| 30 | 2026-07-21 | antes | [Caricatura Se acabó el Mundial](https://razonpublica.com/caricatura-se-acabo-el-mundial/) |
| 31 | 2026-07-28 | antes | [Caricatura Tigre odia Bogotá](https://razonpublica.com/caricatura-tigre-odia-bogota/) |
| 32 | 2026-08-04 | antes | [Caricatura Casa Blanca Barranquilla](https://razonpublica.com/caricatura-casa-blanca-barranquilla/) |
| 33 | 2026-08-22 | después | [Caricatura Balones defensores Abelardo](https://razonpublica.com/caricatura-balones-defensores-abelardo/) |
| 34 | 2026-08-27 | después | [Caricatura Directora del ICBF](https://razonpublica.com/caricatura-directora-del-icbf/) |
| 35 | 2026-08-31 | después | [Caricatura presupuesto Abelardo austero](https://razonpublica.com/caricatura-presupuesto-abelardo-austero/) |
| 36 | 2026-09-08 | después | [Caricatura Muertos en bolsas Abelardo](https://razonpublica.com/caricatura-muertos-en-bolsas-abelardo/) |
| 37 | 2026-09-20 | después | [Caricatura Mheo](https://razonpublica.com/caricatura-mheo/) |
| 38 | 2026-09-21 | después | [Caricatura Ecopetrol corrupción](https://razonpublica.com/caricatura-ecopetrol-corrupcion/) |
| 39 | 2026-09-28 | después | [Caricatura Abelardo armado](https://razonpublica.com/caricatura-abelardo-armado/) |
| 40 | 2026-10-05 | después | [Caricatura Sergio Niño Poeta](https://razonpublica.com/caricatura-sergio-nino-poeta/) |

---

## 5. Recuento (director)

| | I | D | C | M | F | X | Total |
|---|---:|---:|---:|---:|---:|---:|---:|
| Antes del 07-08-2026 | 2 (leves) | 0 | 6 | 9 | 1 | 9 | 27 |
| Desde el 07-08-2026 | 0 | 0 | 0 | 1 | 2 | 1 | 4 |
| **Total** | **2** | **0** | **6** | **10** | **3** | **10** | **31** |

**Si se cuentan los rótulos y no las piezas**, la lectura es parecida:
- **Rótulos descalificadores contra la derecha o sus candidatos:** 9 piezas (n.º 9, 13, 16, 17, 18, 20, 21, 22 y 28). Son «caverna», «cerril», «fascismo estridente y ramplón», «patán exitoso», «la visión del poder es la del dictador», «narcisista, machista y homófobo» y «abelardadas».
- **Rechazo de fondo del programa de la izquierda o de su candidato:** 5 piezas (n.º 16, 18, 21, 22 y 23). La 3 reparte a los dos lados y no entra en ninguna lista.
- **Fiscalización del presidente de turno:** 1 de Petro (n.º 11), más el «presidente irresponsable» de la 22, y 2 de De la Espriella (n.º 30 y 31).

La proporción es de 9 a 5, lejos de 3 a 1, y **ninguna de esas piezas está después del cambio salvo la 28**, que además exculpa al presidente en lo jurídico.

---

## 6. Miembros del Consejo Directivo que firman

En el feed del 2026-10-10 firman dos personas que «Quiénes somos» lista en el «CONSEJO DIRECTIVO FUNDACIÓN RAZÓN PÚBLICA»: Marcela Anzola («Iglesias, derecha y poder: ¿Quién usa a quién?», 2026-10-09, y «Comercio y trabajo forzoso…», en el boletín del 2026-10-05) e Iván Jaramillo (la pieza de salud del 2026-10-05). Las dos figuran también en «ASOCIADOS RAZÓN PUBLICA». **Sus piezas no se barrieron.**

**Criterio propuesto** (es del responsable editorial):
- **Por defecto son terceros**, porque firman con nombre propio y el consejo de una fundación gobierna la entidad, no la redacción. La misma lógica usa la regla de quien dirige ampliada (2026-10-07): lo que cuenta es dónde reside la decisión editorial, y eso se acredita con documento.
- **Pasan a voz de la casa solo si un documento del medio da al consejo autoridad editorial**, como el estatuto de Semana. Hoy no hay ninguno: el sitio no publica estatutos. La única pista es la página de 2009, que describe una asamblea de fundadores, autores, donantes y equipo, y no dice nada de quién decide qué se publica.
- **Se declaran aparte en la ficha**, como una tercera categoría («firmas del órgano de gobierno»), con su recuento cuando se haga. No mueven el número, pero el lector tiene derecho a saber que quien firma gobierna la fundación.

---

## 7. Veredicto por condición

| Condición | ¿Se cumple? | Por qué |
|---|---|---|
| 1. Voz de la casa | Sí, para el director | Firma el director y editor general. Los boletines y las síntesis del «Equipo» atribuyen todo a terceros, y las caricaturas no se leyeron |
| 2. A los dos lados del cambio | **No** | Después del 07-08 hay 4 piezas: 2 F, 1 M y 1 X. **Ninguna con postura que cuente** |
| 3a. ≥10 piezas con postura en una dirección | **No** | 2 (I leves), 0 D |
| 3b. ≥3 a cada lado del cambio | **No** | 2 antes y 0 después |
| 3c. Proporción ≥3 a 1 | **No aplica** | Con 2 piezas no hay proporción. Por rótulos sale 9 a 5 |
| 4. Contrapesos escritos | Sí | §5 y §8 |
| 5. Reproducible | Sí | Tablas de §2 a §4, con URL y fecha |

**La regla no se activa. Es nivel 5 y no mueve el número**, en ninguna dirección.

---

## 8. Lo que el barrido sí dice (nivel 5, declarado)

- **La voz de la casa se declara de centro** y lo practica: recomienda a una candidata de centroizquierda (López, 07-03 y 31-05) y a un candidato de centroderecha (Fajardo, 20-04 y 31-05), rechaza los programas de los dos polos y no endosa a nadie en la segunda vuelta (15-06).
- **Misma conducta con los dos gobiernos:** fiscaliza a Petro mientras manda (23-02; «presidente irresponsable», 01-06) y a De la Espriella desde que manda (20-09 y 05-10). Defiende el mando de Petro hasta el último día frente al presidente electo (27-07). Es el patrón que el polo fijo llama mixta. **Pero después del cambio son solo 3 piezas con contenido**, menos que las 15 de Chocó 7 Días, que se aceptaron como «0,00 con evidencia».
- **Contrapeso hacia la izquierda, con su peso:** el tono. Los rótulos más duros van contra la derecha (9 piezas con rótulo, frente a 5 con rechazo de fondo a la izquierda). La primera recomendación de voto del año es para López, «progresista institucionalista». Y en política internacional la crítica a Trump es constante (n.º 2, 4, 6, 7 y 15). Peso medio: inclina el tono, no la recomendación.
- **Contrapeso hacia la derecha, con su peso:** el fondo. Petro y Cepeda están «completamente equivocados en materias de paz, economía, políticas sociales y política internacional» (06-04). De Cepeda dice que es «el peligro que representa para Colombia» (01-06). Fajardo, «la centroderecha moderna», «tiene razón» (20-04). Y exculpa al presidente en lo jurídico (10-08). Peso medio.
- **Nada de esto sostiene −0,40.** El −0,40 es izquierda moderada, en el centro de la banda. Lo que el barrido describe es mixta, con el tono algo inclinado a la izquierda.

---

## 9. PROPUESTA (pendiente de la decisión del responsable editorial)

- **Aplicación literal de las reglas 2 y 3: −0,40 se queda, sin firmar y con la ficha marcada como incompleta.** El barrido no llega a los mínimos y es nivel 5. La segunda precisión dice que un barrido que no llega «no deshace nada». La regla 2 decide entre dos bandas cuando hay evidencia con la que decidir, y no sirve de vía para mover un número que la regla 3 congela.
- **Pero el −0,40 no tiene evidencia.** Es la razón del alta del 2026-07-27, que la propia ficha llama «impresión de lectura», y el protocolo excluye esas impresiones por escrito. La salida que el responsable editorial ya tomó para tres medios del mismo tipo (Vorágine, Cuestión Pública y Revista RAYA, sesión del 16-09, código del 18-09) fue **`bias: null`, «sin medir»**. Es la recomendación aquí: no afirma una banda que nadie ha medido, ni la izquierda ni la mixta.
- **«0,00 con evidencia»** sería el valor mejor apoyado, pero exige una precisión nueva: que un barrido simétrico de la voz de la casa pueda sustituir un valor heredado sin evidencia. Hoy la regla no la tiene, y con solo 3 piezas posteriores al cambio la base es delgada. Si el responsable editorial la adopta, debe aplicarse a la vez a todas las fichas con valores heredados.
- **Revisión:** recontar en diciembre de 2026 las piezas del director posteriores al 07-08, y leer las caricaturas posteriores al cambio, con sus imágenes.
