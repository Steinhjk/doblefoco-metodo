# Barrido editorial histórico — Seguimiento.co (Santa Marta)

| | |
|---|---|
| **Medio** | Seguimiento.co (`seguimiento`), Santa Marta, Magdalena |
| **Fecha del barrido** | 2026-10-09 |
| **Quién lo hizo** | Claude Code (Claude Opus 5.5), a petición del responsable editorial; ciclo 2, tanda 5 |
| **Regla que aplica** | `PROTOCOLO_JUICIO_EDITORIAL.md`, «Evidencia editorial histórica» (condición 5: reproducible) |
| **Resolución de la que sale** | `revision-externa/respuestas/opus-5-5-seguimiento.md` (objeciones 7 y 8) |
| **Ficha** | `fichas/seguimiento.md` (valor actual 0,00 por reglas 2 y 3) |
| **Estado** | **DECIDIDO el 2026-10-09: se queda en 0,00**, con la centroderecha como tensión, por el responsable editorial; firmado en bloque el 2026-10-10 (`DECISIONES.md`, «2026-10-09 · Reexamen de cinco fichas cerradas con la regla nueva»). Lo que más abajo dice «propuesta» o «pendiente» es el estado anterior a la decisión y se conserva como historia |
| **Decisión (2026-10-09)** | el responsable editorial: **se queda en 0,00, por la regla 2.** Con el recuento estricto no llega (9 piezas; 2 después del cambio) y después del 07-08 se leyó como mucho la mitad de lo publicado. El +0,15 que propone este barrido no se aplica. El barrido de agosto a octubre se completa antes del 2026-11-10 (`DECISIONES.md`, «Reexamen de cinco fichas cerradas con la regla nueva»; ver la ficha) |

Este archivo existe para que cualquiera pueda recontar las piezas y llegar, o
no, al mismo número. Quien lo hizo es de la misma casa que el autor de la
ficha, el revisor y el verificador: que coincidan no es aval.

**Aviso de cobertura, antes de nada.** El barrido se cerró antes de terminar la
descarga, por tiempo. **Después del cambio de gobierno la cobertura es la
mitad, o menos, de la de antes** (ver §1, «Lagunas»). Las condiciones se juzgan
con lo leído, y la propuesta lo tiene en cuenta.

---

## 1. Método

- **robots.txt** de seguimiento.co (2026-10-09): un solo bloque
  `User-agent: *`, con `Crawl-delay: 15` y, entre otras, `Disallow: /search/`,
  `Disallow: /taxonomy/` y `Disallow: /*?page=`. No menciona a ClaudeBot,
  Claude-Web ni anthropic-ai.
  - El índice `https://seguimiento.co/sitemap.xml` (permitido) remite a cuatro
    páginas `sitemap.xml?page=1..4`, que **casan con `Disallow: /*?page=`**.
    **No se descargaron del sitio.** No hay API (Drupal 7; `/jsonapi` da 404).
  - Las páginas de artículo están permitidas. Las del sitio vivo se bajaron
    con `curl -sL --ssl-no-revoke`, UA de navegador y **15 s entre peticiones**.
- **No se tocaron** eltiempo.com, cambiocolombia.com ni lasillavacia.com. No
  hubo buscador web.
- **Universo de URL** (solo para descubrir URL):
  1. **Las cuatro páginas del sitemap archivadas por Internet Archive** el
     2026-05-01 (`web.archive.org/web/20260501…id_/…sitemap.xml?page=N`):
     152.420 URL. Cubren hasta el nodo ≈ 86000 (finales de abril de 2026).
  2. **El índice CDX de Internet Archive** para todo el dominio, del
     2025-10-01 al 2026-10-09 (`matchType=domain`, `collapse=urlkey`,
     `statuscode:200`): 239.337 líneas.
  - Las URL de artículo terminan en el número de nodo (`…-89137`), que es
    correlativo con la fecha. **Ventana: nodos 81700 a 89800** (del
    06-10-2025 al 05-10-2026); fuera de ella no se cuenta nada.
  - **Calidad del CDX:** donde hay sitemap, el CDX trae 3.328 de sus 3.354
    nodos (99 %). Después de mayo de 2026 trae entre 240 y 320 nodos por
    bloque de 500, frente a 360-400 antes: **falta, a ojo, una cuarta parte
    de las piezas de mayo a octubre**. Prueba de ello: la pieza de la
    «depuración» que cita la resolución (sufijo 88444) no está en el universo.
