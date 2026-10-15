# Respuesta — Claude Opus 5.5 sobre El Isleño

| | |
|---|---|
| **Modelo** | Claude Opus 5.5 |
| **Versión exacta** | `claude-opus-5-5` |
| **Fecha de la consulta** | 2026-10-10 |
| **Quién la hizo** | Claude Code, a petición del responsable editorial (ciclo 2, fase 2, tanda 7; revisor de la misma casa que el autor de las fichas, ver DECISIONES.md 2026-10-07) |
| **¿Tuvo acceso a la red?** | sí |

> **Se pega LITERAL lo que devolvió el modelo, sin editar ni resumir.** Si se
> recorta, se pierde justo lo que pueda incomodar. Los comentarios nuestros van
> al final, en la sección de resolución, claramente separados.
>
> **Única edición, declarada al principio de la resolución:** cuatro enlaces a
> datos.gov.co se sustituyen por «[enlace retirado: …]», porque las páginas a
> las que llevan muestran el documento de identidad de una persona natural
> (regla de DATOS PERSONALES). El texto que los rodea no se toca.

---

## RESPUESTA LITERAL

```
DECLARACIÓN PREVIA DE CONFLICTO
Soy Claude Opus 5.5 (claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Por eso he buscado sobre todo en fuentes que la ficha no usa (el RUES abierto, SECOP I y II, la sección Editorial del propio medio y su feed RSS) y no en lo que yo «sepa» del medio. Mi juicio sobre dónde va el medio no es evidencia. Las conclusiones de abajo valen lo que valgan sus fuentes.
Fecha de todas las comprobaciones: 2026-10-10.

MÉTODO Y DÓNDE BUSQUÉ
1. Dominio. La ficha no cita la URL del medio. elisleno.com, www.elisleno.com, elisleno.co, elisleno.com.co, elisleno.net, elisleno.org y periodicoelisleno.com dan NXDOMAIN (consultados en el resolvedor local, en 8.8.8.8 y en 1.1.1.1). RDAP de Verisign para elisleno.com: HTTP 404, es decir, no está registrado. El dominio real salió de un contrato de SECOP I (ver objeción 2): «elisleño.com», que en IDN es xn--elisleo-9za.com.
2. robots.txt de xn--elisleo-9za.com, leído el 2026-10-10: «User-agent: *» con Disallow solo para carpetas de sistema de Joomla (/administrator/, /cache/, /components/, /images/, etc.). No nombra a ClaudeBot, Claude-Web ni anthropic-ai, así que descargué. Para las2orillas.co el robots.txt solo excluye /wp-admin/. Para welcomesanandres.com, robots.txt da 404 y la portada dice «Coming Soon». casawelcome.com no responde.
3. Descargas con curl -sL, User-Agent de navegador y --ssl-no-revoke, todas en t7\isleno-dl:
   - la portada;
   - el feed RSS (/index.php?format=feed&type=rss);
   - la categoría Editorial (id=48), de limitstart=0 a limitstart=55: 12 páginas de 5 piezas, que cubren de mayo de 2025 a octubre de 2026;
   - el texto completo de 4 editoriales (ids 32636, 33162, 33873, 33121).
   Todas las citas del medio salen de ese HTML crudo.
4. RUES abierto (datos.gov.co c82u-588k). Consultas por razón social con camara_comercio='SAN ANDRES' y los patrones %ISLE%O%, %WELCOME% y %LUNAZZI%. Después, el registro completo de las matrículas 32677, 28606 y 39548.
5. SECOP II (jbjy-vk9h). Primero documento_proveedor='900475712', igualdad exacta y sin dígito de verificación, como manda la regla. Después proveedor_adjudicado like '%EDITORIAL WELCOME%'. Por último documento_proveedor='9004757129'.
6. SECOP I (f789-7hwg): identificacion_del_contratista='900475712', igualdad exacta.
7. Buscador web, usado 4 veces: «El Isleño» con «Casa Editorial Welcome», «El Isleño» con Lunazzi, «Casa Editorial Welcome» San Andrés, y «director de El Isleño». Estuvo disponible y no se agotó, pero aportó poco: una columna de Las2orillas de 2016. No consulté MOM-RSF, la MOE, ColombiaCheck ni Issuu más allá de los enlaces de la portada.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré evidencia de que haya cambiado. La sociedad editora sigue igual en el RUES: CASA EDITORIAL WELCOME S.A.S, matrícula 32677 de la Cámara de Comercio de San Andrés, NIT 900475712-9, estado «ACTIVA», matriculada el 2011-11-08, último año renovado 2026 (fecha_renovacion 20260330), fecha_actualizacion del registro 2026/05/29. El RUES abierto no trae accionistas de una SAS, así que con esta fuente no puedo afirmar ni negar que se hayan transferido acciones. La portada sigue diciendo, literalmente: «Editorial Welcome. todos los derechos reservados 2010».
  Fuente: [enlace retirado: la página muestra el documento de identidad del representante legal, persona natural; consulta al RUES abierto, conjunto c82u-588k, por la matrícula 32677 de San Andrés] (consultado el 2026-10-10).

- La persona que la ficha nombra como titular o director, ¿sigue viva y en el cargo?
  La ficha no nombra a nadie, así que no hay nada que comprobar. El RUES da como representante legal vigente a LUNAZZI EDUARDO GABRIEL (dato del 2026-10-10, registro actualizado el 2026-05-29). En 2016 Las2orillas describía El Isleño como «periódico quincenal dirigido por Billy Lunazzi» (https://www.las2orillas.co/pa-que-voy-a-salir-al-mar/, datePublished 2016-08-11). No está probado que «Billy Lunazzi» y el representante legal sean la misma persona: puede ser un apodo o una homonimia. Además, la cita es de hace diez años y no vale para el presente.

- ¿Quién dirige hoy la redacción?
  No encontré nombre. En la portada no hay mancha ni página de equipo. El feed RSS firma 8 de sus 10 piezas como «(Redacción)», con un buzón de «dirección» del dominio welcomesanandres.com, y las otras 2 con nombres de columnistas. Ninguna pieza dice quién dirige.

- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que la ficha cita?
  Sí. La ficha no cita ninguna fuente de propiedad, y el RUES abierto tiene la sociedad con renovación de 2026-03-30 (ver objeción 1). No es un emisor de valores.

## OBJECIONES

OBJECIÓN 1 — Sí hay sociedad, NIT y representante legal: la laguna de nivel 1 no se sostiene
- QUÉ afirma la ficha: «NIT / razón social: no constan», «Propietario / director: no constan» y «No aparece en los espejos del RUES».
- POR QUÉ es incorrecto: el RUES abierto devuelve la sociedad con una búsqueda trivial por razón social, %WELCOME% en la Cámara de San Andrés. Registro literal:
  - "razon_social":"CASA EDITORIAL WELCOME S.A.S"
  - "nit":"900475712", "digito_verificacion":"9"
  - "organizacion_juridica":"SOCIEDADES POR ACCIONES SIMPLIFICADAS SAS"
  - "estado_matricula":"ACTIVA", "ultimo_ano_renovado":"2026", "fecha_renovacion":"20260330"
  - "cod_ciiu_act_econ_pri":"7310" (publicidad), "cod_ciiu_act_econ_sec":"5911"
  - "representante_legal":"LUNAZZI EDUARDO GABRIEL"
  Que esta sociedad es la editora de El Isleño no lo infiero yo: lo prueban dos cosas. El pie de la web enlaza «Casa Editorial Welcome», y el contrato de SECOP I de la objeción 2 paga a ese mismo NIT por publicar en el «PORTAL WEB EL ISLEÑO.COM».
  Lo que sigue faltando: los socios o accionistas y el beneficiario final. El RUES abierto no los publica para una SAS. El representante legal no es el dueño: es un hecho que se declara, no la propiedad completa.
- FUENTE Y FECHA: [enlace retirado: la página muestra documentos de identidad de personas naturales; conjunto c82u-588k de datos.gov.co] (matrícula 32677 de la Cámara de San Andrés), consultado el 2026-10-10. Registro actualizado el 2026/05/29.
- NIVEL: propiedad (nivel 1, parcial: razón social, NIT, estado y representante legal, sin accionistas).

OBJECIÓN 2 — El dominio no es elisleno.com: es elisleño.com, y eso explica que «su sitio no se pueda preguntar»
- QUÉ afirma la ficha: no da URL. El envío anota que «su sitio no se puede preguntar».
- POR QUÉ: elisleno.com no existe (NXDOMAIN; RDAP de Verisign devuelve 404). El sitio vive en el dominio internacionalizado elisleño.com, xn--elisleo-9za.com en punycode. Responde HTTP 200 y su <title> es «elisleño.com». Su feed RSS (/index.php?format=feed&type=rss) devuelve lastBuildDate «Sat, 10 Oct 2026 18:25:29 +0000» y 10 ítems publicados entre el 08 y el 10-10-2026. Generador: «Joomla! 1.5».
  El enlace documental está en SECOP I. Contrato «ODS 012» de la Cámara de Comercio de San Andrés, firmado el 2024-08-09, con objeto literal: «PRESTAR SERVICIOS DE DIFUSION DE INFORMACION DE INTERESES GENERAL PARA LA COMUNIDAD EMPRESARIAL DEL DEPARTAMENTO A TRAVES DE PORTAL WEB EL ISLEÑO.COM Y REDES SOCIALES EL ISLEÑO». Contratista: NIT 900475712, «CASA EDITORIAL WELCOME».
  Consecuencia práctica: el ingestor tiene que usar la forma punycode. Publica a diario: el 2026-10-10 hay piezas con ids 34195 a 34198. La afirmación de la ficha de que «publica al día» queda confirmada.
- FUENTE Y FECHA: https://xn--elisleo-9za.com/index.php?format=feed&type=rss (2026-10-10); SECOP I, constancia 24-4-14132255 (datos.gov.co f789-7hwg), firmado el 2024-08-09.
- NIVEL: registro externo, más conducta observable (frecuencia).

OBJECIÓN 3 — La ficha no revisa la contratación pública, y la casa editora tiene un cliente institucional recurrente
- QUÉ afirma la ficha: nada sobre contratación.
- POR QUÉ: con el NIT 900475712 aparecen 16 contratos:
  - SECOP I: 14 contratos con un solo cliente, la «CÁMARA DE COMERCIO DE SAN ANDRÉS; PROVIDENCIA Y SANTA CATALINA ISLAS» (NIT de la entidad 892400080). Van del 2019-02-14 (OPS 005, $3.900.000) al 2026-02-02 (CONTRATO 001, $5.400.000). Todos son de régimen especial y tienen objetos de «publicidad» o «divulgación». Suman $61.513.333.
  - SECOP II: 2 contratos con PROVIDENCE AND KETTLINA UTILITIES COMPANY SAS ESP, con objeto «SERVICIOS DE PUBLICACION EN PERIODICO REGIONAL DE LOS INDICADORES DE GESTION SOCIAL». Uno es de la vigencia 2024, firmado el 2026-03-16 por $2.800.000 (CO1.PCCNTR.9395201). El otro es de la vigencia 2023, con fin el 2024-04-19 y $2.300.000 (CO1.PCCNTR.6547316).
  - Últimos 12 meses (2025-10-10 a 2026-10-10): $8.200.000, que son $5.400.000 de la Cámara de Comercio más $2.800.000 de P&K.
  - Total histórico: $66.613.333.
  - Ningún contrato con la Gobernación, la Alcaldía de Providencia ni entidades nacionales.
  Una advertencia de método, que es en sí una objeción al protocolo. En SECOP II el proveedor está registrado con el dígito de verificación pegado: documento_proveedor «9004757129». La consulta reglamentaria, NIT sin DV con igualdad exacta, devuelve 0 filas. Solo lo encontré buscando por nombre del proveedor y luego por «9004757129» exacto.
  Lectura: la Cámara de Comercio es un cliente estable desde hace siete años. Además es la entidad que custodia el registro mercantil de la propia editora. Esto es dependencia comercial e institucional local, no un alineamiento izquierda-derecha. Por sí solo no mueve el número, pero hay que declararlo como conflicto potencial en la cobertura de la Cámara y del sector empresarial.
- FUENTE Y FECHA:
  - [enlace retirado: la página muestra el documento de identidad del representante legal; SECOP I, conjunto f789-7hwg, por el NIT 900475712] (constancias 19-4-9047793 … 26-4-14676292)
  - [enlace retirado: la página muestra el documento de identidad y el domicilio del representante legal; SECOP II, conjunto jbjy-vk9h, por «9004757129»]
  Ambas consultadas el 2026-10-10.
- NIVEL: registro externo.

OBJECIÓN 4 — Sí hay voz editorial propia, semanal, y a ambos lados del 07-08-2026 sostiene la misma línea frente a dos gobiernos de signo opuesto
- QUÉ afirma la ficha: no menciona editoriales ni voz de la casa. Solo trata el medio como «un nombre comercial».
- POR QUÉ: el sitio tiene una sección «Opinión > Editorial» (category id=48) con aproximadamente un editorial por semana, casi siempre en domingo. Revisé todos los de los últimos 12 meses: unas 50 piezas, del 2025-10-05 al 2026-10-04. Su agenda es abrumadoramente local y cívica: aeropuerto, salud, violencia en la isla, la Reserva Seaflower, residuos en Magic Garden, cultura raizal y kriol (Emancipation Week), turismo, la feria del libro y necrologías.
  Las pocas piezas que tocan la política nacional muestran continuidad, no giro, con el cambio de gobierno:
  a) 2025-12-21, «El Barco Ebrio, la Casa Tomada y otra Crónica Anunciada», id 32636, bajo el gobierno saliente. Critica la fiesta en la embajada en Managua con el exdirector de la DNI y pide «la necesaria e impostergable presencia de un embajador (a) en propiedad en Managua». Es fiscalización.
  b) 2026-04-05, «La silla vacía en Managua», id 33162, también bajo el gobierno saliente: «La ausencia de un embajador en propiedad en Managua desde el 31 de enero de 2025 va dejando un vacío diplomático que trasciende lo protocolario.»
  c) 2026-08-09, «El cierre de las embajadas en Nicaragua y Barbados», id 33873, ya con el gobierno entrante: «El anuncio del presidente Abelardo De la Espriella de cerrar 14 embajadas colombianas […] ha generado especial preocupación en el Archipiélago», «resulta difícil comprender que Colombia considere prescindible su misión oficial en Managua», «Desde aquí queremos formular, respetuosamente, una solicitud al Señor Presidente: antes de cerrar estas dos embajadas, mire hacia el Caribe y escuche al Archipiélago.»
  La misma demanda territorial (canales con Managua y pescadores raizales) se dirige con el mismo tono al gobierno saliente y al entrante. Según la regla del polo fijo, es el patrón de «sigue fiscalizando con el entrante», o sea, orientación mixta. Tampoco hay endosos electorales en la ventana.
  Barrido para la regla de evidencia editorial histórica:
  - Piezas con postura sobre el eje nacional izquierda-derecha: 0 que no sean fiscalización. Las tres de arriba lo son, y por regla no cuentan.
  - No se alcanzan ni las 10 piezas ni las 3 por lado: la regla no se activa y no hay asimetría.
  - Reproducible: categoría id=48, limitstart 0 a 55, extracción de título, fecha y entradilla. Texto completo de los ids 32636, 33162, 33873 y 33121.
- FUENTE Y FECHA:
  - https://xn--elisleo-9za.com/index.php?option=com_content&view=category&layout=blog&id=48&Itemid=85 y sus páginas &limitstart=5…55 (consultadas el 2026-10-10)
  - https://xn--elisleo-9za.com/index.php?option=com_content&view=article&id=32636&catid=48&Itemid=85 (2025-12-21)
  - https://xn--elisleo-9za.com/index.php?option=com_content&view=article&id=33162&catid=48&Itemid=85 (2026-04-05)
  - https://xn--elisleo-9za.com/index.php?option=com_content&view=article&id=33873&catid=48&Itemid=85 (2026-08-09)
- NIVEL: hecho editorial de los últimos 12 meses / declaración del propio medio (voz de la casa).

## LO QUE NO PUDE VERIFICAR

- Accionistas y beneficiario final de Casa Editorial Welcome S.A.S. El RUES abierto no los publica. Haría falta el certificado de existencia y representación de la Cámara de San Andrés, que es de pago, o los estados financieros y el libro de accionistas. No los obtuve.
- Si «Billy Lunazzi», a quien Las2orillas nombraba director en 2016, es la misma persona que el representante legal inscrito. No hay fuente que lo pruebe, así que no lo afirmo.
- Relación entre «GRUPO WELCOME S.A.» (matrícula 28606 de la Cámara de San Andrés, NIT 900134609, CIIU 7911 de agencias de viaje, activa, renovada en 2026, con otro representante legal en el RUES) y la casa editora. Comparten la palabra «Welcome» y el negocio turístico, pero no encontré ningún documento que las vincule. Puede ser coincidencia de nombre.
- Quién dirige hoy la redacción. Busqué en la portada, el feed y una búsqueda web: no hay nombre.
- Periodicidad actual de la edición impresa. La portada enlaza a issuu.com/el_isleno/docs/el_isle_o_233 y, en febrero de 2026, un editorial cita «la reciente edición de EL ISLEÑO impreso», pero no comprobé fechas en Issuu.
- Si hay otro medio de San Andrés ya cubierto en el catálogo. El envío no menciona ninguno, no veo el catálogo y no hice un barrido de medios del archipiélago.

## LO QUE FALTA

- La URL del medio y la del feed. La ficha no las cita, y el dominio sin eñe no existe.
- El bloque de propiedad completo: la razón social, el NIT y el representante legal del RUES (objeción 1) y la declaración explícita de que los accionistas no constan en fuente abierta.
- La contratación pública: 12 meses y total histórico (objeción 3), con la nota de que en SECOP II el NIT figura con el dígito de verificación pegado.
- La dependencia publicitaria visible en la portada:
  - banners de Sopesa (sopesa.com), Decameron y varios hoteles;
  - en el feed del 2026-10-10, una pieza titulada «Sopesa informa a usuarios y a la población isleña en general», que tiene forma de comunicado de la empresa de energía.
  Es dependencia comercial local y turística, y hay que declararla como conflicto potencial. No es evidencia de eje.
- La pregunta de la ficha sobre si el medio es «raizal o continental» no debe resolverse con el origen étnico de sus titulares. La Ley 1581 trata ese dato como sensible y este revisor no lo consigna. Lo comprobable es la agenda. En los últimos 12 meses los editoriales dedican piezas a:
  - Emancipation Week (2026-08-02);
  - la lengua kriol, en «La naturaleza del Creole» (2026-02-22);
  - la defensa de «familias raizales» frente a la SAE (2025-08-24, fuera de la ventana por semanas).
  Eso es una agenda territorial isleña observable.
- Un dato que no es objeción pero conviene anotar: el editorial del 2026-03-29, «Rendición de cuentas, ejercicio contra viento y marea» (id 33121), es favorable a la gestión del gobernador Nicolás Gallardo Vásquez. Dice: «evidencia una administración enfocada en la inversión social y la infraestructura», a pesar de la nulidad electoral que el mismo texto menciona. Es complacencia con el poder local, no un eje nacional. En SECOP no hay contratos de la Gobernación con este NIT.

## EVIDENCIA QUE NO MUEVE EL NÚMERO

- Ningún endoso electoral ni editorial partidista en la ventana de 12 meses. Se ve en el barrido completo de la categoría Editorial.
- Las demandas al Estado central se dirigen igual a los dos gobiernos, saliente y entrante (objeción 4, piezas a, b y c).
- La actividad registrada principal de la editora es publicidad (CIIU 7310), y sus productos hermanos son revistas turísticas (Welcome Caribe, Welcome San Andrés). Es una casa cuya «línea» es el comercio y el turismo local, del tipo que el contexto describe como mixta.
- Frecuencia: publica a diario. Feed RSS con fechas: 10 ítems entre el 2026-10-08 y el 2026-10-10. Existen unas 33.000 piezas en portada, según la paginación limitstart=32994 del 2026-10-10.
- El editorial del 2025-11-23, «No hay salud, sin salud mental», menciona «narrativas instaladas por las corrientes del pensamiento negacionista». Es un guiño aislado y no basta para nada.
- Fuera de ventana, solo para que conste: el editorial «Le dispararon a la democracia» (2025-06-09) es una reproducción declarada de El Tiempo («Tomado de El Tiempo»). No cuenta como voz propia ni entra en los 12 meses.

## VIABILIDAD DEL ALTA (respuesta al encargo)

- Con lo encontrado, el alta es viable. Ya existe un nivel 1 parcial y documental: sociedad activa, NIT, representante legal en el RUES y vínculo contractual sociedad–portal en SECOP I. Hay un feed RSS operativo con fechas y voz editorial propia y estable.
- Lo que sigue abierto es quién controla la SAS, es decir, los accionistas. Hay que declararlo como hueco.
- Valor provisional según las reglas:
  - No hay evidencia de nivel 1 a 3 que sitúe al medio a un lado del eje.
  - El barrido editorial no activa la excepción de la regla de 2026-10-09: 0 piezas con postura que no sean fiscalización.
  - Ante la duda, la regla 2 lleva a lo más cercano a la mixta.
  - Valor provisional: 0,00 (orientación mixta), con la tensión declarada de la dependencia comercial e institucional local: la Cámara de Comercio como cliente recurrente, anunciantes turísticos y Sopesa, y un tono complaciente con la gobernación.
  - Sin corpus (0 artículos en la ventana del 2026-08-31 al 2026-10-10, porque no está ingerido), no hay nivel 2 medido. Ese número no debería firmarse hasta ingerir el feed (forma punycode) durante 90 días.
- Aporte frente a otro medio de San Andrés: el envío no menciona ninguno cubierto y la ficha lo presenta como «el único candidato del archipiélago». No lo pude contrastar.

## SIN OBJECIÓN
No aplica: hay 4 objeciones.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-10. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: cuatro enlaces retirados, ningún número.**
- El revisor no copió cédulas, teléfonos ni direcciones de personas naturales, ni la nacionalidad, el origen étnico o el lugar de nacimiento de nadie. Cuando habla de lo raizal, se niega expresamente a resolverlo por el origen de los titulares y lo lleva a la agenda del medio. Las cifras largas de su texto son NIT de sociedades o entidades (900475712, 9004757129 con el dígito de verificación pegado, 892400080 y 900134609), matrículas, constancias y cuantías.
- **Pero cuatro de sus enlaces llevan a páginas que muestran el documento de identidad del representante legal**, una persona natural:
  - la consulta del RUES por la matrícula 32677: el registro trae el campo `num_identificacion_representante_legal`;
  - el conjunto `c82u-588k` sin filtro: lista personas naturales con su número;
  - la de SECOP I por el NIT: las filas traen `identific_representante_legal`;
  - y la de SECOP II por «9004757129»: trae el documento del representante legal, su domicilio y los documentos de supervisores y ordenadores del gasto.
- Se sustituyen en la respuesta literal por «[enlace retirado: …]», como en las respuestas de Al Aire Noticias y El Morichal. El texto de alrededor queda intacto. Más abajo van consultas equivalentes con `$select`, que devuelven los mismos datos sin esos campos (comprobado: 0 apariciones de «identif» en las tres respuestas).
- Esta resolución tampoco escribe ese documento ni su tipo.

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar (2026-10-10):
  - xn--elisleo-9za.com: «User-agent: *» y Disallow solo de carpetas de Joomla (/administrator/, /cache/, /images/, /media/, /templates/…). No nombra a ningún agente de Anthropic. Literal al del revisor.
  - las2orillas.co: «Disallow: /wp-admin/».
  - welcomesanandres.com: 404. casawelcome.com: «Disallow:» vacío. issuu.com: no excluye a Claude.
  - datos.gov.co: `Crawl-delay: 1`; se usó solo `/resource`, con un segundo entre consultas.
  - No se tocaron eltiempo.com, cambiocolombia.com, lasillavacia.com, diariodelsur.com.co, quibdo-choco.gov.co ni vlex.
- **Sitio del medio**, con `curl -sL --ssl-no-revoke` y User-Agent de navegador, en `scratchpad/t7/isleno-ver`:
  - portada y feed (`/index.php?format=feed&type=rss`), 200;
  - las 13 páginas de la categoría Editorial (id 48, `limitstart` 0 a 60): 65 piezas, del 2025-01-26 al 2026-10-04;
  - el texto completo de **30 editoriales** de los últimos 12 meses, 20 de antes del 07-08-2026 y 10 de después.
  - **Aviso:** tras unas 50 peticiones en unos 10 minutos, el sitio empezó a responder «Bot Verification» («Verifying that you are not a robot…»), incluido el feed, con un 403. Va detrás de Cloudflare y de LiteSpeed. Cuatro descargas más (dos editoriales fuera de la ventana y el par repetido 32976/32977) no se pudieron hacer, y se dejó de pedir. Ver «Ingesta» en las decisiones.
- **DNS y RDAP:** `elisleno.com` da «Non-existent domain» en 8.8.8.8, y el RDAP de Verisign devuelve 404. `xn--elisleo-9za.com` resuelve a direcciones de Cloudflare. Su RDAP da registro el 2010-01-28 y caducidad el 2027-01-28. Los otros seis dominios que cita el revisor no se comprobaron.
- **Registros**, en datos.gov.co:
  - RUES (`c82u-588k`): por `nit=900475712`; por razón social, `%WELCOME%` e `%ISLE%O%` en la Cámara de San Andrés; y por `%LUNAZZI%` en la razón social o en el representante legal.
  - SECOP I (`f789-7hwg`): `identificacion_del_contratista`, con `900475712` y con `9004757129`, igualdad exacta. Por razón social, `%WELCOME%`.
  - SECOP II (`jbjy-vk9h`): `documento_proveedor`, con `900475712` y con `9004757129`, igualdad exacta. `proveedor_adjudicado like '%EDITORIAL WELCOME%'`.
  - RUES de la contratante de SECOP II (`nit=901352888`).
- **Terceros:**
  - la columna de Las2orillas de 2016;
  - la edición 233 en Issuu;
  - welcomesanandres.com y casawelcome.com.
- **Repositorio:**
  - las fichas `el-isleno.md` y `archipielago-press.md`, y el envío;
  - `fichas/LEEME.md`, `MEDIOS_CANDIDATOS_DEPARTAMENTOS.md` y `COBERTURA_DEPARTAMENTAL.md`;
  - `scripts/armarEnvio.mjs`, `vercel.json` y `src/services/csp.test.js`;
  - `server/services/ingestDaemon.js`: `canonicalizeLink`, `urlDeImagenValida`, `extractImage`, `parsePublishedAt` y `techoDelFeed`;
  - `shared/mediaRegistry.js`, `shared/mediaOwnership.js` y `shared/mediaOwnership.test.js`;
  - `src/pages/MediaMap.jsx` y `src/data/mediaLogos.js`.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | Sí hay sociedad, NIT y representante legal en el RUES; los socios no constan | sí | sí | **Aceptada.** Todas las cifras coinciden. Añadidos: está inscrita como proponente, y el representante legal tiene además matrícula activa como persona natural comerciante. Sus enlaces muestran el documento de esa persona y se retiran |
| 2 | El dominio es elisleño.com (`xn--elisleo-9za.com`), no elisleno.com, «y eso explica que su sitio no se pueda preguntar» | sí | sí | **Parcial.** Son exactos el dominio, el RDAP, el feed, el `<title>` y el contrato ODS 012. **Se rechaza la causalidad:** el repositorio ya tenía el feed en punycode desde agosto, la frase del envío es una plantilla para medios fuera del centinela y la ficha nunca escribió «elisleno.com». La objeción que sí se sostiene es que **la ficha no cita ni URL ni feed** |
| 3 | La ficha no revisa la contratación: 16 contratos por $66.613.333, $8.200.000 en 12 meses; el DV pegado en SECOP II | sí | sí | **Aceptada, con una corrección.** SECOP I coincide al peso: 14 contratos, $61.513.333. En SECOP II, CO1.PCCNTR.6547316 está «enviado Proveedor» y **sin fecha de firma**, así que no consta como contratado. Total firmado: **15 por $64.313.333**. Los 12 meses ($8.200.000) son exactos. El fallo del DV está confirmado: 0 filas sin el DV, 2 con él |
| 4 | Voz editorial semanal propia, con la misma línea ante los dos gobiernos; la regla histórica no se activa | sí | sí, 30 piezas leídas enteras | **Aceptada en lo sustancial, con la cifra corregida.** Son **43 editoriales en 12 meses, no «unas 50»**. En las 30 leídas hay 0 piezas con postura en el eje nacional, y las citas son literales. Pero la «continuidad» descansa en 3 piezas nacionales: alcanza para anotarla, no para llamar al 0,00 «con evidencia» |

### Lo verificado, objeción por objeción

**1 · RUES.**
- Por `nit=900475712`, una sola fila, literal:
  - «"camara_comercio":"SAN ANDRES"», «"matricula":"32677"», «"razon_social":"CASA EDITORIAL WELCOME S.A.S"», «"nit":"900475712"», «"digito_verificacion":"9"»;
  - «"organizacion_juridica":"SOCIEDADES POR ACCIONES SIMPLIFICADAS SAS"», «"estado_matricula":"ACTIVA"», «"fecha_matricula":"20111108"», «"fecha_renovacion":"20260330"», «"ultimo_ano_renovado":"2026"»;
  - «"cod_ciiu_act_econ_pri":"7310"», «"cod_ciiu_act_econ_sec":"5911"», «"representante_legal":"LUNAZZI EDUARDO GABRIEL"», «"fecha_actualizacion":"2026/05/29 19:02:13.630000000"».

  **Exacto.**
- **Lo que el revisor no dice:**
  - «"inscripcion_proponente":"000000000837"»: la sociedad está inscrita para contratar con el Estado, como Al Aire Comunicar.
  - La búsqueda `%LUNAZZI%` devuelve, además de la sociedad, una **matrícula de persona natural a nombre del representante legal**: ACTIVA, renovada en 2026, CIIU 4719 (comercio al por menor). No consta relación con el medio y no se propone para la ficha. Se anota porque en Al Aire se anotó la equivalente.
  - Hay también **otra persona inscrita con el mismo apellido y el nombre de pila «Billy»**, representante legal de una fundación de San Andrés. Esto hace aún más débil la identificación entre el «Billy Lunazzi» de 2016 y el representante legal. No se escribe su nombre completo, no se afirma parentesco y no se afirma que sea el director de 2016.
  - Esas consultas no se enlazan, porque muestran documentos de personas naturales.
- **Fuente citable sin el documento del representante:**
  `https://www.datos.gov.co/resource/c82u-588k.json?$select=camara_comercio,matricula,razon_social,nit,digito_verificacion,organizacion_juridica,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,cod_ciiu_act_econ_pri,cod_ciiu_act_econ_sec,representante_legal,inscripcion_proponente,fecha_actualizacion&nit=900475712`
