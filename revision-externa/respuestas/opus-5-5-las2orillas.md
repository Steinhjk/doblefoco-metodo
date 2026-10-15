# Respuesta — Claude Opus 5.5 sobre Las2Orillas

| | |
|---|---|
| **Modelo** | Claude Opus 5.5 |
| **Versión exacta** | `claude-opus-5-5` |
| **Fecha de la consulta** | 2026-10-10 |
| **Quién la hizo** | Claude Code, a petición del responsable editorial (ciclo 2, fase 2, tanda 9; revisor de la misma casa que el autor de las fichas, ver DECISIONES.md 2026-10-07) |
| **¿Tuvo acceso a la red?** | sí |

> **Se pega LITERAL lo que devolvió el modelo, sin editar ni resumir.** Si se
> recorta, se pierde justo lo que pueda incomodar. Los comentarios nuestros van
> al final, en la sección de resolución, claramente separados.
>
> **No ha hecho falta ninguna edición.** El revisor no copió cédulas,
> teléfonos ni direcciones, y sus dos consultas a datos.gov.co ya llevan
> `$select` con campos que no devuelven documentos de identidad (comprobado).
> Los procesos de SECOP II y las constancias de SECOP I los cita como texto.

---

## RESPUESTA LITERAL

```
REVISIÓN EXTERNA — Las2Orillas — ciclo 2 (tanda 9)
Revisor: Claude Opus 5.5 (claude-opus-5-5), Anthropic. Fecha de la revisión: 2026-10-10.

DECLARACIÓN PREVIA DE CONFLICTO
Soy un modelo de Anthropic, la misma casa del modelo que redactó la ficha. Mi acuerdo con la ficha no vale como aval independiente. Para compensarlo he trabajado casi solo con fuentes que la ficha NO usa: SECOP II, SECOP I y RUES en datos.gov.co, y la API pública de WordPress de las2orillas.co (autor, categoría y fecha de cada pieza). La ficha cita una única fuente, «Quiénes somos», y la releí también. Las clasificaciones de postura de las piezas son juicio mío. Las dejo listadas para que otra persona pueda rehacerlas y discrepar.

MÉTODO Y DÓNDE BUSQUÉ
- robots.txt de las2orillas.co (2026-10-10): solo «Disallow: /wp-admin/» para «User-agent: *». No excluye a ClaudeBot, Claude-Web ni anthropic-ai, así que descargué. robots.txt de datos.gov.co: «User-agent: *», «Crawl-delay: 1» y prohibiciones solo en /browse, /page, /catalog. /resource no está prohibido y no se menciona a ningún agente de IA.
- Todo se descargó con curl -sL y UA de navegador (--ssl-no-revoke) y se citó desde el HTML o JSON crudo. Los archivos están en t89\las2orillas-dl.
- Páginas del medio: https://www.las2orillas.co/quienes-somos/ y unas 25 piezas sueltas (URL en cada cita).
- API del medio: /wp-json/wp/v2/posts filtrada por categoría Poder (id 142) desde 2025-10-10. Son 693 piezas, todas descargadas con título, autor y fecha. También usé búsquedas «Espriella» desde 2026-08-07 (361 resultados, revisé los 200 primeros) y «Registraduría» entre 2025-12-01 y 2026-08-01 (98 resultados, todos). Miré además la categoría Opinión (id 129): 913 piezas en 12 meses, revisé las 100 más recientes. Y busqué categorías y etiquetas «editorial».
- Identidad de autor: el id 457 y el id 2 publican como «Las Dos Orillas» (<meta name="author" content="Las Dos Orillas"/>, ruta /author/l2oadm/ y /author/2orillas/), y la pieza lleva «Por Las Dos Orillas». Esa es la VOZ DE LA CASA. Otros ids son periodistas de plantilla con firma (Elisa Pastrana, Adriana Arcila, Mauricio Cárdenas, Daniel Murcia, Jorge González, Andrés Felipe Páez…) o columnistas. A esos los separé.
- Contratación: SECOP II (jbjy-vk9h) y SECOP I (f789-7hwg) por NIT con igualdad exacta: 900615503 (sin DV) y 9006155038 (con el DV pegado). RUES (c82u-588k) igual.
- Buscador web: DISPONIBLE. Hice una sola consulta («Las2orillas María Elvira Bonilla 2026 Registraduría contrato»), excluyendo los dominios vetados. No apareció cobertura de terceros sobre los contratos con la Registraduría ni sobre cambios de propiedad. No hubo antibots.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré nada de eso. Es una ESAL (fundación) y no tiene acciones que vender. RUES, consultado el 2026-10-10:
  https://www.datos.gov.co/resource/c82u-588k.json?$select=camara_comercio,matricula,razon_social,numero_identificacion,fecha_matricula,ultimo_ano_renovado,estado_matricula,organizacion_juridica,fecha_actualizacion&numero_identificacion=900615503
  Respuesta literal: «"camara_comercio":"BOGOTA","matricula":"90044286","razon_social":"FUNDACION LAS DOS ORILLAS","fecha_matricula":"20130419","ultimo_ano_renovado":"2026","estado_matricula":"ACTIVA","organizacion_juridica":"LAS DEMÁS ORGANIZACIONES CIVILES,CORPORACIONES,FUNDACIONES","fecha_actualizacion":"2026/04/24 …"». Con el DV pegado (9006155038) da [] (vacío).
- La titular y directora que nombra la ficha (María Elvira Bonilla), ¿sigue viva y en el cargo?
  Sí, según el propio medio. «Quiénes somos» (consultado el 2026-10-10) dice: «fundadora - DIRECTORA María Elvira Bonilla». La pieza de la casa del 2026-09-11 (https://www.las2orillas.co/las2orillas-en-el-top-5-de-los-portales-nativos-elegidos-por-los-lideres-de-opinion-para-informarse/) dice: «desde su fundación ha estado dirigido por la veterana periodista María Elvira Bonilla». Es una declaración del propio medio. No encontré ningún registro externo de su cargo.
  Nota: la lista «Fundadores & Asociados» de «Quiénes somos» incluye hoy a «Margarita Londoño (Q.E.P.D.)» y a «Martha Cecilia Ruíz Naranjo (r)». La ficha no nombra a ninguna de las dos, así que no hay error, pero la lista mezcla a vivos, fallecidos y retirados.
- ¿Quién dirige hoy la redacción?
  María Elvira Bonilla como directora. La editora de opinión es Elisa Pastrana («fuNDADORA - EDITORA DE OPINIÓN Elisa Pastrana», Quiénes somos, 2026-10-10). No encontré un jefe de redacción distinto.
- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que cita la ficha?
  Sí: el RUES de arriba, renovado en 2026 y actualizado el 2026-04-24. Confirma el NIT y que la entidad está activa. No da composición del consejo ni de los asociados. No encontré estados financieros publicados.

## OBJECIONES

### Objeción 1 — La financiación no es un hueco: hay contratación pública de 2025-2026 y pauta declarada
- QUÉ afirma la ficha: «LA FINANCIACIÓN NO ESTÁ DOCUMENTADA. Su "Quiénes somos" declara la figura jurídica y el NIT, pero no de dónde salen los ingresos. Es un hueco de nivel 1».
- POR QUÉ es incorrecto:
  (a) SECOP II, por NIT 900615503 con igualdad exacta (con DV 9006155038 da []). Consultado el 2026-10-10:
  https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=nombre_entidad,proveedor_adjudicado,valor_del_contrato,fecha_de_firma,objeto_del_contrato,id_contrato&documento_proveedor=900615503
  Aparecen tres contratos, todos con «nombre_entidad":"RNEC"» (Registraduría Nacional del Estado Civil):
   · CO1.PCCNTR.8682255. Firmado el 2025-12-09, «valor_del_contrato":"500000000"». Objeto literal: «Contratar los servicios de diseño e implementación de la estrategia integral de medios que incluya; producción; ejecución; divulgación y promoción de las piezas de comunicación del proceso de inscripción de cédulas y de las elecciones de Congreso de la República y Presidencia a llevarse a cabo en las vigencias 2025 y 2026». Otros campos, con $select=id_contrato,modalidad_de_contratacion,estado_contrato,fecha_de_inicio_del_contrato,fecha_de_fin_del_contrato,valor_pagado: «"Contratación directa"», «"En ejecución"», inicio 2025-12-10, fin 2026-07-30, «"valor_pagado":"500000000"». Proceso en SECOP II, como texto: CO1.NTC.9257181.
   · CO1.PCCNTR.8343257. Firmado el 2025-09-19, 200 000 000 COP, contratación directa, terminado el 2025-10-30. Objeto: «Prestación de servicios para la promoción; divulgación y pedagogía de las elecciones de Consejos Municipales y Locales de Juventud vigencia 2025».
   · CO1.PCCNTR.7159140. Firmado el 2024-12-20, 11 900 000 COP. Objeto: «divulgación de la audiencia de rendición de cuentas 2024 de la Registraduria Nacional del Estado Civil; en el Portal Las2Orillas».
  En los últimos 12 meses entran el contrato de 500 millones completo y la ejecución del de 200 millones (hasta el 2025-10-30). La búsqueda por nombre («%DOS ORILLAS%», «%LAS2ORILLAS%») no añade ningún otro contrato.
  (b) SECOP I (f789-7hwg), mismo NIT, igualdad exacta. Con DV da []. Hay siete contratos de 2018-2020: Telemedellín (cinco, de «PUBLICACIoN DE PAUTA PUBLICITARIA EN EL SITIO WEB LAS DOS ORILLAS»), Telepacífico (2020-11-24, 20 000 000) y Cámara de Comercio de Medellín (2020-12-01, 3 570 000). Constancias como texto: 18-12-8299188, 18-4-7634293, 19-4-9075709, 19-4-10035807, 20-4-10738044, 20-4-11356543, 20-4-11376562. Son historia y no cuentan por sí solos, pero muestran que la pauta pública es una fuente de ingresos recurrente.
  (c) «Quiénes somos» (2026-10-10) sí declara la pauta como fuente: «Pauta […] Resultados Más de 50 marcas, entre ellas: agencias de medios, marcas comerciales y entidades confían en nuestros resultados». El menú del sitio tiene además una sección «EDICTOS». Hecho: existe esa sección. Inferencia: es ingreso por avisos legales.
- FUENTE Y FECHA: las URL de arriba, consultadas el 2026-10-10. Contratos firmados el 2024-12-20, 2025-09-19 y 2025-12-09.
- NIVEL: registro externo (contratación pública) y declaración del propio medio.
- Qué cambia: la ficha debe pasar de «no documentada» a «pauta comercial y pública declarada; en 12 meses, al menos 500 millones COP pagados por la Registraduría en contratación directa». No tiene dirección izquierda-derecha. La Registraduría es un órgano autónomo y no el Gobierno. Pero es un conflicto de interés que la ficha no tiene (ver Objeción 2).

### Objeción 2 — Conflicto de interés no declarado: cobertura laudatoria de la Registraduría durante el contrato, sin etiqueta de patrocinio
- QUÉ omite la ficha: el medio cubrió las elecciones de 2026 mientras cobraba a la autoridad electoral por «producción; ejecución; divulgación y promoción de las piezas de comunicación» de esas mismas elecciones.
- EVIDENCIA (hecho): entre el 2025-12-10 (un día después de la firma) y el 2026-05-26 hay 16 piezas firmadas por «Las Dos Orillas» o por plantilla, con «Registraduría», «registrador» o «Penagos» en el título. Todas están en las categorías Actualidad, Célula Actualidad o Poder. Ninguna está en «Contenido Patrocinado» (id 236066, «count":0» según /wp-json/wp/v2/categories) ni en «Contenido Invitado». En las cuatro que descargué, la cadena «Contenido Invitado» solo aparece en el CSS del menú, y no hay «patrocinado», «publirreportaje» ni «en alianza con».
   2025-12-10 https://www.las2orillas.co/la-estrategia-con-la-que-la-registraduria-quiere-que-el-voto-en-el-exterior-incline-la-balanza-de-las-elecciones-en-2026/
   2025-12-12 https://www.las2orillas.co/asi-ha-modernizado-la-registraduria-sus-operaciones-en-el-pais-de-cara-a-las-elecciones-2026/. Cita: «La Registraduría Nacional llegó al cierre de 2025 con la sensación de haber avanzado más de lo previsto […] un trabajo constante por recuperar la confianza […] la entidad que dirige Hernán Penagos se movió entre retos logísticos […] con resultados visibles». Firma: «Por Las Dos Orillas».
   2025-12-26 https://www.las2orillas.co/la-registraduria-se-toma-transmilenio-entre-portales-y-estaciones-busca-facilitar-el-voto-en-bogota/
   2026-01-21 https://www.las2orillas.co/asi-reviso-la-registraduria-las-31-millones-de-firmas-que-entregaron-los-candidatos-a-presidente-y-40-fueron-anuladas/
   2026-01-22 https://www.las2orillas.co/la-estrategia-de-la-registraduria-para-mantener-en-secreto-el-voto-de-los-colombianos-en-las-consultas-presidenciales/
   2026-02-06 https://www.las2orillas.co/asi-garantizara-la-registraduria-cada-voto-en-las-proximas-elecciones-ante-las-amenazas-de-fraude-y-violencia-en-el-pais/
   2026-02-13 https://www.las2orillas.co/la-registraduria-pone-a-prueba-el-sistema-electoral-asi-avanzan-los-simulacros-rumbo-al-congreso-2026/
   2026-02-13 https://www.las2orillas.co/el-plan-de-la-registraduria-para-que-la-tragedia-en-cordoba-no-frene-las-elecciones-este-8-de-marzo/
   2026-02-17 https://www.las2orillas.co/la-nueva-apuesta-digital-de-la-registraduria-para-resolver-dudas-electorales-desde-el-celular/
   2026-03-08 https://www.las2orillas.co/hernan-penagos-el-caldense-que-paso-de-ser-mensajero-a-ser-el-encargado-de-dirigir-las-elecciones-2026/
   2026-04-17 https://www.las2orillas.co/asi-es-como-la-registraduria-esta-identificando-a-cientos-de-ninos-wayuu-en-la-guajira/
   2026-04-21 https://www.las2orillas.co/el-plan-del-registrador-hernan-penagos-para-acabar-con-el-fantasma-del-fraude-en-las-elecciones-presidenciales/. Cita: «el registrador ha decidido poner las cartas sobre la mesa y proponer un plan de auditorias». Firma: «Por Las Dos Orillas».
   2026-04-23 https://www.las2orillas.co/la-jugada-de-la-registraduria-para-blindar-las-elecciones-abrir-su-sistema-y-someterlo-a-auditoria-internacional/
   2026-05-06 https://www.las2orillas.co/de-la-capital-al-exterior-el-gigantesco-despliegue-logistico-de-la-registraduria-para-la-primera-vuelta/
   2026-05-26 https://www.las2orillas.co/el-plan-con-el-que-la-registraduria-busca-blindar-el-escrutinio-de-las-elecciones-presidenciales-en-colombia/
   (Fuera de la lista, el 2026-03-03 hay otra pieza de la casa sobre el escrutinio, pero su título no nombra a la Registraduría.)
  Para comparar, con el mismo método de búsqueda: entre 2025-01-01 y 2025-09-18 solo hay 3 títulos con «Registraduría», y son avisos de empleo. Esa búsqueda devuelve como máximo 100 resultados, así que el recuento puede quedarse corto. Entre 2025-09-18 y 2025-12-09 hay 4, uno de ellos una columna crítica («La Registraduría no se hace respetar», 2025-10-16). Entre 2026-07-31 y 2026-10-10 hay 2.
- INFERENCIA (la marco como tal): el aumento de piezas institucionales y de tono favorable coincide con la vigencia del contrato y con su objeto. Es verosímil que parte de ellas sean entregables pagados y se publicaran sin etiqueta. No tengo el anexo técnico del contrato para confirmarlo.
- FUENTE Y FECHA: las URL de arriba, con sus fechas de publicación, y SECOP II (Objeción 1). Todo consultado el 2026-10-10.
- NIVEL: conducta observable y registro externo.
- Qué cambia: no da dirección en el eje. La ficha debe declarar el conflicto. Es el mismo tipo de hallazgo que apareció en el caso Diario La Libertad.

### Objeción 3 — La voz de la casa no sostiene el −0,35: el barrido de 12 meses no muestra asimetría hacia la izquierda, y tras el 07-08-2026 se muestra más bien cálida con el gobierno de derecha
- QUÉ afirma la ficha: −0,35 (izquierda moderada), por «colocación relativa». La propia ficha admite que el nivel 2 dice que «se aparta, no hacia dónde».
- BARRIDO (reproducible): autor «Las Dos Orillas» (ids 457 y 2) en la categoría Poder, del 2025-10-10 al 2026-10-10 (256 de las 693 piezas de Poder). Lo completé con las piezas de la casa de Al Minuto y Actualidad que traen «Espriella» en el título después del 2026-08-07. De las 99 piezas de Poder con títulos políticos, clasifiqué la postura. Clases: FI = favorable a actor o gobierno de izquierda, o desfavorable a un actor de derecha que no gobierna. FD = lo simétrico. FISC = fiscaliza al gobierno de turno (no cuenta). N = neutral. [lead] = leí la entrada en el HTML; [título] = clasificado solo por el titular.
  ANTES del cambio (2025-10-10 → 2026-08-06):
   FI1 2025-10-27 [lead] https://www.las2orillas.co/la-batalla-mas-grande-que-ha-ganado-ivan-cepeda-no-fue-la-de-este-domingo-sino-cuando-derroto-el-cancer/
   FI2 2025-10-28 [título] https://www.las2orillas.co/dos-mujeres-los-pilares-en-la-vida-de-ivan-cepeda/
   FI3 2025-11-16 [título] https://www.las2orillas.co/la-frenada-de-petro-a-temu-y-shein-que-ayudara-a-los-confeccionistas-colombianos/
   FI4 2026-01-10 [título] https://www.las2orillas.co/dos-mujeres-le-dan-la-fuerza-a-ivan-cepeda-el-sucesor-de-petro-que-no-la-tiene-facil-con-abelardo-de-la-espriella/
   FI5 2026-05-23 [título] https://www.las2orillas.co/quien-es-el-estratega-de-paloma-valencia-senalado-de-ser-un-experto-desinformando-en-redes/
   FI6 2026-06-04 [lead] https://www.las2orillas.co/mas-de-11-billones-invertidos-desde-2022-entre-las-cifras-que-dejo-la-gestion-del-gobierno-petro-en-la-salud-colombiana/. Reproduce el informe de logros de MinSalud: «figuran entre los principales resultados que el Ministerio de Salud […] destacó en su informe de logros».
   FI7 2026-06-22 [lead] https://www.las2orillas.co/el-camino-de-ivan-cepeda-a-una-presidencia-que-se-le-escapo-por-250-mil-votos/. Cita: «aguerrido senador defensor de las victimas».
   FD1 2025-10-10 [título] https://www.las2orillas.co/la-valiente-lucha-contra-el-regimen-chavista-que-le-dio-a-maria-corina-machado-el-nobel-de-paz/
   FD2 2026-01-30 [título] https://www.las2orillas.co/la-joven-monteriana-esposa-de-abelardo-de-la-espriella-a-quien-la-vida-le-dio-un-vuelco-total/
   FD3 2026-05-31 [lead] https://www.las2orillas.co/abelardo-de-la-espriella-el-antipolitico-que-se-conecto-con-el-pais-y-gano/. Título: «el antipolítico que se conectó con el país y ganó».
   FD4 2026-06-16 [lead] https://www.las2orillas.co/el-triunfo-de-abelardo-de-la-espriella-y-jose-manuel-restrepo-en-primera-vuelta-han-despertado-confianza-internacional/. Cita: «ha dado un dado una señal positiva frente a los mercados internacionales».
   FD5 2026-06-21 [lead] https://www.las2orillas.co/el-camino-de-abelardo-de-la-espriella-para-lograr-la-presidencia-de-colombia-en-6-meses/
   FD6 2026-07-08 [título] https://www.las2orillas.co/la-primera-banda-criminal-que-se-entregara-ante-el-ultimatum-de-de-la-espriella-la-cual-tiene-azotada-a-barranquilla/
   FISC del gobierno Petro (no cuenta), por ejemplo: 2026-07-21 https://www.las2orillas.co/por-que-se-disparo-la-mineria-ilegal-en-el-gobierno-de-gustavo-petro/ (cita: «mostró la mano blanda con la que serían tratados») y 2025-11-21 «El proyecto secreto del gobierno de convertir la inteligencia financiera en instrumento de lucha política» (firmada «Unidad Investigativa Las 2 Orillas»). Hay además una docena de títulos sobre Benedetti, Alcocer, Juliana Guerrero, Roa y la Lista Clinton.
  DESPUÉS del cambio (2026-08-07 → 2026-10-10):
   FD7 2026-09-12 [título] https://www.las2orillas.co/las-2-fundaciones-a-las-que-abelardo-de-la-espriella-les-va-entregar-su-primer-salario-52-millones/
   FD8 2026-09-13 [título] https://www.las2orillas.co/el-pacto-liderado-por-cepeda-mais-por-la-investigada-peralta-y-en-marcha-por-cristo-son-la-fragil-oposicion/
   FD9 2026-09-19 [lead] https://www.las2orillas.co/la-mano-dura-de-de-la-espriella-con-120-presos-para-hacerle-la-guerra-a-la-extorsion-en-buenaventura/. Reproduce sin contrapeso la frase presidencial: «En Colombia se acabó la contemplación y la alcahuetería con la delincuencia».
   FD10 2026-09-21 [lead] https://www.las2orillas.co/adios-a-los-delincuentes-de-cuello-blanco-en-carceles-de-privilegio-12-politicos-ya-fueron-trasladados/. Título celebratorio; en el texto: «es hasta hoy el funcionario más felicitado por el presidente Abelardo De la Espriella».
   FD11 2026-10-07 [título] https://www.las2orillas.co/el-respaldo-de-ee-uu-a-de-la-espriella-ya-empieza-a-sentirse-con-poderosos-drones-militares-para-rastrear-narcos/
   FD12 2026-10-10 [lead] https://www.las2orillas.co/la-promesa-cumplida-de-de-la-espriella-reabriendo-embajada-en-jerusalen-a-donde-llega-una-gilinski/. Título: «La promesa cumplida de De la Espriella».
   FI después del cambio: no encontré ninguna en la voz de la casa.
   FISC del gobierno De la Espriella (no cuenta, pero muestra continuidad fiscalizadora):
    2026-08-26 https://www.las2orillas.co/a-excepcion-de-minhacienda-y-el-canciller-todos-los-ministros-de-de-la-espriella-llegan-endeudados/
    2026-09-02 https://www.las2orillas.co/estos-son-los-escogidos-que-el-presidente-de-la-espriella-quiere-sentar-en-la-junta-directiva-de-ecopetrol/ (cita sobre el estratega del presidente: «No es experto en energía»)
    2026-09-06 https://www.las2orillas.co/el-regreso-de-alejandro-ordonez-a-la-vida-publica-de-colombia-con-mas-poder-que-nunca-en-la-era-del-tigre/
    2026-09-17 https://www.las2orillas.co/a-la-embajada-clave-para-el-tema-de-derechos-humanos-llega-otro-de-los-abogados-de-de-la-espriella-lawyers/
    2026-09-21 https://www.las2orillas.co/el-debut-del-embajador-de-de-la-espriella-en-la-onucon-un-voto-minoritario-alineado-con-trump-contra-palestina/
   Sobre el expresidente después del cambio (no lo conté; si se contara como FD, la cuenta posterior subiría a 9): 2026-08-13 «Eva Ferrer destapa la banda…», 2026-08-27 «A quiénes puso Petro… Procolombia» y 2026-10-03 https://www.las2orillas.co/por-fin-gustavo-petro-tiene-casa-propia/.
- RECUENTO: 25 piezas con postura (umbral ≥10: se cumple). Antes del cambio: FI 7 / FD 6. Después: FI 0 / FD 6. Total: FD 12 frente a FI 7 (1,7:1). No llega al 3:1 en ninguna dirección, y antes del cambio no hay asimetría. Por tanto, NO hay nivel 2 por la regla del 2026-10-09 en ningún sentido.
- LO QUE SÍ MUESTRA (hecho e inferencia separados):
  · Hecho: en 12 meses no aparece una sola pieza de la voz de la casa con asimetría hacia la izquierda. Los perfiles cálidos de Cepeda (FI1, FI2, FI4, FI7) tienen su gemelo en los de De la Espriella (FD2, FD3, FD5). La casa no tiene sección editorial: no existe la categoría «editorial» (/wp-json/wp/v2/categories?search=editorial devuelve []), y la etiqueta «editorial» (id 185884) solo agrupa reseñas de libros. Tampoco encontré endoso en la voz de la casa.
  · Inferencia: el giro posterior al 07-08 va hacia la derecha (FD9–FD12 celebran medidas del nuevo gobierno). Pero antes del cambio la casa también trató bien al gobierno de turno (FI3, FI6). El patrón encaja más con deferencia al gobierno de turno, que la regla del polo fijo no mide, que con una línea de izquierda. Y es compatible con un medio que vive en parte de pauta pública (Objeción 1).
- NIVEL: hecho editorial de los últimos 12 meses (voz de la casa).
- Qué cambia: la única evidencia de dirección disponible contradice el signo de la ficha. Por la regla «ante la duda entre dos bandas, la más cercana a la mixta», y sin nivel 1-3 que dé dirección, el −0,35 no tiene apoyo. Como mínimo, la ficha debe declarar que la voz de la casa no lo respalda.
- LÍMITES: 13 de las 25 piezas las clasifiqué solo por el titular. La clasificación es mía y otro revisor puede discrepar pieza a pieza. No barrí Actualidad ni Al Minuto antes del 2026-08-07 con el mismo detalle: allí solo revisé los títulos de Registraduría.

### Objeción 4 (menor) — Un fundador y asociado aparece como analista en una pieza de la casa sin que se declare el vínculo
- QUÉ dice la ficha: menciona a León Valencia solo como «desvelamiento» de contexto.
- EVIDENCIA: la pieza «Qué le espera a Colombia con Abelardo De La Espriella a partir del 7 de agosto», del 2026-07-27, firmada «Por Las Dos Orillas» (https://www.las2orillas.co/que-le-espera-a-colombia-con-abelardo-de-la-espriella-a-partir-del-7-de-agosto/), es una conversación con Valencia. Lo presenta como «una de las voces más autorizadas para leer los cambios del poder en el país. Escritor, analista político y director de la Fundación Paz y Reconciliación». En el texto no aparecen «fundador», «asociado» ni «Las2orillas». Pero «Quiénes somos» lo pone en «Fundadores & Asociados».
- NIVEL: conducta observable de los últimos 12 meses. No mueve el número. Es una práctica de transparencia que la ficha debería anotar.

## LO QUE NO PUDE VERIFICAR
- Composición actual del consejo o junta de la fundación y su representante legal. El RUES abierto no trae esos campos y no pedí certificado de existencia (es de pago). No sé si los «Fundadores & Asociados» de la web coinciden con los órganos registrados.
- Que Rafael Santos «pertenece a la familia Santos» y que «fue directivo de EL TIEMPO». La ficha no da fuente y no lo busqué: no puedo afirmar parentescos por apellido, y no usé el dominio vetado. Si se mantiene, necesita una fuente propia.
- Estados financieros o informe de gestión de la ESAL. No encontré ninguno publicado en el sitio. Solo revisé «Quiénes somos» y el pie de página.
- Si las piezas sobre la Registraduría fueron entregables del contrato. Haría falta el anexo técnico o los informes de supervisión del proceso CO1.NTC.9257181 en community.secop.gov.co, que no consulté.
- La pregunta de la ficha («si el filtro de opinión ciego para 22 medios invalida el nivel 2 de todos») exige el corpus del proyecto, y no lo tengo.

## LO QUE FALTA
- Los contratos con la RNEC (Objeciones 1 y 2), declarados como financiación y como conflicto.
- La voz de la casa identificada por autor: en la API de WordPress, autor «Las Dos Orillas» (ids 457 y 2). Las categorías Opinión (id 129) y Nota Ciudadana (id 222) permiten separar la opinión de la reportería sin depender de la URL, al menos en este medio.
- Las cifras de nivel 2 de la ficha (174 artículos en 30 días, 55 historias, socios La República, Pulzo…) están superadas por las del envío (504 en 40 días, 36 historias, 75 % de agenda propia, coincide con El Espectador, Infobae y Cablenoticias). La ficha debería reescribirse con estas.
- El cambio de gobierno (De la Espriella, desde el 07-08-2026) no aparece en la ficha. Es justo la prueba que pide el protocolo.

## EVIDENCIA QUE NO MUEVE EL NÚMERO
- Sin endoso de la casa en las presidenciales de 2026: no hay categoría editorial ni piezas de la casa que pidan el voto. El único resultado de «votaremos por» es una columna de un tercero (autor 453, categoría Opinión) a favor de De la Espriella: https://www.las2orillas.co/mi-voto-no-es-por-una-paloma-mi-voto-es-por-un-ave-llamada-abelardo/ (2026-05-31).
- El grupo de columnistas es plural y critica a ambos lados después del cambio. Son terceros y pesan poco. Contra el gobierno: «La movilización del 14 de octubre no es una acción terrorista como quiere hacerla parecer el gobierno abelardista» (2026-10-07, https://www.las2orillas.co/la-movilizacion-del-14-de-octubre-no-es-una-accion-terrorista-como-quiere-hacerla-parecer-el-gobierno-abelardista/) y «¿Qué estado quiere De la Espriella?» (2026-09-22). Contra Petro: «¿Petro engañó deliberadamente a los colombianos para ganar las elecciones?» (2026-09-18, https://www.las2orillas.co/petro-engano-deliberadamente-a-los-colombianos-para-ganar-las-elecciones/) y «Petro y su reforma para quedarse con la casa…» (2026-10-10).
- Los análisis firmados por Juan Manuel Ospina en Poder (autor 18) critican a los dos gobiernos a la vez: «El MinEducación de Petro y las 2 de El Tigre padecen el mismo mal: no saben de educación y su ideología va por delante» (2026-09-30) y «Petro y De la Espriella son dos polos opuestos que se parecen en la forma de gobernar el país» (2026-10-08).
- Rectificación publicada por la casa a petición de De la Espriella Lawyers (2026-10-09, https://www.las2orillas.co/rectificacion-3/): «Es falsa la existencia de una "red de alianzas" entre Rojas Fiallo Consultores & Abogados y De la Espriella Lawyers». Es conducta de corrección y no tiene dirección.
- La fiscalización continúa a ambos lados del cambio (FISC en la Objeción 3). Bajo el polo fijo no es orientación, pero corrobora la banda mixta.
- RUES activo y renovado en 2026, y la misma directora desde 2013: no hubo cambios estructurales en 12 meses.

## SIN OBJECIÓN
No aplica: hay cuatro objeciones.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal:** ninguna. Las dos URL de datos.gov.co del revisor (RUES `c82u-588k` y SECOP II `jbjy-vk9h`) llevan `$select` con campos de la sociedad y del contrato, y se comprobó que no devuelven documentos de identidad. **Esta resolución tampoco escribe ni enlaza ningún documento de identidad:**
- las consultas que cita llevan `$select`;
- los procesos de SECOP II y las constancias de SECOP I van como texto;
- los PDF del proceso (estudio previo, cotización, informes) se nombran y no se enlazan, porque algunos traen datos personales del representante legal y del personal comercial del medio. Ninguno de esos datos pasa aquí.

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada (2026-10-10):
  - las2orillas.co: `User-agent: *`, `Disallow: /wp-admin/`, `Allow: /wp-admin/admin-ajax.php` y tres sitemaps. No nombra a ningún agente de Anthropic. El revisor omite el `Allow` y los sitemaps, que no cambian nada.
  - datos.gov.co: `Crawl-delay: 1` y exclusiones de `/browse` y `/page`. Se usó solo `/resource`, con más de un segundo entre consultas.
  - community.secop.gov.co: `/robots.txt` responde 404. La ficha del proceso pide captcha. Los documentos se bajaron por el enlace de descarga que publica el dataset abierto `dmgg-8hin`, sin captcha.
  - No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex. **No hubo buscador web.**
- **Sitio**, en crudo con `curl -sL --ssl-no-revoke -A "Mozilla/5.0 … Chrome/126.0 Safari/537.36"`, con 3 a 4 segundos entre peticiones:
  - «Quiénes somos»;
  - la pieza del 2026-09-11 del «Top 5»;
  - las 36 piezas sobre la Registraduría (las 32 entregables de los dos contratos y las 4 del revisor que no lo son);
  - **las 469 piezas del barrido de la voz de la casa**, una por una;
  - y la API de WordPress: `posts` por categoría y por búsqueda, `categories` y `tags`.
- **Registros** (datos.gov.co, 2026-10-10):
  - RUES (`c82u-588k`) por `numero_identificacion` = `900615503` y `9006155038`.
  - SECOP II contratos (`jbjy-vk9h`) por `documento_proveedor` = `900615503` y `9006155038`, y por `proveedor_adjudicado like '%DOS ORILLAS%' / '%2ORILLAS%' / '%2 ORILLAS%'`.
  - SECOP II procesos (`p6dx-8zbt`) por `id_del_portafolio`.
  - SECOP II archivos (`dmgg-8hin`) por `proceso`.
  - SECOP I (`f789-7hwg`) por `identificacion_del_contratista` = `900615503` y `9006155038`, y por razón social.
- **Documentos del proceso de 500 M** (CO1.BDOS.9227867), leídos enteros:
  - el estudio previo («3.1GCFL04EstudisoPrevios.pdf», 15 páginas);
  - la cotización del medio («7.2Cotizacion.pdf»);
  - los cuatro informes de actividades y de pago;
  - el informe final («informe_final_cto092_2025_LASDOSORILLAS.pdf»).
- **Documentos del proceso de 200 M** (CO1.BDOS.8778903): la propuesta («9. Propuesta Alianza informativa REGISTRADURÍA.pdf») y el informe de actividades («INFORME_ACTIVIDADES_CTO063_2025_LASDOSORILLAS.pdf»).
- **Repositorio:**
  - el envío;
  - `fichas/las2orillas.md`;
  - las entradas de `shared/mediaRegistry.js` y `shared/mediaOwnership.js`;
  - `shared/centinela.js`, donde el medio no está;
  - las menciones en otras fichas;
  - el protocolo;
  - DECISIONES.md del 2026-10-07 al 2026-10-10 y la entrada de RTVC del 2026-08-08;
  - `LOG_IMPLEMENTACIONES.md` y `CONTEXTO_ALGORITMO_SESGO.md` (la exclusión del 2026-07-30);
  - y el historial de git del valor (commit `3296b22`).
- **El barrido**, reproducible, está en `revision-externa/barridos/las2orillas.md`.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | La financiación no es un hueco: 3 contratos directos con la Registraduría (500 M, 200 M y 11,9 M), 7 de SECOP I y pauta declarada en «Quiénes somos» | sí | sí | **Aceptada.** Los tres contratos, los siete registros de SECOP I y la cita de «Quiénes somos» coinciden, literal. **Una corrección de forma:** el revisor escribe «pagado entero». SECOP II trae `valor_pagado` igual al valor en los contratos de 500 M y de 200 M, pero el protocolo pide «contratado», y así va en la línea propuesta |
| 2 | Conflicto no declarado: 16 piezas laudatorias sobre la Registraduría durante el contrato, sin rótulo; que sean entregables es inferencia | sí | sí, con los documentos del proceso | **Aceptada, y deja de ser inferencia.** El objeto incluye «producción; ejecución; divulgación». El estudio previo encarga «la divulgación a través de sus medios» y obliga a entregar los guiones y borradores «para la aprobación» de la Oficina de Comunicaciones de la Registraduría. La cotización vende 24 «super Artículo web» descritos como «Artículo patrocinado» que «Se etiqueta como #AliadoComercial o #Publicidad». Los informes al supervisor listan **25 piezas publicadas** como entregables del contrato de 500 M (más 7 del de 200 M, vendidas como «contenido orgánico»). **Ninguna de las 32 lleva rótulo.** Es **pauta informativa pagada no declarada**, como en Ecos del Combeima. **Correcciones:** su lista tiene 15 piezas, no 16. De ellas, 11 son entregables y 4 no constan en los informes |
| 3 | La voz de la casa no sostiene el −0,35: 25 piezas con postura (7 a la izquierda y 12 a la derecha), 1,7:1, sin nivel 2; propone la banda mixta | sí | sí, pieza por pieza y ampliado | **Aceptada en la conclusión; el recuento se rehace.** Su lista tiene **19 piezas, no 25**, y marca 10 como clasificadas por el título, no 13. Su universo es asimétrico: añadió piezas de fuera de Poder solo después del cambio. Con el universo simétrico (469 piezas) y los cuerpos leídos, salen **23 con postura: 9 a la izquierda (todas antes del 07-08, 1 plena) y 14 a la derecha (5 antes y 9 después, todas leves)**, una proporción de 1,6:1. **No hay nivel 2 en ninguna dirección**, y la única asimetría va contra el signo vigente. **De sus 19, 10 no cuentan:** su FD4 es texto de la campaña de De la Espriella; su FI6, un comunicado de MinSalud; su FD1, internacional; y siete más son mixtas, descriptivas o investigan una candidatura |
| 4 (menor) | León Valencia, fundador y asociado, aparece como analista el 27-07-2026 sin que se declare el vínculo | sí | sí | **Aceptada y ampliada.** La cita es literal y la pieza no dice «fundador», «asociado» ni «Las2Orillas». **Añadido:** dos piezas de la casa (07-03 y 08-03-2026) basan sus listas de candidatos cuestionados en datos de la Fundación Paz y Reconciliación, que él dirige, sin declararlo |

### Lo verificado, objeción por objeción

**Nivel 1 (qué cambió este año).**
- **RUES**, consulta `https://www.datos.gov.co/resource/c82u-588k.json?$select=camara_comercio,matricula,razon_social,fecha_matricula,ultimo_ano_renovado,estado_matricula,organizacion_juridica,fecha_actualizacion&numero_identificacion=900615503` (2026-10-10). Devuelve, literal: «"camara_comercio":"BOGOTA"», «"matricula":"90044286"», «"razon_social":"FUNDACION LAS DOS ORILLAS"», «"fecha_matricula":"20130419"», «"ultimo_ano_renovado":"2026"», «"estado_matricula":"ACTIVA"», «"organizacion_juridica":"LAS DEMÁS ORGANIZACIONES CIVILES,CORPORACIONES,FUNDACIONES"», «"fecha_actualizacion":"2026/04/24 12:36:44.680000000"». Con el DV pegado (`9006155038`), `[]`. **Exacto, como dice el revisor.**
- **«Quiénes somos»** (2026-10-10), literal:
  - «fundadora - DIRECTORA María Elvira Bonilla»;
  - «fuNDADORA - EDITORA DE OPINIÓN Elisa Pastrana»;
  - «Fundadores & Asociados María Elvira Bonilla, León Valencia, Jorge Enrique Botero, Martha Cecilia Ruíz Naranjo (r), Natalia Orozco, Adriana Arcila, Ricardo Correa, Sergio Álvarez Guarín, Adriana Mejía Londoño, Fernando Otoya, Margarita Londoño (Q.E.P.D.), Rafael Santos, Elisa Pastrana»;
  - «Está conformado como una fundación sin ánimo de lucro, a través de la Fundación Las Dos Orillas, NIT 900.615.503-8».

  Son 13 nombres, como dice la ficha, y la lista incluye a una persona fallecida y a una retirada.