- **Selección (sistemática, por términos sobre toda la ventana).** Entra toda
  URL de la ventana cuyo *slug* (que es el titular) casa con alguna de estas
  expresiones:
  - **lista estricta (670 URL):**
    ```
    petro|petris|espriella|abelardo|cepeda|pacto-historico|uribe|uribis|presidente|presidencia|gobierno-nacional|gobierno-del-cambio|nuevo-gobierno|paz-total|consulta-popular|constituyente|candidat|centro-democratico|primera-dama|segunda-vuelta|primera-vuelta|oposicion|izquierda|derecha|progresis|bukele|emergencia-economica|ley-de-financiamiento|frente-amplio|casa-de-narino|benedetti|sarabia|gobierno-de-abelardo|gobierno-de-petro
    ```
  - **ampliación (172 URL más):** `gobierno|ministr|reforma|encuesta|decreto|valencia|…`
    (la expresión completa está en el guion del barrido; añade sobre todo
    piezas de medidas del Gobierno).
- **Descarga.** Un tercio de la lista estricta, del sitio vivo; el resto, de
  la instantánea más antigua del CDX (`id_`, HTML original). De cada pieza se
  sacó: la fecha (`dc:date`), el titular (`h1.title-main`), la entradilla
  (`field-name-field-subtitulo`), la firma (`autor-detail`), las etiquetas y el
  cuerpo. Se leyeron el titular y la entradilla de **todas** las piezas
  descargadas, y el primer y el último párrafo de todas las que se clasifican
  distinto de A.
- **Resultado: 710 piezas leídas dentro de la ventana: 644 antes del
  07-08-2026 y 66 desde ese día.**
- **Voz.** Firmas en las 710: «Seguimiento.co» 629; periodistas de la casa
  (Vanessa Redondo Peña 37, Karen Olmos 24, Linda Ospino Escalante 2);
  «Convenio Zona Cero» 17; columnista Alberto De Luque Palencia 1.
  - **Cuentan como voz de la casa** los titulares, entradillas y párrafos
    propios de las piezas firmadas «Seguimiento.co» y de las de sus
    periodistas de plantilla. Es un criterio declarado: un recontador más
    estricto puede quitar las de firma personal (solo afecta a 88944).
  - **No cuentan:** las de «Convenio Zona Cero» (contenido de otro medio), las
    columnas de «Opinan los expertos», los refritos declarados de otros medios
    y lo que es contenido de campaña (código P).
  - **No hay sección editorial** ni editoriales sin firma. La voz de la casa es,
    entera, la de los titulares y entradillas de la sección de noticias.

### Lagunas (declaradas)

1. **No leídas: 113 URL de la selección** (de 842), casi todas posteriores a junio:
   1 a 3 por bloque de 500 nodos hasta el 87499; **13 en 87500-87999, 26 en
   88000-88499, 26 en 88500-88999, 17 en 89000-89499 y 12
   en 89500-89800.** La descarga del sitio vivo, con 15 s por petición, no
   terminó y se cortó por tiempo. Se leyeron los *slugs* de las no leídas
   posteriores al 07-08 (son el titular sin puntuación): ver §6.
2. **El universo de URL, a su vez, pierde una cuarta parte** de mayo a
   octubre (ver arriba). No se usaron las páginas del sitemap vivo porque
   `robots.txt` las excluye.
3. **Resultado neto:** de julio a octubre de 2026 se leyó, como mucho, **la
   mitad** de lo que el medio publicó con los términos del barrido. Antes de
   mayo, la cobertura es casi completa.
4. **No se leyeron las piezas de la sección «la samaria» sobre la Alcaldía de
   Pinedo** que no casan con los términos. No son del eje nacional, pero son
   donde vive el conflicto de interés de la ficha.

---

## 2. Clasificación

Cada pieza lleva un código. **Solo D y C entran en la cuenta** de la
condición 3.