- **El vínculo sociedad–medio está probado por tres fuentes independientes:**
  - el pie del sitio, literal: «elisleño.com es un producto de la Casa Editorial Welcome. todos los derechos reservados 2010». La ficha decía bien «fechado en 2010»;
  - el objeto del contrato ODS 012, que nombra el «PORTAL WEB EL ISLEÑO.COM» y paga al NIT 900475712;
  - Issuu: «EL ISLEÑO 233 by Casa Editorial Welcome», con `datePublished` 2026-09-08. La edición impresa sigue viva, y eso confirma lo que la ficha decía de Issuu, que el revisor no comprobó.
- **GRUPO WELCOME S.A.** (matrícula 28606, NIT 900134609): ACTIVA, renovada el 19-02-2026, CIIU 7911 y 7912 (agencias de viaje), con otro representante legal. Coincide con lo que dice el revisor. Tiene un contrato en SECOP I con una alcaldía de Boyacá (2019) y nada que la ligue a la editora. **No se afirma relación.**
- **`casawelcome.com` no está caído, como dice el revisor:** responde y redirige con un 301 a un mercado de dominios, con el título «CasaWelcome.com is for sale». El enlace «Casa Editorial Welcome» del pie lleva hoy a un dominio en venta. `welcomesanandres.com`: 200, «Coming Soon».

