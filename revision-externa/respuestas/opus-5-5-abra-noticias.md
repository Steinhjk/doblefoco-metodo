# Respuesta — Claude Opus 5.5 sobre Abra Noticias

| | |
|---|---|
| **Modelo** | Claude Opus 5.5 |
| **Versión exacta** | `claude-opus-5-5` |
| **Fecha de la consulta** | 2026-10-08 |
| **Quién la hizo** | Claude Code, a petición del responsable editorial (ciclo 2, fase 2, tanda 5; revisor de la misma casa que el autor de las fichas, ver DECISIONES.md 2026-10-07) |
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
Soy Claude Opus 5.5 (id: claude-opus-5-5), de Anthropic: la misma casa que el modelo que escribió la ficha. Mi acuerdo no vale como verificación independiente. Por eso he buscado sobre todo donde la ficha no miró: la API pública de WordPress del propio medio (/wp-json/), su categoría «Opinión», sus autores y los registros públicos de contratación y mercantiles. Mi juicio sobre dónde va el medio no es evidencia. Lo que sigue son hechos con su fuente y las inferencias van marcadas como tales.
Fecha de todas las comprobaciones: 2026-10-08 (hora de Colombia, por la noche).

MÉTODO Y DÓNDE BUSQUÉ
- robots.txt de abranoticias.com (2026-10-08): «User-agent: * / Allow: /». No excluye a ClaudeBot, Claude-Web ni anthropic-ai. robots.txt de datos.gov.co: solo prohíbe rutas /browse?…, y no usé ninguna.
- Sitio del medio, HTML en crudo con curl -sL --ssl-no-revoke y User-Agent de navegador: portada (https://abranoticias.com/), /category/opinion/, /author/atisbernal/, /feed/ y cinco artículos sueltos (las URL van más abajo).
- API REST pública de WordPress del medio, en JSON crudo:
  /wp-json/ (nombre del sitio);
  /wp-json/wp/v2/categories?slug=opinion (id 11, «count»: 23);
  /wp-json/wp/v2/posts?categories=11&per_page=30 (las 23 entradas de Opinión, con fecha, autor y contenido);
  /wp-json/wp/v2/users (cuentas que publican);
  /wp-json/wp/v2/posts?search=Petro, ?search=director y ?search=Atis (40 resultados por búsqueda, solo titulares);
  cabecera X-WP-Total: 1662 entradas en total.
- RUES abierto (datos.gov.co c82u-588k):
  razón social LIKE «%ABRA NOTICIAS%», «%ABRANOTICIAS%» y «%ATIS BERNAL%», y «%ABRA %» en las cámaras de Pasto e Ipiales;
  después, por número de identificación (igualdad exacta) de la persona natural que se describe abajo.
- SECOP I (f789-7hwg): por razón social LIKE «%ABRA NOTICIA%» / «%ATIS BERNAL%», y después por identificacion_del_contratista con igualdad exacta.
- SECOP II (jbjy-vk9h): por proveedor_adjudicado, objeto y descripción LIKE «ABRA NOTICIAS» / «ATIS BERNAL», y después por documento_proveedor con igualdad exacta.
- Buscador web: una sola consulta («"Atis Bernal" "Abra Noticias"»). No devolvió nada pertinente (solo resultados sobre Abra, Filipinas). No lo usé más para no gastar el cupo compartido.
- No toqué eltiempo.com, cambiocolombia.com ni lasillavacia.com. No usé Wikipedia: no encontré entrada sobre el medio y no la busqué.

## NIVEL 1 — QUÉ CAMBIÓ ESTE AÑO

- ¿Cambió de dueño, se vendió, se fusionó o se escindió en los últimos 12 meses?
  No encontré nada. Tampoco hay un dueño registrado contra el que comprobarlo. El RUES no tiene ninguna matrícula a nombre de «ABRA NOTICIAS» ni «ABRANOTICIAS» (consulta del 2026-10-08, 0 filas). El nombre del sitio en /wp-json/ sigue siendo «Abra Noticias», con la descripción «Noticias de Pasto, Noticias de Ipiales, Noticias de Nariño, Noticias del Cauca».

- La persona que la ficha nombra como titular o director, ¿sigue viva y en el cargo?
  La ficha no nombra a nadie, así que no hay nada que comprobar. Sí hay un nombre identificable: lo explico en la objeción 3. La cuenta que publica sigue activa. La última entrada es del 2026-10-08T13:50:53 y el feed trae pubDate «Thu, 08 Oct 2026 23:52:00 +0000».

- ¿Quién dirige hoy la redacción?
  No encontré ningún nombre publicado como director. Lo más cercano (es inferencia, no está probado): la cuenta de WordPress que firma todo el contenido tiene slug «atisbernal» y nombre visible «ABRA NOTICIAS» (/wp-json/wp/v2/users: «"id":2,"name":"ABRA NOTICIAS"…"slug":"atisbernal"»). Además, una columna de la casa va firmada «Por: Rober Atis Bernal» (2025-11-04). Ver la objeción 3.

- ¿Hay un registro mercantil o un reporte de emisor más reciente que la fuente que la ficha cita?
  No. La ficha no cita ningún registro y yo no encontré ninguno: ni sociedad en el RUES, ni matrícula mercantil de la persona natural citada en la objeción 3 (consulta por identificación exacta en c82u-588k, 0 filas).

## OBJECIONES

### OBJECIÓN 1 — Sí hay sección de opinión, y no todo va firmado por la cabecera

QUÉ AFIRMA LA FICHA
«Sus piezas van firmadas por la cabecera y no hay sección de opinión identificable». Y en LO QUE FALTA: «Todas sus piezas van firmadas por la cabecera».

POR QUÉ ES INCORRECTO
- La portada enlaza a una categoría «Opinión» (https://abranoticias.com/category/opinion/).
- La API la describe así: «"id":11,"count":23,…"name":"Opinión","slug":"opinion"».
- De esas 23 entradas, al menos 13 llevan firma de autor en el cuerpo del texto. Ejemplos:
  · «Por: Harold Ruiz» (2026-10-08)
  · «Por: Pablo Emilio Obando A.» (2026-08-24, 2026-07-28, 2026-07-24, 2026-07-09, 2026-07-05, 2026-06-30)
  · «Por: Fernando Alexis Jiménez» / «Por: Alexis Fernando Jiménez» (2026-08-16, 2026-07-31, 2026-07-17, 2026-07-10, 2026-07-04)
  · «Por: Enrique Herrera Enríquez.» (2026-07-06)
  · «Por: Rober Atis Bernal» (2025-11-04)
- Otras columnas no llevan firma en el cuerpo. Por ejemplo, la del 2026-09-01 que cito en la objeción 2. Son textos de opinión de la casa, en el sentido que la ficha dice no encontrar.

DE DÓNDE PUEDE VENIR EL ERROR (inferencia)
El feed marca las 10 entradas que trae con «<dc:creator><![CDATA[ABRA NOTICIAS» (comprobado el 2026-10-08), y la portada no muestra la firma. La firma está dentro del texto y la sección está en el menú.

FUENTE
https://abranoticias.com/category/opinion/ y https://abranoticias.com/wp-json/wp/v2/posts?categories=11&per_page=30 — consultados el 2026-10-08. Fechas de las piezas: las indicadas arriba.

NIVEL DE EVIDENCIA
Declaración del propio medio y conducta observable.

### OBJECIÓN 2 — «Nada de lo observable lo sitúa en el eje» no se sostiene

QUÉ AFIRMA LA FICHA
0,00 por la Regla 2, porque «nada de lo observable lo sitúa en el eje».

POR QUÉ ES INCORRECTO
Es justo lo que la ficha dice que falta: columnas de la casa y titulares de noticias con asimetría a uno y otro lado del cambio de gobierno de agosto de 2026. Aplico la regla del polo fijo: no traigo crítica al gobierno sin más, sino toma de partido y trato desigual.

a) Columna sin firma en Opinión (cuenta «ABRA NOTICIAS»), 2026-09-01, después del cambio de gobierno
   URL: https://abranoticias.com/abelardo-de-la-espriella-comenzo-a-censurar-medios-de-comunicacion-como-lo-hizo-hugo-chavez-en-el-2004/
   Citas literales del HTML crudo:
   - «Hoy, esas críticas de los políticos de la extrema derecha que ayudaron a elegir a un fantoche presidente de la oligarquía…»
   - «…no puede ser apagado por un presidente fantoche y payaso.»
   - «Ese cuento la extrema derecha quiso amilanar al gobierno progresista, a quien lo acusaron de llegar al poder censuraría a la prensa […] lo cual nunca sucedió…»
   Por qué cuenta: no se limita a fiscalizar una medida (restringir ruedas de prensa). Insulta al presidente entrante y absuelve expresamente al gobierno saliente, al que llama «gobierno progresista». Esa es la asimetría que pide el protocolo.

b) Columna firmada «Por: Rober Atis Bernal», 2025-11-04, durante el gobierno Petro
   URL: https://abranoticias.com/se-juntan-los-viejitos-canosos-temen-a-ivan-cepeda/
   Citas literales:
   - «La extrema derecha que por más de 200 años ha gobernado a Colombia…»
   - «los de la derecha confabulados con grupos ilegales…»
   - «esa reunión de los ‘jefes’ de la banda de la ‘Derecha’…»
   - «Y temen que nuevamente les gane el poder la izquierda con el senador y hoy candidato del Pacto Histórico, Iván Cepeda…»
   Por qué cuenta: no fiscaliza al poder de entonces, porque en ese momento la derecha era oposición. Ataca a un bando en plena campaña presidencial. Eso es tomar partido, y la regla del polo fijo dice expresamente que lo sigue midiendo.
   Está dentro de la ventana de 12 meses: 11 meses y 4 días antes de la comprobación.

c) Piezas de la sección de noticias sin firma
   - 2026-09-10, sobre el expresidente Petro frente a Blu Radio y El Tiempo. El texto propio de la casa, fuera de la cita, dice: «dos periodistas del Blu Radio y El Tiempo, medios arrodillados al establecimiento». El titular: «Frenan a periodistas del establecimiento y les dicen que son vampiros del periodismo en Colombia».
     URL: https://abranoticias.com/frenan-a-periodistas-del-establecimiento-y-les-dicen-que-son-vampiros-del-periodismo-en-colombia/
   - 2025-10-16, titular: «CELAG dice que Gustavo Petro ‘Mejor Presidente de la historia de Colombia’». El cuerpo lleva un subtítulo de la casa: «Presidente Petro, el mejor presidente de la historia».
     URL: https://abranoticias.com/celag-dice-que-gustavo-petro-mejor-presidente-de-la-historia-de-colombia/
   - En los 40 titulares que devuelve la API para «Petro» (2025-03-27 a 2026-10-08) no vi ninguno crítico con su gobierno. Ejemplo: «Petro desmintió y lo peinó a Duque» (2025-03-27). Aviso: esto es un barrido de titulares, no de cuerpos. La ausencia es una inferencia limitada.

d) Columna firmada «Por: Harold Ruiz», 2026-10-08
   URL: https://abranoticias.com/la-nueva-derecha-vs-la-izquierda/
   Cita: «Frente a la feroz arremetida de la nueva derecha, le corresponde a las fuerzas progresistas y de izquierda, salir del impacto de la pasada derrota electoral…»
   Es un colaborador, no la casa, así que pesa menos. Encaja con lo anterior, y la casa decide a quién publica.

