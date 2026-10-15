# Barrido editorial: Cuestión Pública (cuestionpublica.com)

| | |
|---|---|
| **Medio** | Cuestión Pública (`cuestion-publica`), Bogotá. No noticioso, fuera del mapa (`noNoticioso: true`) |
| **Valor vigente** | **sin medir** (`bias: null`), decisión del responsable editorial del 2026-09-16, aplicada el 2026-09-18 (commit `fa77249`). La cabecera de `fichas/cuestion-publica.md` dice «−0,45»: está desfasada |
| **Regla aplicada** | «EVIDENCIA EDITORIAL HISTÓRICA» (`PROTOCOLO_JUICIO_EDITORIAL.md`, 2026-10-09), con sus dos precisiones |
| **Ventana** | 2025-10-10 → 2026-10-10 (regla del presente) |
| **Cambio de gobierno** | 07-08-2026: Petro hasta el 06-08; De la Espriella desde el 07-08 |
| **Resolución de origen** | `revision-externa/respuestas/opus-5-5-cuestion-publica.md`. El revisor contó 11 piezas con postura contra la derecha (5 antes y 6 después) frente a 4 contrapesos, o 11:2 si se quitan dos dudosas |
| **Quién lo hizo** | Claude Opus 5.5 (`claude-opus-5-5`), verificador del ciclo 2, tanda 8, a petición del responsable editorial, el 2026-10-10. Es de la misma casa que el autor de la ficha y que el revisor, así que su acuerdo no es aval |
| **Estado** | **DECIDIDO el 2026-10-10: sin medir** (se queda; la ficha decía −0,45), por el responsable editorial (`DECISIONES.md`, «2026-10-10 · Tandas 8 y 9 del ciclo 2: el barrido manda sobre los números sin evidencia»). Lo que más abajo dice «propuesta», «recomendada» o «pendiente» es el estado anterior a la decisión y se conserva como historia |
| **Resultado** | **NO cumple los mínimos.** En la lectura estricta hay 5 piezas con postura (4 antes y 1 después) frente a 3 contrapesos. En la amplia, 10 piezas (7 y 3) frente a 6. En las dos lecturas falla la proporción de 3:1, y en la estricta fallan además el mínimo de 10 y el de 3 piezas después del cambio. **Por la segunda precisión del 2026-10-09, el valor se queda donde estaba: sin medir** |

> Quien lo rehaga puede llegar a otro número. Para eso están aquí las URL, las
> fechas, los fragmentos y el método. **La clasificación de cada pieza es el
> juicio de un solo lector.**

---

## 1. Método

- **robots.txt** de `cuestionpublica.com` (2026-10-10): el bloque general solo veta `/wp-admin/` y las rutas de WooCommerce; el de Yoast dice `User-agent: *` / `Disallow:`. No nombra a ningún agente de Anthropic.
- **Universo.** La API pública de WordPress: `https://cuestionpublica.com/wp-json/wp/v2/posts?after=2025-10-10T00:00:00&per_page=100&page=N&_fields=date,link,title,categories`.
  - La cabecera da `x-wp-total: 340`. Son 263 entradas antes del 07-08-2026 y 77 desde ese día, del 2025-10-10 al 2026-10-09.
  - La página 1 que descargué es **idéntica byte a byte** a la del revisor (`cmp`).
  - Las páginas 2 a 4 y las entradillas (`excerpt`) se tomaron de la descarga del revisor, hecha el mismo día. El sitio me devolvió `303` al pedir `excerpt` y luego dejó de responder a mi IP (timeouts desde las 17:55 del 10-10, hora de Bogotá).
  - **Aviso de procedencia:** todo lo que no sea la página 1 descansa en los ficheros crudos del revisor (`t89/cuestion-dl`). Los leí como datos y no ejecuté nada desde esa carpeta.
- **Lectura.**
  - Se leyeron los **340 titulares y sus entradillas**.
  - Se leyó el **texto completo** de 21 piezas, en el HTML crudo descargado por el revisor el 2026-10-10: entre ellas las dos columnas de la directora, todas las de su lista y cinco que no citó.
  - Las demás se clasifican por titular y entradilla, y donde pesa se dice.