**2 · Dominio y feed.**
- `<title>elisleño.com</title>` en la portada. El feed responde 200, `application/rss+xml`, con 10 ítems, «Joomla! 1.5», `<language>es-es` y `lastBuildDate` «Sat, 10 Oct 2026 18:32:39 +0000». La fecha la genera el servidor en cada petición; la del revisor es de 7 minutos antes.
- **Fechas legibles:** todas en RFC 822 con zona (`+0000`). `new Date()` las lee sin error (`parsePublishedAt`).
- **El orden no es cronológico:**

  | pubDate (UTC) | id | sección | firma |
  |---|---|---|---|
  | 10-10 12:54 | 34198 | deportes | (Redacción) |
  | 10-10 10:33 | 34195 | ambiental | (Redacción) |
  | 09-10 15:53 | 34193 | salud | (Redacción) |
  | 10-10 12:03 | 34197 | columnas | columnista |
  | 10-10 11:30 | 34196 | columnas | columnista |
  | 09-10 20:04 | 34194 | ambiental | (Redacción) |
  | 09-10 12:51 | 34192 | cultura | (Redacción) |
  | 09-10 11:57 | 34191 | **anuncios** | (Redacción) |
  | 08-10 16:25 | 34189 | ambiental | (Redacción) |
  | 09-10 10:29 | 34190 | ambiental | (Redacción) |

  Es el orden de portada de Joomla. A la ingesta no le afecta: el techo es 15 (`ITEMS_PER_FEED`), mayor que 10, y cada fecha se lee por separado. Los ids van seguidos (34189 a 34198), así que el feed lleva toda la producción, no una selección. Al ritmo de unas 5 piezas al día, 10 ítems cubren unas 48 h: solo se pierde algo si la ingesta pasa más de dos días sin leerlo.