- **La pieza del 2026-09-11** (cuenta 456, «Las2orillas.»): «desde su fundación ha estado dirigido por la veterana periodista María Elvira Bonilla.» **Literal.**
- **Sin cambio de dueño ni de dirección en 12 meses.** Es una ESAL, sin acciones. Lo que cambia la ficha es la financiación (objeción 1).
- **Fecha de fundación.** El estudio previo de la Registraduría dice «Fundada el 25 de mayo de 2011». La matrícula es del 19-04-2013, y la ficha dice 2013. Es efeméride y no pesa. Se deja «matriculada en 2013 (RUES)».

**1 · Contratación pública.**
- **SECOP II**, `https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=id_contrato,nombre_entidad,proveedor_adjudicado,valor_del_contrato,fecha_de_firma,fecha_de_inicio_del_contrato,fecha_de_fin_del_contrato,modalidad_de_contratacion,objeto_del_contrato&documento_proveedor=900615503` (2026-10-10). Tres contratos, los tres con «"nombre_entidad":"RNEC"», «FUNDACION LAS DOS ORILLAS» y «Contratación directa»:
  - **CO1.PCCNTR.8682255** (proceso CO1.BDOS.9227867; aviso CO1.NTC.9257181; «CTO DE PRESTACIÓN DE SERVICIOS No. 092 DE 2025»). Firmado el 2025-12-09, $500.000.000, del 2025-12-10 al 2026-07-30. Estado «En ejecución», aunque el acta de recibo a satisfacción se cargó el 2026-08-03. El objeto, literal, como lo cita el revisor. Categoría UNSPSC del proceso: V1.82101603, que el estudio previo nombra como «Publicidad en internet».
  - **CO1.PCCNTR.8343257** (CO1.BDOS.8778903; «No. 063 de 2025»). Firmado el 2025-09-19, $200.000.000, terminado el 2025-10-30. Objeto: «Prestación de servicios para la promoción; divulgación y pedagogía de las elecciones de Consejos Municipales y Locales de Juventud vigencia 2025…».
  - **CO1.PCCNTR.7159140** (CO1.BDOS.7205512; «CD-RNEC-057-2024»). Firmado el 2024-12-20, $11.900.000. Objeto: «…divulgación de la audiencia de rendición de cuentas 2024 de la Registraduria Nacional del Estado Civil; en el Portal Las2Orillas…».

  Con el DV pegado, 0 filas. Por razón social, los mismos tres. **Exacto.** Justificación de la contratación directa, en el estudio previo: «es titular de la marca mixta "Las2Orillas"… no existe pluralidad de oferentes».