- **Voz de la casa (condición 1).**
  - **Cuentan:**
    - las columnas de **La Tribuna** firmadas por la directora;
    - las piezas «Por Cuestión Pública»;
    - los titulares y entradillas propios, que en la API llevan todos autor «Cuestión Pública».
  - **No cuentan:**
    - las columnas de terceros (Teresita Goyeneche, 04-06-2026, elogiosa con Susana Muhamad);
    - las piezas cuyo titular o entradilla atribuye la valoración a un invitado («…: Wilson Arias», «…: Diana Otavo», «para el abogado y columnista Ramiro Bejarano…»).
  - El pie de La Tribuna dice «Sus contenidos no comprometen al medio». Se registra como contrapeso, pero **no saca de la voz de la casa** una columna firmada por la directora: el protocolo cuenta expresamente lo «firmado por la casa o su director».
- **Clases.**
  - **I**: postura en voz propia contra la derecha o el Gobierno entrante, o a favor de la izquierda. Comprende rótulos ideológicos o descalificadores, encuadre asimétrico entre candidatos y celebraciones o elogios. **Cuenta.**
  - **I-leve**: la postura existe pero es lateral, va en forma de pregunta o se superpone a la fiscalización. **Cuenta solo en la lectura amplia.**
  - **F**: solo fiscaliza a quien manda, o investiga a un candidato, sin rótulo en voz propia. **No cuenta.** Se declara (precisión del 2026-10-09).
  - **C**: contrapeso. Crítica en voz propia con valoración contra Petro, su Gobierno o la izquierda, o elogio a la derecha. Se cuenta **con generosidad**, con el mismo criterio que el barrido de El Informador, que contó como contrapeso la crítica al Gobierno del propio lado aunque fuera fiscalización. **C-leve** entra solo en la amplia.
  - **V**: postura de valores sin destinatario político (aborto, feminismo). **No cuenta para el eje.** Es la línea que la casa declara (nivel 4).
  - **Fuera**: piezas internacionales (María Corina Machado, Trump, Maduro, Gaza), igual que Kast en El Informador; terremoto, servicio y efemérides.

---

## 2. Piezas que cuentan

Las URL son `https://cuestionpublica.com<ruta>`.

### 2.1 Antes del cambio (2025-10-10 → 2026-08-06)

| # | Fecha | Ruta | Clase | Fragmento literal | Leído |
|---|---|---|---|---|---|
| 1 | 2026-06-16 | `/no-todas-las-amenazas-a-la-democracia-son-iguales/` (La Tribuna, «Por Diana Salinas», directora) | **I** | «Estamos, claramente, frente a un autoritario»; «no hay equivalencia posible entre ambos proyectos políticos»; «la férrea idea de gritar si volvía a llegar un fascista al poder» | cuerpo |
| 2 | 2026-06-22 | `/abelardo-de-la-espriella-el-presidente-electo-que-llega-al-poder-lleno-de-banderas-rojas-y-con-media-colombia-en-oposicion/` | **I** | «asume un rol protagónico como el nuevo referente de la ultraderecha nacional»; «una campaña marcada más por los símbolos y las polémicas que por las propuestas» | cuerpo |
| 3 | 2026-06-26 | `/en-vivo-pride-2026-en-tu-cara-presidente-electo/` | **I** | «¡En tu cara presidente electo!»; «la caminata contra la ultraderecha» | cuerpo |
| 4 | 2026-07-14 | `/el-gobierno-de-adle-sera-un-puto-loop/` (La Tribuna, «Por Diana Salinas») | **I** | «el reencauche del Partido Conservador más radical»; «Este es el popurrí de los neoconservadores de Colombia. No hace falta decir fascistas, porque sería redundar.» | cuerpo |
| 5 | 2026-06-17 | `/segunda-vuelta-electoral-colombia-se-juega-su-destino/` (vídeo) | I-leve | «Por eso nos preguntamos ¿hay peligros para el país si gana Abelardo?». Solo se pregunta por uno de los dos candidatos | entradilla = cuerpo |
| 6 | 2026-06-22 | `/preconteo-gano-abelardo-se-viene-la-ultraderecha-para-colombia/` (vídeo) | I-leve | Titular: «¿se viene la ultraderecha para Colombia?» | entradilla = cuerpo |
| 7 | 2025-12-12 | `/verdades-a-medias-y-datos-manipulados-el-discurso-de-las-bodegas-y-candidatos-de-derecha-para-las-elecciones/` | I-leve | «el discurso de las 'bodegas' y candidatos de derecha». Es un chequeo, oficio, pero el blanco es solo un lado | titular y entradilla |