- **La pieza de Sopesa va en la sección «anuncios»** (`catid=66:anuncios`). El revisor dice que «tiene forma de comunicado»; el propio medio la clasifica como anuncio, firmada «(Redacción)». El corpus recibirá anuncios y columnas de terceros, como en otros medios.
- **ODS 012**, constancia 24-4-14132255, literal: «PRESTAR SERVICIOS DE DIFUSION DE INFORMACION DE INTERESES GENERAL PARA LA COMUNIDAD EMPRESARIAL DEL DEPARTAMENTO A TRAVES DE PORTAL WEB EL ISLEÑO.COM Y REDES SOCIALES EL ISLEÑO; DE CONFORMIDAD CON LA PROPUESTA PRESENTADA; […]». Firmado el 2024-08-09, «Régimen Especial». **Exacto.** El revisor omite la cola «DE CONFORMIDAD…», que no altera el sentido.
- **Por qué se rechaza la causalidad.** El dominio punycode ya estaba en el repositorio:
  - `MEDIOS_CANDIDATOS_DEPARTAMENTOS.md:53` da el feed `xn--elisleo-9za.com/index.php?format=feed&type=rss`;
  - `COBERTURA_DEPARTAMENTAL.md:110` da «`elisleño.com` | Joomla, punycode».

  La línea del envío, «su sitio no se puede preguntar, o su ficha no se apoya en ningún nombre publicado», es la plantilla de `scripts/armarEnvio.mjs:338` para todo medio que no vigila el centinela. Este no está en el catálogo, y por eso no lo vigila. Tampoco la ficha dice en ningún sitio «elisleno.com». **Lo que sí falla es la ficha:** perdió la URL y el feed que el repositorio ya tenía.
