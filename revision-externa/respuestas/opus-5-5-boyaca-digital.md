# Respuesta — Claude Opus 5.5 sobre Boyacá Digital

| | |
|---|---|
| **Modelo** | Claude Opus 5.5 |
| **Versión exacta** | `claude-opus-5-5` |
| **Fecha de la consulta** | 2026-10-07 |
| **Quién la hizo** | Claude Code, a petición del responsable editorial (ciclo 2, fase 2, tanda 1; revisor de la misma casa que el autor de las fichas, ver DECISIONES.md 2026-10-07) |
| **¿Tuvo acceso a la red?** | sí |

> **Se pega LITERAL lo que devolvió el modelo, sin editar ni resumir.** Si se
> recorta, se pierde justo lo que pueda incomodar. Los comentarios nuestros van
> al final, en la sección de resolución, claramente separados.
>
> **Edición:** retirados enlaces que pueden mostrar documentos de identidad, y un número de móvil (PROTOCOLO, Datos personales; decisión del responsable editorial, 2026-10-10).

---

## RESPUESTA LITERAL

```
DECLARACIÓN PREVIA. La ficha la escribió otro modelo de Claude y yo también lo
soy (Claude Opus 5.5). Para compensar ese sesgo de casa he buscado sobre todo en
fuentes que la ficha NO usa: SECOP (datos.gov.co), la captura de archive.org de
la página caída, la página /equipo del medio, el JSON-LD (schema.org) de ambos
sitios y Wikidata. Todas las citas literales se sacaron del HTML crudo bajado con
curl -sL -A "Mozilla/5.0" el 2026-10-07, salvo donde se marca otra cosa.

Cómo busqué (para que sea auditable):
- boyacadigital.com: portada, /equipo, /sobre-nosotros, /politica-editorial,
  /politica-de-privacidad, /terminos, /opinion, /escenario-politico, /columnista/,
  /rss.xml, tres piezas de /opinion y la búsqueda interna /buscar?q= con
  «Holding», «Rosas», «Nobsa», «riesgo psicosocial» (la búsqueda interna NO es
  fiable: devuelve listados genéricos; no la uso como prueba de ausencia).
- holdingconsultants.org: /nuestra-organizacion/ (404 hoy), /nosotros/,
  /cobertura/, /servicios/proyectos-de-empleabilidad-e-inclusion-social/.
- web.archive.org: índice CDX y captura de /nuestra-organizacion/. DESDE ESTA
  RED SÍ SE PUDO LLEGAR (la API /wayback/available respondió 429, pero
  web.archive.org/web/... y /cdx/ respondieron 200).
- SECOP: API Socrata de datos.gov.co, conjuntos jbjy-vk9h (SECOP II contratos)
  y rpmr-utcd (SECOP integrado I+II), filtrando documento_proveedor por el NIT
  900143612. No abrí cada proceso en community.secop.gov.co (responde 302 a
  curl); los datos son los del registro abierto, no los del expediente.
- Wikidata: Special:EntityData/Q140398679.json (enlazado desde el propio medio).
- DNS: nslookup -type=NS de boyacadigital.com, holdingconsultants.org,
  holdingsoft.org.
- Búsqueda web («Holding Consultants» «Boyacá Digital» Rosas): sin resultados
  útiles.
- NO consulté RUES ni Cámara de Comercio (no hay certificado de acceso libre por
  API); no hay extracto mercantil en esta respuesta.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré venta ni fusión. Lo que encontré es que el medio es NUEVO: Wikidata
  (Q140398679, enlazado en el sameAs del JSON-LD del propio medio) le asigna
  fecha de creación (P571) «+2025-10-07», con precisión de AÑO (precision 9), es
  decir «2025». Última modificación del ítem: 2026-07-02. Wikidata es editable
  por cualquiera: es un indicio, no un registro. Si es cierto, TODA la vida del
  medio cae dentro de la ventana de doce meses y no hay «línea de la casa»
  previa contra la que medir.
  Fuente: https://www.wikidata.org/wiki/Special:EntityData/Q140398679.json
  (consultado 2026-10-07).

- La persona que la ficha nombra como titular o director, ¿sigue viva y en el
  cargo? La ficha no nombra titular ni director: dice que no hay «una persona con
  nombre que responda». Eso es falso hoy (ver objeción 1). Las dos personas con
  nombre que constan, Carlos O. Rosas Acevedo y Juan Pablo Sáenz, aparecen en
  páginas vivas el 2026-10-07; no encontré noticia de fallecimiento de ninguno
  (búsqueda no exhaustiva: solo las páginas citadas).

- ¿Quién dirige hoy la redacción? El cargo «Editor en Jefe» sigue sin nombre
  publicado. Su contacto, en el HTML crudo, es una dirección protegida por
  Cloudflare (data-cfemail) que decodificada es «[correo omitido]», la
  misma en /sobre-nosotros y /politica-editorial. Y la página /equipo dice,
  literal: «Carlos O. Rosas A. es gerente de Boyacá Digital y columnista de
  opinión.» SOSPECHA, no probada: que el Editor en Jefe sea el gerente, Carlos O.
  Rosas Acevedo. El medio no lo dice expresamente.

- ¿Hay un registro más reciente que la fuente que la ficha cita? Sí, y la ficha
  lo tenía delante: el NIT y la razón social están publicados por la propia
  consultora (objeción 1). Más reciente aún: SECOP II registra contratos públicos
  con ese NIT hasta el 2026-09-15 (objeción 3). No hay extracto de Cámara de
  Comercio en esta respuesta.

## OBJECIONES

1. QUÉ AFIRMA LA FICHA: «Sigue sin haber razón social, NIT ni una persona con
   nombre que responda» y la tabla «Razón social / NIT: no constan»; «Único
   humano con nombre: Juan Pablo Sáenz».
   POR QUÉ ES INCORRECTO:
   (a) La página /nosotros/ de Holding Consultants —que la ficha CITA— dice en su
   pie: «2006–2026 © Holding Consultants® · NIT 900.143.612-6 · Bogotá,
   Colombia.» Y su JSON-LD: "legalName":"Holding Consultants S.A.S.",
   "taxID":"900143612-6". La misma página dice: «Carlos O. Rosas Acevedo / CEO y
   Fundador».
   (b) La página /equipo de Boyacá Digital, bajo «Columnistas invitados /
   Personas reales», dice: «Carlos O. Rosas A. es gerente de Boyacá Digital y
   columnista de opinión.»
   Es decir: la misma persona es CEO y fundador de la consultora y gerente del
   medio. Esto no es ya «evidencia convergente» de nombre y DNS: es una persona
   natural identificada a ambos lados. La ficha omitió el único dato que el
   protocolo pide primero (a qué persona natural llega la propiedad), y lo
   omitió estando en una página que ella misma cita.
   Matiz: «CEO y fundador» no prueba que sea accionista mayoritario; para eso
   falta el certificado de existencia y representación.
   FUENTES Y FECHA: https://www.holdingconsultants.org/nosotros/ y
   https://www.boyacadigital.com/equipo — ambas leídas en HTML crudo 2026-10-07.
   NIVEL: propiedad (declaración de ambas partes, no registro mercantil).

2. QUÉ AFIRMA LA FICHA: que la forma jurídica es, implícitamente, una sociedad
   («Holding Consultants de Colombia», «la empresa dueña»), y que el vínculo se
   prueba por «el mismo par de Cloudflare […] y Cloudflare asigna un par por
   cuenta».
   POR QUÉ ES DÉBIL O INCOMPLETO:
   (a) Forma jurídica en tensión. El sitio dice "Holding Consultants S.A.S.";
   SECOP registra el mismo NIT 900143612 a nombre de «FUNDACION HOLDING
   CONSULTANTS DE COLOMBIA» (3 registros, p. ej. contrato 16-15-5596405 con la
   Alcaldía de Nobsa, 2016), «HOLDING CONSULTANTS DE COLOMBIA» (6) y «Holding
   Consultants» (77); y la propia página de empleabilidad dice que actúa como
   «Agencia Privada No Lucrativa de Gestión y Colocación de Empleo, autorizada
   […] mediante la Resolución 0472 del 19 de diciembre de 2025». Una fundación
   (ESAL) y una S.A.S. no son lo mismo: cambia quién «posee» y cómo se lee la
   propiedad del medio. SOSPECHA, no probada: que la persona jurídica sea una
   entidad sin ánimo de lucro, o que haya cambiado de forma. Solo el certificado
   de Cámara de Comercio lo resuelve.
   (b) El argumento de los servidores de nombres es más débil de lo que la ficha
   dice. Lo comprobé: boyacadigital.com, holdingconsultants.org y también
   holdingsoft.org usan dylan/fatima.ns.cloudflare.com. Pero que Cloudflare
   asigne el par «por cuenta» no implica que el par sea exclusivo de una cuenta:
   no encuentro fuente que diga que un par no se reutiliza entre cuentas
   distintas, y la ficha tampoco la cita. Es indicio, no huella.
   (c) Hay indicios mucho más fuertes que la ficha no usa: el JSON-LD
   NewsMediaOrganization del medio declara "telephone":"[teléfono omitido]", el MISMO
   número que el JSON-LD de Holding Consultants ("[teléfono omitido]"); y el medio
   sirve anuncios de Holding Consultants y HoldingSoft+ marcados en el propio
   código como publicidad de la casa: utm_medium=house (p. ej.
   href="https://www.holdingconsultants.org?utm_source=boyacadigital&amp;utm_medium=house&amp;utm_campaign=v-hc-paper&amp;utm_content=billboard"),
   en portada, /equipo, /opinion, /escenario-politico y las páginas legales. Y
   /terminos dice: «Los textos producidos por la redacción de Boyacá Digital, la
   marca, el logotipo y el diseño del sitio son propiedad de Holding Consultants
   o se usan con licencia.»
   FUENTES Y FECHA: https://www.boyacadigital.com/ (JSON-LD y enlaces),
   https://www.boyacadigital.com/terminos,
   https://www.holdingconsultants.org/servicios/proyectos-de-empleabilidad-e-inclusion-social/,
   SECOP integrado [enlace retirado: puede mostrar documentos de identidad; ver la resolución] filtrado por
   documento_proveedor=900143612 — todo 2026-10-07.
   NIVEL: propiedad / registro externo.

3. QUÉ AFIRMA LA FICHA: el conflicto de interés se formula como «una consultora
   que vende servicios […] a entidades públicas es […] la dueña de un medio cuya
   redacción automatizada cubre a diario las alcaldías y la gobernación de
   Boyacá». Y la ficha da por perdida la prueba de los clientes públicos.
   POR QUÉ: la prueba existe y es más fuerte que la página caída, pero apunta a
   OTRAS entidades que las que la ficha señala.
   (a) Los clientes públicos están documentados en SECOP. En SECOP II (jbjy-vk9h)
   hay 58 registros con el NIT 900143612; en el integrado (rpmr-utcd) 87
   registros, 67 tras quitar duplicados, por unos COP 2.207 millones en total
   entre 2007 y 2026 (incluye algunos contratantes no estatales, como Colsanitas
   y la Cámara de Comercio de Bogotá).
   (b) En los últimos 12 meses (desde 2025-10-07), SECOP II registra 12
   contratos, por unos COP 70,4 millones en total. Entre ellos: Consejo Nacional
   Electoral (CPS-CNE-025-2025, 2025-10-17, $9.789.456), Ministerio de Transporte
   (722-2025, 2025-11-25), Fondo de Previsión Social del Congreso (MC-014-2025,
   2025-11-21), Fondo Rotatorio de la Policía Nacional (CTO 075-2-26,
   2026-07-30, $13.840.000), Departamento de Policía Vichada (44-7-20006-26,
   2026-08-25), CARDER (2026-08-28) y Politécnico Colombiano Jaime Isaza Cadavid
   (55285-2026, 2026-09-15, $15.856.742). Tres de ellos son POSTERIORES al
   cambio de gobierno de agosto de 2026. Antes de esa ventana: Secretaría
   General de la Alcaldía Mayor de Bogotá (4232000-708-2025, 2025-06-12,
   $78.410.640), ICBF (2018, 2019, 2023, 2024), Aerocivil (2023), Supersalud
   (2023), Ejército y MinAmbiente (2021).
   (c) Contra la ficha: en Boyacá solo encontré UN contrato, y es viejo:
   Alcaldía de Nobsa, concurso de méritos CM002/2016, contrato 16-15-5596405,
   firmado 2016-11-15, COP 100.000.000, estado «Liquidado», contratista
   «FUNDACION HOLDING CONSULTANTS DE COLOMBIA». Ningún contrato vigente o
   reciente con la Gobernación de Boyacá ni con alcaldías boyacenses aparece en
   SECOP II ni en el integrado. La frase de la ficha sobre «las alcaldías y la
   gobernación de Boyacá» queda SIN respaldo documental hoy: el conflicto
   documentado es con entidades NACIONALES (CNE, Policía, MinTransporte, Fondo
   del Congreso) y con otras regiones, que el medio también cubre en su sección
   Colombia (p. ej. tenía en portada «Congreso elegirá el 25 de agosto a los
   nuevos magistrados del CNE» y piezas sobre la Policía).
   Matiz: el registro abierto de SECOP no recoge contratos fuera de SECOP ni
   subcontratos; «no aparece» no es «no existe».
   FUENTES Y FECHA: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] y
   [enlace retirado: puede mostrar documentos de identidad; ver la resolución] con
   $where=documento_proveedor like '%900143612%', consultados 2026-10-07;
   contrato Nobsa: [enlace retirado: puede mostrar documentos de identidad; ver la resolución]
   (enlace tomado del registro; no lo abrí).
   NIVEL: registro externo.

4. QUÉ AFIRMA LA FICHA: «Nivel 2 — Conducta medida: NO EXISTE. No está
   ingerido.»
   POR QUÉ: el propio envío trae la medición del 2026-10-07: 1178 artículos, 328
   en alguna historia, 338 historias, agenda propia 20 %. La ficha está
   desactualizada respecto del expediente al que se adjunta. No cambia el número
   por sí sola (37 días, compañía media saturada, y la ficha hace bien en no
   usarla), pero el texto «no existe» es hoy falso.
   FUENTE Y FECHA: tabla «Conducta medida de Boyacá Digital» del envío,
   medición 2026-10-07.
   NIVEL: conducta observable.

5. QUÉ AFIRMA LA FICHA: valor 0,00, «Orientación mixta».
   POR QUÉ: no hay en la ficha ni una sola pieza de evidencia sobre ORIENTACIÓN.
   Lo que hay es: nivel 4 (cómo dice que trabaja) y nivel 1 (quién lo opera, y el
   dueño no determina la orientación). El protocolo dice que una clasificación no
   puede apoyarse solo en los niveles 4 y 5. El 0,00 no es una conclusión de la
   evidencia: es un valor por defecto. Puede ser el valor correcto por la regla
   de «ante la duda, la banda más cercana a la mixta», pero entonces la ficha
   debe decir que es un valor por ausencia de evidencia, no una orientación
   observada. Sin evidencia nueva no traigo un número alternativo.
   FUENTE: la propia ficha y la jerarquía del CONTEXTO.
   NIVEL: —

6. QUÉ AFIRMA LA FICHA: Juan Pablo Sáenz es «columnista de "Escenario
   Político", periodista y estratega en comunicación política».
   POR QUÉ ES INCOMPLETO: /equipo lo describe, literal: «Periodista · Ex
   Funcionario UTL · Estratega en comunicación política · Cofundador de WHITE ·
   Columnista de Boyacá Digital.» La ficha omite «Ex Funcionario UTL» (Unidad de
   Trabajo Legislativo, es decir, trabajó en la oficina de un congresista; el
   medio no dice de cuál y no lo encontré). Para una sección de análisis
   político, que su único firmante humano haya trabajado para un congresista es
   dato relevante. Además: la sección /escenario-politico se presenta como
   «Columnas de opinión y análisis político de columnistas invitados», pero las
   dos piezas que lista hoy van firmadas «Redacción Boyacá Digital · 5 de agosto
   de 2026 · IA», no por Sáenz.
   FUENTES Y FECHA: https://www.boyacadigital.com/equipo y
   https://www.boyacadigital.com/escenario-politico — 2026-10-07.
   NIVEL: declaración del propio medio.

7. QUÉ AFIRMA LA FICHA (sobre la fuente caída): que holdingconsultants.org/
   nuestra-organizacion/ afirmaba «veinte años de actividad […] y clientes en el
   sector privado y en el público», y que la captura de archive.org no se pudo
   consultar.
   POR QUÉ: la captura SÍ es accesible. El índice CDX tiene capturas 200 de esa
   URL entre 2021-08-04 y 2023-03-24 (la última). La de 2023-03-24 dice,
   literal: «En el transcurso de nuestra permanencia en el mercado de quince (15)
   años sostenemos relaciones comerciales con numerosas empresas tanto del sector
   Privado como Público en varias ciudades del País.» La frase sobre el sector
   público QUEDA CONFIRMADA. Pero dice «quince (15) años», no veinte; si la ficha
   leyó una versión posterior que dijera «veinte», esa versión no está en
   archive.org. Los «20 años» sí constan hoy en el JSON-LD del sitio nuevo
   ("20 años de experiencia en Colombia"), de modo que la cifra es defendible,
   pero no por la fuente que la ficha cita. Detalle menor: el sitio actual da la
   fundación como «26 de marzo de 2007» en /nosotros/ y "foundingDate":"2006" en
   su JSON-LD y «2006–2026» en el pie; la ficha toma 2007 sin señalar la
   inconsistencia.
   FUENTES Y FECHA:
   https://web.archive.org/web/20230324172804/https://www.holdingconsultants.org/nuestra-organizacion/
   (captura del 2023-03-24, leída 2026-10-07);
   https://web.archive.org/cdx/search/cdx?url=holdingconsultants.org/nuestra-organizacion/
   NIVEL: declaración de la empresa dueña (archivada). Ojo: por la regla del
   presente, la captura de 2023 solo confirma la frase; la evidencia VIGENTE de
   clientes públicos es SECOP (objeción 3).

## LO QUE NO PUDE VERIFICAR

- Composición accionaria de Holding Consultants y si Carlos O. Rosas Acevedo es
  accionista mayoritario: no consulté RUES ni certificados de Cámara de Comercio
  (no hay acceso abierto por API). Busqué en el sitio de la consultora y en
  SECOP; SECOP no publica accionistas.
- Forma jurídica real (S.A.S. vs. fundación): ver objeción 2. Sin certificado,
  queda en tensión.
- Que el Editor en Jefe sea Rosas: sospecha por el correo gerente@, no probada.
- Para qué congresista trabajó Juan Pablo Sáenz (UTL): no lo encontré; no
  busqué más allá de /equipo.
- Qué proporción de imágenes es generada: no lo medí.
- Si el medio ha publicado piezas sobre las entidades contratantes de su dueño
  con encuadre favorable: la búsqueda interna del sitio no es fiable y no hice
  un barrido pieza a pieza. No tengo evidencia ni a favor ni en contra.
- No abrí los expedientes en community.secop.gov.co (redirección 302 a curl):
  los datos son los del conjunto abierto de datos.gov.co.

## LO QUE FALTA

- NIT 900.143.612-6, razón social y persona natural (Carlos O. Rosas Acevedo,
  CEO y fundador de la consultora, gerente del medio). Está en fuentes públicas
  y la ficha lo declara inexistente.
- La lista de contratos públicos de la dueña (SECOP), con fechas, y la
  corrección del foco: entidades nacionales, no la Gobernación ni alcaldías de
  Boyacá (salvo Nobsa, 2016, liquidado).
- El teléfono compartido y la publicidad de la casa (utm_medium=house) como
  indicios del vínculo, más fuertes que los servidores de nombres.
- La cláusula de /terminos sobre la propiedad de los textos y la marca.
- La sede declarada del medio: el JSON-LD dice "streetAddress":"Carrera 11
  #12-64","addressLocality":"Sogamoso"; la consultora está en Bogotá (Carrera 47
  No. 127D-03).
- La edad del medio (Wikidata: creado en 2025).
- Una constatación que refuerza el reparo 2 de la ficha (pluralidad) con datos
  y no solo como hipótesis: la sección /opinion está hecha, en las piezas que vi,
  de reescrituras de columnas de otros medios (La Silla Vacía, Boyacá 7 Días,
  La República), firmadas «Redacción Boyacá Digital · IA». Ej.: «El columnista
  Juan Pablo Ossa publicó en La Silla Vacía un análisis…»; «Una columna de
  opinión publicada el 4 de octubre de 2026 en Boyacá 7 Días advierte…». Un
  conteo de pluralidad que sume estas piezas cuenta dos veces la misma voz.

## EVIDENCIA QUE NO MUEVE EL NÚMERO

- Después del cambio de gobierno (agosto de 2026), la sección de opinión del
  medio difunde, sin tomar postura propia visible, tanto material crítico con el
  gobierno De la Espriella —«Análisis: dos meses de gobierno de Abelardo de la
  Espriella y sus contradicciones con la Constitución de 1991» (2026-09-27,
  resumen de una columna de La Silla Vacía); «Colombia se alinea con EE. UU. en
  la ONU y rompe con Irán: ¿un giro que le costará su capital diplomático?»
  (2026-09-25)— como material crítico con figuras del gobierno anterior
  —«Subdirector de RCN Radio pide a Sandra Ortiz confesar y pedir perdón por
  caso Ungrd» (2026-09-26)—. Son reescrituras de opiniones ajenas; por la regla
  del polo fijo no son evidencia de orientación, y no encontré endoso editorial
  propio. Lo registro porque es la conducta de la casa en la ventana que importa.
  Fuente: https://www.boyacadigital.com/opinion (2026-10-07).
- El medio cubre Nobsa con frecuencia (varias piezas sobre la alcaldía y el
  Invías), y Nobsa fue cliente de la dueña en 2016. Contrato liquidado hace años:
  por la regla del presente no es conflicto vigente. Fuente: búsqueda interna
  del sitio, no fiable como recuento.
- La autodeclaración de IA es real y visible en cada página (franja «Redacción
  con IA · Contenido elaborado por agentes de inteligencia artificial bajo
  supervisión editorial»), y /equipo separa «Personas reales» de «No son
  personas reales». Lo que la ficha dice al respecto se sostiene.
- El RSS (20 ítems, el más reciente Wed, 07 Oct 2026 22:32:17 GMT) sigue sin
  etiqueta de autor (0 ocurrencias de <author> o dc:creator). Confirma la ficha.
- Los tres dominios (medio, consultora, HoldingSoft) comparten servidores de
  nombres Cloudflare dylan/fatima (nslookup, 2026-10-07). Confirma el dato, no
  su peso (objeción 2b).
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-07. Pendiente de la firma del responsable editorial.**

**Cómo se verificó.** Se partió de la versión de `origin/main` de la ficha y de
`shared/mediaOwnership.js`, la posterior a la PR #67. Todas las páginas que cita
el revisor se descargaron en crudo (`curl -sL -A "Mozilla/5.0"`) el 2026-10-07 y
los pasajes se buscaron en el HTML, no en un resumen. Respondieron con HTTP 200
las 9 páginas de boyacadigital.com (portada, /equipo, /sobre-nosotros,
/politica-editorial, /politica-de-privacidad, /terminos, /opinion,
/escenario-politico, /rss.xml) y 3 de las 4 de holdingconsultants.org.
/nuestra-organizacion/ sigue en 404.

Lo demás se comprobó así:
- **SECOP**, en la API Socrata de datos.gov.co: el conjunto `jbjy-vk9h` (SECOP II)
  filtrando por `documento_proveedor like '%900143612%'`, y el `rpmr-utcd`
  (integrado) filtrando por `= '900143612'` y por `like`.
- **archive.org**: el índice CDX (la primera llamada dio 503 y la segunda, 200) y
  la captura del 2023-03-24 (HTTP 200).
- **Wikidata**: `Special:EntityData/Q140398679.json`.
- **DNS**: `nslookup -type=NS` contra 1.1.1.1.
- **Conducta medida**: `envios/ciclo-2-2026-10-07/boyaca-digital.md`.

Quien resuelve es otro Claude, de la misma casa que el autor y que el revisor.
Que aquí no se contradiga al revisor no cuenta como aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | Hay razón social, NIT y una persona natural, y la ficha los da por inexistentes estando en una página que ella misma cita | sí | sí. SECOP lo refuerza: nombra a Rosas representante legal | **Aceptada** |
| 2a | Forma jurídica: el sitio dice S.A.S.; SECOP registra el mismo NIT como «FUNDACION…»; y se declara «Agencia Privada No Lucrativa» | sí | sí | **Declarada como tensión** |
| 2b | Que dos dominios compartan par de servidores de Cloudflare no prueba que sean de la misma cuenta | sí (nslookup) | sí el dato. Ninguna fuente sostiene la inferencia de la ficha | **Aceptada** (se rebaja a indicio) |
| 2c | Hay indicios más fuertes: el mismo teléfono, publicidad de la casa y la cláusula de /terminos | sí | sí | **Aceptada** |
| 3 | El conflicto de interés existe en SECOP, pero con entidades nacionales y no con las alcaldías ni la gobernación de Boyacá | sí | sí, cifra por cifra, con una fecha deformada que no cambia nada | **Aceptada** |
| 4 | «Nivel 2: NO EXISTE» está desactualizado | sí (el envío) | sí | **Aceptada** |
| 5 | El 0,00 no sale de ninguna evidencia de orientación: es un valor por defecto | sí (la ficha y el protocolo) | sí | **Aceptada** (cambia la redacción, no el número) |
| 6 | La descripción de Juan Pablo Sáenz está incompleta («Ex Funcionario UTL») | sí | sí | **Aceptada como dato**. **Rechazada** como posible evidencia o aviso (ver motivo) |
| 7 | La captura de archive.org sí se puede consultar: confirma los clientes públicos pero dice «quince (15) años» | sí | sí | **Aceptada** |

### Lo verificado, objeción por objeción

**1 · Razón social, NIT y persona.** Literal en el HTML crudo:
- **holdingconsultants.org/nosotros/**: el pie dice «2006–2026 © Holding
  Consultants® · NIT 900.143.612-6 · Bogotá, Colombia». El JSON-LD trae
  `"legalName":"Holding Consultants S.A.S."` y `"taxID":"900143612-6"`. Y en el
  cuerpo: «Carlos O. Rosas Acevedo CEO y Fundador».
- **boyacadigital.com/equipo**, bajo «Columnistas invitados · Personas reales que
  aportan su mirada y opinión»: «Carlos O. Rosas A. es gerente de Boyacá Digital y
  columnista de opinión.»
- **Va más allá de lo que trae el revisor.** En los **58 registros** de SECOP II
  con el NIT 900143612, el campo `nombre_representante_legal` es **«Carlos Octavio
  Rosas Acevedo»**, y el domicilio, «Carrera 47 # 127 D 03», que es la dirección
  del JSON-LD de la consultora. Eso es un registro público, no una autodeclaración:
  la persona natural que representa legalmente a la sociedad consta en el Estado.
- El correo del Editor en Jefe aparece protegido por Cloudflare (`data-cfemail`).
  Decodificado es `[correo omitido]`, tanto en /sobre-nosotros como en
  /politica-editorial. Que el Editor en Jefe sea Rosas sigue siendo una
  **sospecha**: el medio no lo dice.
- **Matiz que se mantiene:** ser representante legal, CEO y fundador no prueba
  que sea el accionista. Eso solo lo dice el certificado de Cámara de Comercio.

**2a · Forma jurídica.** En SECOP integrado, con `like`, salen **87 registros**
con el NIT 900143612. Por razón social: «Holding Consultants» 77, «HOLDING
CONSULTANTS DE COLOMBIA» 6, «FUNDACION HOLDING CONSULTANTS DE COLOMBIA» 3 (dos con
`900143612` y uno con `900143612-6`) y «HOLDING CONSULTANTS» 1. Los tres de
«Fundación» son antiguos, de SECOP I:
- Soacha, 2007-04-27;
- **Nobsa, 2016-11-15, contrato 16-15-5596405, COP 100 000 000, «Liquidado»**;
- Positiva, 2017-02-24.

La página de empleabilidad dice literal: «actúa como Agencia Privada No
Lucrativa de Gestión y Colocación de Empleo, autorizada […] mediante la
Resolución 0472 del 19 de diciembre de 2025». El sitio dice S.A.S. Es una
tensión real, que solo resuelve el certificado. Una posible lectura, sin
confirmar: la entidad nació como fundación y se transformó. Hasta que conste,
**`ownerType: 'conglomerado'` no está respaldado por nada** de lo que se ha
leído. Hay que declararlo.

**2b · Servidores de nombres.** El dato es cierto: `boyacadigital.com`,
`holdingconsultants.org` y también `holdingsoft.org` responden con
`dylan.ns.cloudflare.com` y `fatima.ns.cloudflare.com`. Lo que no tiene fuente es
la inferencia de la ficha («Cloudflare asigna un par por cuenta», leído como si el
par fuera exclusivo de la cuenta). Ni la ficha ni esta verificación tienen un
documento de Cloudflare que diga que un par no se repite entre cuentas. Se
rebaja a indicio. Además deja de hacer falta, por 1 y 2c.

**2c · Indicios fuertes.** Literal:
- El JSON-LD `NewsMediaOrganization` de la portada del medio trae
  `"telephone":"[teléfono omitido]"`. El de la consultora, `"telephone":"[teléfono omitido]"`:
  es el mismo número.
- Hay enlaces con `utm_source=boyacadigital&utm_medium=house` hacia
  holdingconsultants.org y holdingsoft.org: 19 en la portada, 4 en /opinion, 4 en
  /escenario-politico y 1 en cada una de /equipo, /sobre-nosotros,
  /politica-editorial, /politica-de-privacidad y /terminos. Las campañas son
  `v-hc-*` y `v-hs-*`; `v-hc-paper` existe, en la portada, /escenario-politico y
  /politica-de-privacidad.
- **/terminos**: «…y el diseño del sitio son propiedad de Holding Consultants o se
  usan con licencia».
- El JSON-LD del medio sitúa la sede en «Carrera 11 #12-64», Sogamoso, y el de la
  consultora en «Carrera 47 No. 127D-03», Bogotá.

**3 · Contratos públicos.** SECOP II (`jbjy-vk9h`): **58 registros**, todos a
nombre de «Holding Consultants». Desde el 2025-10-07 hay **12 contratos, que
suman COP 70 386 247**. Coinciden con el revisor:

| Entidad | Contrato | Firma | Valor (COP) |
|---|---|---|---|
| Consejo Nacional Electoral | CPS-CNE-025-2025 | 2025-10-17 | 9 789 456 |
| Ministerio de Transporte | 722-2025 | 2025-11-25 | 3 645 200 |
| Fondo de Previsión Social del Congreso | MC-014-2025 | 2025-11-21 | 3 940 000 |
| Fondo Rotatorio de la Policía | CTO 075-2-26 | 2026-07-30 | 13 840 000 |
| Departamento de Policía Vichada (sanidad) | 44-7-20006-26 | 2026-08-25 | 8 800 000 |
| Corporación Autónoma Regional de Risaralda (CARDER) | CO1.PCCNTR.9864279 | 2026-08-28 | 3 808 664 |
| Politécnico Jaime Isaza Cadavid | 55285-2026 | 2026-09-15 | 15 856 742 |

- **Tres firmados después del 07-08-2026**, es decir, ya con el nuevo gobierno:
  los del 25-08, el 28-08 y el 15-09.
- Bogotá, Secretaría General, contrato 4232000-708-2025, del 2025-06-12, por
  78 410 640: correcto.
- **Boyacá**: en SECOP II, **cero** contratos (por departamento: Bogotá 43,
  Antioquia 4 y el resto disperso). En SECOP integrado, **solo Nobsa 2016,
  liquidado**.
- La frase de la ficha sobre «las alcaldías y la gobernación de Boyacá» queda,
  por tanto, sin respaldo en este registro. El conflicto documentado y vigente es
  con entidades nacionales y de otras regiones. Por la regla del presente, el de
  Nobsa no es vigente.
- El totalizado del integrado se reproduce en orden de magnitud: 87 filas, unas
  69 únicas y unos COP 2 240 millones entre 2007-04-27 y 2026-09-15, según cómo se
  quiten los duplicados. El revisor da 67 únicas y 2 207 millones. La diferencia
  es de método y no afecta a nada.
- Sigue en pie su matiz: que algo no aparezca en SECOP no significa que no exista.

**4 · Conducta medida.** Está en `envios/ciclo-2-2026-10-07/boyaca-digital.md`,
medición del 2026-10-07, ventana 31-08 → 07-10 (37 días):
- 1178 artículos, 328 en alguna historia y 338 historias;
- agenda propia del 20 %, 269 historias compartidas y compañía media de 0,141;
- coincide sobre todo con El Colombiano (76), El Tiempo (43) y La Silla Vacía (39).

**5 · El 0,00.** Es correcto. Ni la ficha ni esta verificación tienen evidencia de
**orientación** de nivel 1 a 3. El nivel 1 dice quién es el dueño, y la regla 1
del §5 dice que el dueño no determina la orientación. El nivel 2 tiene 37 días y
mide compañía, no contenido. La ficha ya decía «provisional de alta», pero lo
presenta como «Orientación mixta». Por la regla 3 del §5 («Sin evidencia de nivel
1-3, no se mueve el número. Se deja el actual y se marca la ficha como
incompleta»), el 0,00 se queda, pero etiquetado como **valor por ausencia de
evidencia, ficha incompleta**, no como orientación observada.

**6 · Juan Pablo Sáenz.** En /equipo, literal: «Periodista · Ex Funcionario UTL ·
Estratega en comunicación política · Cofundador de WHITE · Columnista de Boyacá
Digital.» En /escenario-politico, el listado se presenta como «Columnas de opinión
y análisis político de columnistas invitados». La pieza visible (Carlos Amaya y
Carolina Espitia) va firmada «Redacción Boyacá Digital · 5 de agosto de 2026 · IA».
La segunda (Bolívar y Amaya) muestra solo la fecha 2026-08-05, sin firma en el
listado. Que sean «dos piezas firmadas por la Redacción IA» es exacto para una y
no consta para la otra.

**7 · archive.org.**
- **El índice CDX** tiene 6 capturas con HTTP 200 de /nuestra-organizacion/, del
  2021-08-04 al **2023-03-24**, que es la última.
- **La captura del 2023-03-24** (título «Nuestra Organización - Holding
  Consultants de Colombia») dice, literal: «En el transcurso de nuestra permanencia
  en el mercado de quince (15) años sostenemos relaciones comerciales con numerosas
  empresas tanto del sector Privado como Público en varias ciudades del País.» Y
  también: «Contar con la fidelidad de varias empresas que desde 2006 confiaron en
  nosotros».
- **Lo que confirma:** la frase de los clientes públicos.
- **Lo que no confirma:** los «veinte años». Esos constan hoy en el JSON-LD del
  sitio nuevo: «20 años de experiencia en Colombia».
- **La fundación es inconsistente en la propia fuente:** /nosotros da «26 de marzo
  de 2007 Fundación de nuestra organización», mientras el JSON-LD dice
  `"foundingDate":"2006"` y el pie, «2006–2026». La captura habla de clientes
  «desde 2006». SECOP tiene un contrato del 2007-04-27, a nombre de la Fundación.
- **Lo que esto arregla en la PR #67:** el enlace caído se puede sustituir ya por
  la captura, que era la condición que esa PR dejó escrita. Ojo con la regla del
  presente: la captura de 2023 solo prueba que la frase existió. La prueba
  **vigente** de clientes públicos es SECOP (objeción 3), y es mejor.

**Fuera de objeción, comprobado:**
- **Wikidata Q140398679** («Boyacá Digital») tiene
  `P571 = +2025-10-07T00:00:00Z` con `precision: 9` (año), y su última
  modificación es del 2026-07-02. El sitio la enlaza en el `sameAs` del JSON-LD.
  Es un indicio editable por cualquiera: el medio sería de 2025.
- **El RSS** tiene 20 ítems, 0 etiquetas `<author>` o `dc:creator`, y el más
  reciente es del «Wed, 07 Oct 2026 22:32:17 GMT».
- **/equipo** lista 13 «Periodista de IA».
- **/opinion** está hecho de reescrituras atribuidas de columnas ajenas (La Silla
  Vacía, Boyacá 7 Días, La República), con 10 firmas «Redacción Boyacá Digital ·
  … · IA» en el listado. La de «El columnista Juan Pablo Ossa publicó en La Silla
  Vacía un análisis…» es literal en la pieza del 2026-09-27.

### Motivo de cada rechazo

- **Objeción 6, en lo que sugiere.** El revisor llama a «Ex Funcionario UTL» un
  «dato relevante» para la sección política. Se rechaza que sea evidencia de
  orientación o que dispare un aviso:
  - La regla de quien dirige excluye expresamente la «militancia pasada» y la
    «afinidad».
  - Exige una candidatura o un cargo público **vigente** de quien dirige o tiene
    la autoridad editorial, y Sáenz es columnista invitado.
  - El propio revisor no sabe de qué congresista fue.

  Entra en la ficha como dato descriptivo, literal y atribuido al medio, y nada
  más.
- **Ninguna otra objeción se rechaza.** La 2a se declara como tensión porque las
  fuentes públicas (el sitio frente a SECOP) se contradicen y solo un documento
  mercantil la cierra.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inventada.** Las URL resuelven, las citas literales coinciden con
el HTML crudo y las cifras de SECOP se reproducen. Deformaciones y huecos
menores:
- **«Ejército (2021)»: fecha deformada.** El único contrato de la Dirección de
  Sanidad del Ejército es del **2024-05-08** (COP 12 000 000). En 2021 hay contratos
  con la Agencia Logística de las Fuerzas Militares y con DISAN-DMSOC, no con
  «Ejército». No cambia nada.
- **Totales del integrado**: 67 únicas y 2 207 millones, frente a unas 69 y 2 240
  millones aquí. Es diferencia de método de deduplicación, no falsedad.
- **«Dos piezas firmadas Redacción IA» en /escenario-politico**: consta para una;
  la otra no muestra firma en el listado.
- **«Una columna de opinión publicada el 4 de octubre de 2026 en Boyacá 7 Días
  advierte…»: no localizada** en las páginas descargadas (portada y /opinion). Las
  de Boyacá 7 Días que figuran ahí son del 24, el 25 y el 27 de septiembre.
  **No cotejada**. No se usa.
- **El CDX dio 503 en la primera llamada.** El revisor dice que respondió 200.
  Respondió 200 en el segundo intento: es intermitencia, no un error.
- **Un acierto que la ficha no tenía:** la captura de archive.org **sí** se puede
  consultar. La PR #67 la dio por inaccesible por un bloqueo de red de quien
  verificó, no porque no existiera.

---

**Propuesta para la firma**

**(a) Valor. Mantener 0,00, pero no firmar todavía.**
- **Por qué 0,00.** La revisión no aporta ni una pieza de evidencia de
  orientación. Todo lo que añade es de propiedad (nivel 1) y no mueve el número
  (regla 1 del §5).
- **Por qué no firmar.** Lo que falta para hacerlo:
  1. aplicar las correcciones de (b), porque hoy la ficha afirma como inexistente
     una razón social, un NIT y una persona natural que constan en un registro
     público;
  2. reetiquetar el valor como «por ausencia de evidencia; ficha incompleta»
     (regla 3);
  3. el certificado de existencia y representación de NIT 900143612 (RUES), que
     cierra la forma jurídica (2a) y si Rosas es el accionista;
  4. la medición de 90 días con más de 60 historias que la REFUTACIÓN 4 ya prevé,
     junto con la comprobación anotada en la ficha: el trato a las entidades
     contratantes, ahora **nacionales** (CNE, Policía, MinTransporte, Fondo del
     Congreso, Politécnico JIC).

  Firmar antes de 1 y 2 sería firmar un expediente que se sabe erróneo.

**(b) Correcciones de hecho.**

*En `fichas/boyaca-digital.md`:*
1. **Nivel 1.** Sustituir «Sigue sin haber razón social, NIT ni una persona con
   nombre que responda» por lo siguiente:
   - razón social declarada: «Holding Consultants S.A.S.», NIT 900.143.612-6
     (holdingconsultants.org/nosotros/, pie y JSON-LD);
   - representante legal en SECOP II: **Carlos Octavio Rosas Acevedo**, en los 58
     registros del NIT (datos.gov.co `jbjy-vk9h`);
   - la consultora lo presenta como «CEO y Fundador» (/nosotros/), y el medio, como
     «gerente de Boyacá Digital y columnista de opinión»
     (boyacadigital.com/equipo).
   - Accionariado: no consta.
2. **Tabla «La propiedad, rastreada».**
   - «Razón social / NIT: no constan» → «Holding Consultants S.A.S. (según su
     sitio) · NIT 900.143.612-6 · forma jurídica en tensión, ver 3».
   - «Único humano con nombre: Juan Pablo Sáenz» → «Humanos con nombre: Carlos O.
     Rosas A. (gerente del medio y columnista; representante legal de la
     consultora en SECOP) y Juan Pablo Sáenz (columnista)».
   - «Responsable legal»: añadir «contacto publicado: [correo omitido]
     (/sobre-nosotros, /politica-editorial); que sea Rosas no consta».
3. **Tensión de forma jurídica** (texto nuevo):
   - SECOP integrado registra el mismo NIT a nombre de «FUNDACION HOLDING
     CONSULTANTS DE COLOMBIA» en 3 contratos (2007, 2016 y 2017);
   - la consultora se declara «Agencia Privada No Lucrativa de Gestión y
     Colocación de Empleo» (Resolución 0472 del 19-12-2025, en su página de
     empleabilidad);
   - su sitio dice «S.A.S.»;
   - lo resuelve el certificado de Cámara de Comercio.
4. **Tabla de indicios.**
   - Rebajar la fila de servidores de nombres a «comparten el par dylan/fatima
     (también holdingsoft.org); indicio, sin fuente de que el par sea exclusivo de
     una cuenta», y borrar «Cloudflare asigna un par por cuenta» como prueba.
   - Añadir el mismo teléfono [teléfono omitido] en el JSON-LD de los dos sitios.
   - Añadir la publicidad de la casa (`utm_medium=house`) hacia Holding Consultants
     y HoldingSoft en todas las páginas del medio.
   - Añadir /terminos: «son propiedad de Holding Consultants o se usan con
     licencia».
   - Añadir la sede declarada del medio: Carrera 11 #12-64, Sogamoso (JSON-LD).
5. **«Fuente caída (2026-10-06)».**
   - Sustituir el enlace caído por la captura
     `https://web.archive.org/web/20230324172804/https://www.holdingconsultants.org/nuestra-organizacion/`
     y citar literal la frase del sector «Privado como Público».
   - Corregir «veinte años» como cita de esa página: la captura dice «quince (15)
     años», y los 20 años constan hoy en el JSON-LD.
   - Señalar la inconsistencia de la fundación: 2007 en /nosotros, 2006 en el
     JSON-LD y en el pie.