### 2.2 Después del cambio (2026-08-07 → 2026-10-10)

| # | Fecha | Ruta | Clase | Fragmento literal | Leído |
|---|---|---|---|---|---|
| 8 | 2026-09-07 | `/hilo-con-ilva-miriam-hoyos-la-educacion-quedo-en-manos-de-una-de-las-personas-mas-radicales-del-dogmatismo-religioso-en-el-pais/` | **I** | «una de las personas más radicales del dogmatismo religioso en el país»; «#DeMalEnPeor» | cuerpo |
| 9 | 2026-08-14 | `/la-mezquindad-del-gobierno-de-abelardo-con-las-ayudas-internacionales/` (vídeo) | I-leve | «La mezquindad…»; «Pareciera que la ideología se impone sobre el apoyo humanitario en este Gobierno». Fiscaliza con un descalificador | cuerpo |
| 10 | 2026-09-02 | `/liquidar-o-aniquilar-los-miedos-en-el-ministerio-de-igualdad-con-el-pastor-john-milton-rodriguez-como-liquidador/` | I-leve | «un ejemplo más de la "batalla" cultural de este gobierno» | entradilla |

### 2.3 Contrapesos (todos antes del cambio)

| # | Fecha | Ruta | Clase | Fragmento literal |
|---|---|---|---|---|
| C1 | 2025-11-21 | `/la-linea-roja-que-cruzo-el-gobierno-petro-contradicciones-y-preguntas-que-deja-su-decision-de-bombardear-a-menores/` | **C** | «La línea roja que cruzó el Gobierno Petro»; «los atroces bombardeos» |
| C2 | 2026-05-20 | `/hilo-casi-que-no-presidente-petro-se-disculpo-por-llamar-munecas-de-la-mafia-a-las-mujeres-periodistas-de-colombia/` | **C** | «¡Casi que no! Presidente Petro se disculpó…» (ironía en voz propia) |
| C3 | 2026-07-31 | `/petro-acelero-el-reparto-de-notarias-en-la-fase-final-de-su-gobierno/` | **C** | «Hoy nos aguzamos con el gobierno de Gustavo Petro, con la corrupción que se presenta en la izquierda» |
| C4 | 2025-11-18 | `/envivo-muertes-de-menores-en-bombardeos-generan-fuerte-rechazo-en-colombia/` | C-leve | Titular: «Indignante: había otros caminos más allá del bombardeo que mató a niños, dicen expertos». El «Indignante» no se atribuye |
| C5 | 2026-05-08 | `/los-seis-reganos-de-la-corte-al-presidente-petro-por-fomentar-la-violencia-machista-contra-mujeres-periodistas-1/` | C-leve | «…al presidente Petro por fomentar la violencia machista». Es el resumen propio de un fallo |
| C6 | 2026-04-08 | `/primicia-huertas-el-falso-positivo-de-petro/` | C-leve | Titular: «#Primicia \| Huertas: ¿el falso positivo de Petro?» (pregunta) |

Dentro de la pieza 1 hay además una crítica a «los errores y las malas decisiones del gobierno de Gustavo Petro». No se cuenta aparte.

---

## 3. Lo que no cuenta, y se declara

- **F antes del cambio, sobre el Gobierno Petro y su entorno.** Son unas 20 piezas:
  - las casas y la mansión de Benedetti (13-11 y 10-12-2025);
  - Roa (10-02 y 08-04-2026);
  - el Pacto Histórico y la rendición de cuentas (12-02);
  - Berenice Bedoya (17-02);
  - la serie Hollman Morris / RTVC, 7 piezas entre el 18-03 y el 23-04;
  - quiénes rodean a Cepeda (27-05);
  - el general reintegrado por Petro (30-07).

  Es fiscalización de quien mandaba. Con el criterio generoso de contrapesos podrían sumarse a C; aquí no se suman, para no inflar ninguno de los dos lados con fiscalización. **Sumarlas solo bajaría más la proporción.**
- **F antes del cambio, sobre el candidato De la Espriella.** Son unas 12 piezas: «¿Ladrón que roba ladrón?» (27-03), «Otro 'triunfazo' de Abelardo» (16-04), el bufete y los contratos (28-04 y 03-06), los vuelos (22-05), Alex Saab (27-05), los funcionarios inscritos (31-05 y 03-06), «El secreto de Abelardo en primera vuelta» (La Tribuna, Salinas y Buitrago, 10-06), los 25 municipios (18-06)…
  - Es investigación de un candidato, sin rótulo ideológico. No suma.
  - Se declara como **tensión de selección**: contra Cepeda, en el mismo periodo, consta una sola pieza (27-05). La directora lo reconoce: «Cuestión Pública ha puesto atención especial en el candidato Abelardo De la Espriella» (16-06).
