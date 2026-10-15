# Respuesta — Claude Opus 5.5 sobre Diario del Huila

| | |
|---|---|
| **Modelo** | Claude Opus 5.5 |
| **Versión exacta** | `claude-opus-5-5` |
| **Fecha de la consulta** | 2026-10-08 |
| **Quién la hizo** | Claude Code, a petición del responsable editorial (ciclo 2, fase 2, tanda 3; revisor de la misma casa que el autor de las fichas, ver DECISIONES.md 2026-10-07) |
| **¿Tuvo acceso a la red?** | sí |

> **Se pega LITERAL lo que devolvió el modelo, sin editar ni resumir.** Si se
> recorta, se pierde justo lo que pueda incomodar. Los comentarios nuestros van
> al final, en la sección de resolución, claramente separados.

---

## RESPUESTA LITERAL

> **Nota de quien resuelve (2026-10-08):** se han sustituido los números de cédula
> que traía el texto por «[número de cédula omitido: dato personal de una persona
> natural, Ley 1581]». Es la única alteración del texto literal.

```
DECLARACIÓN PREVIA
La ficha la escribió otro modelo de Claude. Yo también soy Claude (Opus 5.5).
Somos de la misma casa: mi acuerdo no debe leerse como validación independiente,
y he buscado a propósito en fuentes que la ficha NO usa (SECOP I y II, prensa de
la competencia en Neiva, la sección de editoriales del propio medio).

MÉTODO Y DÓNDE BUSQUÉ
- robots.txt leído antes de descargar: diariodelhuila.com y lanacion.com.co no
  excluyen a ClaudeBot / Claude-Web / anthropic-ai. diariodelhuila.com prohíbe
  /feed/, /author/ y /*/page/* para todos; no usé esas rutas para extraer datos
  (no pude paginar la sección de editoriales: solo vi su primera página).
- HTML crudo con curl (UA Chrome). Las citas de abajo salen del HTML descargado
  hoy, salvo donde digo lo contrario.
- Páginas leídas: /directorio/, /politica-de-privacidad/, /editoriales/ (primera
  página), el especial "DIARIO DEL HUILA, 60 AÑOS DE HISTORIA" (2026-08-08), seis
  editoriales de 2026 y un perfil de 2021. Pie de página de todos los artículos.
- API WordPress del medio (/wp-json/wp/v2/posts/<id>): fiable pidiendo por id.
  OJO: el endpoint /wp-json/wp/v2/search y el buscador ?s= devolvieron resultados
  idénticos para consultas distintas (caché); no los uso como prueba de ausencia.
- datos.gov.co: SECOP II (jbjy-vk9h) por documento_proveedor; SECOP I (f789-7hwg)
  por identificacion_del_contratista con igualdad exacta, NIT sin DV.
- La Nación (Neiva): portada y dos artículos.
- WebSearch no estuvo disponible en esta sesión (cupo agotado); por eso no
  consulté RUES, Wikipedia ni prensa nacional por buscador. Lo declaro como límite.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré venta ni fusión. El propio medio dice el 2026-08-08: «Actualmente,
  el diario continúa en manos de la familia Duque Rengifo, bajo la dirección de
  María Pía Duque Rengifo» (https://diariodelhuila.com/diario-del-huila-60-anos-historia/,
  publicado 2026-08-08). Es declaración del propio medio, no registro mercantil.
  Lo que SÍ cambió, según SECOP I, es el representante legal que firma los
  contratos de la sociedad Diario del Huila Digital S.A.S. (NIT 901518850): hasta
  marzo de 2025 firma LUISA MARIA DUQUE CERON (CC [número de cédula omitido: dato personal de una persona natural, Ley 1581]); desde 2025-02-06 y en
  todos los contratos de 2025-09 a 2026-07 firma MAXIMILIANO DUQUE RENGIFO
  (CC [número de cédula omitido: dato personal de una persona natural, Ley 1581]). En SECOP II, el contrato del 2026-01-27 (Biorgánicos del Sur del
  Huila) todavía registra a Luisa María Duque Cerón. No sé si son principal y
  suplente o si hubo relevo: no pude leer el certificado de Cámara de Comercio.
- La persona que la ficha nombra como directora, ¿sigue viva y en el cargo?
  Sí, a 2026-10-08: el pie de página de los artículos publicados del 2026-09-15 al
  2026-10-07 dice literalmente «Fundadores:Max Duque Gómez - Max Duque Palma
  Directora María Pia Duque Rengifo»; y el especial del 2026-08-08 la nombra
  directora. No encontré noticia de fallecimiento (búsqueda limitada al sitio).
- ¿Quién dirige hoy la redacción?
  Directora: María Pía Duque Rengifo (fuente anterior). No encontré nombre de
  jefe/editor de redacción en el directorio ni en el pie. Los editoriales que leí
  van firmados por el usuario de CMS «WebMaster», no por una persona.
- ¿Hay un registro más reciente que la fuente que la ficha cita?
  Sí, en parte. La página /directorio/ que la ficha cita tiene, en su propio
  JSON-LD, "dateModified":"2021-05-24T03:09:06+00:00": es una página de 2021.
  Más recientes: (a) el especial del 2026-08-08; (b) el pie de página vivo; (c)
  SECOP I, con representante legal y razón social hasta 2026-07-14. No encontré
  certificado de existencia y representación ni composición accionaria.

## OBJECIONES

1. LA FICHA NO NOMBRA AL REPRESENTANTE LEGAL, Y ESTÁ EN UN REGISTRO PÚBLICO
- QUÉ: La ficha dice que de Diario del Huila solo sabe «quién firma como
  directora y que hay dos sociedades» y deja el control en blanco.
- POR QUÉ: SECOP I registra quién representa legalmente a las dos sociedades.
  Editora del Huila S.A.S. (NIT 891101933): LUISA MARIA DUQUE CERON en los 39
  contratos de 2016-06-07 a 2021-06-25. Diario del Huila Digital S.A.S. (NIT
  901518850): LUISA MARIA DUQUE CERON (2022–2025-03) y MAXIMILIANO DUQUE RENGIFO,
  CC [número de cédula omitido: dato personal de una persona natural, Ley 1581] (2025-02-06 → 2026-07-14, último contrato). Un perfil publicado por
  el propio diario (2021-08-14) cuenta que, tras morir Max Duque Palma, «al asumir
  Max Duque Rengifo la gerencia, hubo una reestructuración». No es accionariado,
  pero sí es quién administra hoy la sociedad que factura: cierra a medias la
  laguna del nivel 1 y la ficha debería decirlo.
  SOSPECHA, no comprobada: María Pía y Maximiliano Duque Rengifo serían hermanos,
  hijos de Max Duque Palma y de María Mercedes Rengifo de Duque (gerente de
  Editora del Huila Ltda. según el perfil de 2021). Solo lo infiero de los
  apellidos; no tengo fuente.
- FUENTE: datos.gov.co, SECOP I (f789-7hwg), consulta
  identificacion_del_contratista='901518850' y ='891101933', hecha 2026-10-08;
  https://diariodelhuila.com/una-mujer-que-levanto-una-empresa-con-rollos-de-papel/
  (2021-08-14, solo como antecedente de la sucesión).
- NIVEL: registro externo (control/administración, no capital).

2. CONFLICTO DE INTERÉS NO DECLARADO: EL REPRESENTANTE LEGAL EN PLEITO
   PATRIMONIAL CON LA ALCALDÍA DE NEIVA
- QUÉ: La ficha (REFUTACIÓN 1) dice que el número se movería «sobre todo si
  aparece capital con vínculo político en el departamento», y no reporta ninguno.
- POR QUÉ: La Nación (Neiva) publicó que la sociedad Construcciones e Inversiones
  D&R, «representada por el empresario Max Duque Rengifo», fue la beneficiaria de
  las mayores «daciones en pago» aceptadas por el exalcalde Gorky Muñoz: «la
  Alcaldía de Neiva aceptó las daciones en pago de cinco predios por un valor
  global de 3.567 millones de pesos, para saldar obligaciones tributarias por una
  suma total de 153,31 millones de pesos de la sociedad Duque Rengifo». La
  alcaldía actual (Germán Casagua) las impugnó como «compraventa simulada». Un
  segundo artículo (2025-07-07) informa que las dos primeras daciones de otros
  propietarios se revocaron; no dice qué pasó con las de D&R.
  Si el Max Duque Rengifo de D&R es el Maximiliano Duque Rengifo que hoy firma
  por Diario del Huila Digital (identidad PROBABLE por nombre y ciudad, NO
  comprobada con cédula), el representante legal del diario tiene un interés
  patrimonial directo frente a la alcaldía de Neiva y a favor de la administración
  anterior. Eso es justo el conflicto que el protocolo dice que hay que declarar.
  No mueve por sí solo el eje izquierda-derecha, pero la ficha no puede firmarse
  sin él.
  Advertencias: (a) los artículos son de 2025-02-11 y 2025-07-07, más de 12 meses;
  vale solo si el pleito sigue vivo, y no pude comprobarlo; (b) la fuente es La
  Nación, competidor directo en Neiva (pie de su web: «COMUNICACIONES OLAVE
  S.A.S.»), así que hay interés competitivo en publicarlo; (c) no pude comprobar
  cómo cubrió Diario del Huila el caso: su buscador devolvió resultados genéricos.
- FUENTE: https://www.lanacion.com.co/daciones-en-pago-enredan-a-max-duque-rengifo/
  (datePublished 2025-02-11); https://www.lanacion.com.co/se-derrumban-canjes-de-predios-por-impuestos/
  (2025-07-07).
- NIVEL: registro externo (prensa) / propiedad-control (vínculo del administrador).

3. LA FICHA DECLARA QUE NO HAY LÍNEA EDITORIAL SIN HABER IDO A LOS EDITORIALES
- QUÉ: «No he encontrado un manifiesto editorial ni una línea declarada: el
  directorio trae la dirección y el contacto, y nada sobre posición.» Y el
  argumento se apoya solo en «coherencia con la banda de los diarios comerciales
  regionales», «no por evidencia que sitúe a este medio en el eje».
- POR QUÉ: El medio tiene una sección /editoriales/ (categoría con 1.682 entradas
  en su API) con editorial casi diario y sin firma personal. La ficha no la cita.
  Leí seis de 2026; la conducta es la siguiente (citas literales):
  · 2026-02-20, gobierno Petro, «Presidente Petro, protestar no es vandalismo»:
    tras el ataque a la sede del Centro Democrático en Neiva, atribuye la
    intolerancia a «sectores radicales del petrismo» y dice que es «alimentada
    desde el discurso del propio presidente Gustavo Petro».
  · 2026-09-15, gobierno De la Espriella, «Autonomía universitaria sí, pero no
    santuarios para la violencia»: explica y respalda el protocolo de ingreso de
    la Fuerza Pública a universidades («la violencia no puede tener fuero»), con
    reservas de proporcionalidad («El reto será demostrar que el protocolo cierre
    esa brecha sin abrir otra: la del abuso de autoridad»).
  · 2026-09-19, «Un fallo que vuelve a poner la justicia en el centro» (Plazas
    Vega): recoge sin reparo la frase presidencial «Se hizo justicia con un héroe
    de la patria» y centra el argumento en que el M-19 fue indultado mientras los
    militares siguieron procesados; pide que «esa memoria no sea selectiva».
  · 2026-09-28, «Seguridad: de los anuncios a los resultados»: presenta un
    operativo en Tello como parte de «una política de seguridad del Gobierno
    Nacional del presidente Abelardo De La Espriella»; el tono es de respaldo con
    exigencia de «continuidad».
  · 2026-10-06, «El salario mínimo no puede ser una apuesta política»: critica el
    aumento del 23 % de 2026 (decisión del gobierno anterior) y pide al nuevo
    gobierno criterio técnico, austeridad y disciplina fiscal.
  · 2026-09-21, «La paz también se mide en respuestas»: sobre la JEP y el
    exsecretariado de las Farc en Pitalito; no rechaza la paz, pero centra la
    exigencia de verdad en los excomandantes.
  Lectura según la REGLA DEL POLO FIJO: con el gobierno saliente, el editorial
  atribuye responsabilidad política al presidente; con el entrante, el editorial
  explica, contextualiza y respalda sus medidas con salvedades, y ninguno de los
  que leí lo fiscaliza con la dureza del de febrero. Eso es asimetría a través del
  cambio de gobierno, en la dirección de la derecha. Además el caso Plazas Vega no
  es fiscalización: es encuadre de memoria histórica alineado con el presidente.
  Esto NO contradice el signo de +0,20; contradice la afirmación de que no hay
  evidencia, y el número dejaría de ser «por coherencia de banda» para pasar a
  apoyarse en conducta editorial. Muestra pequeña (6 piezas, 1 previa a agosto);
  no pude paginar el archivo (robots prohíbe /*/page/*), así que no puedo
  descartar editoriales críticos con De la Espriella que no vi.
- FUENTE: https://diariodelhuila.com/presidente-petro-protestar-no-es-vandalismo/ (2026-02-20);
  https://diariodelhuila.com/autonomia-universitaria-si-pero-no-santuarios-para-la-violencia/ (2026-09-15);
  https://diariodelhuila.com/un-fallo-que-vuelve-a-poner-la-justicia-en-el-centro/ (2026-09-19);
  https://diariodelhuila.com/la-paz-tambien-se-mide-en-respuestas/ (2026-09-21);
  https://diariodelhuila.com/seguridad-de-los-anuncios-a-los-resultados/ (2026-09-28);
  https://diariodelhuila.com/el-salario-minimo-no-puede-ser-una-apuesta-politica/ (2026-10-06).
- NIVEL: hecho editorial de los últimos 12 meses / conducta observable.

4. LA FUENTE CITADA PARA EL NIVEL 1 ES DE 2021 Y NO DICE TODO LO QUE SE LE ATRIBUYE
- QUÉ: La ficha usa /directorio/ como fuente de «hoy», y atribuye al medio que se
  presenta como «el medio más antiguo del Huila y del sur de Colombia» y «el de
  mayor número de lectores del departamento».
- POR QUÉ: (a) /directorio/ declara dateModified 2021-05-24. Los datos coinciden
  con el pie vivo de 2026, así que el hecho se sostiene, pero la cita correcta del
  presente es el pie de página actual o el especial del 2026-08-08. (b) En el texto
  de /directorio/ no aparecen ni «más antiguo» ni «mayor número de lectores»:
  solo «Editora del Huila SA - Diario del Huila Fundado el 8 de Agosto de 1966»,
  dirección, teléfono, fundadores y directora. La ficha no da fuente para esas dos
  autodescripciones. No encuentro fuente para ellas.
- FUENTE: https://diariodelhuila.com/directorio/ (HTML descargado 2026-10-08;
  dateModified 2021-05-24).
- NIVEL: declaración del propio medio.

5. RAZÓN SOCIAL Y PAPEL DE LA «SEGUNDA SOCIEDAD»: HAY DATO PÚBLICO QUE LA FICHA
   NO USA
- QUÉ: «Editora del Huila S.A.» y «La segunda sociedad de 2021 está sin explicar».
- POR QUÉ: (a) En SECOP I y II la sociedad figura como «EDITORA DEL HUILA S.A.S.»
  (NIT 891101933) desde 2016; la política de privacidad del sitio (modificada
  2024-04-19) habla de una tercera denominación, «Diario del Huila S.A.S». El pie
  sigue diciendo «Editora del Huila SA». Hay que pedir el certificado para saber
  cuál es la vigente. (b) La función de la segunda sociedad sí se puede describir
  en parte: Editora del Huila S.A.S. no tiene contratos públicos después del
  2021-06-25 (SECOP I) ni del 2019-10 (SECOP II); desde 2022-01 toda la
  contratación pública pasa a Diario del Huila Digital S.A.S. (NIT 901518850). Es
  hoy el vehículo que factura. Eso no dice quiénes son sus socios, pero sí que no
  es una filial marginal.
- FUENTE: SECOP I (f789-7hwg) y SECOP II (jbjy-vk9h), consultas del 2026-10-08;
  https://diariodelhuila.com/politica-de-privacidad/ (dateModified 2024-04-19).
- NIVEL: registro externo.

6. «NIVEL 2 — CONDUCTA MEDIDA: NO EXISTE» YA ES FALSO
- QUÉ: «No está ingerido. Cero artículos en el corpus.»
- POR QUÉ: La medición adjunta al envío (2026-10-08, ventana de 38 días) da 585
  artículos, 143 en alguna historia, 161 historias, agenda propia del 7 %, y
  coincide sobre todo con Infobae (42), El Colombiano (21) y Caracol Radio (19).
  La ficha (fechada 2026-08-09) está desactualizada. Advertencia: la compañía
  media (0,146) está saturada y NO puede usarse para sostener el +0,20; si la
  próxima versión la usa así, es una objeción válida. Por debajo del umbral de 60
  historias propias que la ficha misma pide en su REFUTACIÓN 2 no está (143
  artículos en historias), pero la ventana es de 38 días y no de 90.
- FUENTE: bloque «Conducta medida» de este mismo envío (2026-10-08).
- NIVEL: conducta medida.

## LO QUE NO PUDE VERIFICAR

- Accionariado de Editora del Huila S.A.S. y de Diario del Huila Digital S.A.S.:
  no hay acceso a RUES ni a certificados desde aquí, y no tuve buscador web. Sigue
  siendo la laguna principal.
- Si el «Max Duque Rengifo» de Construcciones e Inversiones D&R es la misma
  persona que «Maximiliano Duque Rengifo, CC [número de cédula omitido: dato personal de una persona natural, Ley 1581]» de SECOP. Probable, no
  comprobado.
- Estado actual del pleito de las daciones en pago (nulidad, revocatoria o
  acuerdo). Solo tengo los artículos de 2025.
- Parentesco entre María Pía Duque Rengifo, Maximiliano Duque Rengifo y Luisa
  María Duque Cerón. Solo sospecha por apellidos.
- Cómo cubrió Diario del Huila el caso de las daciones y a los alcaldes Gorky
  Muñoz y Germán Casagua: el buscador del sitio y su API de búsqueda devolvieron
  resultados en caché, no relacionados con la consulta.
- Vínculo con La Nación / Olave: no encontré ninguno. La Nación se identifica en
  su pie como «COMUNICACIONES OLAVE S.A.S.» y muestra el nombre «Felipe Olave
  Blackburn»; su buscador da resultados sobre Max Duque Rengifo en clave de
  fiscalización, que es lo contrario de un vínculo. Ausencia no concluyente.
- Militancia o cargo político actual de cualquier Duque Rengifo: no encontré
  fuente (sin buscador web). Que Max Duque Gómez fuera político liberal es
  historia y la regla del presente lo excluye.
- «Sería el primero del departamento en el catálogo»: no tengo acceso al
  catálogo. Si La Nación (Neiva) está catalogada, la frase es falsa.

## LO QUE FALTA

- El representante legal vigente (objeción 1) y el conflicto D&R / alcaldía de
  Neiva (objeción 2), declarados en la ficha aunque no muevan el número.
- La sección de editoriales como fuente de nivel 5 (objeción 3), con piezas
  fechadas antes y después del 7 de agosto de 2026.
- La contratación pública (abajo), que la ficha menciona como hipótesis en su
  REFUTACIÓN 3 pero no consulta.
- El certificado de Cámara de Comercio de Neiva de las dos (o tres) sociedades.

## EVIDENCIA QUE NO MUEVE EL NÚMERO

- CONTRATACIÓN PÚBLICA (datos.gov.co, consultado 2026-10-08; valores
  «contratados», no cobrados):
  · Últimos 12 meses (2025-10-08 → 2026-10-08): $16.110.000 contratados en 7
    contratos, todos con Diario del Huila Digital S.A.S. (NIT 901518850).
    SECOP I: $12.240.000 en 6 contratos: Cámara de Comercio de Neiva $5.800.000
    (2026-03-19); Cámara de Comercio del Huila $3.800.000 (2025-11-14 y
    2025-12-04); E.S.E. Hospital Departamental San Antonio de Pitalito $2.640.000
    (tres contratos de avisos, 2026-03 y 2026-07). SECOP II: Biorgánicos del Sur
    del Huila S.A. E.S.P. $3.870.000 (2026-01-27, pauta).
    Editora del Huila S.A.S.: $0 en el periodo.
  · Total histórico en SECOP: $471.109.867 contratados en 67 contratos.
    SECOP I: Editora del Huila S.A.S. $267.993.867 (39 contratos, 2016-06 →
    2021-06); Diario del Huila Digital $47.428.000 (14, 2022-01 → 2026-07).
    SECOP II: Editora $116.324.000 (8, 2017-10 → 2019-10); Digital $39.364.000
    (6, 2022-11 → 2026-01). Incluye dos registros en «Borrador» por $2.907.000.
  · Contratantes principales históricos: Gobernación del Huila $70.500.000 (todo
    en 2018-2019), Electrificadora del Huila $77.000.000 (último 2021-02), Empresas
    Públicas de Neiva $60.000.000 (2020-08), Municipio de Neiva (SECOP II, avisos y
    suscripciones 2017-2019, ~$115 millones), Cámara de Comercio de Neiva.
  · Lectura: la pauta pública registrada es baja y decreciente; no hay contratos
    con la Gobernación desde 2019 ni con la Alcaldía de Neiva desde 2019 en lo
    registrado. No sostiene la hipótesis de dependencia de pauta estatal de la
    REFUTACIÓN 3. Límite: SECOP no recoge pauta contratada por agencias, órdenes
    de servicio fuera de SECOP ni pauta de campañas.
- Hoy la directora sigue siendo María Pía Duque Rengifo y el medio se declara en
  manos de la familia Duque Rengifo (2026-08-08). Confirma la ficha.
- El especial de los 60 años (2026-08-08) atribuye al diario apertura a
  «Conservadores, liberales, integrantes de la Anapo e incluso sectores
  comunistas». Es historia (regla del presente): no cuenta en ninguna dirección.
- Los editoriales de 2026-09-15 y 2026-09-28 incluyen salvedades frente al
  gobierno entrante (proporcionalidad, abuso de autoridad, continuidad,
  retaliaciones). Es matiz real y lo anoto aunque no alcance a ser fiscalización.
- No encontré endoso editorial explícito a un candidato en las piezas que leí.
  No revisé el periodo de campaña de 2026 (mayo-junio) por la restricción de
  paginación: ausencia no concluyente.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-08. Pendiente de la firma del responsable editorial.**

**Datos personales retirados de la respuesta literal (Ley 1581).** La respuesta del revisor traía en cuatro sitios los números de cédula de Luisa María Duque Cerón y de Maximiliano Duque Rengifo. Se han sustituido por «[número de cédula omitido: dato personal de una persona natural, Ley 1581]». **Es la única alteración del texto literal.** En esta resolución los números se compararon por igualdad entre registros, sin escribirlos.

**Cómo se verificó.**
- **robots.txt, leído hoy y no copiado del revisor.**
  - diariodelhuila.com no menciona a ClaudeBot, Claude-Web ni anthropic-ai. Para todos los agentes excluye `/feed/`, `/author/*`, `/*/page/*`, `/wp-admin/` y `/cgi-bin/`.
  - lanacion.com.co solo excluye rutas técnicas.
  - datos.gov.co no menciona a Anthropic, y las rutas `/resource/` no están excluidas.
- **Páginas.** Las doce URL del revisor se descargaron en crudo el 2026-10-08 con `curl -sL -A "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 Chrome/126.0 Safari/537.36"`. Todas respondieron 200. Las citas se buscaron literalmente en el texto extraído, y las fechas salen del `datePublished` del JSON-LD.
- **Registros.** Se consultaron en datos.gov.co:
  - SECOP I (`f789-7hwg`) con `identificacion_del_contratista` igual a cada NIT;
  - SECOP II (`jbjy-vk9h`) con `documento_proveedor` igual a cada NIT;
  - **el RUES (`c82u-588k`)** por NIT y por razón social. El revisor no lo consultó y dijo que no tenía acceso.
- **Buscador web: no lo hubo.** La única llamada a WebSearch devolvió «cupo de la sesión agotado (200 de 200)». Lo que dependía de prensa de terceros o de la Rama Judicial queda como laguna (ver abajo).
- Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | La ficha no nombra al representante legal, y está en un registro público | sí | sí, y el RUES lo confirma | **Aceptada**. **Rechazada** como evidencia la sospecha de parentesco (no tiene fuente) |
| 2 | Conflicto no declarado: el representante legal pleitea con la Alcaldía de Neiva por las daciones en pago de D&R | sí | sí; la identidad está **confirmada por registro**. Parte del texto del revisor es **falsa** | **Aceptada como desvelamiento** en la ficha de propiedad, y **declarada como tensión**. **Rechazado** el «a favor de la administración anterior» |
| 3 | La ficha dice que no hay línea editorial sin haber ido a los editoriales | sí | sí: las seis piezas existen y las citas son literales | **Aceptada en el hecho** (hay nivel 5 y la ficha lo omitió). La asimetría a través del cambio de gobierno se **declara como tensión**, no como orientación medida |
| 4 | La fuente del nivel 1 es de 2021, y las dos autodescripciones no tienen fuente | sí | sí | **Aceptada**, y se amplía: «sería el primero del departamento» ya es falso |
| 5 | Razón social y papel de la segunda sociedad | sí | sí, con deformaciones menores | **Aceptada y ampliada por el RUES**: Editora del Huila S.A.S. está **en liquidación** |
| 6 | «Nivel 2 — no existe» ya es falso | sí (el envío) | sí | **Aceptada** |

### Lo verificado, objeción por objeción

**1 · Representante legal.**
- **SECOP I**, `nombre_del_represen_legal`, con fechas de firma comprobadas una por una:
  - **Editora del Huila (NIT 891101933).** Firma LUISA MARIA DUQUE CERON en todos los contratos, del 2016-06-07 al 2021-06-25. Una fila dice «LUISA MARIA DUQUE» y otra «DUQUECERON»; el número de documento es el mismo.
  - **Diario del Huila Digital (NIT 901518850).**
    - Luisa María Duque Cerón firma el 2022-01-25, el 2022-01-28, el 2022-02-22, el 2022-05-31, el **2025-03-03** y el **2025-03-19**.
    - Maximiliano Duque Rengifo firma el **2025-02-06** y todos los contratos del 2025-09-08 al **2026-07-14**.
    - Hay solapamiento en febrero y marzo de 2025, como dice el revisor.
- **SECOP II.** Los seis registros de la Digital, incluido el del 2026-01-27, siguen dando a Luisa María Duque Cerón. Los ocho de la Editora dan a «ESPEANZA RODRIGUEZ», un dato que el revisor no menciona. Ese campo sale del perfil del proveedor en la plataforma, no del registro mercantil.
- **RUES, consultado el 2026-10-08.** Cierra lo que el revisor dejó abierto («no sé si son principal y suplente o si hubo relevo»):
  - **DIARIO DEL HUILA DIGITAL S.A.S.**, sigla **DH MEDIA S.A.S.**:
    - NIT 901518850-7, Cámara de Comercio del Huila, matrícula 361081 del **07-09-2021**;
    - renovada el 20-03-2026, **ACTIVA**, CIIU 7310 (publicidad);
    - **representante legal: DUQUE RENGIFO MAXIMILIANO**, con el mismo número de documento que en SECOP I.
  - **EDITORA DEL HUILA S.A.S. EN LIQUIDACION**:
    - NIT 891101933-3, Cámara del Huila, matrícula 15973 del 22-08-1979;
    - último año renovado 2024, `fecha_actualizacion` 2026-01-15;
    - **representante legal: DUQUE CERON LUISA MARIA**, con el mismo documento que en SECOP I.
- **Perfil del 2021-08-14** («Una mujer que levantó una empresa con rollos de papel», sección «Muy personal»). La cita es literal: «al asumir Max Duque Rengifo la gerencia, hubo una reestructuración». El texto contiene también «Rengifo de Duque» y «Editora del Huila Ltda».
- **Parentesco.** Sigue sin fuente. El RUES no lo acredita, y la sospecha no se usa.

**2 · D&R y las daciones en pago.**
- «Daciones en pago enredan a Max Duque Rengifo», La Nación:
  - `datePublished` **2025-02-11**, sección «TEMA DEL DÍA», autor Ricardo Areiza Sandoval;
  - literales: «entre ellos a la sociedad Construcciones e Inversiones D&R, representada por el empresario Max Duque Rengifo»; «la Alcaldía de Neiva aceptó las daciones en pago de cinco predios por un valor global de 3.567 millones de pesos, para saldar obligaciones tributarias por una suma total de 153,31 millones de pesos de la sociedad Duque Rengifo»; y «Max Duque Rengifo, representante legal de la sociedad D&R»;
  - «compraventa simulada» aparece atribuida al alcalde Germán Casagua;
  - **lo que el revisor omitió**: el mismo artículo dice que, «a pesar de una acción de nulidad interpuesta por la administración municipal, las transacciones siguen vigentes. La medida cautelar solicitada no prosperó».
- «Se derrumban canjes de predios por impuestos», La Nación:
  - `datePublished` **2025-07-07**, sección «INVESTIGACIÓN», del mismo autor;
  - **el revisor afirma que «no dice qué pasó con las de D&R». Es falso.** Tiene un apartado titulado «En trámite»: «La otra negociación con la sociedad Construcciones e Inversiones D&R, representada por el empresario Max Duque Rengifo y la Alianza Fiduciaria, sigue en proceso». Añade que en la audiencia de pruebas del **11-06-2025** el Tribunal Administrativo del Huila rechazó una nulidad procesal pedida por Alianza Fiduciaria, y que la administración «dejó vencer en silencio el plazo» que le dio la magistrada Nelcy Vargas.
- **Ambigüedad que el revisor no vio.** La deuda tributaria es «de la sociedad Duque Rengifo», no de «D&R». En el RUES existe **DUQUE RENGIFO S. EN C.**:
  - NIT 891101301, Cámara del Huila, matrícula 10661 de 1976, ACTIVA, renovada el 13-05-2026, CIIU 6810 (inmobiliaria);
  - representante legal: María Mercedes Rengifo de Duque.
  - Puede que La Nación llame así a D&R, o puede que la deudora sea esta comandita. **No consta cuál de las dos es.** La ficha no debe atribuir la deuda a una sociedad concreta.
- **Estado hoy: no comprobado.** Lo último que consta es de julio de 2025, más de 12 meses antes. No hubo buscador para consultar la Rama Judicial ni prensa posterior. El buscador del propio diario devuelve los mismos diez artículos del 07-10-2026 para «daciones en pago», «Gorky» y una cadena sin sentido. Se comprobó aquí, y el revisor también lo dijo: no sirve como prueba de ausencia.
- **La fuente es un competidor directo** (COMUNICACIONES OLAVE S.A.S., ver su resolución del 2026-10-07). Los hechos judiciales que cita (Tribunal, magistrada, fechas de audiencia) son comprobables en un expediente. Las valoraciones («negocio redondo», «enreda») son de La Nación.

**3 · Editoriales.**
- Las seis URL existen, con `articleSection` «Editoriales» y autor de CMS «WebMaster». Las fechas coinciden: 20-02, 15-09, 19-09, 21-09, 28-09 y 06-10-2026.
- Las citas literales están todas en el HTML:
  - «sectores radicales del petrismo» y «alimentada desde el discurso del propio presidente Gustavo Petro»;
  - «la violencia no puede tener fuero» y «El reto será demostrar que el protocolo cierre esa brecha sin abrir otra: la del abuso de autoridad»;
  - «Se hizo justicia con un héroe de la patria» y «esa memoria no sea selectiva»;
  - «una política de seguridad del Gobierno Nacional del presidente Abelardo De La Espriella».
- La categoría tiene `count` 1682 en `/wp-json/wp/v2/categories?slug=editoriales`, como dice el revisor.
- **Precisiones.**
  - El editorial del 20-02 habla de la «vandalización» de la sede del Centro Democrático durante una marcha, no de un «ataque».
  - El 06-10 cita «un incremento del 23 %» y no nombra al gobierno que lo decretó: la atribución es glosa del revisor, aunque sea cierta.
  - El feed de la categoría (`/editoriales/feed/`, no excluido por robots) da los diez últimos editoriales. **Solo dos tratan medidas del gobierno entrante** (28-09 y 06-10). Los demás son de economía, convivencia, salud mental, IA, pensión de las mujeres y la FICCA. Las seis piezas del revisor son una **selección de lo político**, no una muestra de la sección.
- **Aplicación de la regla del polo fijo.**
  - Para hablar de asimetría a través del cambio de gobierno hacen falta piezas de los dos lados. Del gobierno saliente hay **una sola** (20-02-2026), y además es reacción a un hecho de vandalismo contra un partido.
  - Que un editorial reproche al presidente de turno la intolerancia de sus seguidores es fiscalización, y por el polo fijo no cuenta.
  - Lo que sí admite la regla («Qué NO toca esta regla») es el **encuadre** asimétrico: el de Plazas Vega (memoria del M-19 indultado frente a militares procesados) es un indicio de ese tipo.
  - Con 1 pieza antes y 5 después, no hay base para declarar la asimetría medida. Sí hay base para declarar que **la ficha no puede decir «sin evidencia»**: hay nivel 5 y va en el mismo sentido que el +0,20.

**4 · /directorio/.**
- JSON-LD con `datePublished` 2021-05-23 y `dateModified` **2021-05-24**.
- El texto completo es «Editora del Huila SA - Diario del Huila Fundado el 8 de Agosto de 1966 Calle 8 No. 8-06 Neiva-Colombia Teléfono […] Fundadores: Max Duque Gómez - Max Duque Palma Directora María Pia Duque Rengifo». **Cero apariciones** de «antiguo» y de «lectores».
- Las dos autodescripciones de la ficha quedan sin fuente.
- El pie vivo de los editoriales de 2026 repite literalmente el bloque «Fundadores: … Directora María Pia Duque Rengifo».
- El especial del **2026-08-08** dice: «Actualmente, el diario continúa en manos de la familia Duque Rengifo , bajo la dirección de María Pía Duque Rengifo». Es literal, salvo un espacio antes de las comas en el HTML.
- **Error de la propia ficha que el revisor solo apuntó como condicional:** «sería el primero del departamento en el catálogo» es falso hoy. `la-nacion-neiva` está en `mediaRegistry.js` con `departamento: 'Huila'`.

**5 · Las sociedades.**
- **SECOP I no muestra «EDITORA DEL HUILA S.A.S.» desde 2016**, como dice el revisor. La razón social la teclea cada entidad contratante y varía:
  - «EDITORA DEL HUILA LTDA» (2016-06-07 y 2018-04-27);
  - «EDITORA DEL HUILA S.A» (2017-08-11);
  - «S.A.S.» casi siempre desde 2018.
- **El RUES da la vigente: EDITORA DEL HUILA S.A.S. EN LIQUIDACION.** La ficha la llama «Editora del Huila S.A.» y la trata como empresa editora vigente. Las dos cosas son inexactas.
- La política de privacidad (`dateModified` 2024-04-19) dice «Diario del Huila S.A.S» cinco veces. En el RUES no aparece ninguna sociedad con esa razón exacta. Con «DIARIO DEL HUILA» solo salen la Digital y una **PROMOTORA INDUSTRIAL Y COMERCIAL DIARIO DEL HUILA S.A. EN LIQUIDACION**:
  - sigla EDICOHUILA S.A., NIT 900119255;
  - último año renovado 2011;
  - representante legal Blanca Inés Oviedo Forero.
  - Su relación con el medio **no consta**.
- **Lo que sí se sostiene del revisor.** Desde 2022-01 toda la contratación pública registrada va a la Digital. La Editora no tiene contratos en SECOP I después del 2021-06-25, ni en SECOP II después del 2019-10-08. La Digital es hoy el vehículo que factura, y la Editora está en liquidación.

**6 · Corpus.**
- `envios/ciclo-2-2026-10-08/diario-del-huila.md` («Conducta medida»): medición del 2026-10-08, ventana 2026-08-31 → 2026-10-08 (38 días); 585 artículos, 143 en alguna historia, 161 historias, 7 % de agenda propia, 149 compartidas, compañía media 0.146; coincide con Infobae 42, El Colombiano 21 y Caracol Radio 19. **Las cifras del revisor son exactas.**
- El envío del 2026-10-07 daba 592 / 139 / 157 / 6 % / 0.138: el revisor citó el correcto.
- **Precisión:** el umbral de la ficha es de «60 historias suyas», y el revisor lo compara con 143 *artículos*. Son 161 historias. El umbral de historias se supera; el de 90 días, no.

**SECOP recalculado con igualdad exacta por NIT (consultado el 2026-10-08).**

| | Registros | Contratos firmados | Valor contratado |
|---|---|---|---|
| SECOP I · Editora (891101933) | 39 filas | **38**: la constancia 18-13-7949206 (Gobernación, 22-03-2018, $15 000 000) aparece **dos veces con el mismo `uid`** | **$252 993 867** |
| SECOP I · Digital (901518850) | 14 | 14 | $47 428 000 |
| SECOP II · Editora | 8 | 7 (1 borrador de la Policía Metropolitana, $780 000) | $115 544 000 |
| SECOP II · Digital | 6 | 5 (1 borrador de Biorgánicos, $2 127 000) | $37 237 000 |
| **Total** | 67 | **64** | **$453 202 867** desde el 2016-06-07 |

- **Últimos 12 meses (2025-10-08 → 2026-10-08): 7 contratos por $16 110 000, todos de la Digital.** Coincide con el revisor:
  - Cámara de Comercio de Neiva, $5 800 000 (19-03-2026);
  - Biorgánicos del Sur del Huila, $3 870 000 (27-01-2026, SECOP II);
  - Cámara de Comercio del Huila, $3 800 000 (14-11 y 04-12-2025);
  - E.S.E. Hospital Departamental San Antonio de Pitalito, $2 640 000 (14-03, 16-03 y 14-07-2026).
- **Principales contratantes históricos:**
  - Municipio de Neiva, $114 504 000 (5 contratos, 2017-10 → 2019-10);
  - Electrificadora del Huila, $77 000 000 (4; **el último, del 2022-01-25 y ya con la Digital**, no de 2021-02 como dice el revisor);
  - Empresas Públicas de Neiva, $60 000 000 (2020-08);
  - **Gobernación del Huila, $55 500 000** (4 contratos, 2018-2019; **no $70 500 000**: el revisor sumó dos veces la fila duplicada);
  - Cámara de Comercio de Neiva, $46 800 000;
  - E.S.E. Hospital Universitario Hernando Moncaleano Perdomo, $32 260 000;
  - **E.S.E. Carmen Emilia Ospina, $25 000 000** (24-11-2022, SECOP II), que el revisor omite.
- La lectura del revisor se sostiene. La pauta pública registrada es baja y decreciente, y ni el Municipio de Neiva ni la Gobernación contratan con el medio desde 2019. No sostiene la hipótesis de dependencia de la REFUTACIÓN 3.

### Duque Rengifo y D&R: ¿está probada la identidad?

**Sí, por cargo cruzado en un registro público, con una salvedad de enlace.**
- En el RUES, **CONSTRUCIONES E INVERSIONES D&R SOCIEDAD POR ACCIONES SIMPLIFICADA** tiene como representante legal a **MAXIMILIANO DUQUE RENGIFO**:
  - la razón social se escribe así, con una sola «C»;
  - sigla CEIN D&R SAS, NIT 900791618-9;
  - Cámara de Comercio de **Bogotá**, matrícula 2520061 del 18-11-2014, renovada el 06-04-2026, ACTIVA, CIIU 4111 (construcción) y 6810 (inmobiliaria).
- Su número de documento es **idéntico**, por igualdad exacta, a dos registros:
  - el del representante legal de DIARIO DEL HUILA DIGITAL S.A.S. en el mismo RUES;
  - el que SECOP I registra para «MAXIMILIANO DUQUE RENGIFO» en los contratos de la Digital del 2025-02-06 al 2026-07-14.
- **La persona que representa a D&R en el registro mercantil es la misma que representa a la sociedad que hoy factura por el Diario del Huila.**
- **La salvedad.** La Nación no da el NIT de la D&R de su pieza. El enlace entre «Construcciones e Inversiones D&R, representada por Max Duque Rengifo» y el NIT 900791618 descansa en tres cosas:
  - que coinciden la razón social y el representante;
  - que la búsqueda en el RUES de razones sociales con «D&R» y «CONSTRUC» da catorce registros (variantes con espacios como «D & R» no se buscaron), y **solo este** se llama «Construc[c]iones e Inversiones D&R» y la representa un Duque Rengifo;
  - que «Max» es hipocorístico de Maximiliano, el mismo uso que hace el propio diario («Max Duque Rengifo», perfil de 2021).
- **Queda pendiente:** que la sociedad del pleito sea la del NIT 900791618, comprobable en el expediente del Tribunal Administrativo del Huila o en las resoluciones de la Alcaldía, y qué sociedad es la deudora («sociedad Duque Rengifo»).
- **Sin buscador no hubo prensa de terceros.** La prueba adicional es registral, no periodística.
- **Fórmula para la ficha:** «identidad acreditada por registro (RUES: mismo representante legal, con el mismo documento, en D&R y en Diario del Huila Digital); el pleito y la cifra, solo por La Nación, competidor directo, con artículos de 2025».

### Motivo de cada rechazo

- **Obj. 1, la sospecha de parentesco.** Es inferencia por apellidos y el propio revisor lo dice. No hay documento. El protocolo no admite la reputación ni la inferencia, y la sospecha no entra en la ficha. Tampoco hace falta: lo que importa para el nivel 1 es el cargo, y ese está acreditado.
- **Obj. 2, «a favor de la administración anterior».** Que el exalcalde Muñoz aceptara las daciones no hace al representante legal partidario de esa administración. Lo acreditado es un **interés patrimonial en litigio frente al Municipio de Neiva**, que es la institución, sea quien sea el alcalde. Darle color político sería medir contra quién le tocó gobernar, que es lo que el polo fijo prohíbe. También se rechaza que «la ficha no puede firmarse sin él» se convierta en efecto sobre el número: el propio revisor admite que no mueve el eje, y el protocolo lo trata como desvelamiento.
- **Obj. 3, «el número dejaría de ser por coherencia de banda para apoyarse en conducta editorial».** Con 1 editorial antes del 07-08-2026 y 5 después, elegidos entre los políticos, no hay barrido simétrico. El +0,20 pasa a apoyarse en la banda **más** un nivel 5 coherente y declarado pequeño. Es la misma fórmula que ya usa `el-diario-pereira` («la banda regional, con editoriales de 2026 (nivel 5) en el mismo sentido»). No se apoya en asimetría medida.

### Fuentes deformadas o falsas

**Ninguna fuente inexistente.** Las doce URL resuelven, las fechas coinciden y las citas literales están en el HTML. Las deformaciones:
- **«No dice qué pasó con las de D&R» (La Nación, 2025-07-07): falso.** El artículo tiene un apartado «En trámite» que dice que el caso de D&R «sigue en proceso», con una audiencia del 11-06-2025 y una nulidad procesal rechazada. El revisor omitió además que la pieza del 2025-02-11 dice que la medida cautelar «no prosperó» y que las transacciones «siguen vigentes».
- **«No hay acceso a RUES ni a certificados desde aquí»: falso en la primera mitad.** El RUES abierto (`c82u-588k`) estaba disponible. Daba el representante legal de las dos sociedades, la liquidación de la Editora y el cargo cruzado en D&R. Es la omisión que más pesa: el revisor dejó como «probable, no comprobado» algo que un registro público ya resolvía.
- **SECOP, total histórico «$471.109.867 en 67 contratos»: deformado.** Suma dos veces una fila duplicada ($15 000 000, misma constancia y mismo `uid`) y dos borradores ($2 907 000). Lo firmado son **64 contratos por $453 202 867**. Lo avisa de los borradores, pero los incluye en el total.
- **«Gobernación del Huila $70.500.000»: deformado** por el mismo duplicado. Son $55 500 000.
- **«Electrificadora del Huila … (último 2021-02)»: inexacto.** El último es del 2022-01-25, ya con la Digital.
- **«Editora del Huila S.A.S. … desde 2016» en SECOP: inexacto.** En 2016-2018 aparecen «LTDA» y «S.A».
- **Omisiones menores.** No cita la E.S.E. Carmen Emilia Ospina ($25 000 000, 2022). Tampoco dice que SECOP II da otro representante legal para la Editora.
- **«Ataque a la sede del Centro Democrático»:** el editorial dice «vandalización».
- **Obj. 6:** compara el umbral de 60 *historias* con 143 *artículos*. Precisión menor; las cifras son exactas.
- Lo que el revisor dijo de los buscadores del sitio (resultados en caché) **es cierto**: se comprobó aquí.

---

**Propuesta para la firma**

**(a) Valor: mantener +0,20, provisional, y no firmar todavía.**
- Lo que cambia es la razón. Ya no es «por coherencia de banda, sin evidencia», sino:
  - la banda regional;
  - un nivel 5 pequeño y en el mismo sentido (editoriales de 2026 que respaldan con salvedades al gobierno entrante y encuadran el caso Plazas Vega como memoria selectiva);
  - 38 días de corpus, sin uso de la compañía media porque está saturada.
- Nada de lo encontrado empuja hacia la mixta ni más a la derecha con fuerza suficiente para mover la banda.
- No se firma hasta:
  - aplicar las correcciones de (b), porque hoy la ficha da como editora vigente una sociedad en liquidación;
  - declarar la tensión del pleito de D&R.

**(b) Correcciones, con su fuente**

En `fichas/diario-del-huila.md`:
1. **Empresa editora:** «Editora del Huila S.A.» (fuente /directorio/) → **«Diario del Huila Digital S.A.S. (sigla DH MEDIA S.A.S.), NIT 901518850-7, Cámara de Comercio del Huila, matrícula 361081 del 07-09-2021, ACTIVA, renovada el 20-03-2026; representante legal: Maximiliano Duque Rengifo (RUES, datos.gov.co `c82u-588k`, consultado el 2026-10-08). La sociedad histórica, Editora del Huila S.A.S. (NIT 891101933-3, matrícula 15973 de 1979), figura EN LIQUIDACIÓN, con Luisa María Duque Cerón como representante legal; el pie del sitio sigue diciendo "Editora del Huila SA"»**. Sustituye a «RUES / DataCrédito Empresas» como fuente de la segunda sociedad.
2. **«La segunda sociedad de 2021 está sin explicar»** → **«Desde 2022 toda la contratación pública registrada va a Diario del Huila Digital S.A.S., y la Editora está en liquidación: la Digital es hoy el vehículo operativo. Sus socios siguen sin documentar»**. En CONTRA, el párrafo deja de decir «puede ser una reorganización rutinaria» sin dato: el dato es la liquidación.
3. **Directora:** la fuente pasa a ser el pie vivo de los artículos (2026-10) y el especial «DIARIO DEL HUILA, 60 AÑOS DE HISTORIA» (2026-08-08: «el diario continúa en manos de la familia Duque Rengifo, bajo la dirección de María Pía Duque Rengifo»). /directorio/ se conserva con la nota «página de 2021 (`dateModified` 2021-05-24)».
4. **Nivel 4:** quitar «el medio más antiguo del Huila y del sur de Colombia» y «el de mayor número de lectores del departamento». No constan en /directorio/, y la ficha no da otra fuente. Si se encuentra una, se reponen con ella.
5. **Cabecera:** quitar «sería el primero del departamento en el catálogo», porque `la-nacion-neiva` (Huila) ya está.
6. **Nivel 2:** «NO EXISTE / Cero artículos» → **«Medición del 2026-10-08, ventana 2026-08-31 → 2026-10-08 (38 días): 585 artículos, 143 en alguna historia, 161 historias, 7 % de agenda propia; coincide sobre todo con Infobae (42), El Colombiano (21) y Caracol Radio (19). La compañía media (0,146) está saturada y no se usa para sostener el valor. Por debajo de los 90 días del protocolo»**.
7. **Nivel 5 (nuevo):** los seis editoriales con fecha y URL, la lectura del punto 3 y la advertencia de muestra («1 pieza antes del 07-08-2026, 5 después, seleccionadas entre las políticas; de los diez últimos editoriales, solo dos tratan medidas del gobierno entrante»). En ARGUMENTO, «no por evidencia que sitúe a este medio en el eje» → «la banda regional, con un nivel 5 pequeño en el mismo sentido».
8. **Nivel 1, quien administra:** añadir que en SECOP I firma por la Digital Luisa María Duque Cerón hasta el 2025-03-19, y Maximiliano Duque Rengifo desde el 2025-02-06 y en todos los contratos del 2025-09-08 al 2026-07-14. Según el propio diario (2021-08-14), Max Duque Rengifo asumió la gerencia tras la muerte de Max Duque Palma. **Representación legal no es accionariado.**
9. **REFUTACIÓN 1:** «certificado de existencia y representación de Editora del Huila S.A. en la Cámara de Comercio de Neiva» → **«certificados de la Cámara de Comercio del Huila de Diario del Huila Digital S.A.S. (matrícula 361081) y de Editora del Huila S.A.S. en liquidación (matrícula 15973)»**.
10. **REFUTACIÓN 3:** añadir que SECOP no sostiene la hipótesis de dependencia (ver la línea de abajo).

En `shared/mediaOwnership.js`, entrada `diario-del-huila`:

11. `holdings`: reescribir con los puntos 1 y 8.
12. `notes`, la **línea de CONTRATACIÓN PÚBLICA en el formato del protocolo**:

> Contratación pública (SECOP I y II, NIT 901518850-7 —Diario del Huila Digital S.A.S.— y NIT 891101933-3 —Editora del Huila S.A.S., en liquidación—, consultado 2026-10-08): 7 contratos por $16,1 millones **contratados** en los últimos 12 meses, todos de Diario del Huila Digital; 64 por $453,2 millones en total desde 2016. Principales contratantes: Municipio de Neiva ($114,5 millones, 2017-2019), Electrificadora del Huila ($77,0 millones, el último en 2022), Empresas Públicas de Neiva ($60,0 millones, 2020), Gobernación del Huila ($55,5 millones, 2018-2019) y Cámara de Comercio de Neiva ($46,8 millones). El Municipio de Neiva y la Gobernación del Huila son gobiernos que el medio cubre, y ninguno le contrata desde 2019. En los últimos 12 meses contrataron la Cámara de Comercio de Neiva ($5,8 millones), Biorgánicos del Sur del Huila ($3,9 millones), la Cámara de Comercio del Huila ($3,8 millones) y la E.S.E. Hospital Departamental San Antonio de Pitalito ($2,6 millones). Se excluyen dos borradores ($2,9 millones) y una fila duplicada de SECOP I. No consta qué parte de los ingresos representa.

13. `notes`, el **conflicto del administrador**, como desvelamiento:

> «INTERÉS PATRIMONIAL DEL REPRESENTANTE LEGAL EN LITIGIO CON EL MUNICIPIO DE NEIVA. Maximiliano Duque Rengifo, representante legal de Diario del Huila Digital S.A.S., es también representante legal de Construciones e Inversiones D&R S.A.S. (NIT 900791618, Cámara de Comercio de Bogotá); consta en el RUES, con el mismo documento en las dos sociedades. Según La Nación de Neiva —competidor directo del Diario del Huila—, la Alcaldía de Neiva del exalcalde Gorky Muñoz aceptó daciones en pago de cinco predios por 3.567 millones de pesos, de D&R y Alianza Fiduciaria, para saldar 153,31 millones en impuestos. La administración de Germán Casagua las demandó, y en julio de 2025 el caso seguía en el Tribunal Administrativo del Huila (La Nación, 11-02-2025 y 07-07-2025). No consta su estado actual ni cómo lo ha cubierto el Diario del Huila. Representación legal no es propiedad. Se declara para que el lector lo sepa; no es una acusación y no mueve la clasificación.»

14. `sources`: añadir las dos consultas de datos.gov.co (RUES y SECOP), el especial del 2026-08-08, el perfil del 2021-08-14 y las dos piezas de La Nación. Quitar DataCrédito, que queda sustituido por el RUES. Fijar `verifiedAt` cuando firme el responsable editorial.

En `shared/mediaRegistry.js`:

15. `biasRationale`: «Valor provisional por coherencia con la banda regional; el accionariado sigue sin documentar» → **«Valor provisional: la banda regional, con editoriales de 2026 (nivel 5) en el mismo sentido y 38 días de corpus. Lo edita Diario del Huila Digital S.A.S.; la Editora histórica está en liquidación y los socios siguen sin documentar — ver fichas/diario-del-huila.md.»**

En `shared/centinela.js`, entrada `diario-del-huila`:

16. Ampliar el `vigila` de «Duque Rengifo». Además de la continuidad de la directora, debe vigilar:
    - el cambio de representante legal de la Digital;
    - cualquier noticia del pleito de las daciones en pago, por si el propio diario lo cubre.
    - Advertencia: el buscador del sitio hoy devuelve resultados en caché y la consulta puede dar falsos negativos. Conviene declararlo como «no comprobable» mientras no se arregle.

**(c) Tensiones a declarar en la ficha**
1. **El representante legal del vehículo que factura tiene un interés patrimonial en litigio con el Municipio de Neiva, que el diario cubre.** La identidad es registral. El pleito, su cuantía y su estado (vivo en julio de 2025, y hoy no comprobado) salen solo de un competidor directo, con piezas de más de 12 meses. No mueve el eje. Pide mirar, cuando haya corpus de 90 días, cómo cubre el diario a la Alcaldía de Neiva y el caso de las daciones.
2. **Los editoriales de 2026 respaldan con salvedades al gobierno entrante, y la única pieza leída del saliente le atribuye responsabilidad política.** Es asimetría posible, no medida: 1 pieza contra 5, todas seleccionadas. Queda pendiente un barrido simétrico de la sección (junio-julio frente a agosto-octubre de 2026). El sitio prohíbe paginar con `/*/page/*`, así que habrá que hacerlo con el feed de la categoría y la API por id.
3. **El capital sigue sin documentar.** Se sabe quién dirige (María Pía Duque Rengifo) y quién representa a las sociedades (Maximiliano Duque Rengifo en la Digital; Luisa María Duque Cerón en la Editora, en liquidación), pero no de quién son. «Medio de familia» descansa en la declaración del propio medio (2026-08-08) y en los apellidos. Sigue siendo la laguna principal.
4. **Sociedades sin explicar en el RUES.** Hay una «Promotora Industrial y Comercial Diario del Huila S.A.» en liquidación (NIT 900119255, sin renovar desde 2011), con otra representante legal (Blanca Inés Oviedo Forero), y una «Duque Rengifo S. en C.» (inmobiliaria, activa) que podría ser la deudora del pleito. No se afirma ningún vínculo; se anotan para pedirlos con los certificados.

**Lagunas declaradas (sin buscador):** prensa de terceros sobre D&R y las daciones; el estado judicial actual del caso; la cobertura del caso en el propio Diario del Huila; los certificados de Cámara con socios; el parentesco entre los Duque.