| Código | Qué es | ¿Cuenta? |
|---|---|---|
| **D** | Postura en voz de la casa (titular, entradilla o párrafo propio, sin atribuir) que favorece a la derecha frente a la izquierda: antes del cambio, encuadre asimétrico entre candidaturas (burla o sospecha propia hacia la de izquierda, elogio propio a la de derecha); después, celebración del gobierno entrante o crítica propia al expresidente, ya sin poder | sí, a favor de la dirección |
| **C** | Postura en voz de la casa en sentido contrario (favorable al gobierno de Petro o a la izquierda; crítica propia a la derecha o al gobierno entrante) | sí, en contra |
| F | Crítica propia al gobierno en ejercicio antes del 07-08. Regla del polo fijo: fiscalizar al que manda no es orientación | no |
| P | Promoción de candidaturas locales o al Congreso con lenguaje de comunicado de campaña («multitudinaria», «respaldo», «se toma los barrios»), sin rótulo de publicidad | no: probable propaganda o comunicado reescrito; se declara |
| R | Reescritura de otro medio (Zona Cero, refrito declarado de Caracol, Infobae, Cambio) | no |
| A | Atribuida a una fuente (cita, comunicado, informe, fallo) o informativa sin postura propia | no |

«(límite)» marca las piezas que una lectura más amplia pondría en D o en C y
esta no pone. Se dejaron fuera para no inflar la cuenta.

---

## 3. Resultado y las cinco condiciones

| | Antes del 07-08 | Después del 07-08 | Total |
|---|---|---|---|
| Piezas leídas | 644 | 66 | **710** |
| **D** (postura propia hacia la derecha) | **9** | **3** | **12** |
| **C** (postura propia en contra) | **2** | **0** | **2** |
| D (límite), no cuentan | 5 | 1 | 6 |
| C (límite), no cuentan | 2 | 0 | 2 |
| F (fiscalización del gobierno en ejercicio) | 14 | — | 14 |
| P (contenido de campaña sin rótulo) | 19 | 0 | 19 |
| R (Zona Cero y refritos) | ≥ 17 | ≥ 2 | ≥ 19 |
| A (atribuida o informativa) | el resto | el resto | ≈ 625 |

1. **Voz de la casa: se cumple.** Las 14 piezas D y C son titulares,
   entradillas o párrafos propios. Once van firmadas «Seguimiento.co»; una
   (88944), por una periodista de la casa. No cuenta ninguna columna, ninguna
   pieza de Zona Cero ni ninguna cita de terceros.
2. **A los dos lados del cambio, dentro de 12 meses: se cumple, por el
   mínimo.** 9 piezas D antes y **3 después**, justo el mínimo. Antes, encuadre
   asimétrico entre candidaturas, no fiscalización. Después, elogio propio al
   presidente entrante y crítica propia al expresidente. **Esta es la condición
   más frágil**, porque después del 07-08 se leyó la mitad o menos (§1).
3. **Sostenida: se cumple.** 12 piezas con postura (mínimo 10); 9 y 3 a cada
   lado (mínimo 3); proporción **12 a 2 = 6 a 1** (mínimo 3 a 1). Con las de
   límite: 18 a 4 = 4,5 a 1.
4. **Contrapesos escritos: se cumple.** Ver §5.
5. **Reproducible: este archivo.** Las piezas que cuentan, las de límite, las F
   y las P van con URL en §4 a §6. Las A no se listan una a una: son todas las
   demás de la selección, y la selección se reproduce con las expresiones de §1.

**Sensibilidad, dicha sin rodeos.**
- De las 12 piezas D, 9 son claras. Tres son más tenues: 85648 (el «tras meses
  negándose» es un juicio, pero el cuerpo es informativo), 86715 (el titular
  dice «Intolerancia», pero el cierre recoge la denuncia contraria del Pacto) y
  89137 («Ahora sí, se acabó» celebra, pero el cuerpo es informativo).
  **Sin esas tres, quedan 9 y no se llega al mínimo de 10**; y después del
  07-08 quedarían 2, bajo el mínimo de 3.
- En sentido contrario, las seis D (límite) llevarían la cuenta a 18.
- **El lado de después descansa en tres piezas, con la mitad de la cobertura.**
  Lo no leído podría añadir C (ver §6, donde los *slugs* no muestran ninguna) o
  más D (88944 salió de ahí).

---

## 4. Las piezas que cuentan, con su cita

### D, antes del 07-08 (9)