- **SECOP I**, `https://www.datos.gov.co/resource/f789-7hwg.json?$select=numero_de_constancia,nombre_entidad,fecha_de_firma_del_contrato,cuantia_contrato,detalle_del_objeto_a_contratar&identificacion_del_contratista=900615503`. Siete registros, con las mismas constancias que da el revisor:
  - Telemedellín, cinco: 18-4-7634293 ($30.000.000, 2018-01-23), 18-12-8299188 ($29.780.000, 2018-08-02), 19-4-9075709 ($38.000.000, 2019-02-21), 19-4-10035807 ($7.500.000, 2019-10-18) y 20-4-10738044 ($16.600.000, 2020-04-27), todas de «PUBLICACIoN DE PAUTA PUBLICITARIA EN EL SITIO WEB LAS DOS ORILLAS Y SUS REDES SOCIALES»;
  - Telepacífico, 20-4-11356543 ($20.000.000, 2020-11-24, «CONTRATAR LA PUBLICACIoN DE CONTENIDOS ENFOCADOS A TEMAS DE TURISMO…»);
  - Cámara de Comercio de Medellín, 20-4-11376562 ($3.570.000, 2020-12-01).

  Con el DV, 0. **Exacto.**
- **Totales (los calcula este verificador):**
  - 12 meses (2025-10-10 → 2026-10-10): **1 contrato, $500.000.000**. El de 200 M se firmó el 2025-09-19, fuera de la ventana, aunque se ejecutó hasta el 30-10.
  - Desde 2018: **10 contratos, $857.350.000**. RNEC $711.900.000; Telemedellín $121.880.000; Telepacífico $20.000.000; Cámara de Comercio de Medellín $3.570.000.