- **Cómo se escribe un IDN en el catálogo.** Ningún medio del registro usa hoy un IDN. Debe ir en punycode (`xn--elisleo-9za.com`) en `domain`, en `feed.url`, en `imageHosts` y en el `img-src` de `vercel.json`:
  - `new URL('https://elisleño.com/x').hostname` devuelve `xn--elisleo-9za.com` (comprobado con Node). `canonicalizeLink` y `extractImage` comparan contra `hostname`, así que un `domain` escrito con eñe no casaría nunca.
  - La gramática de fuentes de la CSP solo admite ASCII en el host.
  - `src/services/csp.test.js` construye `https://*.${domain}` y `https://${domain}` a partir del registro y exige los dos en `img-src`.
  - Las imágenes del feed son absolutas y del mismo host (`https://xn--elisleo-9za.com/images/…`).
  - **Efecto visible:** `MediaMap.jsx:1179` pinta `media.domain` tal cual, así que el perfil diría «xn--elisleo-9za.com». Arreglarlo es cosa de código (ver las decisiones). No es motivo para escribir el dominio con eñe.

**3 · Contratación.**
- **SECOP I** por `identificacion_del_contratista=900475712`: **14 filas, todas de la «CÁMARA DE COMERCIO DE SAN ANDRÉS; PROVIDENCIA Y SANTA CATALINA ISLAS»**.
  - La entidad tiene NIT 892400080 y figura como «TERRITORIAL DEPARTAMENTAL DESCENTRALIZADO». Los 14 contratos son de «Régimen Especial», están «Celebrado» y no tienen adiciones.
  - Van de OPS 005 (2019-02-14, $3.900.000) a CONTRATO 001 (2026-02-02, $5.400.000, fin el 2026-05-02).
  - **Suma: $61.513.333, exacta.**
  - Objetos: «PRESTAR SERVICIOS DE PUBLICIDAD…» (2019-2023), «DESEMPEÑARSE COMO MEDIO DE DIFUSIÓN…» (2024) y la divulgación de cursos y eventos de la Cámara (2025-2026).
  - Con `9004757129` (con el DV): 0 filas. En SECOP I el NIT está bien escrito.
- **SECOP II**:
  - por `documento_proveedor=900475712` (la regla): **0 filas**;
  - por `9004757129`: 2 filas, las mismas que por `proveedor_adjudicado`. La contratante es PROVIDENCE AND KETTLINA UTILITIES COMPANY SAS ESP (NIT 901352888). En el RUES es una S.A.S. E.S.P. de San Andrés, ACTIVA, CIIU 3600 (captación y distribución de agua). Su naturaleza pública, mixta o privada no consta.
    - CO1.PCCNTR.9395201: firmado el 2026-03-16, del 16-03 al 16-04-2026, $2.800.000, «Modificado», `valor_pagado` 0. Objeto: indicadores de gestión social de la vigencia 2024.
    - CO1.PCCNTR.6547316: **«enviado Proveedor», sin `fecha_de_firma`** ni fecha de inicio, con fin el 2024-04-19, $2.300.000. Vigencia 2023. **No consta firmado**: no se cuenta como contratado.
- **Últimos 12 meses (2025-10-10 → 2026-10-10): 2 contratos por $8.200.000** ($5.400.000 + $2.800.000), por fecha de firma. **Exacto.** El CONTRATO 010 de 2025 se firmó el 11-06-2025 y terminó el 11-10-2025: queda fuera por la fecha de firma, aunque su ejecución roza la ventana.
- **Ningún contrato** con la Gobernación, la Alcaldía de Providencia ni entidades nacionales. **Confirmado** por el NIT.
- **La tensión que el revisor no ve:** dos editoriales posteriores al 07-08 amplifican una carta de gremios firmada por la Cámara de Comercio, su único contratante en SECOP I, sin declarar la relación.
  - «Que alce vuelo de una vez el aeropuerto de San Andrés» (06-09-2026): «Cámara de Comercio, Cotelco, Anato, Acodres, Proarchipiélago y 'Cómo Vamos San Andrés', coinciden en algo esencial».
  - «Aeropuerto en la olla» (20-09-2026): «El documento está suscrito por la Cámara de Comercio de San Andrés y Providencia; y los capítulos isleños de Anato, Cotelco y Acodres».

  La causa es cívica y compartida, y no se insinúa que la pieza sea pagada. Pero la relación contractual es un dato que el lector no tiene. Desvelamiento, no acusación.
- **La Cámara de Comercio** es una entidad privada con funciones públicas, no un gobierno. Es el criterio de Al Aire y de Archipiélago Press. Además lleva el registro mercantil de la propia editora, como señala el revisor.

**4 · Voz de la casa.**
- **Recuento de la categoría Editorial (id 48)**, de las 13 páginas:
  - **43 piezas entre el 2025-10-10 y el 2026-10-10**, 33 antes del 07-08-2026 y 10 después. Con el corte del revisor, desde el 2025-10-05, son 44, no «unas 50».
  - Dos de ellas son el mismo tema en dos versiones (32976 y 32977, «Turismo e inmersión cultural…», ambas del 01-03-2026).
  - Una reproduce un editorial propio de 2020 (32658).
  - Todas van firmadas «Editorial» (`createby`). Casi todas son de domingo. «Un editorial por semana» es correcto como aproximación, con dos huecos: del 10-05 al 07-06-2026 y del 15-06 al 12-07-2026.
- **No hay editorial en ninguna de las dos vueltas presidenciales** (31-05 y 21-06-2026), ni ninguno de tema electoral en 12 meses. Es «evidencia que no mueve el número», y es más fuerte que «sin endosos».
- **Muestreo: 30 piezas leídas enteras.** URL de cada una: `https://xn--elisleo-9za.com/index.php?option=com_content&view=article&id=<id>&catid=48&Itemid=85`.

  | Lado | id | Fecha | Título | Clasificación |
  |---|---|---|---|---|
  | después | 34168 | 04-10-2026 | ¿Y el tratamiento para cuándo? | Salud. Pide al Ministerio que las medidas «se traduzcan en resultados verificables». Exigencia, sin postura |
  | después | 34136 | 28-09-2026 | Disparos y caos perturbaron la paz… | Orden público local. Pide intervención nacional |
  | después | 34127 | 27-09-2026 | El Festival de Teatro Ethnic Roots… | Cultura |
  | después | 34092 | 20-09-2026 | Aeropuerto en la olla | Exige al «nuevo Gobierno Nacional» y a la Aerocivil. Amplifica la carta de la Cámara |
  | después | 34050 | 13-09-2026 | Mirarnos adentro… | Cultura (FILSAI) |
  | después | 34017 | 06-09-2026 | Que alce vuelo de una vez el aeropuerto… | «El llamado al nuevo Gobierno Nacional es, entonces, respetuoso pero inaplazable». Gremios con la Cámara. Soberanía del espacio aéreo (Panamá) |
  | después | 33981 | 30-08-2026 | Puentes solidarios | Solidaridad tras el terremoto |
  | después | 33946 | 23-08-2026 | ¡Manos a la obra! | Turismo y Seaflower. Respalda un plan piloto |
  | después | 33912 | 16-08-2026 | El significado de una decisión | Una ordenación sacerdotal |
  | después | 33873 | 09-08-2026 | El cierre de las embajadas en Nicaragua y Barbados | **Fiscaliza al Gobierno entrante**, con respeto: «Romper puentes puede producir una satisfacción política inmediata…». Citas del revisor, literales |
  | antes | 33843 | 02-08-2026 | Mucho más que una celebración | Emancipation Week |
  | antes | 33794 | 26-07-2026 | Menos discursos, más acciones | Seaflower |
  | antes | 33701 | 12-07-2026 | Cuando el mar pide respuestas | Seguridad marítima. Fiscaliza a autoridades sin nombrarlas |
  | antes | 33561 | 15-06-2026 | Sentido de pertenencia | Residuos, civismo |
  | antes | 33524 | 07-06-2026 | Una emergencia ambiental que no admite más espera | Coralina y Magic Garden |
  | antes | 33363 | 10-05-2026 | La transformación del Infotep | Elogio institucional educativo |
  | antes | 33201 | 12-04-2026 | ¿Violencia normalizada? | Homicidios |
  | antes | 33162 | 05-04-2026 | La silla vacía en Managua | **Fiscaliza al Gobierno saliente** (embajador). Cita literal |
  | antes | 33121 | 29-03-2026 | Rendición de cuentas, ejercicio contra viento y marea | **Favorable al gobernador** («evidencia una administración enfocada en la inversión social y la infraestructura», literal). Eje local |
  | antes | 32942 | 22-02-2026 | La naturaleza del Creole | Lengua kriol. Elogia la obra departamental del Museo Raizal |
  | antes | 32904 | 14-02-2026 | Las cosas por su nombre… | Toponimia (IGAC) |
  | antes | 32844 | 01-02-2026 | La parábola de Serrano | Sostenibilidad. Cita «la reciente edición de EL ISLEÑO impreso» |
  | antes | 32686 | 01-01-2026 | ¿Violencia normalizada? | Violencia en 2025 |
  | antes | 32670 | 28-12-2025 | 2025: otro año de contrastes | Balance del año |
  | antes | 32658 | 25-12-2025 | ¿Todo sigue igual? | Reproduce su editorial de 2020. Pregunta por planes de los gobiernos Santos y Duque. Fiscalización histórica |
  | antes | 32636 | 21-12-2025 | El Barco Ebrio, la Casa Tomada… | **Fiscaliza a la Cancillería del Gobierno saliente.** Cita literal |
  | antes | 32494 | 23-11-2025 | No hay salud, sin salud mental | «desde la dirección de esta Casa Editorial»; «corrientes del pensamiento negacionista» (literal). Un guiño aislado |
  | antes | 32463 | 16-11-2025 | La espinosa eternidad de los asuntos pendientes… | Puerto, energía, acueducto, Estatuto Raizal. Autocrítica isleña |
  | antes | 32298 | 19-10-2025 | ¿Flotando en el viento? | Fiscaliza a la SAE y al Estado |
  | antes | 32268 | 13-10-2025 | La claridad del faro | Necrología. Pide esclarecimiento |