6. **«El conflicto de interés que se declara».**
   - Sustituir «cubre a diario las alcaldías y la gobernación de Boyacá» como
     contraparte documentada por esto: SECOP II registra 12 contratos públicos en
     los últimos 12 meses (COP 70,4 millones) con entidades nacionales y de otras
     regiones: CNE, Ministerio de Transporte, Fondo de Previsión Social del
     Congreso, Fondo Rotatorio de la Policía, Policía Vichada, CARDER y Politécnico
     JIC. Tres son posteriores al 07-08-2026.
   - En Boyacá solo consta Nobsa 2016, liquidado.
   - El medio cubre esas entidades en su sección nacional.
   - Mantener «no se afirma que haya influido en ninguna pieza».
7. **Nivel 2.** Sustituir «NO EXISTE. No está ingerido» por la medición del
   2026-10-07 (cifras en el punto 4 de arriba), con la advertencia de los 37 días.
8. **Cabecera.** «0,00 · Orientación mixta — provisional de alta» → «0,00 · valor
   por ausencia de evidencia de orientación (regla 3 del §5) — ficha incompleta».
9. **Sáenz.** Usar la descripción literal de /equipo, con «Ex Funcionario UTL» y
   «Cofundador de WHITE», atribuida al medio. Sin consecuencia de clasificación.