QUÉ PRUEBA Y QUÉ NO (distingo hecho de inferencia)
- Hecho: el medio publica, como casa y en su sección de noticias, encuadres asimétricos a favor del bloque Petro/Pacto Histórico y en contra de la derecha, antes y después de agosto de 2026.
- Inferencia: con esto la Regla 2 («no hay nada que lo sitúe») deja de cumplirse. No propongo cifra, porque la Regla de la banda más cercana a la mixta sigue en pie.
- La ficha debe justificar ahora el 0,00 contra esta evidencia, o moverlo.

NIVEL DE EVIDENCIA
Hechos editoriales de los últimos 12 meses (las cuatro piezas) y conducta observable.

### OBJECIÓN 3 — «Director / editor: no publicado» y «quién lo dirige o lo escribe» tienen una pista verificable que la ficha no siguió

QUÉ AFIRMA LA FICHA
Director/editor «no publicado»; «Quién lo dirige o lo escribe» figura entre lo que falta.

POR QUÉ
- Hecho: en el sitio publican dos cuentas, según /wp-json/wp/v2/users el 2026-10-08:
  · «"id":1,"name":"adminabra"»
  · «"id":2,"name":"ABRA NOTICIAS",…"slug":"atisbernal"»
  La cuenta 2 firma todas las entradas de Opinión desde 2025 y todo el feed actual. La única columna firmada por una persona con ese apellido es «Por: Rober Atis Bernal» (2025-11-04).