- **Recuento según la regla:**
  - 0 elogios, disculpas o rótulos sobre el eje nacional, a ningún lado.
  - Fiscalización nacional: 2 antes (32636 y 33162) y 1 después (33873), más dos exigencias al nuevo Gobierno sin juicio (34017 y 34092).
  - **La regla no tiene piezas que contar**: no hay 10 piezas con postura ni 3 por lado.
  - Igual que en El Morichal, el 0,00 se queda por la regla 2. La continuidad de Managua es real, pero son 3 piezas: se anota como nivel 5 y no basta para llamar al 0,00 «con evidencia», como en Chocó 7 Días, que tenía 15.
- **No verificado:** «Le dispararon a la democracia» (2025-06-09) como reproducción de El Tiempo, y la pieza de la SAE del 2025-08-24. Las dos están fuera de la ventana, y el bloqueo antirrobot impidió descargarlas. No cambian nada.

**Las2orillas.** `https://www.las2orillas.co/pa-que-voy-a-salir-al-mar/`, con `datePublished` «2016-08-11T06:00:54-05:00». Literal: «El Isleño, periódico quincenal dirigido por Billy Lunazzi». **Exacto.**
- Es historia de hace diez años.
- La identidad con el representante legal no está probada, y el RUES tiene otra persona de nombre «Billy» con ese apellido (ver el punto 1).
- No entra en la ficha como hecho. Basta con una línea en `buscadoEn`.

**Qué aporta un segundo medio isleño (The Archipielago Press, +0,30, sin firmar).** El revisor no podía saberlo: el envío no lo menciona.

| | The Archipielago Press | El Isleño |
|---|---|---|
| Quién | Persona natural (director y fundador), sin sociedad editora; marca a su nombre en 2015, sin vigencia comprobada | S.A.S. activa desde 2011, NIT 900475712, representante legal en el RUES; socios no constan |
| Contratación | Del director, $163.711.569 entre 2018 y 2023, sobre todo con la Gobernación; 0 en 12 meses | De la sociedad, $64.313.333 firmados entre 2019 y 2026, sobre todo con la Cámara de Comercio; $8.200.000 en 12 meses; 0 con la Gobernación |
| Voz de la casa, eje nacional | Asimetría de 26 a 2 hacia la derecha, a los dos lados del 07-08: +0,30 | 0 piezas con postura en 43 editoriales; fiscaliza a los dos gobiernos en la cuestión de Managua |
| Voz de la casa, eje local | Fiscaliza al gobernador Gallardo («maniobras dilatorias»), y su director demanda en el pleito electoral | Editorial favorable al gobernador Gallardo (29-03-2026) |
| Feed | Por tandas; la ingesta pierde unas 4 de cada 10 piezas | Unas 5 al día; 10 ítems cubren unas 48 h; todo dentro del techo |

- **Rompe la dependencia de una sola voz.** El archipiélago tiene hoy un único medio, situado en +0,30.
- **Las dos casas tienen líneas locales opuestas frente a la Gobernación**, y eso es justo lo que la vista departamental quiere mostrar.
- **Ninguna de las dos es «voz raizal» por propiedad, y no debe decidirse así.** Las dos tienen agenda raizal: kriol, Emancipation Week, pescadores, Managua.
- La REFUTACIÓN 3 de la ficha («si aparece un segundo medio del archipiélago, conviene compararlos antes de dar de alta a uno solo») se cumple al revés: el primero ya entró el 2026-08-14, y esta es la comparación.

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se rechazan o corrigen estas partes:
- **Obj. 2:** «por eso "no se podía preguntar"». La frase del envío es una plantilla para medios fuera del centinela, y el repositorio ya tenía el feed en punycode. El fallo es de la ficha, que no lo cita, no de un dominio desconocido.
- **Obj. 3:** «16 contratos… Total histórico: $66.613.333». CO1.PCCNTR.6547316 no tiene fecha de firma y está «enviado Proveedor». Por la regla, se cuenta lo contratado: **15 por $64.313.333**, y el de $2.300.000 se anota aparte como no firmado.
- **Obj. 4:** «unas 50 piezas». Son 43 en 12 meses, o 44 con su corte. Y «orientación mixta» por polo fijo: con 3 piezas nacionales es una anotación de nivel 5, no un 0,00 con evidencia.
- **Métodos:** «casawelcome.com no responde». Responde y redirige a una página de dominio en venta.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente.** Las URL del medio, de Las2orillas y de datos.gov.co resuelven, y las citas son literales. Las cifras del RUES y de SECOP I coinciden al peso. Omisiones y deformaciones:
- **cuatro enlaces que muestran el documento de una persona natural**, retirados;
- la inscripción como proponente;
- la matrícula de persona natural del representante legal;
- el homónimo de nombre «Billy»;
- que CO1.PCCNTR.6547316 no está firmado;
- que la pieza de Sopesa va en la sección «anuncios»;
- los dos editoriales que amplifican la carta de la Cámara;
- que no hay editorial en ninguna vuelta presidencial;
- «unas 50» por 43;
- `casawelcome.com`, que no está caído sino en venta;
- y la causalidad del «no se podía preguntar».

**Errores de la propia ficha (`fichas/el-isleno.md`), para no repetirlos:**
- **«NIT / razón social: no constan» y «No aparece en los espejos del RUES»:** el RUES abierto la devuelve por razón social y por NIT. Es el mismo fallo de método que en Al Aire Noticias, en la misma fecha.
- **«Propietario / director: no constan»:** el representante legal consta. El director no, y los socios tampoco.
- **No cita la URL ni el feed**, aunque `MEDIOS_CANDIDATOS_DEPARTAMENTOS.md:53` y `COBERTURA_DEPARTAMENTAL.md:110` ya los tenían.
- **«es el único candidato del archipiélago»** y **«su ausencia en el catálogo se ve el doble»:** caducaron el 2026-08-14, con el alta de The Archipielago Press, cinco días después de la ficha.
- **No hay contratación pública**: la regla es del 2026-10-07, después de la ficha. **Y no hay voz de la casa**, aunque tiene 43 editoriales en 12 meses.
- **«si el medio es raizal o continental» como pregunta de propiedad:** no se puede resolver con el origen étnico de los titulares (DATOS PERSONALES; decisión de El Morichal, 2026-10-10). Se reformula como agenda.
- **Lo que tenía bien:** «Casa Editorial Welcome», el copyright «2010», las ediciones en Issuu, que no hay página de equipo y que «publica al día».

---

**Propuesta para la firma**

**Alta: sí. Valor: 0,00, provisional y sin firmar.**
- **Regla 3:**
  - el nivel 1 es parcial: sociedad, NIT, estado y representante legal, sin socios;
  - no hay nivel 3;
  - el nivel 2 no existe, porque el medio no está ingerido.
- **Evidencia editorial histórica:** no aplica. Hay 0 piezas con postura en 43 editoriales, y la regla no tiene piezas que contar.
- **Regla 2:** la banda mixta. La continuidad de Managua (2 piezas antes y 1 después) se anota como nivel 5.
- **Por qué alta y no candidatura:**
  - tiene el mismo nivel 1 con el que entró Al Aire Noticias;
  - el feed está vivo, fechado y dentro del techo;
  - tiene voz de la casa propia y semanal;
  - y es la segunda voz de un departamento cuyo único medio está en +0,30.
- **No se firma** hasta conocer los socios (cola de certificados, después del de prueba) y tener corpus. Ver la decisión 6.

**Bloque propuesto para `shared/mediaRegistry.js`** (no escrito en código):

