# El Informador (Santa Marta) — ficha de orientación

| | |
|---|---|
| **Medio** | El Informador · `el-informador` · elinformador.com.co |
| **Valor vigente** | **+0,45** · Derecha moderada — **en catálogo, firmado en bloque el 2026-10-10** (antes, provisional y no firmado; barrido de la voz de la casa y endoso explícito) |
| **Firma** | ☑ **FIRMADA el 2026-10-10 — el responsable editorial** (firma en bloque tras el ciclo 2; ver DECISIONES.md. Lo que más abajo dice «sin firmar», «no se firma» o «provisional» es el estado anterior a esta firma y se conserva como historia) |
| **Alta** | 2026-10-10 · sustituye a la candidatura del 2026-08-09 |
| **Última revisión** | 2026-10-10 · ciclo 2, tanda 7; correcciones de hecho aplicadas; valor decidido por el responsable editorial; firmado en bloque el 2026-10-10 (antes, sin firmar) |
| **Departamento / ámbito** | Magdalena — **segundo medio del departamento en el catálogo**, tras Seguimiento.co |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`el-informador`): 7 fuentes |
| **Recogida** | `https://www.elinformador.com.co/index.php/general?format=feed&type=rss` · vía `direct` |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

> **El +0,45 es un juicio declarado, no una medición, y pasa del tope de
> ±0,30 a propósito.** El protocolo, §1, «Cuánto mueve»: «Sin propiedad
> documentada con posición conocida (nivel 1) **ni endoso explícito**, la
> magnitud no pasa de ±0,30». Aquí hay endoso explícito con nombre, en
> editorial sin firma, el día de la segunda vuelta (21-06-2026). Es la decisión
> del responsable editorial del 2026-10-10. **Mover el valor no hace firmable la ficha:** faltan
> los accionistas.

**+0,45 provisional, sin firmar.** La firma espera al certificado de la Cámara
(accionistas). El barrido se rehace a los seis meses del cambio de gobierno
(febrero de 2027), o antes si se cumple la REFUTACIÓN 3.

### LO QUE HAY QUE HACER

**Pedir el certificado de existencia y representación a la Cámara de Comercio
de Santa Marta para el Magdalena**, ahora solo por los accionistas y por la
discrepancia del representante legal. Va en la cola detrás del certificado de
prueba decidido el 2026-10-09.

## Evidencia

### Nivel 1 — Quién lo edita: la sociedad sí, los socios no