- Inferencia (no probada): el titular de la cuenta que gestiona el medio sería Rober Atis Bernal.
- Registro externo, con la identidad sin probar: en SECOP aparece un contratista persona natural, «ROBER ALBEIRO ATIS BERNAL» (en una fila, «ROBERT ALBEIRO ATIS BERNAL»), con un único número de identificación. No lo escribo porque es su cédula. Contrató como «COMUNICADOR SOCIAL» con la Personería Municipal de Pasto. Coinciden el nombre, la ciudad y el oficio. No hay ningún documento que lo vincule a abranoticias.com, así que la homonimia NO está descartada.

  Contratos (ninguno en los últimos 12 meses):
  · SECOP I — Personería Municipal de Pasto. Firma: 2021-09-02. Cuantía: $6.920.000. Estado: Liquidado. Constancia 21-12-12301118. Objeto: «PRESTAR SUS SERVICIOS PROFESIONALES COMO COMUNICADOR SOCIAL PARA EL FORTALECIMIENTO INSTITUCIONAL; SU VISIBILIZACION DE LA GESTION DE LA ENTIDAD…»
  · SECOP I — Personería Municipal de Pasto. Firma: 2022-01-27. Cuantía: $19.261.000. Estado: Liquidado. Constancia 22-12-12836365. Objeto: «…COMO COMUNICADOR SOCIAL PARA EL APOYO Y ACOMPAÑAMIENTO A LA GESTIÓN DE COMUNICACIONES ESTRATÉGICAS DE LA ENTIDAD.»
  · SECOP II — Personería Pasto. Firma: 2023-02-14. Valor: $21.071.400. valor_pagado: 0 (el campo sale en cero). Estado: Cerrado. Contrato CO1.PCCNTR.4628748. Objeto: «…como COMUNICADOR SOCIAL; para el apoyo y acompañamiento al Procesos Comunicaciones Estratégicas de la Entidad.»

  Total histórico de esa identificación: 3 contratos, $47.252.400, todos con la Personería de Pasto (2021–2023).
  RUES: esa identificación no tiene matrícula (0 filas). Sin representante legal que reportar.

- Por qué importa:
  · Si la identidad se confirma, la ficha tiene un responsable con nombre y un antecedente de comunicador contratado por un organismo de control municipal en Pasto. Ese contrato no está vigente, así que no es un conflicto actual.
  · No consta ningún contrato público del medio ni de esa persona en los últimos 12 meses. Eso también hay que escribirlo.

