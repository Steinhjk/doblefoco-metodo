# Respuesta — Claude Opus 5.5 sobre Quindío Noticias

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
>
> **Edición:** retirados enlaces que pueden mostrar documentos de identidad (PROTOCOLO, Datos personales, 2026-10-10).

---

## RESPUESTA LITERAL

```
DECLARACIÓN PREVIA
La ficha la escribió otro modelo Claude; yo también soy Claude (Opus 5.5). No
soy un revisor independiente de la casa: lo que coincida con la ficha no vale
como aval. He buscado sobre todo en fuentes que la ficha NO usa.

CÓMO BUSQUÉ (2026-10-08)
- robots.txt de quindionoticias.com leído antes de nada: solo excluye /wp-admin/
  y búsquedas internas (?s=, /search/). No excluye ClaudeBot, Claude-Web ni
  anthropic-ai. Descargas con curl y UA de navegador.
- Sitio: portada, /page-sitemap.xml, API pública de WordPress (/wp-json/wp/v2/
  pages, users, categories, posts — permitida por robots.txt).
- SECOP II (datos.gov.co jbjy-vk9h) y SECOP I (f789-7hwg): por nombre «QUINDIO
  NOTICIAS» y, una vez hallado, por documento exacto [número de cédula omitido: dato personal de una persona natural, Ley 1581; consultable en SECOP].
  Aviso técnico: en jbjy-vk9h, `departamento='Quindío'` devuelve 0 filas
  (normalización Unicode); hay que usar `departamento like 'Quind%'`.
- No pude usar buscador web (cupo de búsquedas agotado en esta sesión). No
  consulté RUES ni la Superintendencia de Industria y Comercio (SIPI): ver «Lo
  que no pude verificar».

======================================================================
## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO
======================================================================
- ¿Cambió de dueño / venta / fusión / escisión en 12 meses? No encontré nada
  que lo indique. Pero la pregunta previa es otra: la ficha dice que el dueño
  es desconocido, y SECOP lo identifica (ver Objeción 1).
- ¿El titular/director que nombra la ficha sigue vivo y en el cargo? La ficha
  no nombra a nadie. El titular que yo encuentro, Daniel Andrés Hincapié
  Ramírez (C.C. [número de cédula omitido: dato personal de una persona natural, Ley 1581; consultable en SECOP]), tiene contrato firmado el 2026-01-17 (SECOP II),
  y la cuenta administradora del sitio (usuario WordPress id 1, slug
  «dhincapier») publicó por última vez el 2026-10-06. Comprobado 2026-10-08.
  No tengo prueba de defunción ni de salida; tampoco certificado mercantil.
- ¿Quién dirige hoy la redacción? No encontré un nombre de director publicado.
  Los firmantes del sitio son cuentas genéricas («Editora QN», «Quindío
  Noticias», «Editor QN WEB»). El único nombre propio con cuenta activa
  vinculable al control del sitio es la cuenta id 1 «dhincapier» (sospecha de
  que corresponde a D. Hincapié R.; ver Objeción 1).
- ¿Registro mercantil / reporte más reciente que la fuente de la ficha? No
  encontré certificado mercantil. Sí hay registros SECOP de 2021 y 2025-2026
  más recientes y más precisos que la única fuente de la ficha (el pie de la
  portada).

======================================================================
## OBJECIONES
======================================================================

OBJECIÓN 1 — «Sociedad, NIT y director: no publicados» / «Cualquier nombre
propio» como laguna. La identidad del operador está en SECOP.
- QUÉ afirma la ficha: no hay sociedad, NIT ni nombre; «es la ficha con menos
  asideros del catálogo»; la vía más prometedora sería la SIC.
- POR QUÉ es incorrecto: SECOP I registra un contrato firmado el 2021-11-26 con
  EMPRESAS PÚBLICAS DE ARMENIA, por $3.000.000, cuyo contratista figura con
  razón social «QUINDIO NOTICIAS», tipo de documento «Cédula de Ciudadanía»,
  identificación [número de cédula omitido: dato personal de una persona natural, Ley 1581; consultable en SECOP]. Objeto (texto del dataset): «SERVICIO DE DIFUSIoN
  Y/O PUBLICACIoN DE INFORMACIoN DE UN PORTAL WEB CON COBERTURA EN ARMENIA PARA
  LA TRANSMISION DE LAS CAMPAÑAS INSTITUCIONALES...». Esa misma identificación
  aparece en otros nueve registros de SECOP I y en dieciséis de SECOP II con el
  nombre «DANIEL ANDRES HINCAPIE RAMIREZ».
  Conclusión: Quindío Noticias no opera (al menos ante el Estado) como
  sociedad, sino como persona natural; su «NIT» es la cédula [número de cédula omitido: dato personal de una persona natural, Ley 1581; consultable en SECOP]. Por
  eso la ficha no encontraba razón social: probablemente no la hay.
  Corroboraciones independientes:
   (a) SECOP II registra como domicilio del contratista «[dirección omitida: el titular es una persona natural, Ley 1581] OF 601» en
       todos sus contratos 2025-2026; el propio sitio declara como dirección
       «[dirección omitida: el titular es una persona natural, Ley 1581] EDIFICIO CÁMARA DE COMERCIO – Armenia» (Términos de
       Servicio) y «Carrera 14 # 23-27 Of 1007 Armenia» (Política de
       privacidad). Mismo edificio, distinta oficina.
   (b) La cuenta administradora del WordPress (id 1) tiene el slug
       «dhincapier», y existe además un autor «Daniel Hincapie» (id 11, último
       artículo 2024-09-23). Que «dhincapier» = D. Hincapié R. es inferencia
       mía: SOSPECHA, no prueba.
- FUENTE: SECOP I, datos.gov.co f789-7hwg, consulta
  identificacion_del_contratista='[número de cédula omitido: dato personal de una persona natural, Ley 1581; consultable en SECOP]'; registro con
  ruta [enlace retirado: puede mostrar documentos de identidad; ver la resolución]
  (no abrí la ruta de contratos.gov.co: su robots.txt devuelve un 404 y no lo
  necesité; el dato está en el dataset abierto).
  SECOP II, datos.gov.co jbjy-vk9h, documento_proveedor='[número de cédula omitido: dato personal de una persona natural, Ley 1581; consultable en SECOP]'.
  https://quindionoticias.com/terminos-de-servicio-quindionoticias-com/
  https://quindionoticias.com/politica-de-privacidad/
  https://quindionoticias.com/wp-json/wp/v2/users
- FECHA: contrato 2021-11-26; domicilios en contratos 2025-03-14 a 2026-01-17;
  páginas del sitio actualizadas 2025-08-29 y 2025-04-01; consulta 2026-10-08.
- NIVEL: propiedad (registro público de contratación; no es certificado
  mercantil).

OBJECIÓN 2 — Conflicto de interés omitido: el titular identificado es
contratista vigente o reciente de entidades del Estado en el Quindío, incluida
una de la Gobernación.
- QUÉ afirma la ficha: nada sobre contratación; no hay sección de contratos.
- POR QUÉ importa: la misma cédula [número de cédula omitido: dato personal de una persona natural, Ley 1581; consultable en SECOP] tiene contratos de prestación de
  servicios con entidades públicas del departamento, la mayoría NO de pauta
  sino de servicios profesionales personales:
   · INDEPORTES QUINDÍO (instituto departamental de deportes): 2024-05-02
     $9.300.000; 2024-10-03 $7.750.000; 2025-03-14 $12.400.000 (CSP-131-2025);
     2026-01-17 $12.400.000 (086-CSP-2026, «En ejecución», fin previsto
     2026-05-16).
   · CORPORACIÓN AUTÓNOMA REGIONAL DEL QUINDÍO (CRQ): 2025-05-26 $9.000.000
     (CPS-505-2025); 2025-10-08 $7.500.000 (CPS-920-2025); 2026-01-15
     $19.200.000 (CPS-265-2026, «Modificado», 60 días adicionados), todos en la
     Oficina Asesora de Planeación.
   · GOBERNACIÓN DEL QUINDÍO (Secretaría de Hacienda, Tesorería):
     2020-10-20 $6.533.333; 2021-03-03 $11.540.000; 2021-07-26 $8.655.000;
     2021-11-04 $5.289.167; 2022-01-17 $17.310.000 (más un borrador de 2021 por
     $11.540.000 que no cuento).
   · Contratos de pauta/difusión del medio (todos 2018-2021): Alcaldía de
     Armenia 2018-03-07 $4.800.000 («emisión de contenidos informativos en
     medios digitales alternativos»); CRQ 2018 y 2019 ($3.000.000 y
     $8.000.000); Universidad del Quindío 2019-2021 (cinco registros, uno
     duplicado); Empresas Públicas de Armenia 2021 $3.000.000; Alcaldía de La
     Tebaida 2021-11-12 $2.100.000.
  Con la Alcaldía de Armenia no hay contrato desde 2018 en lo que encontré; con
  la Gobernación central, desde 2022. Pero Indeportes es entidad del orden
  departamental y el contrato de 2026 corre durante el período que la ficha
  debería evaluar.
- FUENTE: datos.gov.co jbjy-vk9h y f789-7hwg, por documento exacto [número de cédula omitido: dato personal de una persona natural, Ley 1581; consultable en SECOP].
- FECHA: contratos 2018-03-07 a 2026-01-17; consulta 2026-10-08.
- NIVEL: registro externo / propiedad (conflicto del titular).
- CIFRA (escribo «contratado»): últimos 12 meses (2025-10-08 → 2026-10-08):
  3 contratos, $39.100.000 contratados (CRQ $26.700.000; Indeportes
  $12.400.000). Si se excluye el contrato firmado exactamente el 2025-10-08:
  $31.600.000. Total histórico: SECOP II 15 contratos, $157.568.554; SECOP I
  9 contratos distintos, $46.030.000. Total: $203.598.554.

OBJECIÓN 3 — «No publica absolutamente nada sobre sí mismo» y «La ausencia es
total»: falso.
- POR QUÉ: el sitio sí publica páginas institucionales, pero no en las rutas que
  la ficha probó; están en su sitemap:
   · «Términos de Servicio – QuindioNoticias.com» (actualizada 2025-08-29):
     «QuindioNoticias.com es un medio de comunicación digital independiente que
     ofrece contenidos de carácter informativo, periodístico y de interés
     general, incluyendo noticias, reportajes, crónicas, columnas de opinión...»;
     «La contratación de publicidad no condiciona ni afecta la independencia
     editorial del medio»; contacto «Teléfono: [teléfono omitido: el titular es una persona natural, Ley 1581] Dirección: [dirección omitida: el titular es una persona natural, Ley 1581]
     EDIFICIO CÁMARA DE COMERCIO – Armenia, Quindío».
   · «Política de privacidad» (2025-04-01): «se refiere a Quindío Noticias,
     (Carrera 14 # 23-27 Of 1007 Armenia, Quindío)».
   · «Contáctenos / Paute con nosotros»: «Somos Quindío Noticias. Periódico
     digital del Eje Cafetero.»
  El aviso del catch-all es correcto (lo confirmé: /quienes-somos/, /about/ y
  una ruta inventada devuelven 200 y los mismos 122.161 bytes de la portada),
  pero la conclusión «no publica nada» no se sigue: bastaba el sitemap.
- FUENTE: https://quindionoticias.com/page-sitemap.xml ;
  https://quindionoticias.com/terminos-de-servicio-quindionoticias-com/ ;
  https://quindionoticias.com/politica-de-privacidad/ ;
  https://quindionoticias.com/contactenos-paute-con-nosotros/
  (texto cotejado del HTML crudo vía /wp-json/wp/v2/pages/<id>).
- FECHA: 2025-08-29, 2025-04-01, 2017-08-14 (fechas de modificación de WP).
- NIVEL: declaración del propio medio.

OBJECIÓN 4 — «Ni sección de opinión identificable»: falso. Hay sección de
opinión con columnista, y en el último año de columnas defendió a la
Gobernación.
- POR QUÉ: la API pública lista las categorías «opinion» (17 entradas),
  «c304-opinion» (92), y columnistas con categoría propia: «oliver-gomez-
  solarte» (75), «jota-dominguez-giraldo» (24), «pablo-jaramillo» (5). Las
  columnas más recientes son de «Finito» (feb.-mar. 2025), entre ellas:
   · 2025-03-16 «Oposición porque sí: falta de argumentos serios en contra del
     empréstito de la Gobernación | Opinión por: Finito». Extracto: «tres
     diputados optaron por votar en contra del empréstito, sin mayor
     argumentación, mostrando una oposición que parece responder más a
     intereses políticos...».
   · 2025-03-09 «El 'Coronell' no tiene quién le crea | Opinión por: Finito».
   · 2025-03-24 «Cortés tenía razón en CRQ: sí había quórum, dicho por el
     Consejo de Estado | Opinión por: Finito».
  OJO con la regla del presente: estas columnas tienen 19 meses; NO las aporto
  como evidencia de orientación, sino para tumbar la afirmación de hecho «no
  hay sección de opinión». La sección existe y su último uso es de 2025 (salvo
  un artículo de 2026-04-08 sobre Smart Fit mal categorizado como opinión).
  La columna sobre la CRQ coincide en el tiempo con contratos del titular con
  la CRQ (2025-05-26 en adelante): coincidencia temporal, no prueba de nada.
- FUENTE: https://quindionoticias.com/wp-json/wp/v2/categories ;
  https://quindionoticias.com/oposicion-porque-si-falta-de-argumentos-serios-en-contra-del-emprestito-de-la-gobernacion-opinion-por-finito-ok/ ;
  https://quindionoticias.com/cortes-tenia-razon-en-crq-si-habia-quorum-dicho-por-el-consejo-de-estado-opinion-por-finito/
- FECHA: 2025-02-23 a 2025-03-24.
- NIVEL: declaración del propio medio (sección), hecho editorial fuera de
  ventana.

OBJECIÓN 5 — Regla del polo fijo: hay asimetría a través del cambio de
gobierno, y la ficha (de 2026-08-14) no la midió. El valor 0,00 «por ausencia»
ya no se sostiene como ausencia.
- POR QUÉ: barrí los titulares de las 605 entradas publicadas entre 2026-08-31
  y 2026-10-08 y las búsquedas «petro», «espriella», «galvis» entre 2026-03-01
  y 2026-08-06 (API pública). Patrón:
   · Gobierno saliente (Petro), antes del 7-ago: titulares de escándalo con
     signo de interrogación y sustantivos cargados: «¿TRAICIÓN A LA PATRIA? El
     escándalo por audios secretos entre el Gobierno Petro y el Clan del Golfo
     desata un terremoto institucional» (2026-06-25); «Se acaba una de las
     banderas del gobierno Petro: ordenan liquidación del Ministerio de
     Igualdad» (2026-06-22, título leído del slug: cita no cotejada).
   · Gobierno entrante (De la Espriella), tras el 7-ago: titulares de
     celebración o de épica: «¡Tiemblan los capos! Presidente firma
     extradiciones a un ritmo frenético: dos criminales por día» (2026-10-01);
     «"Aquí nadie se acobarda": De La Espriella declara guerra sin cuartel a
     estructuras criminales tras carro bomba en Cúcuta» (2026-09-02); slugs
     «el-detalle-que-llamo-la-atencion...-abelardo-de-la-espriella-dona-su-
     primer-sueldo-a-ancianatos» (2026-09-12), «mentiroso-asi-respondio-
     abelardo-de-la-espriella-a-gustavo-petro-por-los-subsidios» (2026-09-24),
     «abelardo-de-la-espriella-entrego-moderno-colegio...» (2026-09-15) (estos
     tres: cita no cotejada, solo slug).
     En el mismo barrido NO encontré ni un titular crítico con el gobierno
     entrante después del 7-ago. Antes del 7-ago sí los hubo («BID aclara que
     los US$60 millones anunciados por De la Espriella ya hacían parte de una
     cartera...», 2026-07-19; «Se está configurando un gobierno paramilitar: la
     fuerte crítica de Cepeda...», 2026-07-08 — slugs, no cotejados).
   · Gobernador Juan Miguel Galvis: tono uniformemente elogioso antes y después
     del cambio: «El Quindío cambia sus vías: el liderazgo de Juan Miguel
     Galvis impulsa tres grandes obras» (2026-09-26; extracto: «Bajo el
     liderazgo del gobernador Juan Miguel Galvis Bedoya...»); slugs
     «prudencia-ante-el-peligro-gobernador-frena-demoliciones-apresuradas...»
     (2026-09-28), «las-ayudas-no-son-del-gobernador-ni-de-los-politicos-el-
     contundente-mensaje-de-juan-miguel-galvis...» (2026-09-14). La crítica
     local recae sobre alcaldías (Quimbaya, Montenegro, Filandia) y el Concejo,
     no sobre la Gobernación. No encontré un solo titular crítico con la
     Gobernación en la ventana.
   · 2026-10-02 «Petro y De La Espriella destapan presunta corrupción del
     hermano de Óscar Marín, quien suena para la Gobernación»: pieza contra un
     posible aspirante a la Gobernación en 2027.
  Lectura según el protocolo: criticar a Petro mientras gobernaba es
  fiscalizar y NO cuenta. Lo que cuenta es el paso a encuadre celebratorio
  cuando llega De la Espriella, y el encuadre asimétrico a favor del gobernador
  incumbente (cuya institución contrató al titular). Advertencias honestas:
  (1) es análisis de TITULARES, no de cuerpos; (2) muchas piezas de la
  Gobernación parecen boletines institucionales reescritos (sospecha, no lo
  comprobé contra los boletines oficiales), lo que puede ser pereza editorial
  y no línea; (3) 38 días.
  No propongo número. Sí digo que «0,00 porque no hay nada» es falso: hay
  conducta observable, la ficha no la miró, y apunta en una dirección
  (gobierno nacional entrante de derecha + oficialismo departamental).
- FUENTE: https://quindionoticias.com/wp-json/wp/v2/posts?after=2026-08-31T00:00:00
  y ?search=petro|espriella|galvis&after=2026-03-01&before=2026-08-07 ;
  URLs: https://quindionoticias.com/tiemblan-los-capos-presidente-firma-extradiciones-a-un-ritmo-frenetico-dos-criminales-por-dia/ ;
  https://quindionoticias.com/aqui-nadie-se-acobarda-de-la-espriella-declara-guerra-sin-cuartel-a-estructuras-criminales-tras-carro-bomba-en-cucuta/ ;
  https://quindionoticias.com/el-quindio-cambia-sus-vias-el-liderazgo-de-juan-miguel-galvis-impulsa-tres-grandes-obras/ ;
  https://quindionoticias.com/traicion-a-la-patria-el-escandalo-por-audios-secretos-entre-el-gobierno-petro-y-el-clan-del-golfo-desata-un-terremoto-institucional-ok/ ;
  https://quindionoticias.com/petro-y-de-la-espriella-destapan-presunta-corrupcion-del-hermano-de-oscar-marin-quien-suena-para-la-gobernacion/
- FECHA: 2026-06-22 a 2026-10-07.
- NIVEL: hecho editorial de los últimos 12 meses / conducta observable.

OBJECIÓN 6 — Omisión: el sitio publica contenido parásito de casinos en
idiomas extranjeros, mezclado en la sección local.
- POR QUÉ: en la portada del 2026-10-08 aparecen enlaces como «wie-sicher-sind-
  personliche-daten-im-nv-casino-wirklich», «quel-est-le-montant-minimum-de-
  depot-chez-vulkan-vegas-casino», «my-empire-casino-garantiza-pagos-rapidos-
  y-seguros...». En la ventana 2026-08-31 → 2026-10-08 conté al menos 13
  entradas de este tipo (de 605), todas en la categoría 71 («noticiasquindio»,
  la principal local), firmadas por la cuenta «Editora QN» (id 14). Esto
  contradice lo que el medio declara en sus Términos («Dichos espacios serán
  siempre identificados como publicidad») y contamina el corpus de conducta
  medida (artículos en alemán/francés sobre casinos cuentan como «agenda
  propia»).
- FUENTE: https://quindionoticias.com/ (HTML crudo, 2026-10-08);
  https://quindionoticias.com/wp-json/wp/v2/posts?after=2026-08-31T00:00:00
- FECHA: 2026-08-31 a 2026-10-08.
- NIVEL: conducta observable (no mueve el eje, pero afecta la calidad del
  corpus y la fiabilidad del medio).

OBJECIÓN 7 — Cifras de volumen: la conducta medida cuenta 496 artículos en la
ventana; la API del sitio da 605 entradas publicadas desde 2026-08-31.
- POR QUÉ: diferencia de ~18 %. Puede deberse al feed (10 ítems por petición)
  o a la exclusión del spam. No es error de la ficha sino del corpus; lo
  anoto porque la «agenda propia 58 %» se calcula sobre solo 51 piezas.
- FUENTE: API WordPress (paginación de /posts?after=2026-08-31T00:00:00).
- FECHA: 2026-10-08.
- NIVEL: conducta medida.

======================================================================
## LO QUE NO PUDE VERIFICAR
======================================================================
- Registro de la marca «Quindío Noticias®» en la SIC: no consulté SIPI
  (aplicación con formularios dinámicos; no lo intenté). No sé si existe el
  registro ni quién es el titular.
- Registro mercantil (RUES / Cámara de Comercio de Armenia) de Daniel Andrés
  Hincapié Ramírez como persona natural comerciante o de alguna sociedad: no
  consultado.
- Vínculos políticos (militancia, cargos, campañas) de D. A. Hincapié Ramírez:
  no encuentro fuente para esto. Sin buscador web disponible, no pude buscar
  en Cuentas Claras, Registraduría ni prensa. Lo único que tengo es el
  historial contractual.
- Que la cuenta WordPress «dhincapier» sea D. A. Hincapié R.: inferencia por
  coincidencia de iniciales y apellido, sin documento que lo confirme.
- Identidad de «Finito» (columnista de 2025): no encontrada.
- Si las piezas de la Gobernación son boletines oficiales copiados: no cotejé
  con gobernacionquindio.gov.co.
- Si existe pauta oficial pagada por canales que no pasan por SECOP (órdenes de
  compra por agencia de medios, pauta de partidos): no verificable desde aquí.

======================================================================
## LO QUE FALTA
======================================================================
1. El titular identificado (C.C. [número de cédula omitido: dato personal de una persona natural, Ley 1581; consultable en SECOP]) y la forma jurídica (persona
   natural), con los registros SECOP como fuente.
2. Una sección de contratación con la cifra de los últimos 12 meses y el
   histórico, distinguiendo pauta del medio (2018-2021) y servicios
   profesionales del titular (2020-2026) con Indeportes, CRQ y Gobernación.
3. La sección de opinión y los textos institucionales (Términos, Privacidad).
4. Un barrido de titulares antes y después del 7-ago-2026 (polo fijo), y de la
   cobertura del gobernador Galvis.
5. Una advertencia sobre el spam de casinos y su efecto en el corpus.
6. Certificado de Cámara de Comercio y consulta en SIC, ahora que hay nombre
   y cédula con los que pedirlos.

======================================================================
## EVIDENCIA QUE NO MUEVE EL NÚMERO
======================================================================
- El aviso del catch-all es exacto: /quienes-somos/, /about/ y
  /estonoexiste12345/ devuelven 200 y 122.161 bytes, idénticos a la portada
  (2026-10-08).
- El pie dice hoy «© 2026 Quindío Noticias® - 2011-2025» (HTML crudo de la
  portada, 2026-10-08): la ficha lo cita bien.
- Hay cobertura no complaciente con el nivel local no departamental: «Colegio
  en ruinas y sin pólizas: la omisión de la Alcaldía de Quimbaya...»
  (2026-09-27), «800 millones, cuatro meses y una presunta cercanía: el
  contrato del alcalde de Montenegro...» (2026-09-23), «¿Peligra el agua del
  Quindío? El escandaloso secreto del Concejo para aprobar territorio Panaca»
  (2026-09-30) (títulos de slug, no cotejados). Es fiscalización y no mueve el
  eje.
- El gobernador Galvis aparece enfrentando al gobierno nacional en temas
  regionales (2026-08-03: «"El Quindío no aguanta otra valorización":
  gobernador pide frenar cobro del INVÍAS», contra una resolución del INVÍAS
  de finales del gobierno Petro): el medio lo recoge como voz del
  gobernador, no como posición propia.
- No encontré endoso electoral explícito del medio en las elecciones de 2026
  (busqué en las categorías de opinión y en los titulares de política
  mar.-oct. 2026). Ausencia de endoso: conducta de la casa, anotada.
- SECOP: ningún contrato de la cédula [número de cédula omitido: dato personal de una persona natural, Ley 1581; consultable en SECOP] ni de «QUINDIO NOTICIAS» con
  la Alcaldía de Armenia después de 2018, ni con la Gobernación central
  después de 2022 (consulta 2026-10-08).

======================================================================
## SIN OBJECIÓN
======================================================================
No aplica: hay objeciones.
```