| # | Fecha | URL | Lo que dice la casa |
|---|---|---|---|
| 82336 | 2025-11-04 | [abelardo-de-la-espriella-sorprende-con-masivo-acto…](https://seguimiento.co/colombia/abelardo-de-la-espriella-sorprende-con-masivo-acto-politico-en-el-movistar-arena-82336) | Titular «sorprende con masivo acto»; cuerpo: «demostró su capacidad de convocatoria»; cierre: «el ‘rugido inicial’ de un movimiento que busca posicionarse como una alternativa fuerte dentro de la derecha» |
| 83744 | 2026-01-19 | [polemicos-aportes-y-gastos…-cepeda](https://seguimiento.co/colombia/polemicos-aportes-y-gastos-por-964-millones-rodean-la-campana-de-cepeda-83744) | «Polémicos aportes y gastos… rodean la campaña de Cepeda»; «quedó bajo fuerte escrutinio» |
| 84797 | 2026-03-10 | [abelardo-revela-su-formula-vicepresidencial…](https://seguimiento.co/colombia/abelardo-revela-su-formula-vicepresidencial-el-economista-jose-manuel-restrepo-84797) | Entradilla: «El destacado exministro de Hacienda… tiene una larga trayectoria» |
| 85210 | 2026-03-29 | [sin-filtro-el-polemico-discurso-de-ivan-cepeda…](https://seguimiento.co/colombia/sin-filtro-el-polemico-discurso-de-ivan-cepeda-que-encendio-medellin-85210) | «¡Sin filtro! El polémico discurso de Iván Cepeda»; «Lejos de ofrecer una disculpa… para profundizar sus denuncias» |
| 85648 | 2026-04-19 | [tras-meses-negandose-los-debates-cepeda…](https://seguimiento.co/colombia/tras-meses-negandose-los-debates-cepeda-ahora-reta-paloma-y-de-la-espriella-85648) | «Tras meses negándose a los debates, Cepeda ahora reta…» |
| 85909 | 2026-05-02 | [ivan-cepeda-en-la-mira…-le-dono-609-millones](https://seguimiento.co/colombia/ivan-cepeda-en-la-mira-compania-con-capital-de-20-millones-le-dono-609-millones-85909) | «Iván Cepeda en la mira… le ‘donó’ $609 millones» (comillas irónicas de la casa) |
| 86124 | 2026-05-12 | [polemica-por-cuentas-de-cepeda…](https://seguimiento.co/colombia/polemica-por-cuentas-de-cepeda-hizo-mas-de-100-tarimazos-y-reporto-cero-gastos-86124) | Cierre propio: «El caso vuelve a poner sobre la mesa las dudas alrededor de la financiación de la campaña de Cepeda» |
| 86715 | 2026-06-05 | [intolerancia-simpatizantes-de-cepeda…](https://seguimiento.co/colombia/intolerancia-simpatizantes-de-cepeda-vandalizan-sede-de-abelardo-en-bogota-86715) | «Intolerancia: simpatizantes de Cepeda vandalizan sede de Abelardo» (el cierre recoge la denuncia contraria) |
| 86754 | 2026-06-08 | [por-que-no-se-van-del-pais-el-polemico-mensaje-de-cepeda…](https://seguimiento.co/colombia/por-que-no-se-van-del-pais-el-polemico-mensaje-de-cepeda-sus-detractores-86754) | «En la recta final de la campaña presidencial, el discurso del oficialismo se endurece y cada vez se radicaliza más» |

### D, después del 07-08 (3)

| # | Fecha | URL | Lo que dice la casa |
|---|---|---|---|
| 88944 | 2026-09-04 | [28-dias-tardo-el-presidente-en-cumplir-su-palabra…](https://seguimiento.co/colombia/28-dias-tardo-el-presidente-en-cumplir-su-palabra-dar-de-baja-alias-el-bendito-menor-88944) | Firmada por Vanessa Redondo Peña. «28 días tardó el Presidente en cumplir su palabra»; «la cuestionada política de ‘Paz Total’ del gobierno Petro, que dio concesiones a las estructuras armadas» |
| 88960 | 2026-09-05 | [cuatro-anos-de-paz-total-y-bendito-menor-seguia-libre…](https://seguimiento.co/colombia/cuatro-anos-de-paz-total-y-bendito-menor-seguia-libre-petro-ahora-cuestiona-su-muerte-88960) | «Cuatro años de ‘Paz Total’ y ‘Bendito Menor’ seguía libre: Petro ahora cuestiona su muerte»; «el fallido proceso de ‘Paz Total’» |
| 89137 | 2026-09-11 | [ahora-si-se-acabo-la-paz-total…](https://seguimiento.co/colombia/ahora-si-se-acabo-la-paz-total-abelardo-cerro-todos-los-dialogos-con-grupos-armados-89137) | «Ahora sí, se acabó la “Paz Total”» |

### C (2)

| # | Fecha | URL | Lo que dice la casa |
|---|---|---|---|
| 83557 | 2026-01-08 | [llamada-petro-trump-una-conversacion-que-desescala-la-tension](https://seguimiento.co/mundo/llamada-petro-trump-una-conversacion-que-desescala-la-tension-83557) | Encuadre propio favorable al gobierno de Petro: «una conversación que desescala la tensión», «marca un punto de inflexión» |
| 84775 | 2026-03-08 | [no-le-alcanzo…-alvaro-uribe-no-llega-al-congreso](https://seguimiento.co/colombia/no-le-alcanzo-con-el-numero-25-de-la-lista-alvaro-uribe-no-llega-al-congreso-84775) | «¡No le alcanzó!»; «En una jugada arriesgada…» (burla propia al jefe del Centro Democrático) |

### Límite (no cuentan)

| # | Fecha | Lado | URL | Por qué queda fuera |
|---|---|---|---|---|
| 87840 | 2026-07-23 | D | [la-ambiciosa-propuesta-de-abelardo](https://seguimiento.co/colombia/barranquilla-como-capital-alterna-de-colombia-la-ambiciosa-propuesta-de-abelardo-87840) | «ambiciosa» puede ser descriptivo; el cuerpo cierra con un elogio citado |
| 87873 | 2026-07-24 | D | [didier-blanco-el-experto…](https://seguimiento.co/colombia/didier-blanco-el-experto-en-derecho-penal-que-llega-la-unp-en-gobierno-de-abelardo-87873) | Perfil elogioso de un nombramiento; formato de perfil |
| 86383 | 2026-05-25 | D | [tras-una-candidatura-que-nunca-despego-caicedo…](https://seguimiento.co/magdalena/tras-una-candidatura-que-nunca-despego-caicedo-se-adhiere-ivan-cepeda-86383) | Burla propia a Caicedo, pero **Caicedo es el rival de Pinedo, cliente del medio**: puede ser conflicto local y no eje |
| 85601 | 2026-04-16 | D | [lo-zafaron-caicedo-bota-el-chupo…](https://seguimiento.co/colombia/lo-zafaron-caicedo-bota-el-chupo-tras-no-ser-invitado-debate-presidencial-85601) | «¡Lo zafaron! Caicedo ‘bota el chupo’», «pataleta»: lo mismo que 86383 |
| 87098 | 2026-06-21 | D | [ivan-cepeda-hace-un-sereno-llamado…](https://seguimiento.co/colombia/ivan-cepeda-hace-un-sereno-llamado-la-movilizacion-y-oposicion-tras-su-derrota-87098) | Las comillas de «‘sereno’» son irónicas o no; el cuerpo es neutro |
| 88520 | 2026-08-19 | D | [revelan-que-gobierno-petro-dejo-esquema…](https://seguimiento.co/colombia/revelan-que-gobierno-petro-dejo-esquema-de-seguridad-de-la-unp-para-gabriela-munoz-88520) | Encuadre contra el expresidente, pero lo sostiene un dato atribuido |
| 87106 | 2026-06-21 | C | [el-discurso-conciliador-de-abelardo…](https://seguimiento.co/colombia/voy-gobernar-para-todos-el-discurso-conciliador-de-abelardo-de-la-espriella-87106) | «‘conciliador’» entre comillas puede ser escepticismo; el cuerpo es neutro |
| 82650 | 2025-11-19 | C | [el-gobierno-anuncia-inversion-historica…](https://seguimiento.co/colombia/el-gobierno-anuncia-inversion-historica-de-us150-millones-para-la-salud-mental-82650) | «histórica» es probablemente palabra del Gobierno |

**Fuera del eje colombiano, no cuenta:** 83159 (14-12-2025, firmada por Redondo
Peña), [«Aplastante derrota de la izquierda en Chile»](https://seguimiento.co/mundo/aplastante-derrota-de-la-izquierda-en-chile-jose-antonio-kast-elegido-presidente-83159),
que abre: «El panorama político de América Latina empieza a cambiar». Va en la
misma dirección que D.

---

## 5. Contrapesos (condición 4)

Lo que contradice la dirección, y cuánto pesa:

1. **Dos piezas C claras** (83557, 84775) y dos de límite (87106, 82650).
   Pesan poco: 2 frente a 12.
2. **El contenido de campaña (P) va más a la izquierda que a la derecha.** 19
   piezas, todas firmadas «Seguimiento.co», ninguna rotulada como publicidad:
   - **12 a candidaturas de la izquierda o afines a Petro:**
     - Rafael Noya, a la Gobernación: 81854 («nutrido acompañamiento») y 82317
       («Multitudinaria caravana»);
     - Margarita Guerra, de Fuerza Ciudadana: 82353, 82463, 82479, 82487 y
       82536;
     - Felipe Hernández, del Pacto Histórico, a la Cámara: 83592, 83628,
       83734, 83760 y 83932 («se toma los barrios de Santa Marta»).
   - **7 a candidaturas de la derecha o del centro:**
     - María Claudia Pacheco, del Centro Democrático: 83567, 84506, 84556 y
       84738 («¡… la candidata que llega más pegada a las urnas!»);
     - Isis Navarro, del Centro Democrático: 84510;
     - Luis Santana, a la Gobernación, con el apoyo de Paloma Valencia: 82391 y
       82426.
   - Dos más sin partido claro: 84057 (Ricardo Díazgranados) y 83249 (Pablo
     Acuña).
   - **Lectura:** es conducta comercial o de comunicado, repartida entre todos
     los partidos, y no línea de la casa. Por eso no cuenta. Pero es
     probablemente la «inclinación de izquierda» que se vio en algo. Si alguien
     la contara como voz de la casa, la cuenta quedaría 12 + 7 = 19 D frente a
     2 + 12 = 14 C, y **la regla no se cumpliría**. Este es el contrapeso
     principal, y se deja escrito.
3. **Lo que da voz a los críticos del gobierno entrante** (atribuido, no cuenta
   como C, pero existe): 86853 (Cepeda pide a la CPI investigar a De la
   Espriella), 87511 (Cepeda llama «paramilitares» sus propuestas), 88991
   (Cepeda «arremete contra el presidente»), 89230 (Fecode marchará contra el
   Gobierno) y 89293 y 89472 (jueces le ordenan cosas al Presidente). Estas
   tres últimas, solo por el *slug*. Y las que cita la resolución: la pieza de
   la primera dama (sufijo 89819) da voz a la pregunta del Pacto, y la de
   Sincelejo (sufijo 89799) a la réplica de Yahir Acuña. **Ninguna de las
   tres está en el universo de URL de este barrido:** son la laguna del CDX.
4. **La «depuración» del 16-08-2026** (sufijo 88444, firmada por Redondo
   Peña), según la resolución, se abre como «veeduría» de nombramientos del
   gobierno entrante. Puede leerse en los dos sentidos. No se leyó aquí, porque
   no está en el universo.
5. **La conducta con Petro antes del 07-08 fue fiscalización dura (14 F)**:
   «Gravísimo» (82154), «El absurdo consejo de Petro» (85911), «Petro se
   descara» (86606), «¡Desespero electoral!» (87094), «¿Indolencia?» (85797).
   **No cuenta**, por el polo fijo. **Lo que sí se anota:** en las 66 piezas
   leídas del gobierno de De la Espriella **no hay ni una F equivalente**, ni
   una crítica propia. Pero es poco tiempo (dos meses) y poca cobertura, y no
   se usa como D.
6. **El conflicto de interés de la ficha empuja en otra dirección.** El cliente
   principal es la Alcaldía de Pinedo, y las burlas a Caicedo (85601, 86383)
   pueden venir de ahí. Por eso están en límite.

**F, para que se puedan recontar (no cuentan):**

| # | Fecha | URL |
|---|---|---|
| 82154 | 2025-10-24 | [gravisimo-petro-su-familia…](https://seguimiento.co/colombia/gravisimo-petro-su-familia-y-armando-benedetti-incluidos-en-la-lista-clinton-82154) |
| 84056 | 2026-02-04 | [juicio-investigan-al-presidente-petro…](https://seguimiento.co/colombia/juicio-investigan-al-presidente-petro-por-dineros-de-pipe-tulua-en-su-campana-de-2022-84056) |
| 84238 | 2026-02-12 | [gobierno-petro-prorroga-nombramientos…](https://seguimiento.co/colombia/gobierno-petro-prorroga-nombramientos-de-gestores-de-paz-del-eln-pese-crimenes-84238) |
| 84416 | 2026-02-20 | [escandalo-en-el-gobierno-petro…](https://seguimiento.co/colombia/escandalo-en-el-gobierno-petro-familia-de-mintrabajo-suma-1000-millones-en-contratos-84416) |
| 85288 | 2026-04-01 | [presidente-petro-sube-375-pesos…](https://seguimiento.co/colombia/presidente-petro-sube-375-pesos-la-gasolina-en-plena-semana-santa-asfixia-viajeros-85288) |
| 85552 | 2026-04-15 | [abucheos-marcaron-la-intervencion-de-petro…](https://seguimiento.co/colombia/abucheos-marcaron-la-intervencion-de-petro-en-macrorueda-de-negocios-de-corferias-85552) |
| 85560 | 2026-04-15 | [pese-multa-por-desacato…](https://seguimiento.co/colombia/pese-multa-por-desacato-petro-vuelve-llamar-ladrones-directivos-de-coosalud-85560) |
| 85797 | 2026-04-27 | [indolencia-presidente-postea-fotos…](https://seguimiento.co/colombia/indolencia-presidente-postea-fotos-de-cumpleanos-tras-atentados-terroristas-85797) |
| 85911 | 2026-05-02 | [el-absurdo-consejo-de-petro…](https://seguimiento.co/colombia/el-absurdo-consejo-de-petro-tras-subidon-de-la-gasolina-comprar-vehiculo-electrico-85911) |
| 86606 | 2026-06-01 | [petro-se-descara-en-participacion-politica](https://seguimiento.co/colombia/vamos-ganar-y-yo-mismo-me-pondre-al-frente-petro-se-descara-en-participacion-politica-86606) |
| 87094 | 2026-06-21 | [desespero-electoral…](https://seguimiento.co/colombia/desespero-electoral-petro-pide-escrutinios-para-reconocer-resultados-presidenciales-87094) |
| 87166 | 2026-06-23 | [en-medio-de-retahila…](https://seguimiento.co/colombia/en-medio-de-retahila-petro-reconoce-que-iniciara-el-empalme-y-su-retirada-87166) |
| 87766 | 2026-07-21 | [petro-quedo-solo…](https://seguimiento.co/colombia/petro-quedo-solo-cupula-militar-se-retiro-antes-de-su-discurso-87766) |
| 87868 | 2026-07-23 | [plan-exodo-en-presidencia…](https://seguimiento.co/colombia/plan-exodo-en-presidencia-llevandose-fotos-de-petro-inicio-salida-de-funcionarios-87868) |

**R después del 07-08, no cuentan:** 88839 (gestores de paz desaparecidos;
según la propia pieza, sale de Infobae, que a su vez recoge una columna de
Cambio) y 89754 (madre de Gabriela Muñoz; refrito de 6AM W, según la
resolución).

---

## 6. Después del 07-08: lo no leído, por su *slug*

Son 69 URL de la selección posteriores al 07-08 que no se descargaron. El
*slug* es el titular sin puntuación ni mayúsculas, así que se puede ver si el
titular toma postura. No se leyó la entradilla ni el cuerpo, así que **nada de
esto entra en la cuenta**.

- **Titulares que podrían ser D:**
  - 89550, «De la Espriella ofrece 3.000 millones por ‘Pinocho’: estamos
    respirándole en la nuca» (cita);
  - 89329, «Los vamos a acabar: De la Espriella anuncia captura…» (cita);
  - 89399, «Alias ‘Cholo’ había sido reconocido como negociador de paz durante
    el gobierno Petro». Esta se leyó después: el dato lo atribuye al Presidente,
    así que es A.
- **Titulares que podrían ser C o V:**
  - 89472, «Juez ordena a De la Espriella abstenerse de actos religiosos como
    presidente»;
  - 89293, «Juez ordenó a MinDefensa revelar información sobre vuelos de
    Abelardo de la Espriella»;
  - 89230, «Fecode y centrales obreras marcharán contra el Gobierno»;
  - 88991, «“Hacer diálogos de paz es un derecho y un deber”: Cepeda arremete
    contra el presidente».

  Las cuatro son atribuidas.
- **El resto** son medidas del Gobierno, nombramientos o sucesos, con titular
  informativo.
- **Ninguno de los 69 *slugs* muestra una crítica propia** al gobierno
  entrante.

---

## 7. PROPUESTA (pendiente de la firma del responsable editorial)

**+0,15, dentro de la banda de orientación mixta (−0,20 a +0,20), con
inclinación de centroderecha declarada. Sustituye al 0,00.** Sigue sin
firmarse.

**Por qué se mueve.** Las cinco condiciones se cumplen con el criterio
declarado:
- 12 D frente a 2 C, es decir, 6 a 1;
- 9 D antes del cambio y 3 después;
- todas en voz de la casa, con URL.

La dirección es la misma que la resolución vio, en débil, en las columnas
(objeción 7) y en el encuadre posterior a agosto (objeción 8). Ahora la
sostiene la voz de la casa:
- antes del cambio, sospecha e ironía propias contra la campaña de Cepeda, y
  elogio propio a De la Espriella;
- después, elogio al presidente que «cumplió su palabra» y el «fallido» de la
  política del anterior.

**Por qué no más, y no en la banda moderada (+0,20 o más).** Por la regla 2,
ante la duda entre dos bandas se elige la más cercana a la mixta. Y aquí hay
duda real:
1. **El lado de después del cambio se cumple por el mínimo**: 3 piezas, con la
   mitad de la cobertura o menos (§1, «Lagunas»). Con el recuento más estricto
   (§3, «Sensibilidad») no se llega al mínimo.
2. **Hay un contrapeso grande que no cuenta pero existe**: 19 piezas de
   promoción de campaña sin rótulo, más a la izquierda (12) que a la derecha
   (7). Si fueran voz de la casa, la regla no se cumpliría.
3. **Hay un factor que confunde las cosas**: parte de las burlas a la
   izquierda local (Caicedo) se explica por la rivalidad con el cliente
   principal del medio, la Alcaldía de Pinedo. Por eso van en límite.
4. **Frente a los medios vecinos de la escala:**
   - **Vive el Meta (+0,25)** tiene 12 a 1, con 7 y 5 a cada lado y cobertura
     completa. Seguimiento tiene 12 a 2, con 9 y 3 y media cobertura después
     del cambio, así que va por debajo de Vive el Meta.
   - **El Pilón (+0,20)** tiene editoriales propios con «apoyamos». Seguimiento
     no tiene editorial: solo titulares, así que va por debajo de El Pilón.

**Por qué no 0,00.** El 0,00 con evidencia exige la misma conducta con los dos
lados, y no es la que se ve:
- antes del cambio, la ironía propia va contra una sola campaña presidencial;
- después, el elogio propio va al gobierno entrante y la crítica propia, al
  saliente;
- y no hay ni una crítica propia al gobierno de De la Espriella en lo leído.

Mantener 0,00 «porque no alcanza» sería defendible **solo** con el recuento
estricto. Si el responsable editorial prefiere ese criterio, la alternativa es: **0,00 por la
regla 2, con la dirección de centroderecha declarada como tensión y la
condición 2 pendiente de completar la descarga de agosto a octubre.**

**Qué lo movería:**
- **Hacia +0,20 o más:** completar la descarga posterior al 07-08 (las 69 URL
  de §6 y el hueco del CDX) y encontrar más D sin C.
- **Hacia 0,00:**
  - encontrar en lo no leído crítica propia al gobierno de De la Espriella;
  - o que se acredite que las piezas P son voz de la casa, y no propaganda.

**Lo que NO cambia:**
- el conflicto de interés con la Alcaldía de Santa Marta, que va en la ficha
  como desvelamiento y no mueve el número;
- la firma: mover el valor no hace firmable la ficha.

---

## 8. Avisos

- **La ficha dice Santa Marta (Magdalena).** El encargo de este barrido decía
  «Barranquilla/Caribe». Se siguió la ficha.
- **No se descargó el sitemap vivo** porque `robots.txt` excluye `/*?page=`. Se
  usaron las copias de Internet Archive para descubrir URL, y el texto se leyó
  del sitio o de la instantánea `id_` (HTML original).
- **En este archivo no hay cédulas, teléfonos ni direcciones de personas
  naturales.**
- Los guiones y la descarga cruda están fuera del repositorio, en el
  *scratchpad* de la sesión (`rx/seguimiento/`: `universe.json`,
  `cands.json`, `extracted.json`, `html/`).