FUENTES
- https://abranoticias.com/wp-json/wp/v2/users
- https://abranoticias.com/se-juntan-los-viejitos-canosos-temen-a-ivan-cepeda/
- [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (filtro nom_razon_social_contratista y luego identificacion_del_contratista)
- [enlace retirado: puede mostrar documentos de identidad; ver la resolución] (filtro documento_proveedor)
- [enlace retirado: puede mostrar documentos de identidad; ver la resolución]
Todas consultadas el 2026-10-08.

NIVEL DE EVIDENCIA
Declaración del propio medio (metadatos de autoría) y registro externo (SECOP), con la identidad sin probar.

## LO QUE NO PUDE VERIFICAR

- La razón social y el NIT del medio. Busqué en el RUES por «ABRA NOTICIAS», «ABRANOTICIAS» y «ABRA » en las cámaras de Pasto e Ipiales, y no encontré ninguna matrícula que case. Puede funcionar sin matrícula o a nombre de una persona natural que no pude identificar con certeza.
- Que Rober Atis Bernal sea el dueño o el director: ver la objeción 3. El buscador web no trajo nada (una consulta). No encontré página «Quiénes somos» ni «Contacto». La API /wp-json/wp/v2/pages devuelve una lista vacía.
- Si la casa criticó al gobierno Petro mientras gobernaba. Solo revisé los 40 titulares que devuelve la búsqueda «Petro» y no vi ninguno crítico. No leí los cuerpos ni las 1662 entradas.
- Redes sociales propias: la portada en crudo no enlaza a ninguna cuenta de Facebook, X, Instagram, YouTube ni TikTok.

## LO QUE FALTA

1. La sección de Opinión entera, con sus columnistas firmados y sus textos sin firma: es la conducta editorial más directa del medio.
2. Una lectura de la asimetría a un lado y otro de agosto de 2026 en las piezas de la casa (objeción 2). La ficha no tiene ninguna pieza fechada.
3. Las cuentas que publican (/wp-json/wp/v2/users) y el nombre de la firma «Rober Atis Bernal», con la homonimia declarada.
4. Un barrido de contratación pública declarado. La ficha no dice que se hiciera. Resultado de hoy: nada a nombre del medio; 3 contratos (2021–2023, $47.252.400) de un homónimo probable; ninguno en los últimos 12 meses.

## EVIDENCIA QUE NO MUEVE EL NÚMERO

- Lo que la ficha dice del contacto sigue siendo cierto hoy (2026-10-08). En el HTML crudo de la portada siguen «555-0156», «23 Miller Court», «Hagerstown» y «[correo omitido]», y el pie dice «Copyright © Todos los derechos reservados.» sin titular.
- El feed responde HTTP 200 con 10 ítems. El más reciente es del 2026-10-08 y ningún ítem trae <enclosure> ni media:content (sin imágenes), como dice la ficha. Todos llevan dc:creator «ABRA NOTICIAS».
- Hay columnas de tono pluralista o local, sin carga en el eje:
  · «Hacia un Acuerdo Nacional» (2026-07-10, Alexis Fernando Jiménez): «No podemos seguir enfrentados porque el país, con brechas sociales y problemas urgentes por resolver, amerita que lleguemos a un acuerdo.»
  · Varias columnas de Pablo Emilio Obando A. sobre Nariño (2026-06-30 a 2026-08-24).
- La columna sin firma «Campañas de insultos» (2026-02-04) critica a los candidatos en general: «Las campañas de hoy, no son transparentes ni de propuestas sino se han convertido en un tema de ataques».
- La cobertura de noticias es sobre todo local y de sucesos (Ipiales, Pasto, Putumayo, el caso Comfamiliar de Nariño), de acuerdo con la ficha.
- La conducta medida (6 de 105 artículos en historias, en 38 días) es demasiado escasa para sostener nada. La compañía media (0,25) no debe mover el valor, y la ficha no la usa.

## SIN OBJECIÓN

No aplica: hay tres objeciones.
```

---

## RESOLUCIÓN

**Propuesta de resolución — Claude Code, 2026-10-08. Pendiente de la firma del responsable editorial.**

**Edición de la respuesta literal: ninguna.** El revisor no copió cédulas, teléfonos ni direcciones particulares de personas naturales. Se comprobó: el número de identificación del contratista de SECOP no aparece en el texto, y las cifras largas que contiene son cuantías y números de constancia o de contrato. Esta resolución tampoco escribe ninguno de esos datos. Los datos de contacto de la plantilla «MoreNews» no son de ninguna persona natural.

**Cómo se verificó.**
- **robots.txt**, leído antes de descargar nada:
  - abranoticias.com: «User-agent: * / Allow: /».
  - datos.gov.co: `Crawl-delay: 1` y exclusiones de `/browse`; nada sobre ClaudeBot.
  - No se tocaron eltiempo.com, cambiocolombia.com ni lasillavacia.com. No hubo buscador web.
- **Sitio**, descargado en crudo el 2026-10-08 con `curl -sL --ssl-no-revoke -A "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/126.0 Safari/537.36"`:
  - la portada, `/category/opinion/`, `/author/atisbernal/`, `/feed/` y las siete piezas que el revisor cita o en las que se apoya; todas dieron 200;
  - `/quienes-somos/` y `/contacto/`: **404**.
- **API REST de WordPress**:
  - `/wp-json/`, `/wp/v2/users`, `/wp/v2/categories`, `/wp/v2/pages` (lista vacía) y `/wp/v2/posts?categories=11&per_page=100` (`X-WP-Total: 23`);
  - **el archivo entero**: `/wp/v2/posts?per_page=100&page=1…17`, con 1.662 entradas del 2022-04-21 al 2026-10-08, igual que `X-WP-Total: 1662`.
  - El barrido de la objeción 2 se hizo sobre **los cuerpos**, no solo sobre los titulares. Ventana de 12 meses: 2025-10-08 → 2026-10-08, con 751 entradas (518 antes del 07-08-2026 y 233 después).
  - Las fechas son las de la API (`date`, hora de Colombia: `gmt_offset` −5).
- **Citas.** Las del revisor se buscaron literalmente en el HTML crudo de cada pieza. Las que añade esta resolución salen del `content.rendered` de la API, sin etiquetas y con los espacios normalizados.
- **Registros**, en datos.gov.co:
  - SECOP I (`f789-7hwg`), por `nom_razon_social_contratista` (`like '%ATIS BERNAL%'` y `'%ABRA NOTICIA%'`) y después por `identificacion_del_contratista` con **igualdad exacta**;
  - SECOP II (`jbjy-vk9h`), por `proveedor_adjudicado` (`'%ATIS BERNAL%'`) y por proveedor, descripción y objeto (`'%ABRA NOTICIA%'`), y después por `documento_proveedor` con **igualdad exacta**;
  - RUES (`c82u-588k`), por `razon_social` (`'%ABRA%NOTICIA%'`, `'%ABRANOTICIA%'`, `'%ATIS%BERNAL%'`, y `'%ABRA %'` en las cámaras de Pasto e Ipiales) y por `numero_identificacion` con **igualdad exacta**.
  - El número de identificación se usó dentro de las consultas y no se escribe en ningún sitio.

Quien resuelve es otro Claude, de la misma casa que el autor de la ficha y que el revisor. Que aquí no se contradiga algo no lo convierte en aval.

| # | Objeción | ¿Trae fuente? | ¿Se verificó? | Resultado |
|---|---|---|---|---|
| 1 | Hay sección de Opinión, y no todo va firmado por la cabecera | sí | sí | **Aceptada, y la ficha ya estaba mal el día del alta** (19 de las 23 entradas son anteriores al 14-08-2026). Recuento corregido: 16 firmadas por una persona, 1 «Por: ABRA NOTICIAS» y 6 sin firma |
| 2 | «Nada de lo observable lo sitúa en el eje» no se sostiene: asimetría a favor del bloque Petro / Pacto Histórico, antes y después del 07-08-2026 | sí | sí, con barrido completo de los cuerpos | **Aceptada como hecho de nivel 5, y reforzada.** En 12 meses no aparece ni una pieza de la casa crítica con el gobierno Petro. Hay rótulos y adjetivos de la casa contra la derecha a los dos lados del cambio de gobierno, y la casa absuelve de forma expresa al gobierno saliente. Hay contrapesos y van escritos. **Con la regla vigente no mueve el número** (regla 3). Ver la propuesta (a) y (b) |
| 3 | La firma «Rober Atis Bernal» y la cuenta `atisbernal` son una pista de quién lo hace; un homónimo probable contrató en SECOP | sí | sí | **Aceptada en lo que publica el medio:** la cuenta y **dos** columnas firmadas, no una. **No entra como hecho** la identidad con el contratista de SECOP: homonimia no descartada. Las cifras de SECOP coinciden al peso |

### Lo verificado, objeción por objeción

**1 · Sección de Opinión y firmas.**
- La categoría existe: `"id":11,…"name":"Opinión","slug":"opinion"`, `X-WP-Total: 23`. Va del 2024-01-12 al 2026-10-08, y la portada la enlaza (siete apariciones de `category/opinion` en el HTML crudo).
- **Firmas en el cuerpo de las 23 entradas:**
  - **16 firmadas por una persona:**
    - Pablo Emilio Obando A., 7 (30-06, **03-07**, 05-07, 09-07, 24-07, 28-07 y 24-08-2026). La del 03-07 abre con «Po: Pablo Emilio Obando A.», con la errata, y por eso el revisor no la contó.
    - Fernando Alexis Jiménez / Alexis Fernando Jiménez, 5 (04-07, 10-07, 17-07, 31-07 y 16-08-2026).
    - Rober Atis Bernal, **2** (09-11-2024 y 04-11-2025).
    - Enrique Herrera Enríquez, 1 (06-07-2026).
    - Harold Ruiz, 1 (08-10-2026).
  - **1 firmada «Por: ABRA NOTICIAS»** (10-05-2024).
  - **6 sin firma:** 12-01, 21-01 y 08-02-2024; 04-02, 18-02 y 01-09-2026.
  - El «al menos 13» del revisor es una cota inferior correcta.
- **Ventana de 12 meses: 18 entradas de Opinión.**
  - 14 son de columnistas externos (Obando 7, Jiménez 5, Herrera 1, Ruiz 1).
  - 1 es de Rober Atis Bernal.
  - 3 van sin firma: 04-02 («Campañas de insultos»), 18-02 (contra Noboa) y 01-09 (contra De la Espriella).
- **Autoría técnica:** las 23 tienen `author` 1 («adminabra») o 2 («ABRA NOTICIAS», slug `atisbernal`). Desde abril de 2025, todo lo publicado sale de la cuenta 2.
- Los 10 ítems del feed llevan `<dc:creator><![CDATA[ABRA NOTICIAS`, como dice el revisor. Por eso la frase de la ficha, «todas sus piezas van firmadas por la cabecera», es cierta **en los metadatos** y falsa **en el texto**.
- **Fecha.** 19 de las 23 entradas son anteriores al alta de la ficha (2026-08-14). La laguna declarada se caía ya ese día, que es justo lo que el envío avisaba («ve ahí primero»).

**2 · Asimetría a través del cambio de gobierno.**
- **Las cuatro piezas del revisor tienen citas literales** en el HTML crudo:
  - 01-09-2026: «ayudaron a elegir a un fantoche presidente de la oligarquía», «no puede ser apagado por un presidente fantoche y payaso» y «Ese cuento la extrema derecha quiso amilanar al gobierno progresista […] lo cual nunca sucedió».
  - 04-11-2025: las cuatro citas, y la firma «Por: Rober Atis Bernal».
  - 10-09-2026: «medios arrodillados al establecimiento».
  - 16-10-2025: el subtítulo «Presidente Petro, el mejor presidente de la historia».
  - 08-10-2026: «Frente a la feroz arremetida de la nueva derecha, le corresponde a las fuerzas progresistas y de izquierda…».
- **Qué es voz de la casa y qué no.** Pesa más lo que va sin firma, en Opinión o en la narración propia de las noticias, que las citas de terceros que el medio reproduce. Las columnas de firmantes externos pesan menos que la voz de la casa: la casa decide a quién publica, pero no escribe lo que dicen. **La de Rober Atis Bernal va en medio:** su apellido coincide con el slug de la cuenta que publica todo, pero que sea quien dirige el medio no consta (ver la 3).
- **Barrido sistemático (cuerpos, 12 meses).** Se leyeron las 29 piezas que nombran a Petro, las 40 que nombran a De la Espriella o a «Abelardo» y todas las frases con «Gobierno Nacional», «gobierno de Petro», «Pacto Histórico», «extrema derecha», «ultraderecha», «progresista», «fascis», «oligarquía» y «establecimiento». La clasificación es mía y va pieza a pieza, con cita:

| | Antes del 07-08-2026 (518 entradas) | Desde el 07-08-2026 (233 entradas) |
|---|---|---|
| **Voz de la casa, sin firma, en Opinión** | 04-02 «Campañas de insultos»: neutral, critica a todos los candidatos | **01-09: contra De la Espriella («fantoche y payaso») y absolución expresa de Petro** |
| **Voz de la casa en la narración de noticias, a favor de Petro / Pacto Histórico o contra la derecha** | **5:** 16-10-2025 (CELAG, subtítulo propio); 31-10-2025 (defiende a Petro frente a la OFAC: «el presidente gringo no aprobado sin ninguna documentación lo dicho en días anteriores contra Petro»); 02-06-2026 («Hoy se volvió al lado de la extrema derecha»; enumera en voz propia las propuestas «polémicas» del candidato); 04-06-2026 («quiere continuar con el segundo mandato del gobierno progresista»); 30-06-2026 («Tras la llegada de la extrema derecha al poder, han comenzado a surgir las amenazas de muerte contra los dirigentes»). Y un rótulo de la casa dentro de una nota sobre Cepeda, el 08-07 («elector presidente de la extrema derecha») | **6:** 25-08 («muchos afirman que es una simple vil copia» de Trump); 04-09 («El homicidio de la joven líder social juvenil es una advertencia más de que el actual gobierno abandonará a todos los dirigentes que quedan a merced de sus enemigos de la extrema derecha»); 09-09 («se pasea entre cuerpos de abatidos como si fueran un trofeo»); **10-09 (a favor de Petro: «medios arrodillados al establecimiento»)**; 12-09 UNP («Al parecer ser crítico del actual gobierno, le mandaron a quitar la seguridad»); 14-09 («el presidente de la ultra derecha en Colombia Abelardo de la Espriella contra el expresidente de la izquierda Gustavo Petro») |
| **Voz de la casa crítica con el gobierno Petro** | **0** | **0** (ni con el expresidente) |
| **Voz de la casa neutral o favorable a medidas de De la Espriella** | — (no gobernaba) | **3-4:** 11-09 cárceles («Se acaba los privilegios en los centros penitenciarios en el país», «Los internos no deben tener es nada.»); 12-09 fotomultas (recoge sin reparo que no deben ser instrumentos «para llenar los bolsillos de las empresas encargadas de estos sistemas»); 08-09 ofensiva contra el Eln («la cacería militar no se detiene»); 14-09 universidades (transmisión neutral del ultimátum, con el contexto de los daños de las protestas) |
| **Relevos sin voz propia** (titular o cuerpo con palabras de terceros) | A favor de Petro o contra De la Espriella: 19-11-2025 («La dura respuesta de Petro»), 25-04, 01-06 («La contundente respuesta de Petro»), 08-07 (Cepeda), 24-07, 04-08 (el texto de las demandas de nulidad se publica en primera persona del demandante, con «régimen neofacista y sionista», sin contraparte) y dos cartas de sargentos: 23-11-2025 contra Abelardo y 06-08-2026 de agradecimiento a Petro. **En contra de Petro: 0** | Contra De la Espriella: 03-09, 22-09 («El discurso de odio y mentiroso del irresponsable presidente»), 23-09 («Abelardo mataste a mi hijo») y 27-08 (recusación del Pacto). Equilibrado: 12-09 (Escobar, Petro y De la Espriella) |
| **Columnas firmadas** | Atis Bernal, 04-11-2025 (contra «la extrema derecha», a favor de Cepeda). Obando, 03-07 (desmiente un bulo contra el «presidente electo, doctor Abelardo de la Espriella») y 09-07 (elogia la carta del gobernador al presidente electo: «Nariño no puede darse el lujo de permanecer distante del Gobierno Nacional»). Jiménez, 10-07 («Hay un nuevo presidente electo, nos guste o no»; pide un «Acuerdo Nacional») | Ruiz, 08-10 (militante: «nos permita tener fuerte presencia en las elecciones regionales»). El resto (Jiménez, Obando) no toca el eje |

- **Lectura con el polo fijo.**
  - Lo de después del 07-08 que es **crítica a medidas** (traslados de escoltas, imágenes de cadáveres, UNP) sería fiscalización, que **no** es evidencia.
  - **Sí son evidencia** tres cosas. Primero, los **rótulos ideológicos de la casa a un solo lado** («ultra derecha», «extrema derecha», «fantoche y payaso»): al gobierno saliente nunca se le aplica uno equivalente. Segundo, **la absolución expresa del gobierno saliente** (01-09). Tercero, **la ausencia total de fiscalización al gobierno Petro mientras gobernaba**, junto con piezas de la casa que lo celebran (16-10-2025) o lo defienden (31-10-2025).
  - Ese patrón se sostiene **a los dos lados del cambio de gobierno**, y es la asimetría que pide el protocolo. Se suma la columna de campaña de Atis Bernal (04-11-2025), que **toma partido** en plena campaña.
  - **Dirección: izquierda. Nivel: 5** (hechos editoriales de los últimos 12 meses). No hay nivel 1, 3 ni 4 que lo sitúe, y el nivel 2 no llega a los 90 días.
- **Contrapesos, verificados y que el revisor trae solo en parte.**
  - Después del 07-08, la casa recoge con aprobación medidas de seguridad del gobierno De la Espriella (cárceles, fotomultas, ofensiva contra el Eln).
  - Sus columnistas más frecuentes (Obando, Jiménez) tratan al presidente electo con respeto institucional.
  - La columna sin firma del 04-02 reparte por igual.
  - **El volumen es pequeño:** unas 20 piezas con postura en 751 entradas en 12 meses. El medio es sobre todo de sucesos de Nariño: «Judicial» (209) y «Noticias» (181) son las categorías más usadas en la ventana.
- **Fuera de plazo.** «Petro desmintió y lo peinó a Duque», que el revisor pone como ejemplo, es del **27-03-2025**: más de 12 meses. Por la regla del presente, no cuenta.

**3 · Quién lo hace.**
- `/wp-json/wp/v2/users` (2026-10-08): `{"id":2,"name":"ABRA NOTICIAS",…,"link":"https://abranoticias.com/author/atisbernal/","slug":"atisbernal"}` y `{"id":1,"name":"adminabra",…}`. Literal.
- Por año: la cuenta 1 publica de 2022 a marzo de 2025 (754 entradas) y la cuenta 2 desde abril de 2025 (908).
- **«Rober Atis Bernal» firma dos columnas, no una:**
  - 09-11-2024, «¿En Ipiales todo es culpa de Amilcar?», desde la cuenta 1;
  - 04-11-2025, desde la cuenta 2.
  - El revisor dice que la única es la de 2025. **La de 2024 queda fuera de los 12 meses**, pero prueba que la firma acompaña al medio en sus dos etapas de cuenta.
- **Ninguna pieza ni página del sitio nombra a un director.** En el texto de las 1.662 entradas no aparecen «director de Abra», «Abra Noticias» como sujeto ni «Atis» fuera de esas dos firmas. Las 17 apariciones de «www.abranoticias.com habló/conoció» no nombran a nadie. `/wp/v2/pages` devuelve `[]`, y `/quienes-somos/` y `/contacto/` dan 404.
- **SECOP, recalculado con igualdad exacta sobre la identificación:**
  - SECOP I: 2 contratos, $26.181.000, ambos con la «NARIÑO - PERSONERÍA MUNICIPAL DE PASTO»:
    - 2021-09-02, $6.920.000, Liquidado, constancia 21-12-12301118;
    - 2022-01-27, $19.261.000, Liquidado, constancia 22-12-12836365, a nombre de «ROBERT ALBEIRO ATIS BERNAL».
  - SECOP II: 1 contrato, $21.071.400, «PERSONERIA PASTO», firmado el 2023-02-14, Cerrado, CO1.PCCNTR.4628748, `valor_pagado` 0.
  - **Total: 3 contratos, $47.252.400. Exacto.** Los objetos («COMUNICADOR SOCIAL») son literales.
  - **Ninguno cae en los últimos 12 meses.**
- **RUES:** 0 filas por esa identificación; 0 por «ABRA NOTICIA», «ABRANOTICIA» y «ATIS BERNAL». Por «ABRA » en Pasto e Ipiales salen 6 filas, ninguna del medio (CABRA…, JABRA…, PALABRA…, HABRA…, ABRACADABRA…). Coincide con el revisor.
- **Lo que el revisor no dice y refuerza la cautela:** SECOP I tiene **otra persona natural con los mismos dos apellidos**, con otra identificación (tres contratos con el IDRD de Bogotá, 2018-2019). La combinación de apellidos no es única. Y no hay ningún documento que una la firma del sitio con la cédula de SECOP. **Homonimia no descartada.**

### Motivo de cada rechazo

No se rechaza entera ninguna objeción. Se rechazan como hecho, o se corrigen, estas partes:
- **Obj. 3: la identidad entre la firma del sitio y el contratista de SECOP.** Coinciden nombre, ciudad y oficio, pero eso no basta: hay otra persona con los mismos apellidos, y ningún documento enlaza los dos registros. El revisor lo marca como inferencia. Aquí **no entra como hecho**, igual que las homonimias de la tanda 4 (DECISIONES.md 2026-10-08, punto 6). Tampoco entra que Atis Bernal sea dueño o director: solo consta que firma dos columnas y que el slug de la cuenta lleva su apellido.
- **Obj. 2: el ejemplo «Petro desmintió y lo peinó a Duque» (27-03-2025).** Está fuera de los 12 meses.
- **Obj. 2(c): «no vi ninguno crítico» como barrido de titulares.** Se sostiene, ahora con los cuerpos, pero el barrido es de este verificador, no del revisor.

### Fuentes falsas, inexistentes o deformadas

**Ninguna fuente inexistente.** Todas las URL resuelven (200), las citas son literales y las cifras de SECOP y RUES coinciden al peso. Deformaciones y omisiones:
- **«La única columna firmada por una persona con ese apellido es […] (2025-11-04)»:** falso. Hay otra del 09-11-2024.
- **Obando, «2026-06-30 … 2026-08-24», con seis fechas:** son siete. La del 03-07-2026 va firmada «Po: Pablo Emilio Obando A.» y **es un contrapeso**: desmiente un bulo contra el presidente electo.
- **«La última entrada es del 2026-10-08T13:50:53»:** es la última de **Opinión**. La última del sitio es de las 18:52 (hora de Colombia), que es el pubDate del feed («23:52:00 +0000»). Lo que el revisor dice del feed es exacto; lo que dice de la «última entrada», no.
- **«40 resultados por búsqueda»:** es el tamaño de página que eligió. `X-WP-Total` da 66 para «Petro» y 54 para «director» y para «Atis». Para «Atis», la búsqueda de WordPress devuelve también entradas en las que «Atis» no aparece como palabra (en el texto de las 1.662 entradas solo está en dos firmas). Lo declara como límite, así que no es deformación, pero el barrido quedaba incompleto.
- **Omite los contrapesos de después del 07-08** (cárceles, fotomultas, Eln) y las columnas de Obando del 03-07 y el 09-07. No cambian la dirección, pero el expediente las necesita.
- **Omite el otro titular de los mismos apellidos en SECOP I.**
- **Errores de la propia ficha, para no repetirlos:**
  - «no hay sección de opinión identificable»: falso, también el día del alta;
  - «Todas sus piezas van firmadas por la cabecera»: falso en el texto, cierto solo en los metadatos;
  - «Nada de lo observable lo sitúa en el eje»: falso, ver obj. 2;
  - en `mediaOwnership.js`, «NO PUBLICA NI UN NOMBRE PROPIO más allá de la firma "ABRA NOTICIAS"»: falso, hay una firma personal y un slug con apellido;
  - en `mediaRegistry.js`, «Orientación mixta provisional por ausencia de evidencia»: falso;
  - en `centinela.js` (comentario de cabecera), «ningún nombre publicado»: ya no es exacto, aunque el nombre que hay no es de propietario;
  - falta la línea de contratación pública que exige el protocolo desde el 2026-10-07.
- **Lo que la ficha sí tenía bien, hoy:**
  - el contacto de plantilla («555-0156», «23 Miller Court», «Hagerstown», «[correo omitido]», una aparición de cada uno en el HTML crudo);
  - el pie «Copyright &copy; Todos los derechos reservados.» sin titular;
  - el feed: HTTP 200, 10 ítems, 0 `enclosure`/`media:content`;
  - que no hay página de «quiénes somos» ni de contacto (404).
  - La portada no enlaza a redes propias: «youtube» solo aparece en clases CSS del tema.

---

**Propuesta para la firma**

El responsable editorial está decidiendo si el nivel 2 se sigue exigiendo como «90 días de compañía medida» o si basta la evidencia editorial histórica a los dos lados del cambio de gobierno. Van las dos lecturas.

**(a) Con la regla vigente: mantener 0,00, provisional y NO firmable. Lo que cambia es la razón escrita.**
- **No se mueve**:
  - por la **regla 3**: no hay nivel 1 (no hay sociedad, NIT ni dueño), ni nivel 3, ni nivel 2 suficiente. La conducta medida tiene 38 días, por debajo de los 90, y **solo 6 de 105 artículos entraron en alguna historia**: con esa base, la «agenda propia» del 83 % y la compañía de 0,25 no sostienen nada, y la compañía está además saturada;
  - por la **regla 2**: ante la duda, la banda mixta.
- **La razón actual («nada de lo observable lo sitúa en el eje») ya no se sostiene.** Razón nueva propuesta: «0,00 por la regla 3, no por ausencia de evidencia. En los últimos 12 meses, la voz de la casa se inclina a la izquierda a los dos lados del cambio de gobierno (nivel 5): ninguna pieza propia critica al gobierno Petro; lo celebra (16-10-2025) y lo defiende (31-10-2025); rotula solo a un lado («extrema derecha», «ultra derecha»); insulta al presidente entrante («fantoche y payaso», 01-09-2026) y absuelve de forma expresa al saliente. Una columna firmada por Rober Atis Bernal toma partido en la campaña (04-11-2025). Contrapesos: recoge con aprobación medidas de seguridad del nuevo gobierno, y sus columnistas más frecuentes tratan al presidente con respeto institucional. Sin nivel 1-3 ni 90 días de corpus, el número no se mueve; la tensión se declara».
- Es **la misma solución que Proclama** (izquierda, nivel 5, 0,00) y El Pilón (derecha, nivel 5, se quedó en su valor) en la tanda 4. Moverlo solo a él rompería la simetría.

**(b) Si contara la asimetría editorial histórica sostenida: −0,25 (izquierda moderada), con la magnitud declarada como juicio.**
- **Evidencia que lo sostiene**, toda de nivel 5 y de los últimos 12 meses:
  1. Los rótulos ideológicos de la casa van a un solo lado, antes (02-06, 30-06, 08-07) y después (04-09, 14-09) del 07-08-2026.
  2. La absolución expresa del gobierno saliente y los insultos al entrante, en la única pieza de Opinión sin firma con postura (01-09-2026).
  3. Cero piezas de la casa críticas con el gobierno Petro en las 518 entradas anteriores al cambio (barrido por términos sobre los cuerpos, no lectura íntegra), y dos que lo celebran o lo defienden (16-10 y 31-10-2025).
  4. La toma de partido en campaña de la columna de Atis Bernal (04-11-2025).
- **Por qué −0,25 y no más:**
  - **Regla 2**: se elige la banda más cercana a la mixta, y dentro de ella el valor más bajo que no quede en el borde. Es lo que se hizo con El País (−0,25), que también rotula solo a De la Espriella.
  - **Los contrapesos son reales**: aprobación de medidas de seguridad, columnistas institucionales.
  - **El volumen es pequeño** (unas 20 piezas con postura en 751).
  - **No hay propiedad conocida** ni endoso formal («votaremos por…»). La columna de Atis Bernal toma partido, pero no consta que hable en nombre de la casa.
  - Por eso no se acerca a Colombia Informa (−0,55) ni a VOZ (−0,80), que tienen control orgánico o endoso.
- **Descartado en (b):**
  - −0,20, en el borde: el empate en el umbral es lo que se evitó con El País;
  - −0,35 o más: exigiría un endoso de la casa o una propiedad documentada.
- **Lo que (b) arrastra:** si la regla cambia, **se aplica a la vez** a Proclama del Pacífico (izquierda, nivel 5, más fuerte: endoso del 21-06) y a El Pilón (derecha, nivel 5). Moverlo solo a él sería asimétrico.

**(c) Correcciones de hecho, con su fuente** (valen en las dos lecturas)

En `fichas/abra-noticias.md`:
1. **POR QUÉ 0,00:** retirar «Nada de lo observable lo sitúa en el eje. Sus piezas van firmadas por la cabecera y no hay sección de opinión identificable». Sustituirlo por la razón de (a), o por la de (b) si el responsable editorial cambia la regla.
2. **Nivel 1, fila «Director / editor»:** «no publicado» se mantiene, con esta precisión: «El sitio no nombra director. Publica desde dos cuentas de WordPress, "adminabra" (hasta marzo de 2025) y "ABRA NOTICIAS", cuyo slug es `atisbernal` (desde abril de 2025), según `/wp-json/wp/v2/users` (2026-10-08). Rober Atis Bernal firma dos columnas de Opinión (09-11-2024 y 04-11-2025). Que sea quien dirige o posee el medio no consta». Sin cédula, sin SECOP como suyo.
3. **Nivel 4/5, sección nueva «Opinión»:** 23 entradas (2024-01-12 → 2026-10-08), con el recuento de firmas de arriba y el enlace `https://abranoticias.com/category/opinion/`.
4. **Nivel 5, nuevo:** la tabla del barrido, con los enlaces y las citas verificadas: dirección izquierda (16-10 y 31-10-2025; 04-11-2025; 02-06, 30-06, 08-07, 01-09, 04-09, 10-09, 12-09 y 14-09-2026) y contrapesos (04-02, 03-07, 09-07, 10-07, 08-09, 11-09 y 12-09-2026).
5. **LO QUE FALTA 3:** «Todas sus piezas van firmadas por la cabecera» → «Las noticias van sin firma y con la cuenta de la casa como autor; Opinión tiene columnistas firmados. Falta saber quién dirige: la firma y el slug "Atis Bernal" son la única pista, sin confirmar».
6. **Nivel 2:** las cifras de 38 días con su advertencia, y que **solo 6 de 105 artículos entraron en una historia**. Retirar «Corpus propio. Entra hoy» de REFUTACIÓN 3 o fecharlo.
7. **CONTRATACIÓN PÚBLICA**, línea nueva en el formato del protocolo:

> Contratación pública: NIT no localizado. Por nombre («ABRA NOTICIA»), 0 contratos en SECOP I y II y 0 matrículas en el RUES a 2026-10-08. No se atribuye al medio ninguna contratación de personas naturales: un homónimo probable del firmante de dos columnas tiene 3 contratos (2021-2023, Personería de Pasto) y la identidad no está probada.

8. **REFUTACIÓN:** añadir «si un documento del propio medio, de la Cámara de Comercio o de MinTIC nombra a su director o titular» y, en (a), «si la ingesta alcanza los 90 días con base suficiente en historias».
9. **Tensión declarada:** dirección izquierda en nivel 5, sin nivel 1-3 (ver (a)).

En `shared/mediaOwnership.js`, entrada `abra-noticias`:
10. `notes[2]` («NO PUBLICA NI UN NOMBRE PROPIO…») → «No publica razón social, NIT ni director. Las noticias van con la firma de la casa; la sección Opinión tiene columnistas firmados, y dos columnas (2024 y 2025) van firmadas por Rober Atis Bernal, cuyo apellido coincide con el slug de la cuenta que publica el sitio desde abril de 2025. Que dirija o posea el medio no consta».
11. `buscadoEn`: añadir la consulta a `/wp-json/wp/v2/users` y `/wp/v2/pages` (vacía), y las de RUES, SECOP I y II por nombre, con resultado 0 (2026-10-08). Actualizar «Diez rutas institucionales»: `/quienes-somos/` y `/contacto/` siguen en 404 a 2026-10-08.
12. `falta[2]`: el texto del punto 5.
13. `sources`: añadir `https://abranoticias.com/category/opinion/` y `https://abranoticias.com/wp-json/wp/v2/users`.

En `shared/mediaRegistry.js`:
14. `biasRationale`: sustituir «Orientación mixta provisional por ausencia de evidencia» por la razón de (a) abreviada: «0,00 por la regla 3, no por ausencia de evidencia: su voz propia se inclina a la izquierda a los dos lados del cambio de gobierno (nivel 5), sin propiedad conocida ni corpus suficiente».

En `shared/centinela.js` (comentario):
15. Abra Noticias tiene ahora un nombre publicado (Rober Atis Bernal, firmante de columnas), pero no como titular. **Decisión del responsable editorial:** si se vigila ese nombre, se vigila como firmante, no como dueño. Recomendación: **no** vigilarlo hasta que conste su papel. El comentario se actualiza en cualquier caso.

**(d) Tensiones a declarar**
1. **Dirección izquierda en nivel 5, sin nivel 1-3 ni corpus suficiente** (ver (a)).
2. **Un medio sin dueño conocido ni contacto real, con voz política propia.** No hay a quién atribuir la línea que la casa sostiene sin firma.

**¿Aviso de quien dirige?** No procede: no consta quién dirige, ni candidatura o cargo público vigente de nadie vinculado al medio. El contrato de 2023 con la Personería de Pasto, aunque fuera de la misma persona, no está vigente.

**Lo que NO entra como hecho:**
- que Rober Atis Bernal sea el director, el titular o el administrador de la cuenta `atisbernal`;
- que sea la misma persona que el contratista de SECOP (homonimia no descartada; hay otra persona con los mismos apellidos);
- cualquier contratación pública atribuida al medio;
- la conducta medida como evidencia de dirección (6 artículos en historias);
- el ejemplo de marzo de 2025, por la regla del presente.

**Decisiones para el responsable editorial:**
1. **Regla del nivel 2** (la que está en juego). Recomendación: **(a), mantener 0,00 con la razón nueva**, mientras no cambie la regla. Si la cambia, **(b) −0,25**, aplicado en la misma decisión a Proclama del Pacífico y El Pilón.
2. **Si la ficha nombra a Rober Atis Bernal.** Recomendación: **sí, como firmante de dos columnas y como slug de la cuenta, con el «no consta» escrito**; sin SECOP.
3. **Centinela.** Recomendación: no vigilar el nombre todavía.
4. **Nariño Ahora.** La ficha dice que, si esta no se puede cerrar, convendría reconsiderar `narinoahora.com`. Esta revisión no lo hace necesario: la ficha se puede corregir. Pero sigue sin dueño ni contacto real, y eso pesa en la elección del medio de Nariño. Queda anotado, sin recomendación.