---

## RESOLUCIÓN

> **Sustitución añadida el 2026-10-08, al juntar la tanda 3:** también se omitieron en la respuesta literal el teléfono y la dirección que el sitio publica como contacto. El titular es una persona natural, así que son suyos (regla de DATOS PERSONALES del protocolo). Son 2 sustituciones de teléfono y las de dirección, cada una marcada en su sitio.

**Propuesta de resolución — Claude Code, 2026-10-08. Pendiente de la firma del responsable editorial.**

**Única edición de la respuesta literal.** En la respuesta literal se ha sustituido cada aparición del número de cédula del contratista por «[número de cédula omitido: dato personal de una persona natural, Ley 1581; consultable en SECOP]». La decisión es de esta sesión: el medio opera como persona natural y su documento es un dato personal. No se ha tocado nada más del texto del revisor. Esta resolución tampoco escribe el número. Para identificar a la persona bastan el nombre, la condición de persona natural y la constancia de SECOP I 21-4-12596549 (sin enlace: la página de contratos.gov.co muestra el documento del contratista).

**Cómo se verificó (2026-10-08).**
- **robots.txt**, leído aquí y no copiado del revisor:
  - quindionoticias.com: solo excluye `/wp-admin/` y las búsquedas internas (`?s=`, `/search/`); no menciona a ClaudeBot, Claude-Web ni anthropic-ai, y `/wp-json/` no está excluido;
  - datos.gov.co: solo `User-agent: *`, sin exclusión de `/resource/`;
  - contratos.gov.co/robots.txt devuelve 404, y no se descargó nada de ese dominio.