```js
    {
        /**
         * EL ISLEÑO (San Andrés) — alta propuesta en el ciclo 2, tanda 7
         * (2026-10-10). SEGUNDO MEDIO DEL ARCHIPIÉLAGO, tras The Archipielago
         * Press (+0,30): rompe la dependencia de una sola voz.
         *
         * EL DOMINIO ES UN IDN, elisleño.com, y aquí va en PUNYCODE
         * (xn--elisleo-9za.com): así lo devuelve `new URL(…).hostname`, con el
         * que comparan canonicalizeLink y extractImage; la CSP solo admite
         * hosts ASCII, y csp.test.js arma `https://*.${domain}` desde aquí.
         * elisleno.com, sin eñe, no existe (NXDOMAIN; RDAP 404, 2026-10-10).
         * El perfil del mapa pinta `domain` tal cual: ver la decisión de
         * presentación en la resolución.
         *
         * Joomla 1.5 detrás de Cloudflare y LiteSpeed. El feed trae 10 ítems,
         * unos dos días al ritmo del medio, con fechas RFC 822 y en orden de
         * portada, no cronológico. Tras una ráfaga de unas 50 peticiones, el
         * sitio respondió «Bot Verification» (403), feed incluido: comprobarlo
         * desde la IP de la ingesta antes del alta.
         *
         * Lo edita CASA EDITORIAL WELCOME S.A.S (NIT 900475712), cuyo único
         * contratante en SECOP I es la Cámara de Comercio de San Andrés. Ver
         * fichas/el-isleno.md.
         */
        id: 'el-isleno', name: 'El Isleño', shortName: 'El Isleño',
        domain: 'xn--elisleo-9za.com', departamento: 'Archipiélago de San Andrés', country: 'CO', group: 'Regional Archipiélago',
        bias: 0.0, factuality: null, reviewedAt: null,
        biasRationale: 'Diario digital e impreso del Archipiélago de San Andrés, segundo del departamento en el catálogo. Lo edita Casa Editorial Welcome S.A.S. (NIT 900475712, activa), cuyo representante legal consta en el RUES; no constan los socios. Su contratante público recurrente es la Cámara de Comercio de San Andrés (14 contratos desde 2019). Tiene editorial semanal propio, de agenda local y cívica: en 12 meses, 0 piezas con postura en el eje nacional, ningún editorial electoral, y la misma exigencia sobre Managua al gobierno saliente y al entrante. Orientación mixta provisional por ausencia de evidencia, no por evidencia de equilibrio — ver fichas/el-isleno.md.',
        feed: { url: 'https://xn--elisleo-9za.com/index.php?format=feed&type=rss', via: 'direct', category: 'Política' },
        imageHosts: ['xn--elisleo-9za.com'],
    },
```

- `group`: «Regional Archipiélago», como Archipiélago Press y como Al Aire, que tiene sociedad conocida y va como «Regional Arauca». La otra opción sería «Casa Editorial Welcome», como El Morichal lleva su corporación. Se deja la regional por coherencia con el caso más parecido.
- **`vercel.json`, `img-src`:** añadir `https://*.xn--elisleo-9za.com https://xn--elisleo-9za.com`. Lo exige `csp.test.js` («cubre el dominio de todo medio que puede traer imagen en su feed»).

**Bloque propuesto para `shared/mediaOwnership.js`** (no escrito en código):

```js
    'el-isleno': {
        ownerType: null,
        holdings: [
            'Lo edita CASA EDITORIAL WELCOME S.A.S: «elisleño.com es un producto de la Casa Editorial Welcome. todos los derechos reservados 2010» (pie de su web, 2026-10-10). RUES, datos.gov.co c82u-588k, consultado el 2026-10-10: NIT 900475712-9, Cámara de Comercio de San Andrés, matrícula 32677 del 08-11-2011, renovada el 30-03-2026, ACTIVA, S.A.S., CIIU 7310 (publicidad) y 5911, inscrita como proponente. Representante legal: Eduardo Gabriel Lunazzi (así en el RUES). El RUES abierto no publica accionistas.',
            'La misma casa publica la edición impresa de El Isleño («EL ISLEÑO 233 by Casa Editorial Welcome», Issuu, 08-09-2026) y las revistas turísticas Welcome Caribe y Welcome San Andrés, enlazadas desde su web.',
            'Tiene editorial semanal propio, firmado «Editorial»: 43 piezas entre el 10-10-2025 y el 10-10-2026, casi todas de domingo. Su agenda es local y cívica: aeropuerto, salud, violencia, Seaflower, residuos, kriol, Emancipation Week y Managua.',
        ],
        notes: [
            'SE CONOCE LA SOCIEDAD Y A SU REPRESENTANTE LEGAL, NO A LOS SOCIOS NI A QUIEN DIRIGE LA REDACCIÓN. El sitio no publica equipo; el feed firma «(Redacción)». Que el representante legal sea el dueño o el director no consta, y suponerlo sería inventarlo.',
            'Contratación pública (SECOP I y II, NIT 900475712, consultado 2026-10-10): 2 contratos por $8.200.000 contratados en los últimos 12 meses (2025-10-10 → 2026-10-10); 15 por $64.313.333 en total desde 2019. SECOP I: 14 por $61.513.333 (2019-2026), todos con la Cámara de Comercio de San Andrés, Providencia y Santa Catalina, por publicidad y difusión; uno de ellos (ODS 012, 09-08-2024) nombra el «PORTAL WEB EL ISLEÑO.COM». SECOP II: 1 por $2.800.000 con Providence and Kettlina Utilities Company SAS ESP (16-03-2026), más otro de $2.300.000 de la misma empresa sin firmar («enviado Proveedor»). Ninguno con la Gobernación, las alcaldías ni la Nación. La Cámara de Comercio es una entidad privada con funciones públicas, no un gobierno; el medio la cubre. En SECOP II el NIT figura con el dígito de verificación pegado (9004757129): la consulta por el NIT sin DV devuelve 0.',
            'TENSIÓN DECLARADA (desvelamiento, no acusación): la Cámara de Comercio es su contratante recurrente desde 2019, y dos editoriales de septiembre de 2026 (06-09 y 20-09) respaldan una carta de gremios que ella firma, sin mencionar la relación. Publica además, en su sección «Anuncios», piezas de Sopesa, la empresa de energía de las islas, y en la portada lleva pauta de hoteles y de Decameron. Que alguna pieza concreta sea pagada no consta.',
            'TENSIÓN DECLARADA, EJE LOCAL: el editorial «Rendición de cuentas, ejercicio contra viento y marea» (29-03-2026) es favorable al gobernador Nicolás Gallardo Vásquez («evidencia una administración enfocada en la inversión social y la infraestructura»), pese a la nulidad electoral que el propio texto menciona. No consta contrato con la Gobernación. The Archipielago Press, el otro medio del departamento, fiscaliza al mismo gobernador.',
            'SI ES UN MEDIO «RAIZAL O CONTINENTAL» NO SE RESUELVE POR EL ORIGEN DE SUS TITULARES, que es un dato sensible (Ley 1581). Lo comprobable es la agenda: editoriales sobre el kriol (22-02-2026), Emancipation Week (02-08-2026) y los pescadores raizales ante Nicaragua (05-04 y 09-08-2026).',
        ],
        sources: [
            'https://xn--elisleo-9za.com/',
            'https://xn--elisleo-9za.com/index.php?format=feed&type=rss',
            'https://xn--elisleo-9za.com/index.php?option=com_content&view=category&layout=blog&id=48&Itemid=85',
            'https://issuu.com/el_isleno/docs/el_isle_o_233',
            'https://www.datos.gov.co/resource/c82u-588k.json?$select=camara_comercio,matricula,razon_social,nit,digito_verificacion,organizacion_juridica,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,cod_ciiu_act_econ_pri,cod_ciiu_act_econ_sec,representante_legal,inscripcion_proponente,fecha_actualizacion&nit=900475712',
            'https://www.datos.gov.co/resource/f789-7hwg.json?$select=numero_de_constancia,numero_de_proceso,nombre_entidad,fecha_de_firma_del_contrato,fecha_fin_ejec_contrato,cuantia_contrato,valor_total_de_adiciones,modalidad_de_contratacion,estado_del_proceso,nom_razon_social_contratista,detalle_del_objeto_a_contratar&identificacion_del_contratista=900475712',
            'https://www.datos.gov.co/resource/jbjy-vk9h.json?$select=id_contrato,nombre_entidad,proveedor_adjudicado,fecha_de_firma,fecha_de_fin_del_contrato,valor_del_contrato,estado_contrato,objeto_del_contrato&documento_proveedor=9004757129',
        ],
        verifiedAt: null,

        // ── Ausencia declarada ──────────────────────────────────────────────
        consultadoEl: '2026-10-10',
        buscadoEn: [
            {
                fuente: 'Pie y portada del sitio',
                resultado: '«elisleño.com es un producto de la Casa Editorial Welcome. todos los derechos reservados 2010». Sin página de equipo ni de «quiénes somos». El enlace «Casa Editorial Welcome» lleva a casawelcome.com, que hoy redirige a una página de dominio en venta; welcomesanandres.com dice «Coming Soon» (2026-10-10).',
                url: 'https://xn--elisleo-9za.com/',
            },
            {
                fuente: 'RUES abierto (datos.gov.co c82u-588k), por razón social y por NIT',
                resultado: 'CASA EDITORIAL WELCOME S.A.S, NIT 900475712, matrícula 32677, ACTIVA, renovada el 30-03-2026; representante legal Eduardo Gabriel Lunazzi; sin socios (2026-10-10). La ficha del 2026-08-09 decía que no aparecía en los espejos del RUES: fallo de método, no del registro. GRUPO WELCOME S.A. (agencia de viajes, matrícula 28606) tiene otro representante legal, y no consta relación.',
                url: 'https://www.datos.gov.co/resource/c82u-588k.json?$select=razon_social,nit,matricula,estado_matricula,ultimo_ano_renovado,representante_legal&nit=900475712',
            },
            {
                fuente: 'SECOP I (f789-7hwg) y SECOP II (jbjy-vk9h), por NIT con y sin dígito de verificación, 2026-10-10',
                resultado: 'SECOP I por 900475712: 14 contratos, todos con la Cámara de Comercio de San Andrés. SECOP II por 900475712: 0; por 9004757129: 2 (Providence and Kettlina Utilities Company SAS ESP, uno de ellos sin firmar). Las consultas se citan con $select para no mostrar el documento del representante legal.',
                url: 'https://www.datos.gov.co/resource/f789-7hwg.json?$select=numero_de_constancia,nombre_entidad,fecha_de_firma_del_contrato,cuantia_contrato&identificacion_del_contratista=900475712',
            },
            {
                fuente: 'Sección Editorial del medio (categoría 48), 12 meses',
                resultado: '43 editoriales firmados «Editorial» entre el 10-10-2025 y el 10-10-2026. Ninguno nombra a un director ni a los dueños. El del 23-11-2025 habla desde «la dirección de esta Casa Editorial», sin nombre.',
                url: 'https://xn--elisleo-9za.com/index.php?option=com_content&view=category&layout=blog&id=48&Itemid=85',
            },
            {
                fuente: 'Las2Orillas, 11-08-2016',
                resultado: '«El Isleño, periódico quincenal dirigido por Billy Lunazzi». Tiene diez años: es historia, no dice quién dirige hoy. Que sea la misma persona que el representante legal no está probado (en el RUES hay otra persona con ese apellido y ese nombre de pila).',
                url: 'https://www.las2orillas.co/pa-que-voy-a-salir-al-mar/',
            },
        ],
        falta: [
            'Los socios o accionistas y el beneficiario final: el certificado de existencia y representación de la Cámara de San Andrés, en la cola después del de prueba.',
            'Quién dirige hoy la redacción.',
            'Si Grupo Welcome S.A. tiene relación de capital con la editora.',
            'La naturaleza (pública, mixta o privada) de Providence and Kettlina Utilities Company SAS ESP.',
            'Si las piezas de la sección «Anuncios» y la pauta de la portada incluyen a entidades que el medio cubre en su información.',
        ],
    },
```