10. **Reparo 2 (pluralidad).** Añadir la constatación: /opinion son reescrituras
    atribuidas de columnas de La Silla Vacía, Boyacá 7 Días y La República,
    firmadas «Redacción Boyacá Digital · IA». Ejemplo literal: «El columnista Juan
    Pablo Ossa publicó en La Silla Vacía un análisis…» (pieza del 2026-09-27).
11. **Edad del medio.** Wikidata Q140398679, `P571` 2025 (precisión de año), como
    indicio editable.

*En `shared/mediaOwnership.js`, entrada `boyaca-digital`:*
1. **`holdings[0]`**: sustituir «No se publica el nombre de esa persona, ni razón
   social, ni NIT» por la razón social, el NIT y Rosas, con las tres fuentes del
   punto 1 de arriba. Mantener que el Editor en Jefe no tiene nombre publicado.
2. **`holdings[1]`**: rebajar la frase de los servidores de nombres (punto 4) y
   añadir el teléfono, la publicidad de la casa y /terminos como respaldo del
   vínculo. Cambiar «Holding Consultants de Colombia» por «Holding Consultants
   S.A.S. (según su sitio)».
3. **`notes`, conflicto de interés**: reescribir con las contrapartes nacionales
   de SECOP (punto 6).
4. **`notes`, Sáenz**: añadir «Ex Funcionario UTL · Cofundador de WHITE». Añadir
   una nota sobre Rosas.