- **Pauta declarada.** «Quiénes somos», literal: «Pauta Influencia […] Resultados Más de 50 marcas, entre ellas: agencias de medios, marcas comerciales y entidades confían en nuestros resultados». **Exacto.** Dato añadido, de la cotización del propio medio: sus servicios de publicidad están excluidos del IVA «al tratarse de un medio de comunicación cuyas ventas anuales por concepto de publicidad no superaron las 180.000 UVT al 31 de diciembre del año inmediatamente anterior». Es el único dato de tamaño de ingresos que publica, y es una cota.

**2 · Lo que compró la Registraduría, en sus propios documentos.**
- **Estudio previo del contrato de 500 M** (proceso CO1.BDOS.9227867, archivo «3.1GCFL04EstudisoPrevios.pdf», cargado el 2025-12-04; consulta del listado de archivos sin datos personales: `https://www.datos.gov.co/resource/dmgg-8hin.json?$select=proceso,nombre_archivo,fecha_carga&$where=proceso%20in('CO1.BDOS.9227867','CO1.BDOS.8778903')&$limit=200`). Literal:
  - 2.6, Especificaciones técnicas: «Realizar con FUNDACION LAS DOS ORILLAS. la divulgación a través de sus medios de acuerdo con las siguientes especificaciones técnicas».
  - 2.7, obligación 8: «Proporcionar los guiones, libretos y demás borradores para la aprobación por parte de la Oficina de Comunicaciones y Prensa».
  - 2.7, obligación 10: «Entregar al supervisor del contrato evidencia de las producciones y demás material de piezas realizadas en virtud del contrato».
  - 2.8: «Todo diseño, plano, dibujo, pieza […] creado y/o entregado en cumplimiento del contrato será propiedad de la RNEC».
  - V, sobre el contratista: «una plataforma integral de comunicación que involucra medios digitales, redes sociales y contenidos noticiosos».