**Textos a corregir** (si el responsable editorial aprueba el alta):
1. **`fichas/el-isleno.md`** pasa de ficha de candidatura a ficha de medio:
   - **Cabecera:**
     - «Valor propuesto» → «**0,00** · Orientación mixta — provisional, sin firmar, por ausencia de evidencia»;
     - añadir «Revisión: ciclo 2, tanda 7, 2026-10-10» y «Dominio: elisleño.com (`xn--elisleo-9za.com`)».
   - **«Nivel 1 — Un nombre comercial y nada más»** se sustituye por la tabla del `holdings[0]` de arriba, con fila de socios «no constan» y fila de director «no consta; el feed firma "(Redacción)"». Retirar «No aparece en los espejos del RUES…».
   - **Sección nueva «Contratación pública»:** el `notes[1]` de arriba, en el formato del protocolo.
   - **Sección nueva «Voz de la casa — barrido de 12 meses (2026-10-10)»:**
     - 43 editoriales y 30 leídos;
     - la tabla de esta resolución, o un enlace a ella;
     - 0 piezas con postura, sin editorial en ninguna vuelta presidencial y la continuidad de Managua;
     - «la regla no tiene piezas que contar».
   - **Sección «Tensiones»:** los `notes[2]` y `notes[3]`.
   - **«Nivel 2»:** «No ingerido hasta el alta» y el estado del feed (10 ítems, RFC 822, orden de portada, unas 5 piezas al día, 403 «Bot Verification» tras una ráfaga).
   - **«POR QUÉ NO SE PROPONE NÚMERO»** → «POR QUÉ 0,00», con la razón de la propuesta.
   - **«LO QUE HACE ESTE CASO DISTINTO»:**
     - retirar «es el único candidato del archipiélago» y «su ausencia en el catálogo se ve el doble»;
     - y escribir «Desde el 2026-08-14 el departamento tiene un medio, The Archipielago Press (+0,30); este sería el segundo, con una línea local opuesta frente a la Gobernación».
     - Sustituir el párrafo «raizal o continental» por el `notes[4]`.
   - **REFUTACIÓN:**
     - el punto 1 queda «solo por los socios»;
     - el punto 3 se marca como cumplido, con la comparación de esta resolución;
     - nuevos: «Si un barrido posterior encuentra asimetría en la voz de la casa a los dos lados del 07-08-2026, con los mínimos de la regla» y «Si aparece contrato con la Gobernación o pauta oficial no rotulada».
2. **`fichas/LEEME.md:45`**: si hay alta, la fila sale de la tabla de candidaturas (pasa a ser ficha de medio) y se actualiza el recuento de «Cómo contar bien». Si no hay alta: «Nivel 1 parcial (RUES); pendiente de decisión de alta».
3. **`MEDIOS_CANDIDATOS_DEPARTAMENTOS.md:197`**: «**sin número**: solo un nombre comercial» → «0,00 provisional, sin firmar · editora en el RUES (NIT 900475712), contratista recurrente de la Cámara de Comercio de San Andrés · ciclo 2, 2026-10-10». La línea 53 se queda: el feed es correcto.
4. **`COBERTURA_DEPARTAMENTAL.md:110`**: anotar que San Andrés quedó cubierto con The Archipielago Press el 2026-08-14 y que El Isleño sería el segundo.
5. **`fichas/archipielago-press.md`, «POR QUÉ ENTRA»:** «Sí es la única del departamento en el catálogo» → «Fue la primera del departamento en el catálogo; desde el [fecha del alta], El Isleño es la segunda».

**Lo que NO entra como hecho:**
- que «Billy Lunazzi» (2016) sea el representante legal, ni ningún parentesco entre las personas de apellido Lunazzi;
- que el representante legal sea socio, dueño o director;
- que Grupo Welcome S.A. tenga relación con la editora;
- que los dos editoriales del aeropuerto sean pago o contraprestación del contrato con la Cámara;
- que las piezas de Sopesa sean pagadas: van en «Anuncios», pero el pago no consta;
- el carácter raizal o continental de los dueños;
- la naturaleza pública de P&K;
- el contrato de $2.300.000 de SECOP II como contratado.

**¿Aviso de quien dirige?** No procede. No se sabe quién dirige la redacción, y no consta candidatura ni cargo público del representante legal.

**Decisiones para el responsable editorial:**
1. **Alta.** Recomendación: **sí, con 0,00 provisional y sin firmar**. Mismo nivel 1 que Al Aire Noticias, feed vivo y segunda voz del departamento. El argumento en contra: es la segunda casa del archipiélago con relación contractual recurrente con una entidad que cubre, y su único texto con postura local es complaciente con el gobernador.
2. **«0,00 provisional» o «0,00 con evidencia».** Recomendación: **provisional**. La continuidad de Managua son 3 piezas, y la regla no tiene piezas que contar, como en El Morichal. Chocó 7 Días tenía 15 piezas de fiscalización simétrica.
3. **Cómo se nombra la relación con la Cámara de Comercio.** Recomendación: «**contratante recurrente** (14 contratos desde 2019)», y no «dependencia», que afirma algo del medio que no consta. Es el criterio de Diario de Cundinamarca.
4. **El dominio IDN.** Recomendación: **punycode en el registro** (bloque de arriba). Para que el mapa no pinte «xn--elisleo-9za.com», o se acepta así, o se muestra con `url.domainToUnicode` en `MediaMap.jsx:1179`, o se añade un campo de presentación. Es una decisión de código, pequeña y aparte.
5. **Enlaces de datos.gov.co que muestran el documento del representante legal.** Recomendación: **citar con `$select`**, como en los bloques de arriba. **Aviso:** las fuentes de fichas ya cerradas con consultas por NIT sin `$select` tienen el mismo problema. Por ejemplo, Al Aire Noticias cita `c82u-588k.json?nit=901856069` y `f789-7hwg.json?identificacion_del_contratista=901856069`, y las filas de estos conjuntos traen el documento del representante legal. Conviene una revisión general antes de publicar el método.
6. **Ingesta y firma.**
   - **Antes de activar el feed:** comprobarlo desde la IP de la ingesta (`scripts/verifyFeeds.mjs`). El sitio respondió «Bot Verification» (403) tras una ráfaga.
   - **La firma:** cuando consten los socios y haya corpus. El precedente de El Morichal (40 días con nivel 1 documentado) vale como referencia, no como plazo automático.

**Avisos.**
- El sitio bloqueó a este verificador tras unas 50 peticiones. Un barrido futuro del archivo tiene que ir más despacio.
- La resolución no tocó código ni fichas, y no hizo commits.