- **Los procesos de Álvaro y Santiago Uribe:** unas 40 piezas de cobertura judicial. Se declaran y no cuentan.
- **F después del cambio, sobre el Gobierno De la Espriella.** Casi toda la producción política de los dos meses:
  - el decreto de emergencia (12-08);
  - «Abelardo no me cuida, me cuida mi pueblo» (13-08): ironía en la entradilla, pero el cuerpo es una lista de aplicativos de ayuda;
  - «Se vinieron los gringos…» (13-08): la crítica se atribuye a la senadora Pedraza;
  - «¿Me sirven sólo los que piensan como yo?» (13-08);
  - la primera semana del Gobierno (13-08);
  - la primera dama (20-08);
  - las emisoras de paz (21-08);
  - Santurbán (21-08);
  - «¿El ICE colombiano?» (26-08): pregunta y comparación;
  - el Libro de la Verdad (27-08);
  - «Declaraciones de un cuarto oscuro» («Por Cuestión Pública», 04-09) y su vídeo (09-09);
  - el pastor John Milton Rodríguez (11-09);
  - «Abelardo Airlines» (18-09);
  - la maquinaria digital (18-09);
  - Beltrán (25-09);
  - Lombana (30-09).

  **Por la regla del polo fijo esto es oficio:** fiscalizó a Petro cuando mandaba y fiscaliza a De la Espriella ahora que manda.
- **V:** «#28S ¡CON NUESTROS DERECHOS NO RETROCEDEMOS!» (28-09) defiende el aborto legal sin destinatario de gobierno. Coincide con la línea declarada en Nosotros. No suma.
- **Fuera:**
  - las internacionales: María Corina Machado (10-10-2025, favorable), Trump-Venezuela, ICE de Minneapolis, Gaza, León XIV;
  - las columnas de terceros de La Tribuna: Goyeneche, contrato sindical, datos personales electorales, Acuerdo de Paz (27-07, autor sin comprobar);
  - las piezas con valoración atribuida a invitados: Bejarano 21-05, Wilson Arias 04-08, Luis Carlos Reyes 27-07, Diana Otavo 07-10.
- **Sin comprobar** (el sitio dejó de responder): el autor de «Cronología de una batalla cultural» (La Tribuna, 31-08) y los cuerpos de los puntos 7 y 10. Si la Cronología fuera de la directora y llevara rótulos, sumaría 1 después del cambio. **No cambia el veredicto:** la proporción seguiría por debajo de 3:1.

---

## 4. Recuento

| Lectura | I antes | I después | Total I | Contrapesos | Proporción |
|---|---:|---:|---:|---:|---:|
| **Estricta** (I y C) | 4 | 1 | **5** | **3** (C1-C3) | **1,7 : 1** |
| **Amplia** (+ I-leve y C-leve) | 7 | 3 | **10** | **6** (C1-C6) | **1,7 : 1** |
| La del revisor (sus 11 contra sus 4) | 5 | 6 | 11 | 4 | 2,75 : 1 |
| La del revisor sin sus dos dudosas | 5 | 6 | 11 | 2 | 5,5 : 1 |

**Las dos dudosas del revisor** son C1 (la línea roja) y C3 (las notarías). **Decisión: las dos cuentan como contrapeso.**
- **El criterio:** el revisor cuenta como postura después del cambio piezas que fiscalizan al Gobierno en ejercicio con un adjetivo o una ironía («mezquindad», «¿El ICE colombiano?», «Abelardo no me cuida»). C1 y C3 hacen exactamente eso con el Gobierno Petro: «atroces», «la corrupción que se presenta en la izquierda». La misma vara tiene que servir a los dos lados.
- **Si se aplica la estricta a los dos lados**, de sus seis piezas de después queda una sola, la de Ilva Hoyos, y C1 y C3 siguen siendo contrapesos.
- **Si se aplica la amplia a los dos lados**, entran las suyas y también C4-C6.
- **Lo que no se sostiene** es quitar C1 y C3 y conservar las suyas.