- **Cotización del medio** («7.2Cotizacion.pdf», «PROPUESTA DE COMUNICACIÓN 360°», del 28/11/2025). Literal:
  - «24 super Artículo web (1+) incluye post», línea «SOLUCIONES_PERIODISTICAS», «$ 8.500.000» la unidad y «$ 204.000.000» en total, sobre un subtotal de «$ 500.000.000»;
  - y en los términos del producto: «Artículo patrocinado entre 500-600 palabras […] Se etiqueta como #AliadoComercial o #Publicidad», «Redacción original», «Envía brief, titular y subtítulo propuestos».

  **El propio medio prometía rotularlos.**
- **Informes al supervisor** («informe_actividades_pago1…», «…pago2…», «…pago3…», «informe_pago4…» e «informe_final_cto092_2025_LASDOSORILLAS.pdf»). Cabecera literal: «Las2orillas / Registraduría Nacional del Estado Civil / Campaña: Voto de confianza».
  - Reportan «5 Artículos + 2 bonificados» en diciembre, 7 en enero y febrero, 6 en marzo y abril, y 7 en el último informe.
  - Cada artículo va con su URL de las2orillas.co y sus métricas de alcance.
  - **Se identifican 25 URL distintas**, publicadas del 2025-12-10 al 2026-07-25: 15 con la firma «Las Dos Orillas» y 10 con la de periodistas de plantilla (Páez, González, Moreno y Murcia).
