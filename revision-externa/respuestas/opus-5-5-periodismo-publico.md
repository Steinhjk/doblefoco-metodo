# Respuesta — Claude Opus 5.5 sobre Periodismo Público

| | |
|---|---|
| **Modelo** | Claude Opus 5.5 |
| **Versión exacta** | `claude-opus-5-5` |
| **Fecha de la consulta** | 2026-10-08 |
| **Quién la hizo** | Claude Code, a petición del responsable editorial (ciclo 2, fase 2, tanda 4; revisor de la misma casa que el autor de las fichas, ver DECISIONES.md 2026-10-07) |
| **¿Tuvo acceso a la red?** | sí |

> **Se pega LITERAL lo que devolvió el modelo, sin editar ni resumir.** Si se
> recorta, se pierde justo lo que pueda incomodar. Los comentarios nuestros van
> al final, en la sección de resolución, claramente separados.
>
> **Edición:** retirados enlaces que pueden mostrar documentos de identidad (PROTOCOLO, Datos personales, 2026-10-10).

---

## RESPUESTA LITERAL

```
DECLARACIÓN PREVIA DE CONFLICTO
Soy Claude Opus 5.5 (claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Para compensarlo he buscado sobre todo en fuentes que la ficha NO usa (RUES abierto, SECOP I y II, la API pública del propio sitio y piezas concretas de 2026), y he citado desde el HTML o JSON crudo descargado con curl, no desde resúmenes. Fecha de todas mis comprobaciones: 2026-10-08. No he leído ningún otro archivo del repositorio: solo el envío.

MÉTODO Y DÓNDE BUSQUÉ
- robots.txt leído antes de descargar: periodismopublico.com (solo excluye /wp-admin/ para *; no menciona ClaudeBot, Claude-Web ni anthropic-ai), www.informacolombia.com (Allow: /, excluye /api/), www.datos.gov.co (sin reglas para ClaudeBot/Claude-Web/anthropic-ai; solo rutas de navegación/OData). No toqué eltiempo.com ni cambiocolombia.com. No usé Wikipedia (no hay entrada pertinente que necesitara).
- RUES abierto (datos.gov.co, c82u-588k): búsqueda por razón social con "PERIODISMO" y con "CORPORACION HUMANISTA"; luego por numero_identificacion = 901171544 y = 900268977 (igualdad exacta, sin DV).
- SECOP II (jbjy-vk9h), documento_proveedor = 901171544 y = 900268977 (igualdad exacta, sin DV), más búsqueda de respaldo por proveedor_adjudicado LIKE '%PERIODISMO PUBLICO%' / '%CORPORACION HUMANISTA%'.
- SECOP I (f789-7hwg), identificacion_del_contratista = 901171544 y = 900268977, más búsqueda por nom_razon_social_contratista.
- Sitio del medio: /quienes-somos/ (HTML crudo); listado de categorías del desplegable del sitio; API REST pública de WordPress (/wp-json/wp/v2/posts) por categorías Editorial (243), Informe Alcaldía (47), Publicidad (6), Opinión ciudadana (41), Opinión (9) y Política (8), y búsquedas internas "Cepeda", "Espriella", "Petro" desde 2026-04-01. Leí en crudo cinco piezas de 2026 (enlaces abajo).
- informacolombia.com: la misma página que cita la ficha, en crudo.
- Buscador web: NO lo usé, para no gastar cupo compartido; todo lo de abajo sale de fuentes primarias descargadas. Lo que habría requerido buscador (prensa de terceros sobre el medio, Cámara de Comercio de Soacha) queda como laguna declarada.
- Ley 1581: los registros de RUES y SECOP traen números de cédula del representante legal; los he omitido. No reproduzco teléfonos ni direcciones de personas naturales.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré ningún registro de venta, fusión ni escisión. Lo que SÍ cambió en el registro: la matrícula mercantil 2689863 de PERIODISMO PUBLICO SAS figura CANCELADA en la Cámara de Comercio de BOGOTÁ con "fecha_cancelacion":"20260816" y ACTIVA en la "camara_comercio":"SOACHA" ("codigo_camara":"58"), mismo NIT y misma matrícula. Es un traslado de registro (inferencia: a la nueva cámara con jurisdicción en Soacha), no un cambio de dueño. Fuente: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (consultado 2026-10-08; registro con "fecha_actualizacion":"2026/08/21").
  Además: "ultimo_ano_renovado":"2024", "fecha_renovacion":"20241007". La matrícula no consta renovada para 2025 ni 2026 en el dato abierto.
  Los socios no aparecen en el RUES abierto. No sé quién posee las acciones.

- La persona que la ficha nombra como director, ¿sigue viva y en el cargo? (2026-10-08)
  La página /quienes-somos/ sigue nombrando "Director: Ariel González". Pero el HTML crudo de esa página declara "datePublished":"2009-05-01" y "dateModified":"2020-02-29T22:00:03-05:00". Es decir, el equipo que lista la ficha está sin actualizar desde 2020, y la página no sirve para afirmar que hoy siga así. No encontré nada que indique fallecimiento. Por el lado registral, el RUES (registro de Bogotá cancelado el 2026-08-16) da como representante legal a "ARIEL RICARDO GONZALEZ GONZALEZ". El registro activo de Soacha no trae el campo de representante legal en el dato abierto. Que el director y el representante legal sean la misma persona es muy probable por el nombre, pero no está probado documentalmente (homonimia no descartada).

- ¿Quién dirige hoy la redacción?
  Ariel González según /quienes-somos/ (página modificada por última vez el 2020-02-29). Las piezas de 2026 que leí van firmadas "by Periodismo Público" (autor 1 de WordPress), sin nombre de periodista. No encontré una fuente de 2025-2026 que nombre al director.

- ¿Hay un registro mercantil más reciente que la fuente que la ficha cita?
  Sí. La ficha cita un directorio privado (informacolombia). El RUES abierto (c82u-588k) trae el NIT, la matrícula, el representante legal (registro de Bogotá), los códigos CIIU, la fecha de matrícula 2016-05-23 y el traslado a la cámara de Soacha en agosto de 2026. No es un certificado de existencia con composición accionaria, pero es un primario oficial más reciente que la fuente de la ficha.

## OBJECIONES

OBJECIÓN 1 — «NIT: no publicado» es falso, y lo publica la propia fuente de la ficha.
- QUÉ afirma la ficha: "NIT | no publicado".
- POR QUÉ: la misma página de informacolombia que la ficha cita publica el NIT. En el HTML crudo: "NIT" / "9011715446" y en su JSON-LD "taxID":"9011715446". El RUES abierto lo confirma: "numero_identificacion":"901171544","digito_verificacion":"6","razon_social":"PERIODISMO PUBLICO SAS". La ficha pone como primera tarea pendiente («LO QUE FALTA» 1) algo que ya estaba en su fuente.
- FUENTE: https://www.informacolombia.com/directorio-empresas/informacion-empresa/periodismo-publico-sas (consultado 2026-10-08); [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (consultado 2026-10-08).
- NIVEL: propiedad (registro).

OBJECIÓN 2 — «El certificado de la Cámara de Comercio de Bogotá, que cubre Soacha» ya no es el trámite correcto.
- QUÉ afirma la ficha: (LO QUE FALTA 1) que hay que pedir el certificado a la Cámara de Comercio de Bogotá, «que cubre Soacha».
- POR QUÉ: en el RUES abierto, la matrícula en Bogotá ("codigo_camara":"04") está "estado_matricula":"CANCELADA", "fecha_cancelacion":"20260816". La misma matrícula 2689863 está "ACTIVA" en "camara_comercio":"SOACHA" ("codigo_camara":"58"). El hecho cae dentro de los últimos 12 meses y dos días después del alta de la ficha (2026-08-14). Hecho: el traslado de registro. Inferencia: el certificado vigente hay que pedirlo ahora a la cámara de Soacha. Al mismo registro: "ultimo_ano_renovado":"2024". Sin renovación de 2025 ni de 2026, un certificado podría salir con advertencia de matrícula no renovada (inferencia: no lo he comprobado).
- FUENTE: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (consultado 2026-10-08).
- NIVEL: propiedad (registro).

OBJECIÓN 3 — «Qué relación conserva hoy la Corporación Humanista»: la entidad está cancelada desde 2023, y su representante legal tiene el mismo nombre que la administradora de contenido del medio.
- QUÉ afirma la ficha: "No consta cómo se pasó de aquella corporación a la S.A.S. actual, ni si la corporación conserva participación" (LO QUE FALTA 3). La ficha atribuye el origen a "búsqueda web", sin enlace.
- POR QUÉ: el RUES abierto tiene una "CORPORACION HUMANISTA" (razón social exacta), Cámara de Comercio de Bogotá, NIT 900268977, "tipo_sociedad":"ENTIDAD SIN ANIMO DE LUCRO", "fecha_matricula":"20090223", "estado_matricula":"CANCELADA", "fecha_cancelacion":"20230303", "representante_legal":"DIANA PATRICIA GOMEZ FLOREZ". La página /quienes-somos/ del medio lista como "Administradora de contenido: Diana Patricia Gómez". Hechos: la entidad de ese nombre, matriculada en 2009 (el año que la ficha da como origen), está cancelada. Inferencias, que no he probado: (a) que sea la misma Corporación Humanista que la ficha menciona; (b) que su representante legal sea la misma persona que trabaja en el medio. Hay coincidencia de nombre y año, pero la homonimia no está descartada. Si (a) se confirma, la corporación no puede «conservar participación» como entidad activa. Si (b) se confirma, el vínculo corporación–medio pasa por personas y no se ha disuelto, y la ficha debería decirlo así. El RUES registra además "inscripcion_proponente":"000000054043": la corporación estuvo inscrita en el Registro Único de Proponentes, el registro para contratar con el Estado.
- FUENTE: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (consultado 2026-10-08); https://periodismopublico.com/quienes-somos/ (consultado 2026-10-08; la página declara "dateModified":"2020-02-29").
- NIVEL: propiedad (registro).

OBJECIÓN 4 — «No se ha podido establecer de qué vive el medio» se cae en parte: hay contratación pública documentada para publicar notas favorables a una entidad del departamento, y el sitio tiene una sección de publicidad con anunciantes oficiales.
- QUÉ afirma la ficha: "no se ha podido establecer de qué vive el medio", y el peso de la pauta de Soacha y de la Gobernación de Cundinamarca queda como laguna.
- POR QUÉ: en SECOP I, identificacion_del_contratista = 901171544, hay un contrato: entidad "AGENCIA LOGISTICA DE GESTION INMOBILIARIA Y SERVICIOS DE CUNDINAMARCA" (orden "TERRITORIAL DEPARTAMENTAL DESCENTRALIZADO"), contrato "CPS 394 DE 2021", firmado el 2021-10-01, por $5.400.000, con este objeto: "PRESTACION DE SERVICIOS PARA LA DIFUSION DE NOTAS PERIODISTICAS QUE EXPONGAN LOS AVANCES PROPIOS DE LA EMPRESA INMOBILIARIA Y DE SERVICIOS LOGISTICOS DE CUNDINAMARCA"; estado del proceso "Celebrado". El contratista es "PERIODISMO PUBLICO S.A.S." y el representante legal, el mismo nombre que da el RUES. Tiene más de 12 meses, así que no es conducta del presente. Lo cito porque refuta que el modelo de ingresos sea desconocible: el medio ha vendido a una entidad del departamento la publicación de notas sobre sus avances. Además, la categoría "Publicidad" del sitio tiene piezas con nombre de entidades públicas ("Secretaría de Hacienda", "Banner ESE-3-", "Marca Cundinamarca", "ESE Soacha", "Gif Hacienda"), todas de 2017 a 2019. Y la categoría "Informe Alcaldía" tuvo una entrada el 2024-01-01 ("No se pierda la posesión del nuevo alcalde de Soacha 2024 – 2027"). Hecho: hay pauta oficial en el pasado. Inferencia que no he probado: que siga hoy.
  Contratos de los últimos 12 meses (2025-10-08 a 2026-10-08): NINGUNO en SECOP II ni en SECOP I, ni por el NIT 901171544 ni por el 900268977 (igualdad exacta, sin DV), ni buscando por nombre del proveedor. No hay valor_pagado que reportar. Sin contratos a nombre de la sociedad no se puede excluir la pauta pagada por medio de agencias o centrales de medios, que en SECOP figura a nombre de la agencia.
- FUENTE: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (consultado 2026-10-08); proceso en [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (enlace que da el propio registro; no lo abrí); https://periodismopublico.com/wp-json/wp/v2/posts?categories=6 y ?categories=47 (consultados 2026-10-08).
- NIVEL: registro externo (contratación pública); conducta observable (sección de publicidad).

OBJECIÓN 5 — Encuadre asimétrico en la elección presidencial de 2026: una pieza laudatoria, sin firma y sin etiqueta de contenido pagado, dedicada al coordinador regional de la campaña ganadora.
- QUÉ afirma la ficha: "no hay nada que sitúe a este medio en el eje", y declara solo un método («Denuncia Ciudadana, Investigación Periodística y Opinión Pública»).
- POR QUÉ: el 2026-06-27, en las categorías "Cundinamarca, Política, Principales Noticias", el medio publicó "La mente brillante que lideró la victoria de Abelardo de la Espriella en Cundinamarca", firmada "Periodismo Público". Citas literales: "hubo una estrategia territorial sólida, un equipo comprometido y una dirección política efectiva"; "haber ejercido exitosamente su labor como gobernador encargado en el departamento del Caquetá"; "Su perfil combina experiencia técnica, liderazgo territorial y una profunda vocación de servicio"; "La experiencia, capacidad de gestión y conocimiento institucional de Fabio Parra Beltrán fueron determinantes". La foto es "Foto: campaña Abelardo de la Espriella". En la búsqueda interna del sitio por "Cepeda" desde el 2026-04-01 no aparece ninguna pieza equivalente sobre la campaña perdedora; solo notas de resultados y disturbios. El 2026-08-08 publicó "¿Por qué el exsenador Inti Asprilla terminó como notario segundo de Soacha? Acá las razones", con frases como "quemado en las elecciones parlamentarias", "Muchos catalogan el nombramiento de Asprilla como un premio a la lealtad y respaldo al gobierno Petro" y "No hay que olvidar que Asprilla se dedicó a defender a Petro".
  Hecho: una pieza de perfil elogioso de un operador de la campaña ganadora, sin firma ni etiqueta de publirreportaje. Inferencia, no probada: por su tono y su forma es probable que sea contenido pagado o enviado por la campaña o por el interesado. Si fuera así, sería evidencia sobre el modelo de ingresos más que sobre la línea. Si no lo fuera, sería encuadre asimétrico entre candidatos, que según el contexto del envío la regla del polo fijo NO neutraliza. En ninguno de los dos casos sostiene que "no hay nada": hay al menos una pieza que la ficha debe registrar y explicar. Una sola pieza NO basta para mover el número (ver «Evidencia que no mueve el número»); objeto la afirmación de vacío, no el 0,00.
- FUENTE: https://periodismopublico.com/la-mente-brillante-que-lidero-la-victoria-de-abelardo-de-la-espriella-en-cundinamarca (2026-06-27; consultado 2026-10-08); https://periodismopublico.com/exsenador-inti-asprilla-es-el-nuevo-notario-segundo-de-soacha (2026-08-08; consultado 2026-10-08); https://periodismopublico.com/wp-json/wp/v2/posts?search=Cepeda&after=2026-04-01T00:00:00 (consultado 2026-10-08).
- NIVEL: hecho editorial de los últimos 12 meses / conducta observable.

OBJECIÓN 6 — El equipo «de hoy» viene de una página sin actualizar desde 2020.
- QUÉ afirma la ficha: en "Nivel 1 — Quién lo edita, hoy" presenta director y equipo (contenidos, webmaster, reportería) como vigentes, y dice "Hay ... equipo con nombres y cargos".
- POR QUÉ: el JSON-LD de /quienes-somos/ declara "dateModified":"2020-02-29T22:00:03-05:00". Las piezas de 2026 que leí van firmadas por el usuario genérico "Periodismo Público" (author 1), sin nombre de reportero. Nada en el sitio acredita que esa plantilla siga vigente en 2026. Según la regla del presente, la ficha no puede usarla como «hoy» sin decir la fecha.
- FUENTE: https://periodismopublico.com/quienes-somos/ (consultado 2026-10-08).
- NIVEL: declaración del propio medio (fechada).

## LO QUE NO PUDE VERIFICAR

- Los accionistas de PERIODISMO PUBLICO SAS: el RUES abierto no trae socios. Haría falta el certificado de existencia de la cámara de Soacha (de pago) o el documento de constitución. Busqué en RUES abierto por NIT y razón social.
- Si Ariel González (director, según la web de 2020) y "ARIEL RICARDO GONZALEZ GONZALEZ" (representante legal en el RUES y en SECOP I 2021) son la misma persona. Es muy probable por el nombre, pero no está probado. Tampoco pude comprobar si es socio.
- Si la "CORPORACION HUMANISTA" con NIT 900268977 es la entidad de origen que menciona la ficha, y si su representante legal es la misma Diana Patricia Gómez del medio. Ni la ficha ni /quienes-somos/ mencionan la corporación; busqué "humanista" en el HTML de /quienes-somos/ sin resultado.
- Pauta vigente de la Alcaldía de Soacha o de la Gobernación de Cundinamarca en 2025-2026: SECOP I y II no dan nada por el NIT ni por el nombre. No consulté los portales de transparencia de la Alcaldía de Soacha ni las órdenes de compra de Colombia Compra Eficiente (Tienda Virtual), que están fuera de estos datasets.
- Si la pieza del 2026-06-27 sobre Fabio Parra Beltrán es contenido pagado: el HTML no tiene etiqueta de patrocinio. No usé el buscador para comprobar si el mismo texto apareció en otros medios, lo que indicaría que es un comunicado.
- Que la matrícula no se renovó en 2025-2026: lo dice el campo "ultimo_ano_renovado":"2024" del dato abierto, pero el dataset puede ir con retraso respecto del certificado.

## LO QUE FALTA

1. El NIT (901171544-6) y la referencia al RUES abierto, en vez de "no publicado".
2. El traslado de matrícula a la cámara de Soacha (2026-08-16) y la falta de renovación desde 2024.
3. El representante legal según el registro (Ariel Ricardo González González, en el registro de Bogotá), con la cautela de homonimia frente al director.
4. La cancelación de la Corporación Humanista (2023-03-03) si se confirma que es la misma, y la coincidencia de nombre de su representante legal con la administradora de contenido.
5. El contrato SECOP I CPS 394 de 2021 (difusión de notas sobre los avances de una entidad departamental) y la sección "Publicidad"/"Informe Alcaldía" del sitio, como base documental de la pregunta "de qué vive".
6. Un barrido de la cobertura de la campaña presidencial de 2026 (primera y segunda vuelta) y del cambio de gobierno, que incluya la pieza del 2026-06-27 y diga si es pagada o no.
7. Que la sección Editorial existe (18 entradas) y que su última entrada es del 2025-04-12 (ver abajo).

## EVIDENCIA QUE NO MUEVE EL NÚMERO

- La sección Editorial existe (categoría 243, 18 entradas). La última es "Soacha: una sociedad que se desangra en la trinchera de la polarización" (2025-04-12), fuera de la ventana de 12 meses; la anterior es de 2021-07-05. En los últimos 12 meses el medio no ha publicado editoriales, así que no hay endoso editorial en la elección presidencial de 2026. Es conducta de la casa: no tomó partido en editorial. Fuente: https://periodismopublico.com/wp-json/wp/v2/posts?categories=243 (consultado 2026-10-08).
- La sección Opinión tiene en 2026 una sola pieza en la categoría desde mayo: "En Soacha: ¿Emblema = Problema?" (2026-09-12), de tema ambiental y de ordenamiento local. Fuente: https://periodismopublico.com/wp-json/wp/v2/posts?categories=9&after=2026-05-01T00:00:00 (consultado 2026-10-08).
- Después del cambio de gobierno de agosto de 2026 hay titulares de fiscalización al gobierno entrante: "¡Malas noticias para el bolsillo! De la Espriella prepara aumento que pagarán millones de colombianos" (2026-09-09), que atribuye la información a la ministra de Minas; y "Golpe a la 'Paz Total' de Petro: De La Espriella anuncia qué pasará con los grupos criminales" (2026-09-11), que marca distancia con fórmulas como "según su versión" y "según explicó". Hay también notas neutras o de servicio sobre el nuevo gobierno ("¿Subió o no la gasolina? Abelardo De La Espriella reversa aumento de $46 para octubre", 2026-10-02) y una sobre el gobierno saliente ("¿Quiénes se quedaron sin protección? UNP retira esquemas a varios exfuncionarios de Petro", 2026-09-22). Con la regla del polo fijo esto no orienta; lo registro como continuidad de fiscalización a ambos lados, en una muestra pequeña. Fuentes: https://periodismopublico.com/malas-noticias-para-el-bolsillo-de-la-espriella-prepara-aumento-que-pagaran-millones-de-colombianos ; https://periodismopublico.com/golpe-a-la-paz-total-de-petro-de-la-espriella-anuncia-que-pasara-con-los-grupos-criminales (ambas consultadas 2026-10-08).
- "Frenan posesión de Inti Asprilla como notario segundo de Soacha" (2026-09-01) es una nota documental, apoyada en la carta del gobernador, que "Carta: Valora Analitik" acredita, sin adjetivación propia. Fuente: https://periodismopublico.com/frenan-posesion-de-inti-asprilla-como-notario-segundo-de-soacha (consultado 2026-10-08).
- El volumen del sitio lo domina la información local y de servicio: la categoría Soacha tiene 22.356 entradas y Política 1.642 (desplegable de categorías de /quienes-somos/, consultado 2026-10-08). Encaja con un medio hiperlocal más que con un medio de línea nacional.
- El RUES registra como actividad principal el CIIU 6312 (portales web) y como secundaria el 7310 (publicidad). Hecho registral: la sociedad declara la publicidad como actividad. No mueve el eje, pero es pertinente para la pregunta "de qué vive". Fuente: [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (consultado 2026-10-08).

## SIN OBJECIÓN
No aplica: hay objeciones arriba. Al valor 0,00 en sí no le opongo evidencia suficiente para moverlo. Mis objeciones atacan los datos de propiedad e ingresos de la ficha y su afirmación de que "no hay nada" en el eje. No las presento como aval del número.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-08. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** El revisor no copió cédulas, teléfonos ni direcciones de personas naturales (lo declara él mismo y se comprobó buscando en su texto toda cifra de siete o más dígitos: solo hay NIT de sociedades, matrículas, fechas y el número de constancia de SECOP). El texto va íntegro. Esta resolución tampoco escribe ninguna cédula: cuando se dice abajo que dos registros «coinciden en el número de identificación», el cotejo se hizo en local y el número no se reproduce.

**Cómo se verificó.**
- **Sitio del medio.** Se descargaron en crudo el 2026-10-08, con `curl -sL -A "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 Chrome/126.0 Safari/537.36"`, la portada, `/quienes-somos/`, la página de perfil del director, las cinco piezas que cita el revisor y cuatro páginas más que él no vio (abajo). Todas respondieron 200. Las citas se buscaron literalmente en el texto extraído del HTML. Fechas: `datePublished` y `dateModified` del JSON-LD.
- **API pública de WordPress** (`/wp-json/wp/v2/`): categorías 243 (Editorial), 47 (Informe Alcaldía), 6 (Publicidad) y 9 (Opinión); búsquedas «Cepeda», «Espriella», «Jorge Rey», «Gobernación de Cundinamarca», «Licores» y «humanista»; listado de categorías y páginas.
- **Registros**, en datos.gov.co:
  - RUES (`c82u-588k`) por `numero_identificacion=901171544` y `=900268977`, y por razón social («PERIODISMO PUBLICO», «CORPORACION HUMANISTA»);
  - SECOP I (`f789-7hwg`) por `identificacion_del_contratista` y SECOP II (`jbjy-vk9h`) por `documento_proveedor`, con los dos NIT, en **igualdad exacta y sin DV**. Con DV (`9011715446`, `9002689776`) dan 0 en los dos;
  - de respaldo, por nombre de proveedor y, **cosa que el revisor no hizo**, por el nombre de los dos representantes legales que da el RUES.
- **informacolombia.com:** la página respondió **HTTP 429 (demasiadas peticiones) en cuatro intentos** a lo largo de la sesión. Se leyó la copia descargada en esta misma sesión a las 19:51 (antes del bloqueo) y guardada en el directorio temporal. El NIT que publica lo confirma, además, el RUES de forma independiente.
- **Buscador web: SÍ lo hubo** en esta verificación (dos búsquedas). Se usó solo para ver si la pieza del 27-06-2026 sobre Fabio Parra Beltrán aparece en otros medios, lo que indicaría un comunicado. No aparece en los resultados. Eso no prueba que no sea un texto enviado por la campaña: queda como laguna.

**robots.txt, comprobado aquí:**
- periodismopublico.com: «User-agent: * / Disallow: /wp-admin/». No menciona a ClaudeBot, Claude-Web ni anthropic-ai.
- videos.periodismopublico.com (donde están las imágenes de los banners): sin `robots.txt` (404). Solo se pidieron las cabeceras de tres imágenes.
- www.informacolombia.com: «User-Agent: * / Allow: / / Disallow: /api/».
- www.datos.gov.co: solo `Crawl-delay` y exclusiones de `/browse`; ninguna regla para ClaudeBot, Claude-Web ni anthropic-ai.
- contratos.gov.co: no se tocó (el revisor tampoco abrió el enlace del proceso; lo dice).
- No se tocaron eltiempo.com ni cambiocolombia.com (aparecieron en los resultados del buscador y no se abrieron). Wikipedia no se usó.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | «NIT: no publicado» es falso, y lo publica la propia fuente de la ficha | sí | sí | **Aceptada**. El mismo error está en `mediaOwnership.js` («NO publica NIT») |
| 2 | El certificado ya no es de la Cámara de Bogotá: la matrícula se canceló allí y está activa en Soacha | sí | sí | **Aceptada** en los hechos. La inferencia sobre un certificado con advertencia queda sin verificar |
| 3 | La Corporación Humanista está cancelada desde 2023, y su representante legal se llama como la administradora de contenido | sí | los registros, sí; **la identidad, no** | **Aceptada como pista, rechazada como hecho**: homonimia no descartada, tanto de la entidad como de la persona. Pero la verificación encontró un primario que el revisor no vio: los **términos y condiciones del propio sitio** dicen que el portal «es de propiedad de La CORPORACIÓN HUMANISTA» |
| 4 | «No se ha podido establecer de qué vive» se cae en parte: contrato de 2021 para publicar notas favorables y sección de publicidad | sí | sí | **Aceptada**, y **se queda corta**: el representante legal contrata como persona natural la pauta del sitio (cinco contratos que nombran periodismopublico.com) y la difusión de la Alcaldía de Soacha (2024 y 2025), y **hoy** el sitio exhibe tres banners de la Gobernación de Cundinamarca y su licorera. **Se declara como tensión** |
| 5 | Pieza laudatoria, sin firma ni etiqueta, del coordinador en Cundinamarca de la campaña ganadora | sí | sí | **Aceptada** en el hecho: la ficha no puede decir que «no hay nada». **Rechazada** la sub-inferencia «probablemente pagada» (sin prueba). **Declarada como tensión**; no mueve el número |
| 6 | El equipo «de hoy» viene de una página sin actualizar desde 2020 | sí | sí | **Aceptada** |

### Lo verificado, objeción por objeción

**1 · NIT.**
- RUES, literal: «razon_social":"PERIODISMO PUBLICO SAS"», «numero_identificacion":"901171544"», «digito_verificacion":"6"». Exacto.
- informacolombia (copia de las 19:51 del 2026-10-08): el título de la página es literalmente «Periodismo Publico Sas: NIT, teléfono y contacto». El cuerpo trae «NIT» / «9011715446», y el JSON-LD, «"taxID":"9011715446"». Exacto.
- Por tanto, la ficha («**NIT** | **no publicado**») y `mediaOwnership.js` («NO publica NIT, NI representante legal, NI socios») se equivocan sobre su propia fuente. Lo de los socios y el representante legal sí es cierto: informacolombia no los publica.

**2 · Matrícula, Bogotá y Soacha.** RUES por NIT, dos registros con la misma matrícula 2689863:
- «codigo_camara":"04","camara_comercio":"BOGOTA"», «estado_matricula":"CANCELADA"», «fecha_cancelacion":"20260816"», «representante_legal":"ARIEL RICARDO GONZALEZ GONZALEZ"», actualizado «2026/08/16».
- «codigo_camara":"58","camara_comercio":"SOACHA"», «estado_matricula":"ACTIVA"», sin campos de representante legal, actualizado «2026/08/21».
- En los dos: «fecha_matricula":"20160523"», «fecha_renovacion":"20241007"», «ultimo_ano_renovado":"2024"», «organizacion_juridica":"SOCIEDADES POR ACCIONES SIMPLIFICADAS SAS"», CIIU principal 6312 y secundario 7310.
- Todo exacto. «Traslado» es una lectura razonable de dos registros con la misma matrícula, uno cancelado y otro activo; el dato abierto no dice el motivo. Que un certificado salga con advertencia por falta de renovación no se comprobó.

**3 · Corporación Humanista.**
- RUES por NIT 900268977, literal: «razon_social":"CORPORACION HUMANISTA"», Cámara de Bogotá, matrícula 90033781, «tipo_sociedad":"ENTIDAD SIN ANIMO DE LUCRO"», «fecha_matricula":"20090223"», «ultimo_ano_renovado":"2022"», «estado_matricula":"CANCELADA"», «fecha_cancelacion":"20230303"», «inscripcion_proponente":"000000054043"», «representante_legal":"DIANA PATRICIA GOMEZ FLOREZ"». Exacto.
- **Matiz que el revisor no da:** el RUES tiene otras nueve entidades cuyo nombre empieza por «CORPORACION HUMANISTA» (Medellín, Montería, Manizales, Bogotá, Aburrá Sur). Solo una se llama así, sin más. Es un indicio a favor de la identidad, no una prueba.
- `/quienes-somos/`, literal: «Administradora de contenido: Diana Patricia Gómez». Exacto.
- **Lo que el revisor no encontró** (buscó «humanista» solo en `/quienes-somos/`). La API del sitio devuelve, entre otras:
  - **«Términos y Condiciones»** (`/terminos-y-condiciones`, publicada y modificada por última vez el 2011-03-17, hoy en línea, sin enlace desde la portada ni desde `/quienes-somos/`): «El portal www.periodismopublico.com es de propiedad de La CORPORACIÓN HUMANISTA» y «Esta página de Internet y su contenido son de propiedad de La CORPORACIÓN HUMANISTA».
  - **«Horacio Alberto Robledo no labora con Periodismopublico.com»** (2014-07-03): habla de la «Corporación Humanista, entidad propietaria de la página de noticias», y dice que «las únicas personas autorizadas para tomar desiciones periodísticas y comerciales frente a www.periodismopublico.com son los directivos del medio: Ariel González, Alejandro López y Diana Gómez».
  - «Corporación Humanista continúa construyendo redes comunicativas» (2013-04-15): la presenta como «entidad encargada de llevar al cabo el proyecto de construcción de la Red de Comunicaciones de la Localidad de Bosa».
- **Consecuencia.** El origen que la ficha atribuye a «búsqueda web» tiene ahora fuente primaria del propio medio: **en 2011 y en 2014 el medio declaró que el portal era propiedad de la Corporación Humanista**. Es historia (regla del presente), salvo por un detalle: los términos de 2011 **siguen publicados** y siguen diciendo eso hoy, mientras el registro muestra una S.A.S. desde 2016.
- **Lo que no está probado:** que la «CORPORACIÓN HUMANISTA» del medio sea la del NIT 900268977, y que su representante legal sea la Diana Gómez del medio. Ningún documento del medio da el NIT de la corporación ni el apellido completo de la directiva. Ver «Motivo de cada rechazo».

**4 · De qué vive.**
- SECOP I por NIT 901171544: **1 registro**. Entidad, literal, «BOGOTÁ - AGENCIA LOGISTICA DE GESTION INMOBILIARIA Y SERVICIOS DE CUNDINAMARCA» (orden «TERRITORIAL DEPARTAMENTAL DESCENTRALIZADO»), «CPS 394 DE 2021», firmado el 2021-10-01, $5.400.000, «Celebrado», objeto «PRESTACION DE SERVICIOS PARA LA DIFUSION DE NOTAS PERIODISTICAS QUE EXPONGAN LOS AVANCES PROPIOS DE LA EMPRESA INMOBILIARIA Y DE SERVICIOS LOGISTICOS DE CUNDINAMARCA», contratista «PERIODISMO PUBLICO S.A.S.», representante «ARIEL RICARDO GONZALEZ GONZALEZ». Exacto (el revisor omite el prefijo «BOGOTÁ - » del nombre de la entidad, que es una etiqueta del dataset).
- SECOP II por NIT 901171544: **0**. SECOP I y II por NIT 900268977: **0**. Por nombre de proveedor: solo el mismo contrato de 2021. **«Ningún contrato en los últimos 12 meses» a nombre de la sociedad: confirmado.**
- Categoría Publicidad (6): 30 entradas. Están «Secretaría de Hacienda» (2019-08-03), «Banner ESE-3-» (2018-12-30), «Gif Hacienda» (2018-12-03), «Marca Cundinamarca» (2018-01-11) y «ESE Soacha» (2017-07-05 y «Ese Soacha», 2017-06-16). Exacto. Matiz: la categoría tiene entradas de 2009 a 2023 («Paute en Periodismo Público», 2009; «Banner Ariel», 2015); lo de «2017 a 2019» vale para las de entidades públicas.
- Categoría Informe Alcaldía (47): 9 entradas. La última es «No se pierda la posesión del nuevo alcalde de Soacha 2024 – 2027» (2024-01-01); las otras ocho son de 2011-12-20. Exacto.
- **Lo que el revisor no encontró, y es lo más importante de esta resolución:**
  - **Contratos del representante legal como persona natural.** SECOP por nombre «ARIEL RICARDO GONZALEZ GONZALEZ»: **16 contratos, $264.436.932, de 2018 a 2025** (SECOP I: 12 por $162.917.232, 2018-2022; SECOP II: 4 por $101.519.700, 2022-2025). **Ninguno firmado en los últimos 12 meses.** En 14 de los 16, el número de identificación del contratista es idéntico al del representante legal de PERIODISMO PUBLICO SAS en el RUES (y en el contrato de 2021 de la S.A.S.). Los otros dos son de la Empresa de Licores y llevan una variante del número (uno con un dígito de más, otro distinto), pero el mismo nombre y el mismo objeto que nombra el sitio. El cotejo se hizo en local y **no se publica ningún número**.
    - **Empresa de Licores de Cundinamarca (SECOP I): 5 contratos, $37.150.000** (2018-01-26, 2019-03-04, 2020-08-18, 2021-03-24 y 2022-01-21), todos con objeto literal «PUBLICIDAD DE LOS PRODUCTOS DE LA EMPRESA DE LICORES DE CUNDINAMARCA; MEDIANTE BANNER EN EL ACCESO PRINCIPAL EN LA PAGINA WEB PERIODISMOPUBLICO.COM.» **La pauta del sitio se ha contratado a nombre del representante legal, no de la sociedad.**
    - **E.S.E. Empresa de Salud de Soacha** (2018-01-26, $14.300.000): «PRESTAR LOS SERVICIOS DE PAUTA PUBLICITARIA A TRAVeS DE UN BANNER DE 300 X 130 PIXELES Y TRES(03) NOTAS PERIODiSTICAS MENSUALES». Cuadra con las entradas «ESE Soacha» y «Banner ESE-3-» de la categoría Publicidad.
    - **Concejo Municipal de Soacha** (2018-07-27, $15.000.000): «EL SERVICIO PUBLICIDAD E IMAGEN INSTITUCIONAL DEL CONCEJO MUNICIPAL DE SOACHA».
    - **Alcaldía de Soacha** (SECOP I, 4 contratos, $93.067.232, 2018-2019): capacitación en «EL USO DE LOS MEDIOS DE COMUNICACIoN COMO FUENTES DE INVESTIGACIoN» en los colegios oficiales.
    - **Personería de Soacha**: 2022-03-24, $3.400.000 (SECOP I), y 2022-11-16, $1.963.500 (SECOP II, CO1.PCCNTR.4219763), servicio de comunicaciones en medios.
    - **Secretaría de la Mujer de Cundinamarca** (2023-07-15, $32.800.000, CO1.PCCNTR.5223921): asesoría de comunicación.
    - **EPUXUA E.I.C.E.**, entidad territorial con sede en Soacha según SECOP II: CO1.PCCNTR.6686199, firmado el 2024-08-27, $24.733.800, y **CO1.PCCNTR.8216647, firmado el 2025-08-20, $42.022.400, ejecución del 2025-08-28 al 2025-12-31, estado «En ejecución», `valor_pagado` 0**. Objeto del segundo, literal: «PRESTACIÓN DEL SERVICIO PARA LA DIFUSIÓN EN MEDIOS DE COMUNICACIÓN MASIVA Y DIFUSIÓN EN MEDIOS DIGITALES Y STREAMING; DE LOS PROGRAMAS; PROYECTOS; CAMPAÑAS; NOTICIAS; CONTENIDOS Y ACTIVIDADES QUE REQUIERA LA ALCALDÍA MUNICIPAL DE SOACHA; EN EL MARCO DE LA GERENCIA INTEGRAL DEL CONTRATO INTERADMINISTRATIVO N.º 1918-2025 …». No nombra el sitio. **Se firmó siete semanas antes de la ventana de 12 meses, y su ejecución entró en ella (hasta el 2025-12-31).**
  - **Banners vigentes en el sitio, hoy.** En la portada y en la barra lateral de las seis páginas descargadas el 2026-10-08 aparecen:
    - un widget titulado «Empresa de Licores de Cundinamarca», con imagen `BANNER_EMPRESA DE LICORES.jpg` (alt «Empresa de Licores de Cundinamarca-Néctar») que enlaza a elc.com.co; `Last-Modified` de la imagen: 2026-10-06;
    - un widget «Gobernación de Cundinamarca – Índice de pobreza» que enlaza a `facebook.com/JorgeReyCundinamarca`; `Last-Modified`: 2026-09-21;
    - en la portada, una imagen `Gobernación-de-Cundinamarca-la-apuesta-por-Soacha.png` que enlaza a cundinamarca.gov.co; `Last-Modified`: 2026-09-01.
    - **Hecho:** el sitio exhibe hoy publicidad de la Gobernación de Cundinamarca y de su empresa de licores, renovada en septiembre y octubre de 2026. **No consta** contrato en SECOP que la pague en los últimos 12 meses, ni a nombre de la sociedad ni del representante legal. Puede pagarse por una central de medios o por otra vía, o no pagarse: **no se sabe, y no se afirma**.
  - **Cobertura del anunciante.** «Empresa de Licores de Cundinamarca ha producido más de 7,7 millones de botellas para Meta y Nariño» (2026-08-31), firmada «Periodismo Público», sin etiqueta de patrocinio, es una nota favorable a la licorera con declaraciones de su gerente. Una sola pieza: va como dato junto a la tensión, no como patrón.

**5 · La pieza del 27-06-2026.**
- «La mente brillante que lideró la victoria de Abelardo de la Espriella en Cundinamarca»: `datePublished` 2026-06-27T11:21:58-05:00; autor en el JSON-LD «Periodismo Público» (`/author/webero`, autor 1 en la API); categorías 2, 8 y 236 = Cundinamarca, Política y Principales Noticias. Exacto.
- Las cuatro citas son literales, y también «Foto: campaña Abelardo de la Espriella». La pieza llama a Parra Beltrán «coordinador de la Campaña en Cundinamarca». El HTML no tiene «publirreportaje», «patrocinado» ni «contenido pagado».
- «¿Por qué el exsenador Inti Asprilla terminó como notario segundo de Soacha? Acá las razones» (2026-08-08, categorías Política, Principales Noticias y Soacha): las tres citas son literales.
- Búsqueda «Cepeda» desde el 2026-04-01: 5 resultados (votaciones del 31-05 y del 21-06, preconteo, disturbios del 22-06, UNP del 22-09). Exacto.
- «Frenan posesión de Inti Asprilla…» (2026-09-01): se apoya en la carta del gobernador Jorge Emilio Rey; pie literal «Carta: Valora Analitik». Exacto.
- «¡Malas noticias para el bolsillo!…» (2026-09-09) y «Golpe a la 'Paz Total' de Petro…» (2026-09-11): existen y tienen esas fechas; «según su versión» y «según explicó» son literales en la segunda.
- Editorial (243): 18 entradas; la última, «Soacha: una sociedad que se desangra en la trinchera de la polarización», del 2025-04-12; la anterior, del 2021-07-05. Opinión (9) desde el 2026-05-01: una sola, «En Soacha: ¿Emblema = Problema?» (2026-09-12). Desplegable de categorías: «Soacha (22.356)», «Política (1.642)». Todo exacto (la API da 1.615 para Política sin subcategorías; el desplegable las suma).
- **Lectura.** La regla del polo fijo no toca el encuadre asimétrico entre candidatos. Pero un perfil elogioso del coordinador **ganador**, publicado seis días después de la segunda vuelta, no tiene contraparte natural en el perdedor. No demuestra por sí solo una asimetría entre candidatos. Lo que sí demuestra es que la ficha no puede decir que «no hay nada». Es **nivel 5, una pieza, dirección derecha**, y no mueve el número.

**6 · Equipo.** `/quienes-somos/`: «datePublished":"2009-05-01T04:00:00-05:00"», «dateModified":"2020-02-29T22:00:03-05:00"». La página de perfil del director, `/ariel-gonzalez-director-de-periodismo-publico`: publicada el 2009-07-07 y modificada el 2020-03-08; su cuerpo **solo tiene el título**, «Ariel González, director de Periodismo Público», sin texto. Las cinco piezas de 2026 van firmadas por el usuario genérico. Confirmado.

### Ariel González: ¿director, representante legal y contratista son la misma persona?

**Sí en lo que importa aquí, con un matiz.** No es homonimia por nombre suelto:
- **Representante legal y contratista:** el número de identificación del representante legal de PERIODISMO PUBLICO SAS en el RUES coincide con el del contratista «ARIEL RICARDO GONZALEZ GONZALEZ» en 14 de sus 16 contratos y con el del representante en el contrato de la S.A.S. Es la misma persona.
- **Contratista y medio:** cinco de esos contratos venden, literalmente, banners «EN LA PAGINA WEB PERIODISMOPUBLICO.COM». El documento ata a la persona con el medio.
- **Director:** el sitio nombra «Director: Ariel González» (2020) y, en 2014, a «Ariel González» entre los «directivos del medio». Lo que liga este nombre corto con el completo es el nombre más todo lo anterior. **El matiz:** que dirija la redacción **hoy** no consta con fecha del presente (objeción 6).

**Consecuencia.** Entra como hecho: el representante legal de la sociedad editora es Ariel Ricardo González González (RUES, registro de Bogotá cancelado el 2026-08-16), y ha contratado a su nombre la pauta del sitio y la difusión de la Alcaldía de Soacha. Que sea el «director» se escribe como lo que es: el nombre que da la web en 2020. **Si es socio sigue sin constar.**

### Motivo de cada rechazo

- **Obj. 3, como hecho.** Lo que ata la «CORPORACIÓN HUMANISTA» del medio con la entidad del NIT 900268977 es el nombre exacto, el año de matrícula (2009) y la cámara (Bogotá, que cubría Soacha). Lo que ata a su representante legal con la «Diana Patricia Gómez» del medio es solo el nombre. Ningún documento del medio da el NIT de la corporación ni el segundo apellido de la directiva. Es la regla de El Pilón (DECISIONES 2026-10-08): **homonimia no descartada no entra como hecho**. Lo que sí entra: la declaración del propio medio (términos de 2011, nota de 2014) de que la corporación era propietaria del portal.
  - **Contratos de la homónima.** SECOP por «DIANA PATRICIA GOMEZ FLOREZ» devuelve 11 contratos personales (SENA, Alcaldía de Soacha, IDECUT de Cundinamarca; uno vigente, CO1.PCCNTR.8883405, firmado el 2026-01-15, $53.500.000). Su número coincide con el de la representante legal de la corporación del RUES, pero **no con nada del medio**. Ninguno es de medios ni nombra el sitio. **No entran en la ficha**: atribuirlos a una trabajadora del medio por su nombre sería la falta que el protocolo persigue. Quedan en el expediente interno, sin cédulas.
- **Obj. 5, «probablemente sea contenido pagado o enviado por la campaña».** No hay etiqueta, no hay contrato y la búsqueda web no encontró el texto en otros medios. Es una conjetura por el tono. No entra.
- **Obj. 2, «un certificado podría salir con advertencia».** No se comprobó. No entra.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente.** Todas las URL resuelven y las citas aparecen literales. Las consultas de SECOP y del RUES, rehechas con igualdad exacta, **coinciden**. Deformaciones y omisiones:
- **«Ni la ficha ni /quienes-somos/ mencionan la corporación»** (LO QUE NO PUDE VERIFICAR). La ficha sí la menciona, dos veces; lo que no hace es dar su NIT ni su fuente. Error menor de lectura.
- **Omisión mayor:** no buscó por el nombre del representante legal, que él mismo había obtenido del RUES. Por eso no vio los 16 contratos personales, cinco de ellos de pauta en el sitio, ni los dos de la Alcaldía de Soacha vía EPUXUA. Su conclusión «No hay valor_pagado que reportar» y «no se puede excluir la pauta pagada por medio de agencias» sigue siendo cierta para la sociedad, pero deja fuera la vía que de hecho se usó.
- **Omisión:** no miró la barra lateral ni la portada, donde está hoy la publicidad de la Gobernación de Cundinamarca y de su licorera.
- **Omisión:** buscó «humanista» solo en `/quienes-somos/`; la búsqueda del sitio lleva a los términos y condiciones que nombran a la corporación propietaria.
- **«Las piezas … todas de 2017 a 2019»** (Publicidad): vale para las de entidades públicas, no para la categoría (2009-2023). Precisión menor.
- **Errores de la propia ficha, para no repetirlos:**
  - «**NIT** | **no publicado**», cuando su fuente lo publica; y en `mediaOwnership.js`, «NO publica NIT» como resultado de la consulta a informacolombia;
  - «Origen … | búsqueda web», sin enlace, cuando hay primario del propio medio;
  - «como uno de sus tres proyectos»: **sin fuente**. Lo más parecido es la pieza de 2013, que habla de «tres propuestas comunicativas» (web, radio en línea e impreso) de la **Red de Comunicaciones de Bosa**, otra cosa;
  - «entidad sin ánimo de lucro de Soacha»: el RUES la registra en la Cámara de Bogotá y el dato abierto no da su domicilio. Sin fuente para «de Soacha»;
  - «Director», «Equipo» y «Hay … equipo con nombres y cargos» presentados como de hoy, con una página de 2020;
  - «el certificado de la Cámara de Comercio de Bogotá, que cubre Soacha»: desde el 2026-08-16 la matrícula activa está en la cámara de Soacha;
  - «no hay nada que sitúe a este medio en el eje»: ver objeción 5.

---

**Propuesta para la firma**

**(a) Valor: mantener 0,00, provisional y NO firmable todavía.**
- **No se mueve**:
  - por la **regla 3**: no hay evidencia de nivel 1-3 que lo sitúe. El accionariado sigue sin constar, no hay corpus medido en el envío y no hay editoriales en 12 meses;
  - por la **regla 2**: lo único con dirección es una pieza de nivel 5 (el perfil del 27-06-2026) y una nota de tono duro sobre Asprilla (08-08-2026), con contrapesos (notas de septiembre que toman distancia del gobierno entrante, 09-09 y 11-09). No basta.
- **Lo que cambia es la razón escrita.** Ya no es «nada de lo observable lo sitúa en el eje» ni «no se ha podido establecer de qué vive». Pasa a ser: **«0,00 por la regla 2. Sin editoriales desde abril de 2025 y sin endoso en 2026; una pieza laudatoria, sin firma ni etiqueta, del coordinador en Cundinamarca de la campaña ganadora (27-06-2026), como nivel 5 aislado, y notas de septiembre que toman distancia del gobierno entrante (09-09 y 11-09-2026). Medio hiperlocal cuya pauta documentada viene de entidades públicas de Soacha y de Cundinamarca, contratada a nombre de su representante legal.»**
- **No se firma** mientras no conste quién posee la S.A.S. (certificado de la cámara donde hoy está activa la matrícula 2689863) y mientras la ficha no declare la contratación y la publicidad oficial vigente.

**(b) Correcciones de hecho, con su fuente**

En `fichas/periodismo-publico.md`:
1. **NIT:** «no publicado» → **«901171544-6 (RUES, datos.gov.co `c82u-588k`, consultado el 2026-10-08; también lo publica informacolombia)»**.
2. **Sociedad**, fila nueva o ampliada: **«PERIODISMO PUBLICO SAS, S.A.S., matrícula 2689863 del 23-05-2016; CIIU 6312 (portales web) y 7310 (publicidad). Matrícula cancelada en la Cámara de Bogotá el 16-08-2026 y activa en la de Soacha (actualización del 21-08-2026). Último año renovado: 2024 (dato abierto, puede ir con retraso)»**.
3. **Representante legal**, fila nueva: **«Ariel Ricardo González González (RUES, registro de Bogotá; el de Soacha no publica el campo)»**.
4. **Director y Equipo:** añadir **«según /quienes-somos/, modificada por última vez el 29-02-2020; no hay fuente de 2025-2026 que confirme director ni equipo. Las piezas de 2026 van sin firma personal»**. Quitar «Hay … equipo con nombres y cargos» de la entradilla o fecharlo.
5. **Origen:** «búsqueda web» → **«Los términos y condiciones del sitio (2011, aún en línea) dicen que el portal "es de propiedad de La CORPORACIÓN HUMANISTA"; una nota del medio de 2014 la llama "entidad propietaria de la página de noticias"»**. Retirar «como uno de sus tres proyectos» y «de Soacha» (sin fuente).
6. **«El origen sin ánimo de lucro no es el dueño de hoy»:** añadir **«Una entidad llamada exactamente CORPORACION HUMANISTA (NIT 900268977, Cámara de Bogotá, matriculada en 2009) figura cancelada en el RUES desde el 03-03-2023. Que sea la del medio es probable pero no está documentado»**. Y la tensión: **los términos del sitio siguen atribuyendo la propiedad a la corporación, cuando el registro muestra una S.A.S. desde 2016**.
7. **«El punto ciego que sí importa»:** «no se ha podido establecer de qué vive el medio» → el texto de la tensión 1 de (c).
8. **CONTRATACIÓN PÚBLICA**, línea nueva en el formato del protocolo:

> Contratación pública (SECOP I y II, NIT 901171544, consultado 2026-10-08): 0 contratos en los últimos 12 meses (2025-10-08 → 2026-10-08); 1 por $5.400.000 en total desde 2021 (SECOP I: Agencia Logística de Gestión Inmobiliaria y Servicios de Cundinamarca, 2021-10-01, «difusión de notas periodísticas que expongan los avances propios» de la entidad; SECOP II: 0). Su representante legal, Ariel Ricardo González González, ha contratado además como persona natural 16 contratos por $264.436.932 entre 2018 y 2025 (SECOP I: 12 por $162.917.232; SECOP II: 4 por $101.519.700), ninguno firmado en los últimos 12 meses. Cinco, con la Empresa de Licores de Cundinamarca ($37.150.000, 2018-2022), son «publicidad … mediante banner en el acceso principal en la página web periodismopublico.com». El último, con EPUXUA E.I.C.E. ($42.022.400, firmado el 2025-08-20 y ejecutado hasta el 2025-12-31), es para la difusión de los programas «que requiera la Alcaldía Municipal de Soacha». La Alcaldía de Soacha, su Concejo, su Personería y su E.S.E., y la Gobernación de Cundinamarca y sus empresas, son entidades que el medio cubre.

9. **Nivel 5, nuevo:** el perfil del 27-06-2026 y la nota del 08-08-2026 sobre Asprilla, con las citas verificadas; como contrapeso, las del 09-09 y 11-09-2026; y que la sección Editorial no publica desde el 12-04-2025 (sin endoso en 2026).
10. **Entradilla:** «no hay nada que sitúe a este medio en el eje» → **«no hay evidencia suficiente para situarlo: una pieza de nivel 5 no basta»**.
11. **LO QUE FALTA:** el 1 pasa a **«el certificado de existencia de la cámara donde hoy consta activa la matrícula 2689863 (Soacha, según el RUES): socios y fecha de constitución»**. El 3 pasa a **«documentar si la CORPORACIÓN HUMANISTA de los términos del sitio es la del NIT 900268977, cancelada en 2023, y cuándo y cómo pasó el portal a la S.A.S.»**. El 4 pasa a **«quién paga hoy los banners de la Gobernación de Cundinamarca y de la Empresa de Licores (no hay contrato en SECOP en los últimos 12 meses)»**.
12. **REFUTACIÓN 2:** «Que se documente dependencia de pauta oficial» → ya está documentada la pauta oficial histórica y la publicidad oficial vigente; lo que falta es su peso frente al ingreso privado.

En `shared/mediaOwnership.js`, entrada `periodismo-publico`:

13. `holdings[0]`: añadir NIT, matrícula, el cambio de cámara y el representante legal (puntos 1-3). `holdings[1]`: el texto del punto 5. `holdings[2]`: fechar el equipo («según su web, modificada el 29-02-2020»).
14. `notes`: añadir la línea de contratación del punto 8 y la publicidad vigente de la Gobernación (tensión 1). Añadir la laguna: **«La Corporación Humanista que el sitio declara propietaria en sus términos de 2011 coincide en nombre exacto con una entidad cancelada en 2023 (NIT 900268977); la identidad no está documentada»**.
15. `buscadoEn`, fila de informacolombia: «NO publica NIT, NI representante legal, NI socios» → **«Publica el NIT (9011715446, con DV). NO publica representante legal ni socios»**. Añadir filas para el RUES, SECOP I y II y los términos y condiciones. `consultadoEl` → `'2026-10-08'`.
16. `falta`: como el punto 11.
17. `sources`: añadir la consulta del RUES por NIT, las dos de SECOP por NIT, la consulta de SECOP por el nombre del representante legal, `/terminos-y-condiciones` y la nota de 2014.

En `shared/mediaRegistry.js`:

18. `biasRationale`: sustituir «su sociedad editora no publica socios y nada de lo observable lo sitúa en el eje» por la razón de (a), y añadir «su pauta documentada es de entidades públicas de Soacha y Cundinamarca».

En `shared/centinela.js`:

19. La consulta «Corporación Humanista»: su `vigila` dice que «no consta cuál de las dos lo edita hoy». Reescribir: **la S.A.S. es la sociedad registrada, y la corporación de nombre exacto figura cancelada en 2023**. Añadir una consulta por «PERIODISMO PUBLICO SAS» o por su NIT.

**(c) Tensiones a declarar en la ficha**
1. **Un medio que fiscaliza a la administración local vive, en lo documentado, de pauta de la administración local y departamental.** Entre 2018 y 2025, el representante legal contrató a su nombre la pauta del sitio con la Empresa de Licores de Cundinamarca, la E.S.E. de Soacha y el Concejo de Soacha, y la difusión de la Alcaldía de Soacha vía EPUXUA. Hoy el sitio exhibe banners de la Gobernación de Cundinamarca (uno enlaza a la página de Facebook del gobernador Jorge Rey) y de su licorera, renovados en septiembre y octubre de 2026. El 31-08-2026 publicó una nota favorable a esa licorera, sin etiqueta. **Desvelamiento, no acusación.** No mueve el eje.
2. **Una pieza laudatoria del coordinador de la campaña ganadora, sin firma ni etiqueta** (27-06-2026), con foto de la campaña. Nivel 5, una pieza, con contrapesos en septiembre. No mueve el número. Si se documenta que fue pagada, pasa a la tensión 1.
3. **Lagunas declaradas, no tensiones:**
   - quién posee la S.A.S. y en qué porcentaje, y si Ariel González es socio;
   - si la Corporación Humanista del medio es la del NIT 900268977 y si su representante legal es la Diana Gómez del medio (**homonimia no descartada**);
   - director y equipo vigentes;
   - quién paga hoy la publicidad de la Gobernación.
   - Lo que cierra las tres primeras es el certificado de la cámara de Soacha.

**¿Aviso de quien dirige?** No procede. No consta candidatura ni cargo público vigente de Ariel González. Sus contratos de prestación de servicios con entidades públicas (el último terminó el 2025-12-31) no son un cargo público.

---

### Nota posterior (2026-10-08, Claude Code)

**El envío no llevó la conducta medida.** Se armó sin regenerar `data/conducta.json`, que solo tenía los cinco medios de la tanda 3, así que el revisor no recibió cifras de nivel 2 y esta resolución no las usó. Medido después con `npm run conducta` (ventana 2026-08-31 → 2026-10-09, 38 días): 213 artículos, 36 en alguna historia, 38 historias, 29 % de agenda propia, 27 compartidas, compañía media 0,183; coincide con Caracol Radio (11), El Nuevo Siglo (8) y El País Cali (5). Con 38 días no se llega a los 90 que pide el protocolo, así que **la propuesta para la firma no cambia**. Las cifras entran en el nivel 2 de la ficha con su advertencia.