5. **`notes`, «La página de la consultora…»**: sustituir por la confirmación desde
   la captura del 2023-03-24 (sector público confirmado; dice 15 años, no 20).
   Borrar el comentario «FUENTE CAÍDA» del código.
6. **Nueva `note` de tensión**: S.A.S. frente a Fundación frente a «Agencia
   Privada No Lucrativa». Añadir que **`ownerType: 'conglomerado'` no está
   respaldado**. Que el responsable editorial decida si se queda o pasa a un tipo que no presuponga
   forma societaria hasta tener el certificado.
7. **`sources`**:
   - **sustituir** `https://www.holdingconsultants.org/nuestra-organizacion/` por
     la URL de la captura;
   - **añadir** `https://www.boyacadigital.com/terminos` y
     `https://www.boyacadigital.com/` (JSON-LD);
   - **añadir** `https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=id_contrato,nombre_entidad,proveedor_adjudicado,fecha_de_firma,valor_del_contrato,modalidad_de_contratacion,objeto_del_contrato,estado_contrato&$where=documento_proveedor%20like%20%27%25900143612%25%27`
     y `https://www.datos.gov.co/resource/rpmr-utcd.json?$select=nombre_de_la_entidad,nom_raz_social_contratista,numero_del_contrato,fecha_de_firma_del_contrato,valor_contrato,objeto_del_proceso,origen&$where=documento_proveedor%20like%20%27%25900143612%25%27`.
8. **`verifiedAt`**: sigue en `null` hasta la firma del responsable editorial.

**(c) Tensiones a declarar.**
1. **Forma jurídica:** S.A.S. (sitio), Fundación (SECOP 2007-2017) y «Agencia
   Privada No Lucrativa» (2025). La cierra el certificado de Cámara de Comercio.
2. **Persona natural frente a dueño:** Rosas es representante legal (SECOP), CEO y
   fundador (sitio) y gerente del medio. Que sea el accionista **no consta**.
3. **Editor en Jefe sin nombre**, con el correo `gerente@`. Que sea Rosas es una
   sospecha, y no se afirma. Hoy no consta candidatura ni cargo público de Rosas,
   así que la regla de quien dirige no se dispara.
4. **El conflicto de interés existe, pero con otra contraparte** que la que
   suponía la ficha: entidades nacionales, no Boyacá. La comprobación de nivel 2
   anotada en la ficha debe apuntar a ellas.
5. **El 0,00 es un valor por defecto, no una medición**, y el medio tiene 37 días
   de corpus y, según Wikidata, un año de vida.