- **Contrato de 200 M.** Propuesta del 27-08-2025, campaña «Grandes por elección». Literal: «Solución periodística de contenido orgánico (8 artículos): […] Un periodista de amplia trayectoria y credibilidad desarrollará un (1) artículo semanal», «8 artículos orgánicos que formaran parte del contenido web». Su informe se titula «Informe de pauta» y reporta «8 Artículos + 2 bonificados». **Se identifican 7 URL**, del 26-09 al 19-10-2025, las 7 con la firma «Las Dos Orillas».
- **Ninguna de las 32 piezas lleva rótulo.** Se buscó en su HTML: «AliadoComercial», «#Publicidad», «patrocinad», «publirreportaje», «Contenido Patrocinado» y «en alianza con». Solo aparecen dos falsos positivos en el perfil de Penagos, que no es entregable («patrocinado por una discoteca» y «en alianza con el uribismo»). La categoría «Contenido Patrocinado» existe (id 236066) con «"count":0». La búsqueda `search=AliadoComercial` devuelve `[]`. Las 32 están en Actualidad, Célula Actualidad, Al Minuto o Poder.
- **Las 15 del revisor** (escribe «16»): 11 son entregables. Las otras 4 no constan en los informes: Transmilenio (26-12), firmas (21-01), el perfil de Penagos (08-03) y los niños wayuu (17-04). Que esas cuatro sean pagadas no consta.
- **Contrapeso que el revisor no cita.** El 20-03-2026, en plena vigencia del contrato, una pieza de la casa que **no** es entregable respalda la duda del presidente Petro sobre el preconteo frente a la Registraduría: «esa cifra no responde la pregunta que realmente importa». La casa no fue uniformemente laudatoria con su cliente.
- **Comparación de títulos con «Registraduría»** (búsqueda de la API, todos los autores): 3 del 01-01 al 18-09-2025; 4 del 18-09 al 09-12; 17 del 09-12-2025 al 31-07-2026; 2 del 31-07 al 10-10-2026. Coincide con el revisor. Su aviso de que la búsqueda tiene un tope de 100 resultados no aplica: la primera ventana trae 45 en total.
- **Lectura.** El objeto, el estudio previo, la cotización y los informes dicen lo mismo. La Registraduría compró **espacio informativo** en el medio: artículos redactados por el medio, presentados como periodismo, con borradores sometidos a la aprobación de la entidad y que el propio medio prometía rotular. Se publicaron sin rótulo, con la firma de la casa o de su plantilla. Es el caso de la línea que DECISIONES.md (2026-10-10, Ecos del Combeima) traza entre la publicidad institucional y un medio «cuyo espacio informativo se vende». **No es evidencia del eje:** la Registraduría es un órgano autónomo y no un gobierno de un signo. Es una **tensión fuerte de independencia y de transparencia** con el árbitro de las elecciones que el medio cubría.
- **Lo que no consta:** que la Registraduría aprobara o corrigiera cada texto en concreto (las actas de reunión mensuales no se leyeron); que haya otros clientes con piezas sin rótulo, aunque «Más de 50 marcas» lo hace plausible; y que alguna de las 25 sea favorable a la entidad por encargo y no por criterio propio.

**3 · El barrido** (completo en `revision-externa/barridos/las2orillas.md`).
- **Universo:** las 257 piezas de la casa en Poder de los 12 meses, más las 212 de la casa de cualquier otra categoría cuyo título nombra a Petro, De la Espriella, Cepeda, Paloma, el gobierno o el presidente, **a los dos lados del cambio**. Total, 469: 402 antes del 07-08 y 67 después. Las 324 con política nacional en el título se leyeron por la entrada y las frases evaluativas; las 19 del revisor y las 23 que cuentan, enteras.
- **El recuento:**

| | Izquierda (plena + leve) | Derecha (plena + leve) | F, solo fiscaliza (no suma) |
|---|---|---|---|
| Antes del 07-08-2026 | 9 (1 + 8) | 5 (0 + 5) | 53 |
| Desde el 07-08-2026 | 0 | 9 (0 + 9) | 7 |
| **Total** | **9** | **14** | 60 |

- **Por destinatario:**
  - **candidatos que no gobiernan:** 4 piezas de Cepeda frente a 5 de figuras de derecha;
  - **medidas del gobierno de turno:** 5 con Petro (en 300 días) frente a 9 con De la Espriella (en 65 días).

  **La casa trata bien a quien gobierna**, a los dos lados, y fiscaliza a los dos.
- **Mínimos:** ≥10, sí (23). ≥3 por lado, solo hacia la derecha (5 y 9). ≥3:1, **no** (1,6:1). **No hay nivel 2.**
- **Exclusiones que el revisor no hizo**, porque son textos que no son de la casa, aunque lleven su firma:
  - «* Con información suministrada por la Campaña de Abelardo de la Espriella» (su FD4, 16-06-2026);
  - «* Con información del Ministerio de Salud y Protección Social» (su FI6, 04-06-2026);
  - «* Con información suministrada por Asocaña» (11-05-2026);
  - dos piezas con «Texto escrito por: …»;
  - una reimpresión de Revista Raya.

  **Que la firma de la casa sirva también para texto de campaña y para entregables pagados es un hallazgo en sí** (barrido, §5).