| Dato | Valor | Fuente |
|---|---|---|
| Sociedad | **EDITORIAL MAGDALENA S.A.** | RUES, datos.gov.co `c82u-588k`, 2026-10-10 |
| NIT | 819003317-4 | ídem |
| Matrícula | 60801, Cámara de Comercio de Santa Marta para el Magdalena, del 05-01-2000; renovada el 27-03-2026; ACTIVA; sociedad anónima; CIIU 5813; proponente | ídem |
| Representante legal | Alfonso Vives Campo (RUES, actualizado el 28-03-2026) | ídem |
| Socios | **no constan**: el RUES abierto no los publica | — |
| Director de la redacción | **no consta**: el medio no publica créditos | portada y sección Editorial, 2026-10-10 |
| Sede | Santa Marta | [elinformador.com.co](https://www.elinformador.com.co/) |

Hay NIT, matrícula activa y representante legal en el RUES abierto
(2026-10-10), que la búsqueda del 2026-08-09 en espejos no encontró. Lo que
falta son los accionistas, que están en el certificado de pago de la Cámara.

Consulta sin datos personales (con `$select`):
[RUES, NIT 819003317](https://www.datos.gov.co/resource/c82u-588k.json?nit=819003317&$select=razon_social,nit,matricula,camara_comercio,estado_matricula,fecha_renovacion,organizacion_juridica,cod_ciiu_act_econ_pri,representante_legal,fecha_actualizacion).

### Nivel 2 — Evidencia editorial histórica (regla del 2026-10-09)

Barrido completo y reproducible:
[`revision-externa/barridos/el-informador.md`](../revision-externa/barridos/el-informador.md).

- **Universo:** el archivo mensual de la categoría Editorial (id 37) de 2025-10
  a 2026-09 y el feed de la sección para octubre: 360 páginas leídas enteras;
  353 dentro de la ventana; 343 únicas (10 editoriales se publicaron dos
  veces). Ninguna lleva autor ni firma: es voz de la casa.
- **Recuento:**

  | | Suman (D + leves) | Contrapesos | F, solo fiscaliza (no suma) |
  |---|---|---|---|
  | Antes del 07-08-2026 | **67** (58 + 9) | 2 parciales | 62 |
  | Desde el 07-08-2026 | **33** (28 + 5) | 1 pleno + 2 parciales | 0 |
  | **Total** | **100** (86 + 14) | **5** | 62 |

- **Mínimos de la regla:** ≥10 → 100; ≥3 a cada lado del 07-08 → 67 y 33 (sin
  las leves, 58 y 28); ≥3:1 → 20:1 (solo desde el 07-08, 11:1). **Se cumplen
  las cinco condiciones, con mucho margen.**
- **El endoso**, literal en el HTML de
  [«Abelardo De La Espriella o Iván Cepeda»](https://www.elinformador.com.co/index.php/opinion/37-editorial/354190-abelardo-de-la-espriella-o-ivan-cepeda)
  (`datePublished` 2026-06-21, sin autor; recomprobado el 2026-10-10): «con
  Abelardo habrá institucionalidad, democracia y libertad; con Cepeda habrá
  instituciones propias, tiranía y abolición hasta de la libertad de prensa».
- **Tomas de partido previas:** 08-03-2026, «A votar por la libertad y la
  democracia» (348748), día de legislativas, enumera los partidos por los que
  votar; 11-05-2026, «Primera vuelta presidencial» (352007): «los palomistas
  […] deberán depositar su voto por Abelardo».
- **Contrapesos:** el reparo al porte legal de armas (358422, 09-09-2026),
  pleno y de peso medio; parciales el 31-12-2025, el 14-03-2026, el 11-09 y el
  29-09-2026. La pieza sobre la reforma de Kast (30-08-2026) es internacional y
  no cuenta.

### Nivel 2 — Conducta medida en el corpus

No hay corpus todavía: el medio entra hoy. El número descansa en la voz de la
casa y en el endoso, no en la cobertura.

### Lo que NO cuenta, aunque salga en todas partes

«El diario tradicional del Departamento», «fundado en 1958», «decano de la
prensa samaria». Son efemérides y **la regla del presente las excluye**. La
antigüedad no es una posición.

## Barrido de 12 meses

| | |
|---|---|
| **Barrido** | [`revision-externa/barridos/el-informador.md`](../revision-externa/barridos/el-informador.md) |

## Argumento

### POR QUÉ +0,45

- **La regla «Evidencia editorial histórica» se cumple con mucho margen**
  (100 a 5; 67 y 33 a los dos lados del cambio de gobierno).
- **Hay endoso explícito**, que por el §1 del protocolo levanta el tope de
  ±0,30. Es la lectura de los barridos anteriores («Si en cambio llega un
  endoso con nombre en la próxima elección, el tope de ±0,30 dejaría de
  aplicarse», `barridos/el-diario-pereira.md`, §7).
- **Por encima de los vecinos sin endoso.** The Archipielago Press (+0,30)
  llegó ahí con 26 piezas y sin endoso; El Colombiano (+0,35) celebró después
  de la elección, sin endoso previo confirmado. El Informador pidió el voto por
  Abelardo el 11-05 y lo endosó el 21-06, y rotula al gobierno anterior
  («tirano», «terrorista dictatorial») como ninguno de ellos.
- **Por debajo de El Nuevo Siglo (+0,55), que también endosó.** Faltan los
  socios (nivel 1 incompleto); la lectura es de un solo verificador de la
  misma casa; hay 3 reparos, débiles, al Gobierno entrante; y es la primera
  vez que se pasa de ±0,30 con esta excepción.
- **Alternativas declaradas:** +0,30 si se lee la regla 3 del §5 como tope sin
  salvedad; +0,55 si pesan más el endoso y los rótulos que la falta de socios.
  El barrido no sostiene 0,00 ni otra dirección.

## El mejor caso en contra

**Hacia abajo, a +0,30 (el más fuerte):**

- **Es la primera vez que se pasa de ±0,30 por la salvedad del endoso**, y el
  nivel 1 está incompleto: constan la editora, el NIT y el representante legal,
  no los socios. Leída la regla 3 del §5 como tope sin salvedad, la dirección no
  cambia y la magnitud baja a +0,30 (alternativa declarada en el barrido, §9).
  El §5 recoge la salvedad desde el 2026-10-10; lo que queda del argumento es
  que el valor exacto es un juicio contra los vecinos, no una medición.
- **La lectura es de un solo verificador**, de la misma casa que el autor de la
  ficha.
- **Hay contrapesos**: un reparo pleno al Gobierno entrante, el del porte legal
  de armas (09-09-2026), de peso medio; dos parciales también al entrante (11-09
  y 29-09-2026), y dos reconocimientos parciales a Petro antes del cambio
  (31-12-2025 y 14-03-2026). Son 5 frente a 100, y débiles.
- **Unas 170 de las 343 piezas únicas no son partidistas** (internacionales,
  locales, de servicio o deporte): la casa no habla solo de política (barrido,
  §4).

**Hacia arriba, a +0,55**, a la par de El Nuevo Siglo, que también endosó: El
Informador enumeró el 08-03-2026 los partidos por los que votar, pidió el voto
por Abelardo el 11-05 y lo endosó el 21-06; rotula al gobierno anterior
(«tirano», «terrorista dictatorial», «líder intergaláctico») sin equivalente en
Archipiélago Press ni en El Colombiano; y en las 343 piezas no hay ninguna
favorable a un candidato o gobierno de izquierda. La ficha lo deja por debajo
por la falta de socios y por no estrenar la salvedad en el techo de la banda.

**Lo que no es contra:** el elogio editorial al alcalde de Santa Marta, cabeza
de su mayor contratante, es relación con el gobierno local (tensión declarada) y
no se lee en el eje. El barrido no sostiene 0,00 ni otra banda que la derecha.

## Qué cambiaría el número

1. **El certificado de la Cámara**, por los socios: si muestra socios con
   posición conocida, el número se recalcula sobre el nivel 1.
2. **Si aparece capital de familias con cargo político en el Magdalena**, eso
   es lo primero que hay que declarar, antes que cualquier número.
3. **Si en los próximos meses la casa critica el programa del Gobierno De la
   Espriella en más de un editorial sin contrapartida**, o si el certificado
   muestra socios cuya posición contradiga la dirección.

## Tensiones declaradas

- **El mayor contratante y la voz de la casa.** Dos editoriales sin firma
  elogian al alcalde de Santa Marta, Carlos Pinedo Cuello, cabeza del mayor
  contratante, sin declarar la relación:
  [«El renacer samario»](https://www.elinformador.com.co/index.php/opinion/37-editorial/345540-el-renacer-samario)
  (31-12-2025, 35 días después del contrato de $72 M): «Hay que reconocer la
  labor del Alcalde, Carlos Pinedo Cuello…»; y
  [«La ciudad engalanada con los turistas»](https://www.elinformador.com.co/index.php/opinion/37-editorial/349934-la-ciudad-engalanada-con-los-turistas)
  (02-04-2026): «El alcalde de Santa Marta, Carlos Pinedo Cuello, ha dispuesto
  lo necesario…». Literales, recomprobados el 2026-10-10. **Desvelamiento, no
  acusación:** no consta que un editorial sea consecuencia de un contrato. No
  mueve el número. Seguimiento.co, el otro medio del Magdalena, tiene a la
  misma Alcaldía como principal cliente público.
- **El representante legal, en dos versiones** (ver HALLAZGOS). Se toma el
  RUES.

## Contratación pública

Contratación pública (SECOP I y II, NIT 819003317, consultado 2026-10-10):
**5 contratos por $112.000.000 contratados en los últimos 12 meses**
(2025-10-10 → 2026-10-10): Alcaldía Distrital de Santa Marta $72.000.000
(26-11-2025), CORPAMAG $20.000.000 (25-08-2026) y Cámara de Comercio de Santa
Marta $20.000.000 en tres avisos; **110 por $2.518.714.541 en total desde
2017** (SECOP II: 22 por $1.653.090.949; SECOP I: 88 por $865.623.592, uno de
ellos registrado con el dígito de verificación pegado al NIT). Principales
contratantes: **Alcaldía Distrital de Santa Marta** ($1.444.000.000, 10
contratos de 2020 a 2025, todos por contratación directa), Gobernación del
Magdalena ($270.090.949, el último en 2023), CORPAMAG ($241.000.000),
Universidad del Magdalena ($226.121.592, 2020-2022) y Cámara de Comercio de
Santa Marta ($187.910.000, 44 avisos). La Alcaldía y la Gobernación son
gobiernos que el medio cubre. Es valor **contratado**: SECOP II marca 0 pagado
en los de la Alcaldía.

- Constancias de SECOP I citadas (como texto, sin enlace: la página muestra
  datos personales del representante): 26-4-14686743 (20-02-2026, avisos «en
  portada de la edición impresa») y 26-4-14738224 (08-07-2026, «los 68 años
  de este medio»); 20-12-10943479 (CORPAMAG, 06-12-2019, la del NIT con el
  dígito pegado).
- Consultas sin datos personales (con `$select`):
  [SECOP II](https://www.datos.gov.co/resource/jbjy-vk9h.json?documento_proveedor=819003317&$select=id_contrato,nombre_entidad,fecha_de_firma,valor_del_contrato,modalidad_de_contratacion,descripcion_del_proceso,proveedor_adjudicado),
  [SECOP I](https://www.datos.gov.co/resource/f789-7hwg.json?identificacion_del_contratista=819003317&$select=numero_de_constancia,nombre_entidad,fecha_de_firma_del_contrato,cuantia_contrato,detalle_del_objeto_a_contratar,nom_razon_social_contratista&$limit=200)
  y [SECOP I con el dígito pegado](https://www.datos.gov.co/resource/f789-7hwg.json?identificacion_del_contratista=8190033174&$select=numero_de_constancia,nombre_entidad,fecha_de_firma_del_contrato,cuantia_contrato,detalle_del_objeto_a_contratar,nom_razon_social_contratista).
  Comprobadas el 2026-10-10: 22, 87 y 1 filas, sin ningún campo de
  identificación personal.

Es desvelamiento, no acusación, y no mueve la clasificación.

## Recogida

```
https://www.elinformador.com.co/index.php/general?format=feed&type=rss
HTTP 200 · application/rss+xml · 25 ítems · <language>en-gb (falso: publica en español)
```

Comprobado el 2026-10-10 a las 20:44 UTC: 25 ítems; los 2 primeros son viejos
(06-08 y 04-03-2026) y quedan fuera por la ventana de 72 h de la ingesta; los
otros 23 van del 09-10 05:00 al 10-10 19:29 UTC, en un orden casi
cronológico. `npm run feed:descubrir -- elinformador.com.co` encuentra el
feed raíz (`index.php?format=feed&type=rss`, 10 ítems, el último de hace 9 h):
desordenado y escaso, **no se usa**. Alternativa local:
`/index.php/la-ciudad?format=feed&type=rss`. Imágenes absolutas en
`www.elinformador.com.co`.

## Fuentes

- [Portada](https://www.elinformador.com.co/) y [sección Editorial](https://www.elinformador.com.co/index.php/opinion/37-editorial), 2026-10-10.
- Archivo mensual de la categoría 37: `https://www.elinformador.com.co/index.php?option=com_content&view=archive&year=AAAA&month=M&catid%5B%5D=37&limit=0`.
- [RUES](https://www.datos.gov.co/resource/c82u-588k.json?nit=819003317&$select=razon_social,nit,matricula,camara_comercio,estado_matricula,fecha_renovacion,organizacion_juridica,cod_ciiu_act_econ_pri,representante_legal,fecha_actualizacion), [SECOP II](https://www.datos.gov.co/resource/jbjy-vk9h.json?documento_proveedor=819003317&$select=id_contrato,nombre_entidad,fecha_de_firma,valor_del_contrato,modalidad_de_contratacion,descripcion_del_proceso,proveedor_adjudicado) y [SECOP I](https://www.datos.gov.co/resource/f789-7hwg.json?identificacion_del_contratista=819003317&$select=numero_de_constancia,nombre_entidad,fecha_de_firma_del_contrato,cuantia_contrato,detalle_del_objeto_a_contratar,nom_razon_social_contratista&$limit=200), consultados el 2026-10-10 con `$select` (regla del responsable editorial del 2026-10-10: nunca devuelven documentos de identidad).
- El barrido: [`revision-externa/barridos/el-informador.md`](../revision-externa/barridos/el-informador.md).

## Historial

### HALLAZGOS DEL CICLO 2 (2026-10-10)

Cada hallazgo se comprobó de nuevo en su fuente el 2026-10-10. Origen:
`revision-externa/respuestas/opus-5-5-el-informador.md` (RESOLUCIÓN,
«Propuesta para la firma»), con las decisiones del responsable editorial del 2026-10-10.

- **La editora está en el registro mercantil.** EDITORIAL MAGDALENA S.A., NIT
  819003317-4, matrícula 60801 de la Cámara de Comercio de Santa Marta para el
  Magdalena, del 05-01-2000, renovada el 27-03-2026, ACTIVA, sociedad anónima,
  CIIU 5813 (edición de periódicos), inscrita como proponente. Representante
  legal: **Alfonso Vives Campo** (RUES, datos.gov.co `c82u-588k`, registro
  actualizado el 28-03-2026; comprobado el 2026-10-10). La ficha del
  2026-08-09 decía que no aparecía en los espejos del RUES: fallo de método,
  no del registro. **Los socios no constan.**
- **Que esa sociedad edita el periódico consta en SECOP:** 60 de sus 87
  registros de SECOP I y 10 de sus 22 contratos de SECOP II nombran «El
  Informador» en el objeto. El medio no publica la razón social.
- **Contratación pública**, obligatoria desde el 2026-10-07: 110 registros por
  $2.518.714.541 desde 2017; 5 por $112.000.000 en los últimos 12 meses. Su
  mayor cliente público es la **Alcaldía Distrital de Santa Marta**. Ver
  «Contratación pública».
- **Hay voz de la casa, y mucha.** La sección Editorial publica un editorial sin
  firma casi a diario. El barrido de los 12 meses (353 piezas en la ventana,
  343 únicas, leídas enteras) da **100 piezas con postura en la misma
  dirección frente a 5 contrapesos**, 67 antes del 07-08-2026 y 33 después.
  La ficha decía «Nivel 2: NO EXISTE» sin haber mirado esa sección.
- **Endoso explícito con nombre** el 21-06-2026, día de la segunda vuelta, y
  peticiones de voto previas (08-03 y 11-05-2026). Ver «Nivel 2».
- **Tensión con el mayor contratante:** dos editoriales sin firma elogian al
  alcalde de Santa Marta sin declarar la relación. Desvelamiento, no
  acusación.
- **El representante legal no coincide entre RUES y SECOP.** Los 22 contratos
  de SECOP II (2020-2026) y 42 de los 87 de SECOP I consignan en ese campo a
  otra persona natural. **El representante legal se toma del RUES**; la otra
  persona no se nombra aquí. Puede ser un suplente, una gerencia o un dato de
  proveedor sin actualizar: no consta cuál. Lo resuelve el certificado de la
  Cámara.
- **El feed raíz no sirve para ingerir**: 10 ítems desordenados. Se ingiere
  por la categoría `general` (ver «El feed»).
- **«Es el más activo de Magdalena»** se retira: no tiene fuente.

**Lo que NO entra como hecho:**

- **Quiénes son los socios**, ni el beneficiario final.
- **Quién dirige la redacción.** El medio no publica créditos; la única fuente
  que nombraba a un director (un estudio en vlex.com.co, sin fecha) está vetada
  por su robots.txt para los agentes de Anthropic y no se usa.
- **Cualquier parentesco o cargo político** del representante legal o de la
  persona que SECOP consigna. Las coincidencias de apellido, incluida la de la
  cancelada Editorial Santa Marta Limitada, no prueban nada y no se afirman.
- **Que algún editorial sea consecuencia de un contrato** con la Alcaldía.
- **Qué fuerza política gobierna la Alcaldía.** Aquí solo consta el nombre del
  alcalde, por los propios editoriales.
- **La fecha de fundación (1958)** como evidencia: es efeméride.

### REVISIÓN EXTERNA

☑ **Ciclo 2 hecho** (Claude Opus 5.5, `claude-opus-5-5`, resuelto el
2026-10-10): `revision-externa/respuestas/opus-5-5-el-informador.md`. Cinco
objeciones, ninguna rechazada entera: la 1 (RUES) y la 4 (propiedad sin
fuente), aceptadas; la 2 (contratación), aceptada con un contrato más (110 y
$2.518.714.541); la 3 (voz de la casa), aceptada en la dirección y con el
recuento corregido de 24 a 100; la 5 (feed), parcial. El responsable editorial decidió el
2026-10-10 el alta, el +0,45 y anotar sin nombre la discrepancia del
representante legal. **No se firma todavía.** El revisor, quien resolvió y
quien aplica son de la misma casa que el autor de esta ficha: su acuerdo no
cuenta como aval.

**Lo que se recomprobó al aplicar (2026-10-10):** robots.txt (el de Joomla por
defecto); el RUES y las tres consultas de SECOP con `$select` (1, 22, 87 y 1
filas, sin campos personales); el endoso del 21-06 y los dos editoriales sobre
el alcalde, literales y con su fecha; el feed `general`, 25 ítems. Nada de lo
que la resolución daba dejó de sostenerse.