Además, la de María Corina Machado (C1 del revisor) es **internacional y queda fuera**, como Kast en El Informador. Con eso, su propia cuenta queda en 11:3. Tampoco cuentan, por lo dicho en §3, sus P6 y P7 (F), su P9 (F) ni su P11 (V).

---

## 5. Veredicto por condición

| Condición | ¿Se cumple? | Números |
|---|---|---|
| 1. Voz de la casa | se aplicó | Las columnas de la directora y los titulares y entradillas propios. Las columnas de terceros y las valoraciones de invitados, aparte |
| 2. A los dos lados del cambio | **no** en la estricta (4 y 1); **por los pelos** en la amplia (7 y 3, con dos leves) | Después del 07-08 casi todo es fiscalización del Gobierno en ejercicio |
| 3. Sostenida (≥10; ≥3 por lado; ≥3:1) | **NO** | Estricta: 5, 4/1, 1,7:1. Amplia: 10, 7/3, 1,7:1 |
| 4. Contrapesos escritos | sí | §2.3 y §3, más el pie de La Tribuna y el «No hinchamos por ningún presidente o candidato presidencial» (16-06) |
| 5. Reproducible | sí | Este archivo |

**Un barrido que no llega a los mínimos no deshace nada** (precisión del 2026-10-09). El valor sigue siendo **sin medir**.
- **Tampoco sostiene un 0,00 «con evidencia».** La conducta no es igual con los dos lados: los rótulos ideológicos («ultraderecha», «autoritario», «fascistas», «dogmatismo radical») van todos a la derecha, y la crítica a la izquierda se hace por conducta (bombardeos, machismo, corrupción) y nunca por ideología.
- **Esa dirección se declara como tensión.**

---

## 6. ¿Es un endoso la columna del 16-06? (decide el tope)

**No es endoso explícito.** Es encuadre asimétrico entre candidatos, de primer orden, y por eso entra en el barrido como I. Pero no levanta el tope de ±0,30.

| | El Informador, 21-06-2026 | Cuestión Pública, 16-06-2026 |
|---|---|---|
| Forma | Editorial sin firma: la institución | Columna firmada en La Tribuna, con el pie «no comprometen al medio» |
| Qué dice | «con Abelardo habrá institucionalidad, democracia y libertad; con Cepeda habrá […] tiranía»; «Tenemos la plena seguridad de que Abelardo se constituirá en el líder hispanoamericano» | «no hay equivalencia posible entre ambos proyectos políticos»; De la Espriella, «un autoritario»; de Cepeda, ninguna decisión fuera de la Constitución |
| ¿Pide el voto o declara apoyo? | Sí. Además, el 11-05 pidió votar por Abelardo («deberán depositar su voto por Abelardo») | No. Lo niega: «No hinchamos por ningún presidente o candidato presidencial»; «No creemos que Cepeda sea el candidato perfecto» |

- El protocolo no define el «endoso explícito», pero el adjetivo pide que la toma de partido esté dicha, y aquí el texto la niega.
- Firmar como directora y representante legal pesa a favor de que sea voz de la casa, y por eso cuenta en el barrido. No convierte en endoso un texto que rehúsa serlo.
- Ante la duda, regla 2.
- Aunque el responsable editorial lo leyera como endoso, **el endoso levanta el tope, pero no sustituye al barrido.** Con el barrido por debajo de los mínimos, el número no se mueve por esta vía.

---

## 7. PROPUESTA (pendiente de la firma del responsable editorial)

**Recomendada:** `bias: null` (sin medir), `noNoticioso: true`. Se reescribe la razón: ya no es que «su volumen no da», porque publica 340 piezas al año. Es que el barrido de 12 meses no alcanza los mínimos, y la inclinación a la izquierda en su voz propia queda como tensión.

**Alternativa declarada:** −0,25, si el responsable editorial acepta la lectura del revisor sin sus dos dudosas (11:2).
- Eso pide contar como postura la fiscalización con tono del Gobierno entrante y no la del saliente.
- Con tope de ±0,30, porque no hay endoso.
- Quedaría por debajo de CasaMacondo (−0,35 entonces, puesto por declaración y sin firmar; desde el 2026-10-10 está en 0,00 con evidencia).
- **No se recomienda:** usa dos varas.

**Cuándo se rehace:** en diciembre de 2026, con 4 meses del Gobierno De la Espriella. Si aparecen rótulos o tomas de partido propias en las piezas de después, sin contrapesos equivalentes, se reabre el número.