- **El −0,35, de dónde sale.** El commit `3296b22` (2026-08-24) lo introduce con este `biasRationale`: «su seleccion y encuadre son sostenidamente progresistas. Valor propuesto por comparacion con CasaMacondo (-0,35) y por debajo de la investigacion militante (Voragine, Cuestion Publica). SIN FIRMAR.» No cita ninguna pieza ni ningún registro. No hay entrada en DECISIONES.md que lo apruebe. La ficha lo llama «colocación relativa», y CasaMacondo salió del mapa el 2026-09-16. Antes del alta, el 2026-07-30, el medio estaba fuera precisamente porque «no tiene una línea editorial propia que clasificar».

**4 · León Valencia.** La pieza del 2026-07-27, literal: «Juan Manuel Ospina conversa con León Valencia, una de las voces más autorizadas para leer los cambios del poder en el país. Escritor, analista político y director de la Fundación Paz y Reconciliación». En el cuerpo no aparecen «fundador», «asociado» ni «Las2Orillas». **Exacto.** Una precisión: la conversación la conduce Juan Manuel Ospina, colaborador del medio, aunque la pieza va con la firma de la casa. **Añadido:** «Los 30 candidatos más cuestionados que aspiran al Senado» (07-03-2026) y «Desde las regiones 20 candidatos cuestionados…» (08-03-2026) se basan en «la Fundación Paz y Reconciliación», sin declarar el vínculo. Es desvelamiento y no mueve el número.

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se corrigen estas partes:
- **Obj. 1, «pagado entero»:** el protocolo pide «contratado» («SECOP no registra los pagos de forma fiable»). El dato `valor_pagado` existe y se puede citar como dato del registro, no como afirmación del verificador.
- **Obj. 2, «16 piezas»:** son 15 en su lista, y 11 de ellas son entregables. **«Que sean entregables es inferencia»:** ya no lo es, para 25 piezas del contrato de 500 M y 7 del de 200 M (ver arriba).
- **Obj. 3, cifras:**
  - 25 → 19 en su propia lista;
  - «13 de 25» por el título → 10;
  - el universo, asimétrico;
  - FD1 internacional, FD4 de campaña y FI6 comunicado, que no cuentan;
  - FD3 y FD5 mixtas; FI5 investiga una campaña; FI7, FD6, FD8 y FD11 descriptivas.

  Con todo corregido, la conclusión del revisor se mantiene, y con más fuerza: no hay asimetría a la izquierda, y la débil que aparece va en el sentido contrario.
- **Obj. 3, «propone banda mixta»:** se comparte, con una salvedad de reglas que el revisor no ve: «Un barrido que no llega a los mínimos no deshace nada». Ver la propuesta.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente ni cita inventada.** Todas las URL resuelven. Las citas de RUES, SECOP, «Quiénes somos» y las piezas son literales (comprobadas por programa contra el texto de cada página). Lo que hay son errores de conteo (25 por 19; 16 por 15; 13 por 10), un universo asimétrico, tres piezas contadas como voz de la casa que no lo son y una palabra que el protocolo no admite («pagado»).

**Errores de la propia ficha, para no repetirlos:**
- **«LA FINANCIACIÓN NO ESTÁ DOCUMENTADA»:**
  - el medio declara la pauta en «Quiénes somos»;
  - SECOP registra 10 contratos desde 2018;
  - el de 500 M es de los últimos 12 meses.

  Es la laguna-tipo del ciclo: una ausencia que se cae yendo al registro.
- **Sin la línea de contratación pública**, obligatoria desde el 2026-10-07.
- **El −0,35 sin una sola pieza citada** («sostenidamente progresistas»). La ficha lo admitía como «colocación relativa», pero lo mantuvo como valor con dirección.
- **Las cifras de nivel 2 (174 artículos, 55 historias, 13 socios) están superadas** por las del envío del 2026-10-10: 504 artículos en 40 días, 36 historias, 75 % de agenda propia, 9 compartidas y compañía media 0,062. Esa compañía media no puede mover ningún valor.
- **«Rafael Santos […] pertenece a la familia Santos»:** sin fuente. El protocolo no admite parentescos sin fuente (DECISIONES 2026-10-08, «lo que NO entra como hecho»). Lo que consta es solo que figura entre los fundadores y asociados.
- **«Fundado en 2013»:** la matrícula es de 2013, pero el estudio previo dice 2011. Es efeméride.
- **La cita de «Quiénes somos» en `mediaOwnership.js` no es literal.** Dice «le da la palabra a la ciudadanía»; la página dice «le damos la palabra a la ciudadanía para que publique, de primera mano, sus historias».
- **Lo que la ficha sí tenía bien:**
  - que el −0,35 no tenía evidencia de nivel 1 a 3;
  - que el nivel 2 dice que el medio «se aparta, no hacia dónde»;
  - y que el contra más serio era un defecto propio (el filtro de opinión por URL), corregido el 2026-09-15.

---

**Propuesta para la firma**

**Valor: 0,00, sin firmar, como «0,00 con evidencia» y no por defecto.**
- **Base:**
  - el −0,35 nunca tuvo evidencia de nivel 1 a 3 (commit `3296b22`; ficha del 2026-09-08);
  - el único barrido sistemático de su voz de la casa (469 piezas) no encuentra asimetría hacia la izquierda (1 pieza plena en 12 meses, 0 desde el cambio) y sí la misma conducta con los dos gobiernos (§1 del protocolo: «sostiene el 0,00 como evidencia»);
  - la regla 2 dice, literal: «El error de clasificar de más es más caro que el de clasificar de menos: acusa».
- **Alternativa literal: −0,35**, por «un barrido que no llega a los mínimos no deshace nada». Si se elige, la ficha tiene que decir que el barrido contradice el signo y que el número se sostiene solo por la regla 3.
- **Descartado: un valor positivo.** Las 9 piezas amables con el Gobierno De la Espriella son leves, caen en 65 días de luna de miel y no llegan a 3:1.
- **Firmable: no todavía.** Falta decidir el tratamiento de la pauta informativa no rotulada (decisión 2). El barrido se recuenta a los 90 días del cambio.

**Bloque propuesto para `shared/mediaRegistry.js`** (solo el `biasRationale` y el valor; no se escribe en código):

```js
        bias: 0.00, factuality: 0.80, reviewedAt: null,
        biasRationale:
            'Portal nativo digital de análisis, columna y nota ciudadana, de la Fundación Las Dos Orillas (ESAL). 0,00 CON EVIDENCIA, no por defecto: el barrido de su voz de la casa (autor «Las Dos Orillas», 469 piezas, 10-10-2025 a 10-10-2026) no encuentra asimetría hacia la izquierda — 9 piezas a la izquierda, todas antes del 07-08 y solo 1 plena, frente a 14 leves a la derecha (5 antes y 9 después), 1,6 a 1, por debajo del mínimo — y sí la misma conducta con los dos gobiernos: fiscaliza a quien manda (53 piezas con Petro, 7 con De la Espriella) y trata bien sus medidas (5 y 9). El −0,35 anterior era una colocación relativa sin evidencia. TENSIÓN FUERTE: la Registraduría le contrató 500 M en 2025-2026 para «divulgación a través de sus medios», con 25 artículos entregados y publicados sin rótulo de patrocinio (más 7 de otro contrato de 200 M en 2025). Sin firmar — ver fichas/las2orillas.md y revision-externa/barridos/las2orillas.md.',
```

**Bloque propuesto para `shared/mediaOwnership.js`** (entrada `'las2orillas'`; no se escribe en código):