- **Descargas**: todo en crudo con `curl -sL` y el UA de navegador que pide la sesión.
- **SECOP**: se consultaron SECOP I (`f789-7hwg`) y SECOP II (`jbjy-vk9h`) con **igualdad exacta por documento**. Los totales se recalcularon aquí, quitando duplicados por `uid` en SECOP I y los borradores en SECOP II.
- **Sitio**:
  - sitemap de páginas, Términos, Privacidad y Contáctenos, con el texto extraído del HTML;
  - API pública de WordPress: `users`, `categories` y las 605 entradas desde el 2026-08-31, descargadas enteras;
  - búsquedas «petro», «espriella» y «galvis» entre el 2026-03-01 y el 2026-08-07;
  - cinco artículos abiertos en crudo.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | La identidad del operador está en SECOP: persona natural, Daniel Andrés Hincapié Ramírez | sí | sí | **Aceptada**. La equivalencia de «dhincapier» con él sigue como **sospecha** |
| 2 | Conflicto omitido: el titular es contratista de entidades del Quindío; cifras de 12 meses e histórico | sí | sí; cifras exactas y listado incompleto | **Aceptada con el listado completado** |
| 3 | «No publica nada sobre sí mismo» es falso: Términos, Privacidad y Contáctenos están en el sitemap | sí | sí | **Aceptada** |
| 4 | Sí hay sección de opinión (columnas de «Finito», 2025, en defensa de la Gobernación) | sí | sí | **Aceptada como hecho**. **Rechazada** la «coincidencia temporal» con la CRQ |
| 5 | Polo fijo: asimetría Petro / De la Espriella y trato elogioso al gobernador Galvis; el 0,00 «por ausencia» ya no se sostiene | sí | sí, en titulares | **Declarada como tensión**. **Rechazado** el «paso» de encuadre en el 7-ago |
| 6 | Spam de casinos en idiomas extranjeros, mezclado en la sección local | sí | sí; el revisor **se queda corto** | **Aceptada** (19 entradas, no «al menos 13») |
| 7 | La API da 605 entradas en la ventana y el corpus mide 496 | sí | sí | **Aceptada como nota de corpus**; no es un error de la ficha |