```js
    'las2orillas': {
        // 2026-10-10 (ciclo 2, tanda 9): financiación documentada por SECOP
        // y por la propia página del medio. Las consultas de datos.gov.co van
        // con $select (Ley 1581): la respuesta completa trae documentos de
        // identidad de representantes legales y supervisores.
        ownerType: 'independiente',
        controlGroup: 'las2orillas-fundacion-las-dos-orillas',
        holdings: [
            'Fundación Las Dos Orillas, NIT 900.615.503-8, ESAL, matrícula 90044286 de la Cámara de Comercio de Bogotá (19-04-2013), ACTIVA, renovada en 2026 (RUES, actualizado el 24-04-2026). La figura jurídica y el NIT los declara también el medio en «Quiénes somos».',
            'Portal nativo digital de análisis, columna y periodismo ciudadano: su propia descripción dice «le damos la palabra a la ciudadanía para que publique, de primera mano, sus historias».',
        ],
        notes: [
            'NO TIENE DUEÑO ÚNICO NI GRUPO EMPRESARIAL DETRÁS: es una fundación con trece fundadores y asociados declarados (una de ellas fallecida y otra retirada, según la propia lista), entre ellos María Elvira Bonilla (fundadora y directora), Elisa Pastrana (fundadora y editora de opinión), Adriana Arcila (fundadora), León Valencia, Jorge Enrique Botero y Rafael Santos.',
            'DESVELAMIENTO, NO ACUSACIÓN: León Valencia, fundador y asociado, dirige la Fundación Paz y Reconciliación (Pares). El medio lo entrevistó como analista el 27-07-2026, y basó dos piezas sobre candidatos cuestionados (07 y 08-03-2026) en datos de Pares, sin declarar el vínculo en ninguna de las tres.',
            'FINANCIACIÓN: declara la pauta como fuente de ingresos («Más de 50 marcas, entre ellas: agencias de medios, marcas comerciales y entidades», «Quiénes somos», 10-10-2026). No publica estados financieros.',
            'Contratación pública (SECOP I y II, NIT 900615503, consultado 2026-10-10): 1 contrato por $500.000.000 contratado en los últimos 12 meses; 10 por $857.350.000 en total desde 2018. Principales contratantes: Registraduría Nacional del Estado Civil ($711.900.000, 3 contratos directos: 11,9 M el 20-12-2024, 200 M el 19-09-2025 y 500 M el 09-12-2025), Telemedellín ($121.880.000, 5, 2018-2020), Telepacífico ($20.000.000, 2020) y Cámara de Comercio de Medellín ($3.570.000, 2020). La Registraduría es la autoridad electoral cuyas elecciones el medio cubría.',
            'TENSIÓN DECLARADA — PAUTA INFORMATIVA SIN RÓTULO: el contrato de 500 M (proceso CO1.BDOS.9227867) encarga «la divulgación a través de sus medios» y la entrega de borradores «para la aprobación» de la Oficina de Comunicaciones de la Registraduría. La cotización del medio vende 24 «super Artículo web» como «Artículo patrocinado» que «Se etiqueta como #AliadoComercial o #Publicidad». Los informes al supervisor listan 25 artículos publicados del 10-12-2025 al 25-07-2026, y ninguno lleva rótulo. El contrato de 200 M (CO1.BDOS.8778903) vendió 8 artículos de «contenido orgánico» sobre las elecciones de juventud, y se identifican 7, también sin rótulo. No mueve el eje: la Registraduría es un órgano autónomo, no un gobierno de un signo.',
        ],
        sources: [
            'https://www.las2orillas.co/quienes-somos/',
            'https://www.datos.gov.co/resource/c82u-588k.json?$select=camara_comercio,matricula,razon_social,fecha_matricula,ultimo_ano_renovado,estado_matricula,organizacion_juridica,fecha_actualizacion&numero_identificacion=900615503',
            'https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=id_contrato,nombre_entidad,proveedor_adjudicado,valor_del_contrato,fecha_de_firma,fecha_de_inicio_del_contrato,fecha_de_fin_del_contrato,modalidad_de_contratacion,objeto_del_contrato&documento_proveedor=900615503',
            'https://www.datos.gov.co/resource/f789-7hwg.json?$select=numero_de_constancia,nombre_entidad,fecha_de_firma_del_contrato,cuantia_contrato,detalle_del_objeto_a_contratar&identificacion_del_contratista=900615503',
            "https://www.datos.gov.co/resource/dmgg-8hin.json?$select=proceso,nombre_archivo,fecha_carga&$where=proceso%20in('CO1.BDOS.9227867','CO1.BDOS.8778903')&$limit=200",
            'https://www.las2orillas.co/que-le-espera-a-colombia-con-abelardo-de-la-espriella-a-partir-del-7-de-agosto/',
        ],
        verifiedAt: '2026-10-10',
    },
```

La nota de Rafael Santos («fue directivo de EL TIEMPO y pertenece a la familia Santos») **sale** hasta que tenga una fuente propia que no sea de un dominio vetado. El parentesco no entra como hecho.

**Textos a corregir** (los aplica quien el responsable editorial decida; aquí no se toca nada):

En `fichas/las2orillas.md`:
1. **Cabecera:**
   - «Valor actual | −0,35» → «**0,00** (desde −0,35; barrido de la voz de la casa, 2026-10-10), sin firmar».
   - «Propuesta | NO FIRMAR todavía…» → «No firmar hasta decidir el tratamiento de la pauta informativa sin rótulo».
   - Fecha 2026-10-10.
2. **Nivel 1:**
   - el párrafo de los fundadores, con la nota de que la lista incluye a una persona fallecida y a una retirada;
   - retirar «pertenece a la familia Santos» y «fue directivo de EL TIEMPO» (sin fuente);
   - añadir la entrevista a León Valencia y las dos piezas basadas en Pares, sin declaración del vínculo.
3. **Sustituir el recuadro «LA FINANCIACIÓN NO ESTÁ DOCUMENTADA»** por:
   - la pauta declarada;
   - la línea de contratación pública (la del bloque de arriba);
   - y una sección **«TENSIÓN: PAUTA INFORMATIVA SIN RÓTULO»** con el estudio previo, la cotización, los informes y las 25 + 7 URL, enlazando esta resolución.
4. **Nivel 2:**
   - sustituir las cifras del 2026-09-08 por las del envío del 2026-10-10: 504 artículos en 40 días, 36 historias, 75 % de agenda propia y 9 compartidas, con la advertencia de que la compañía media no mueve nada;
   - añadir el barrido de la voz de la casa (23 piezas con postura, 9 frente a 14, 1,6:1, sin nivel 2; la misma conducta con los dos gobiernos) con enlace al archivo del barrido.
5. **«ARGUMENTO — por qué −0,35 y no 0,00»** → «POR QUÉ 0,00»:
   - el −0,35 era una colocación relativa sin evidencia (commit `3296b22`);
   - el barrido no la sostiene;
   - y la regla 2.

   Y la alternativa literal declarada.
6. **«CONTRA»:**
   - añadir la inclinación débil hacia el gobierno entrante (9 piezas leves en 65 días frente a 5 en 300 con Petro) como lo que podría mover el número **a la derecha** en el recuento;
   - añadir que la firma de la casa la usan también textos de campaña, comunicados y entregables pagados.
7. **«REFUTACIÓN»:**
   - (a) «Si en el recuento del 05-11-2026 la casa suma 3:1 en una dirección, con al menos 3 piezas a cada lado del cambio».
   - (b) «Si aparecen más piezas pagadas sin rótulo, de cualquier cliente».
   - (c) «Si la Registraduría u otro contratante consta como aprobador de textos concretos».
8. **Sección «REVISIÓN EXTERNA»:** esta resolución, con modelo, versión y fecha.

En `shared/mediaRegistry.js`: el valor y el `biasRationale` de arriba.

En `shared/mediaOwnership.js`: el bloque de arriba, con `verifiedAt: '2026-10-10'`. `ownerType` sigue en `'independiente'`: es una ESAL sin dueño único, y eso consta en el RUES y en el propio medio.

**Lo que NO entra como hecho:**
- que la Registraduría aprobara textos concretos (consta la obligación del contrato, no su ejercicio pieza por pieza);
- que las 4 piezas sobre la Registraduría que no están en los informes sean pagadas;
- que haya otros clientes con piezas sin rótulo;
- que la inclinación posterior al 07-08 sea línea, y no la luna de miel de un gobierno nuevo;
- el parentesco de Rafael Santos;
- y cualquier intención detrás de no declarar el vínculo con Pares.

**¿Aviso de quien dirige?** No procede: no consta candidatura ni cargo público vigente de la directora ni de la editora de opinión.

**Decisiones para el responsable editorial:**
1. **Valor.** Recomendación: **0,00 con evidencia**. Alternativa: −0,35 por la lectura literal de «no deshace nada», declarando que el barrido contradice el signo.
2. **La pauta informativa pagada sin rótulo** (25 artículos de 500 M y 7 de 200 M). Es la línea que se trazó con Ecos del Combeima, pero este medio ya está en el catálogo y su control es conocido. Recomendación: **se queda en el catálogo, con la tensión declarada en la ficha y en el `biasRationale`**, y sin firma hasta que el medio rotule o explique. Considerar si afecta a `factuality` (0,80), que hoy no tiene fuente medida. No se recomienda la baja: la regla 3 frena números, no altas, y la tensión no tiene dirección en el eje.
3. **Precisión de protocolo.** Recomendación: añadir al §1 que «un valor sin evidencia de nivel 1 a 3 que un barrido sistemático contradice en el signo pasa a 0,00, aunque el barrido no llegue a los mínimos de asimetría». Así queda resuelto el choque entre «no deshace nada» y «el 0,00 con evidencia».
4. **Barridos de medios con firma de la casa compartida.** Aquí la cuenta de la casa publica también textos de campaña, comunicados y pauta. Recomendación: que todo barrido busque las notas «Con información suministrada por» y las cruce con SECOP antes de contar, como se hizo aquí.
5. **Centinela.** El medio no está en `shared/centinela.js`. Recomendación: añadir «Quiénes somos» (directora, editora de opinión y fundadores) a la vigilancia semanal.
6. **Recuento del barrido** el 05-11-2026, con el mismo universo y el mismo método.