### Lo verificado, objeción por objeción

**1 · Identidad.**
- SECOP I, constancia **21-4-12596549**, contrato CS-430-2021 con Empresas Públicas de Armenia, firmado el **2021-11-26**, $3 000 000:
  - `nom_razon_social_contratista` «QUINDIO NOTICIAS», tipo «Cédula de Ciudadanía», representante legal «DANIEL ANDRES HINCAPIE RAMIREZ»;
  - el objeto es literal: «SERVICIO DE DIFUSIoN Y/O PUBLICACIoN DE INFORMACIoN DE UN PORTAL WEB CON COBERTURA EN ARMENIA PARA LA TRANSMISION DE LAS CAMPAÑAS INSTITUCIONALES».
- El mismo documento aparece, con el nombre de la persona, en otras 9 filas de SECOP I (8 contratos, porque uno está duplicado) y en las 16 de SECOP II.
- En tres registros de la Universidad del Quindío el tipo de documento es «Nit de Persona Natural». Refuerza que no hay sociedad.
- **Domicilio.**
  - Fuente de la dirección: el registro de SECOP I no trae dirección; la dirección sale de SECOP II.
  - Lo que dice SECOP II: el campo `domicilio_representante_legal` dice «[dirección omitida: el titular es una persona natural, Ley 1581] OF 601» en **las 16 filas, de 2018 a 2026**, no solo en las de 2025-2026 como escribe el revisor. Es un dato del perfil del proveedor, no de cada contrato.
  - Lo que dice el sitio:
    - Términos: «Dirección: [dirección omitida: el titular es una persona natural, Ley 1581] EDIFICIO CÁMARA DE COMERCIO – Armenia, Quindío – Colombia»;
    - Privacidad: «se refiere a Quindío Noticias, (Carrera 14 # 23-27 Of 1007 Armenia, Quindío)».
  - Conclusión: es el mismo edificio, con oficina distinta.
- **WordPress** (`/wp-json/wp/v2/users`):
  - el usuario id 1 tiene el nombre visible «Quindío Noticias» y el slug «dhincapier»;
  - el id 11 se llama «Daniel Hincapie», y su última entrada es del 2024-09-23;
  - el id 1 firma 110 de las 605 entradas de la ventana, la última del 2026-10-06.
  - Que el id 1 sea el administrador no se puede ver en la API pública: es el primer usuario creado, nada más.
  - Que «dhincapier» sea esta persona sigue siendo inferencia.
- **Homónimo, o error de digitación, que el revisor no vio.** SECOP I tiene otra fila con el mismo nombre y un documento que difiere en **dos dígitos contiguos**: constancia 19-13-9321865, Alcaldía de Armenia, contrato 2002, firmado el 2019-04-30, $12 000 000. Su objeto es el mismo que el del contrato de pauta de 2018 («emisión de contenidos informativos en medios digitales alternativos»). Es muy probablemente la misma persona con el documento mal digitado. **Por la regla de igualdad exacta no se suma**, pero se declara.

**2 · Contratación.** El recálculo da lo mismo que el revisor:

| | Contratos | Valor contratado |
|---|---|---|
| SECOP II, sin el borrador HAC743-PSP-2021 | 15 | $157 568 554 |
| SECOP I, sin el duplicado OCONT-628 | 9 | $46 030 000 |
| **Total 2018-2026** | **24** | **$203 598 554** |
| **Últimos 12 meses** (firmados del 2025-10-08 al 2026-10-08, ambos incluidos) | **3** | **$39 100 000** |

- Los tres contratos de los últimos 12 meses son:
  - CRQ CPS-920-2025, 2025-10-08, $7 500 000;
  - CRQ CPS-265-2026, 2026-01-15, $19 200 000, «Modificado», 60 días adicionados;
  - Indeportes 086-CSP-2026, 2026-01-17, $12 400 000, fin previsto el 2026-05-16.
- Sin el contrato del 2025-10-08, la cifra es $31 600 000. El revisor lo dice bien.
- Por contratante, 2018-2026:

| Contratante | Contratos | Valor |
|---|---|---|
| Gobernación del Quindío | 5 | $49 327 500 |
| Indeportes Quindío | 4 | $41 850 000 |
| CRQ (SECOP II $35 700 000 + SECOP I $11 000 000) | 5 | $46 700 000 |
| Empresas Públicas de Armenia | 2 | $18 480 000 |
| RAP Eje Cafetero | 1 | $16 000 000 |
| IGAC | 1 | $12 591 054 |
| Universidad del Quindío | 4 | $11 750 000 |
| Alcaldía de Armenia | 1 | $4 800 000 |
| Alcaldía de La Tebaida | 1 | $2 100 000 |

- **Dos naturalezas distintas**, que el revisor distingue bien:
  - *Pauta del medio* (difusión institucional), 2018-2021: $32 650 000. Son Alcaldía de Armenia 2018, CRQ 2018 y 2019, Universidad del Quindío, EPA 2021 y La Tebaida.
  - *Servicios profesionales personales del titular*, 2018-2026: $170 948 554. Son Tesorería de la Gobernación 2020-2022, Indeportes 2024-2026, la Oficina Asesora de Planeación de la CRQ 2025-2026, el IGAC 2018, la RAP 2023 y EPA 2022.
- **Omisiones del listado del revisor.** Las tres entran en sus totales, pero no aparecen en el texto:
  - IGAC 2018, $12 591 054;
  - RAP Eje Cafetero 2023, $16 000 000;
  - EPA 2022 (CS-246-2022), $15 480 000, de servicios profesionales.
- **Precisión sobre la Gobernación.** Los contratos con la Gobernación central son de 2020-2022, antes del gobernador actual, Juan Miguel Galvis, que asumió en 2024. Con Galvis, el vínculo departamental es **Indeportes**, instituto descentralizado del departamento (2024-05-02 en adelante). La CRQ es una corporación autónoma, no la Gobernación. Por eso «cuya institución contrató al titular» (obj. 5) es impreciso: lo exacto es «un instituto del departamento».
- **Vigencia.** Ningún contrato tiene fecha de fin posterior al 2026-10-08 en los datos abiertos.

**3 · Páginas institucionales.**
- El `page-sitemap.xml` lista:
  - Términos (lastmod 2025-08-29);
  - Privacidad (2025-04-01);
  - Contáctenos / Paute con nosotros (2017-08-14);
  - Contacto (2015).
- Las tres citas del revisor son **literales** en el HTML:
  - «QuindioNoticias.com es un medio de comunicación digital independiente que ofrece contenidos de carácter informativo, periodístico y de interés general»;
  - «La contratación de publicidad no condiciona ni afecta la independencia editorial del medio»;
  - «Somos Quindío Noticias. Periódico digital del Eje Cafetero.».
- Teléfono: [teléfono omitido: el titular es una persona natural, Ley 1581].
- Catch-all confirmado: una ruta inventada devuelve 200 y 122 161 bytes, los mismos que la portada. La ficha decía 106 kB el 2026-08-14.

**4 · Opinión.**
- Categorías, por la API:
  - `opinion` (id 14): 17 entradas;
  - `c304-opinion` (77): 92;
  - `oliver-gomez-solarte` (340): 75;
  - `jota-dominguez-giraldo` (290): 24;
  - `pablo-jaramillo` (335): 5.
- Las columnas de «Finito» de 2025-03-02 a 2025-03-24 existen.
- El extracto del 2025-03-16 es literal: «tres diputados optaron por votar en contra del empréstito, sin mayor argumentación, mostrando una oposición que parece responder más a intereses políticos».
- La entrada más reciente de las categorías de opinión es la de Smart Fit (2026-04-08).
- **Dato que el revisor no da:** las columnas de «Finito» están archivadas en la categoría de **Oliver Gómez Solarte** (340). No prueba que sea la misma persona.

**5 · Polo fijo.**
- Los titulares citados por el revisor existen, y con las fechas que da:
  - «¡Tiemblan los capos!…», 2026-10-01;
  - «“Aquí nadie se acobarda”…», 2026-09-02;
  - «El Quindío cambia sus vías…», 2026-09-26, con el extracto «Bajo el liderazgo del gobernador Juan Miguel Galvis Bedoya» literal;
  - «Las ayudas no son del gobernador…», 2026-09-14;
  - «¡Prudencia ante el peligro!…», 2026-09-28;
  - «Mentiroso…», 2026-09-24;
  - «…dona su primer sueldo a ancianatos», 2026-09-12;
  - «…entregó moderno colegio…», 2026-09-15;
  - «¿TRAICIÓN A LA PATRIA?…», 2026-06-25;
  - «Se acaba una de las banderas del Gobierno Petro…», 2026-06-22;
  - «BID aclara…», 2026-07-19;
  - «“Se está configurando un gobierno paramilitar”…», 2026-07-08;
  - «Petro y De La Espriella destapan…», 2026-10-02.
- De los 33 titulares políticos de la ventana, **ninguno es crítico con el presidente ni con el gobernador**.
- **Pieza que el revisor omitió, y que refuerza su lectura:** «¿Gobernador con el Presidente y los alcaldes en contra? : El pulso que de los mandatarios de Armenia, Filandia y Quimbaya contra De La Espriella» (2026-09-25, cuenta id 1).
  - Lo único que se parece a una oposición al gobierno entrante lo encuadra contra los alcaldes.
  - Cita: «existiría un marcado interés de los mandatarios locales por manejar la chequera y ejecutar estos recursos de manera directa, evadiendo los conductos estructurados por el nivel central».
- **Lo que matiza la lectura, y el revisor no lo dice:**
  - **El encuadre celebratorio de De la Espriella no empieza el 7-ago.** Como presidente electo ya tenía «¡MANO DURA! De la Espriella lanza estrategia radical…» (2026-07-05) y «“Cogí la culebra por la cabeza”…» (2026-07-03). No hay un «paso» en la transición. Hay un trato asimétrico de los dos lados, sostenido de junio a octubre.
  - **Los titulares «críticos» que el revisor pone antes del 7-ago** son voces de la oposición (Cepeda) o aclaraciones de terceros (BID), no críticas de la casa. La comparación no es homogénea.
  - **La ventana coincide con el terremoto del Quindío** («A un mes del terremoto…», 2026-09-10). Las visitas presidenciales y las obras del departamento son noticia por sí mismas. Muchas piezas del gobernador las firma la cuenta id 5 con aire de boletín, aunque eso no se cotejó con los boletines oficiales.
  - **Petro solo se ve en sus últimas seis semanas**, y como saliente.

**6 · Casinos.**
- En la ventana hay **19 entradas** de casino o apuestas en alemán, francés, inglés, rumano, polaco, italiano, portugués y español. Todas son de la cuenta «Editora QN» (id 14) y de la categoría 71 sola. Una muestra:
  - `problemes-courants-sur-instant-casino…` (2026-10-08);
  - `crownpokies-server-stabilitat…`;
  - `so-verfolgen-sie-den-wettfortschritt-fur-den-spinboss-willkommensbonus`;
  - `ghidul-zorabet-pentru-boleto`;
  - `uprawnienia-aplikacji-twindor-wyjasnione`;
  - `winnita-free-cash-sulla-verifica-e-reale`;
  - `granawin-mercados-de-apostas-de-cricket`;
  - `on-which-slots-does-malina-casino-give-free-spins` (2026-08-31).
- La portada del 2026-10-08 enlaza **17** URL de ese tipo, entre ellas las tres que cita el revisor (`wie-sicher-sind…nv-casino…`, `quel-est-le-montant…vulkan-vegas…`, `my-empire-casino…`). Esas tres tienen fecha del 2025-12-22, el 2025-12-24 y el 2026-02-21: el spam viene de antes de la ventana.
- **El revisor se queda corto («al menos 13»), no exagera.**
- Que los Términos digan «Dichos espacios serán siempre identificados como publicidad» es literal.
- No se ha determinado si es pauta vendida o una cuenta comprometida.

**7 · Volumen.**
- `X-WP-Total` = **605** para `after=2026-08-31`.
- Según el envío del 2026-10-08, el corpus da 496 artículos, de los que 51 están en alguna historia, en 53 historias, con un 58 % de agenda propia.
- La diferencia es del 18 %. Los 19 de casino no explican toda la diferencia, y si entran por el feed, contaminan el corpus.

### Motivo de cada rechazo

- **Obj. 4, «la columna sobre la CRQ coincide en el tiempo con contratos del titular con la CRQ».**
  - La columna es del 2025-03-24 y el primer contrato de la CRQ en SECOP II, del 2025-05-26: dos meses después. No coinciden.
  - Lo que sí coincide es otra cosa, y el revisor no la vio: la columna en defensa del empréstito de la Gobernación (2025-03-16) sale dos días después de firmado el CSP-131-2025 con Indeportes (2025-03-14).
  - Ni una cosa ni la otra prueban nada, y las columnas tienen 19 meses: quedan fuera de la regla del presente. Se rechaza como indicio y se conserva solo el hecho de que la sección existe.
- **Obj. 5, «el paso a encuadre celebratorio cuando llega De la Espriella».** La celebración ya estaba con el presidente electo (julio de 2026). Lo que hay es una asimetría sostenida entre los dos lados, que es justo lo que el polo fijo admite como evidencia. Pero no puede mover el número todavía, por cuatro motivos:
  - se leyeron titulares, no cuerpos;
  - son 38 días;
  - el terremoto confunde la cobertura;
  - el protocolo mueve el número solo con corpus (regla 3).
  Por eso queda como **tensión** y no como cambio de valor.
- **Obj. 1, que la cuenta id 1 sea «la cuenta administradora».** La API pública no expone roles. Se rechaza la palabra «administradora», no la objeción.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente.** Todas las URL resuelven, las citas cotejadas son literales y las cifras de SECOP cuadran al peso. Hay deformaciones y omisiones:
- **SECOP, listado incompleto.** Omite del texto tres contratos que sí suma (IGAC 2018, RAP 2023, EPA 2022: $44 071 054). Quien lea solo el listado no llega al total.
- **«Con la Alcaldía de Armenia no hay contrato desde 2018»: incompleto.** Hay uno de 2019 por $12 000 000 con el mismo nombre y el documento con dos dígitos cambiados. No se suma, pero el revisor no lo vio.
- **«Domicilio en todos sus contratos 2025-2026»: impreciso.** El campo está en las 16 filas de 2018 a 2026, y es del perfil del proveedor.
- **«Cuya institución contrató al titular» (el gobernador Galvis): impreciso.** La Gobernación central contrató en 2020-2022, antes de Galvis. Con Galvis contrata Indeportes.
- **Obj. 4, «coincide en el tiempo»: falso.** Hay dos meses de distancia (ver motivo).
- **Obj. 5:** no cita la pieza del 2026-09-25, que refuerza su tesis, y presenta como cambio en la transición un encuadre que ya existía en julio.
- **Obj. 6: «al menos 13» es un recuento corto.** Son 19.
- **Cuenta id 1, «administradora»:** afirmado sin fuente.

---

**Propuesta para la firma**

**(a) Valor: mantener 0,00 por Regla 2, cambiar su razón y no firmar todavía.**
- La razón escrita, «la ausencia es total», es falsa: hay páginas institucionales, una sección de opinión, un titular identificado y conducta observable.
- El 0,00 se sostiene porque la conducta que apunta a un lado (oficialismo nacional entrante y departamental) está medida solo en titulares, durante 38 días y con el terremoto de por medio. El protocolo pide 90 días de corpus para mover el número.
- No se firma hasta aplicar (b) y declarar (c).

**(b) Correcciones de hecho**

En `fichas/quindio-noticias.md`:
1. **Titular.** Cambiar «Sociedad: no publicada / NIT: no publicado» por «**Opera como persona natural: Daniel Andrés Hincapié Ramírez**. Así figura ante el Estado: contrato de SECOP I con razón social "QUINDIO NOTICIAS" y cédula de ciudadanía (EPA, 2021-11-26, constancia 21-4-12596549). El documento no se publica por ser un dato personal de una persona natural (Ley 1581); es consultable en SECOP. No hay sociedad conocida». Añadir:
   - el domicilio de SECOP II («[dirección omitida: el titular es una persona natural, Ley 1581] OF 601»), en el mismo edificio que el de los Términos y la Privacidad del sitio;
   - que la cuenta WordPress id 1, con slug «dhincapier», firma 110 de 605 entradas de la ventana. **Que sea él es sospecha.**
2. **Director / editor.** Sigue «no publicado». Añadir: «No consta candidatura ni cargo público. Un contrato de prestación de servicios no es cargo público, así que no se dispara el aviso de quien dirige».
3. **Contratación pública**, en el formato del protocolo:
   > Contratación pública (SECOP I y II, contratista persona natural Daniel Andrés Hincapié Ramírez, documento omitido por Ley 1581, consultado 2026-10-08): 3 contratos por $39 100 000 **contratados** en los últimos 12 meses (2025-10-08 → 2026-10-08); 24 por $203 598 554 en total desde 2018 (SECOP I: 9 por $46 030 000; SECOP II: 15 por $157 568 554). Principales contratantes: Gobernación del Quindío ($49 327 500, 2020-2022), CRQ ($46 700 000, 2018-2026), Indeportes Quindío ($41 850 000, 2024-2026), Empresas Públicas de Armenia ($18 480 000) y RAP Eje Cafetero ($16 000 000). **Son entidades que el medio cubre**: Indeportes es un instituto del departamento que gobierna Juan Miguel Galvis, y la CRQ es la autoridad ambiental del Quindío. De la cifra total, $32 650 000 son pauta del medio (2018-2021) y $170 948 554, servicios profesionales personales del titular. Hay además un contrato de pauta con la Alcaldía de Armenia (2019-04-30, $12 000 000, SECOP I constancia 19-13-9321865) a nombre de la misma persona, con un documento que difiere en dos dígitos: no se suma.
4. **«No publica absolutamente nada sobre sí mismo» / «La ausencia es total»** pasa a «Publica Términos de Servicio (2025-08-29), Política de privacidad (2025-04-01) y Contáctenos, enlazados desde su `page-sitemap.xml`, no desde las rutas habituales. Se declara "medio de comunicación digital independiente" y que "la contratación de publicidad no condiciona ni afecta la independencia editorial"». Dirección y teléfono, con fuente. El aviso del catch-all se conserva y se actualiza a 122 161 bytes.
5. **«Ni sección de opinión identificable»** pasa a «Tiene categorías de opinión y de columnistas (Oliver Gómez Solarte, Jota Domínguez Giraldo, Pablo Jaramillo). La última columna firmada es de marzo de 2025 ("Finito", archivada bajo Gómez Solarte), fuera de la ventana del presente».
6. **«Lo que falta»**:
   - quitar «Cualquier nombre propio» y «La razón social»;
   - mantener la consulta de la marca en la SIC;
   - añadir la matrícula mercantil en el RUES / Cámara de Comercio de Armenia como persona natural comerciante, y el barrido de 90 días.

En `shared/mediaOwnership.js`, entrada `quindio-noticias`:

7. `ownerType` pasa a persona natural, con el titular y la fuente de la constancia, **sin número de documento**. Hay que quitar de `notes` «ni dirección, ni teléfono» y «NO PUBLICA ABSOLUTAMENTE NADA».
8. En `buscadoEn`, añadir SECOP I (`f789-7hwg`) y SECOP II (`jbjy-vk9h`) con el resultado de (b)3, y el `page-sitemap.xml`. `consultadoEl` pasa a 2026-10-08.
9. En `sources`, añadir la URL de la constancia 21-4-12596549, la de Términos y la de Privacidad.

En `shared/mediaRegistry.js`:

10. `biasRationale`: quitar «No publica absolutamente nada sobre sí mismo: ni sociedad, ni nombres, ni cargos» y poner «Opera como persona natural (Daniel Andrés Hincapié Ramírez, según SECOP), contratista de entidades del Quindío. Orientación mixta provisional por Regla 2: 38 días de corpus».

**(c) Tensiones a declarar**
1. **El titular es contratista de entidades que el medio cubre.** Firmó $39 100 000 en 12 meses con la CRQ e Indeportes, y antes trabajó en la Tesorería de la Gobernación (2020-2022). Es desvelamiento, no acusación, y no mueve el número.
2. **Trato asimétrico en titulares, junio-octubre de 2026.**
   - Escándalo para el gobierno saliente.
   - Celebración para el presidente De la Espriella, ya desde que era electo.
   - Elogio uniforme al gobernador Galvis, y la oposición de los alcaldes encuadrada contra ellos (2026-09-25).
   - Ningún titular crítico con el presidente ni con el gobernador en la ventana.
   - Sin medir en cuerpos, con el terremoto de por medio y con piezas que parecen boletines. Si se sostiene en 90 días de corpus, es la evidencia de polo fijo que movería el número a la derecha.
3. **Spam de casinos, confirmado.**
   - 19 entradas en idiomas extranjeros en la ventana, de la cuenta «Editora QN» y de la categoría local principal. La portada del 2026-10-08 enlaza 17.
   - Sin identificar como publicidad, contra lo que dicen los propios Términos.
   - Afecta a la fiabilidad del medio y puede contaminar el corpus. Hay que comprobar si entran por el feed y, en ese caso, excluirlas antes de medir la agenda propia.
4. **El corpus no ve todo lo que publica**: 496 artículos medidos frente a 605 publicados. Antes de usar el 58 % de agenda propia hay que conciliar esa diferencia.
