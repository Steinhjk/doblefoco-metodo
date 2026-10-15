# Diario del Sur (Pasto) — ficha de orientación

| | |
|---|---|
| **Medio** | Diario del Sur (Pasto) · `diario-del-sur` · — |
| **Valor vigente** | **ninguno** — **sin alta**: dos bloqueos, de gobernanza y técnico |
| **Firma** | ☐ no procede: no hay número que firmar |
| **Alta** | 2026-08-09 (candidatura) |
| **Última revisión** | ciclo 2, tanda 6, 2026-10-10 · **sigue sin alta**, con los dos bloqueos reescritos (decisión del responsable editorial, 2026-10-10) |
| **Departamento / ámbito** | Nariño |
| **Fuentes de propiedad** | — |
| **Recogida** | — |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

> **Dos bloqueos independientes, y cualquiera de los dos basta.** Uno es de
> gobernanza: la sociedad editora histórica está **en liquidación, con la
> matrícula activa**, y una sociedad distinta y activa (NIT 901804010),
> constituida en Bogotá en 2024, factura publicidad en el periódico **sin que
> conste quién la controla**. El otro es técnico: el feed de agosto venía sin
> fechas; hoy no es comprobable por nosotros y la ruta que se conocía da 404. Su
> robots.txt excluye a los agentes de Anthropic, de modo que ni siquiera podemos
> comprobarlo con la revisión habitual.

> **Nota de método.** diariodelsur.com.co **no se consulta en las revisiones**:
> su robots.txt excluye a ClaudeBot, anthropic-ai, Claude-Web y Claude-User
> (2026-10-10; en febrero y marzo de 2026 ya excluía a ClaudeBot). Lo que solo
> consta allí queda como «no verificable por exclusión de robots.txt». **Es un
> bloqueo de revisión, no de ingesta**: el motor se presenta como `DobleFocoBot`
> (`shared/userAgent.js`) y ese robots abre a «User-agent: *» con «Allow: /».
> Del dominio solo se leyó el robots.txt.

## Evidencia

### Nivel 1 — Quién lo posee, hoy: no consta

| Dato | Valor | Fuente |
|---|---|---|
| Empresa editora (histórica) | **Grupo Editorial Diario del Sur S.A.S. en liquidación**, NIT 891222292, matrícula 13825 de Pasto | [RUES abierto](https://www.datos.gov.co/resource/c82u-588k.json?$select=razon_social,sigla,nit,camara_comercio,matricula,organizacion_juridica,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,fecha_cancelacion,cod_ciiu_act_econ_pri&nit=891222292), registro actualizado el 2025-03-11, consultado el 2026-10-10 |
| Matrícula RUES | **Activa, en liquidación**; última renovación 2024 (RUES abierto y DataCrédito, 2026-10-10). Un agregador ([empresas.larepublica.co](https://empresas.larepublica.co/colombia/narino/pasto/grupo-editorial-diario-del-sur-sas-891222292)) la da por cancelada, sin fecha. **Falta el certificado de la Cámara de Comercio de Pasto** | ídem |
| Constitución | 26-08-1983 (el RUES da como fecha de matrícula el 29-08-1983) | DataCrédito Empresas; RUES |
| **Otra sociedad con el nombre del diario** | **Ediciones Periodísticas Diario del Sur S.A.S.**, NIT 901804010, matrícula 3786278 de Bogotá, constituida el 22-02-2024, activa, renovada el 14-07-2026; CIIU 1811 (impresión) y 5813 (edición de periódicos); representante legal según el RUES: Miguel Ángel Arellano Cantillo. Factura publicidad «en el periódico Diario del Sur» (SECOP I, 24-07-2025). **No consta que sea la editora, ni quiénes son sus socios** | [RUES abierto](https://www.datos.gov.co/resource/c82u-588k.json?$select=razon_social,sigla,nit,camara_comercio,matricula,organizacion_juridica,estado_matricula,fecha_matricula,fecha_renovacion,ultimo_ano_renovado,fecha_cancelacion,cod_ciiu_act_econ_pri,representante_legal&nit=901804010), 2026-10-10; [SECOP I](https://www.datos.gov.co/resource/f789-7hwg.json?$select=numero_de_constancia,nombre_entidad,nom_razon_social_contratista,fecha_de_firma_del_contrato,cuantia_contrato,valor_total_de_adiciones,detalle_del_objeto_a_contratar,estado_del_proceso&identificacion_del_contratista=901804010) |
| Propietario y gerente | **no constan en un registro actual** (ver la nota) | — |
| Circulación | Nariño y Putumayo, de lunes a domingo | Wikipedia (nivel 4) |
| Gremio | Afiliado a Andiarios, **según una página de 2010** | Wikipedia, que remite a Andiarios (2010) |

**Nota sobre propietario y gerente.** Según la Wikipedia (`dateModified`
2026-09-17), que remite a una página de Andiarios archivada en 2010, el
propietario y director es Hernando Suárez Burgos y el gerente, Ronald Tupaz
Bustos. Esta ficha los atribuía a DataCrédito Empresas, y su página pública no
los trae. Ningún registro de 2025-2026 consultado los une a ninguna de las dos
sociedades. Su única fuente verificable tiene 16 años: no se usan como dato de
propiedad.

**El problema no es solo lo que la información dice, sino que no consta quién
edita hoy el periódico.** (Esta ficha decía el 2026-08-09 que el nivel 1 estaba
«mejor cubierto aquí que en varias fichas del catálogo»: se retira.)

### Nivel 2 — Conducta medida: NO EXISTE, y hoy no es comprobable

**El 2026-08-09, el feed traía los `<pubDate>` vacíos.** Se descargó y se miró:
diez artículos, la etiqueta presente en los diez, sin contenido dentro.

```xml
<title>Karol G sorprende a sus seguidores con novedades sobre su nuevo álbum</title>
<pubDate></pubDate>
```

**Hoy no se ha podido comprobar.** El Internet Archive registra
`https://www.diariodelsur.com.co/feed/` como `application/rss+xml 200` en trece
capturas entre el 2026-01-01 y el 2026-05-01 y, el 2026-10-06, `/feed/` → 308 →
`/feed` 404, con un `sitemap.xml` nuevo (200) en lugar del `sitemap_index.xml`
de Yoast. No se comprobó directamente: el robots.txt (2026-10-10) excluye a
ClaudeBot, anthropic-ai, Claude-Web y Claude-User. Tampoco hay copia de agosto
del robots.txt, así que no se puede saber si la descarga del 2026-08-09 lo
respetaba (cambió de un mes a otro: en febrero y marzo excluía a ClaudeBot; en
enero, abril y mayo era solo el bloque de Yoast).

**Por qué un feed sin fechas es descalificante y no un detalle de formato:**

- Sin `publishedAt`, la **poda por retención** no sabe cuándo caducan sus
  artículos: se quedarían en el corpus indefinidamente o se irían todos a la vez.
- **«Más recientes» no puede ordenarlos.** Entrarían al feed en una posición
  arbitraria.
- La **cronología de cobertura** de cualquier historia que toquen quedaría
  falseada.

Y la salida fácil —ponerles la fecha de la descarga— es justamente la que no se
puede tomar: **convertiría a Diario del Sur en el medio más al día del catálogo
por un defecto de su feed**, y sería un dato inventado presentado como medido.
Eso es la fabricación que este proyecto se quitó de encima en la Fase 0.

### Sobre el titular que salió en la muestra

El artículo más reciente de su feed era sobre el nuevo álbum de Karol G. Un
titular no es una muestra y **no lo uso como evidencia de nada** — se anota
solo porque quien lea esta ficha verá el ejemplo de arriba y merece saber que no
se eligió para insinuar nada sobre su agenda.

## Argumento

### POR QUÉ NO SE PROPONE NÚMERO

Ninguna evidencia sitúa al medio en el eje. Lo que hay pone en duda quién edita
hoy el periódico y si su feed sirve, no su línea. Regla 4 del protocolo: *es
mejor que quede sin firmar.*

## Qué cambiaría el número

### REFUTACIÓN — qué reabriría el expediente

1. **Que el responsable editorial compruebe, sin pasar por un agente de Anthropic, que el sitio
   publica un feed con fechas** (`npm run feed:descubrir -- diariodelsur.com.co`,
   ejecutado por él), y que el uso que haría DobleFoco encaje en su
   «Content-Signal».
2. **Que un certificado de existencia y representación, o un documento del
   propio medio, diga qué sociedad edita hoy el periódico y quién la controla.**
3. **Que se documente el papel actual de Hernando Suárez Burgos** con una fuente
   posterior a 2010.

## Tensiones declaradas

### TENSIONES (2026-10-10)

1. **Una sociedad activa con el nombre del diario cobra a gobiernos locales por
   publicar en él, y no se sabe quién la controla.**
2. **Pauta y arrendamiento con la Alcaldía de Pasto (2018-2019) y con el
   departamento (EDINAR, 2019)**, gobiernos que el medio cubre. No están
   vigentes.
3. El «Content-Signal: … ai-train=no, use=reference» es una reserva de derechos
   del medio. Si mostrar titulares y enlaces encaja en «use=reference» es una
   decisión del responsable editorial, que esta ficha no toma.

**Sin aviso de quien dirige:** el medio no está en el catálogo y no consta quién
lo dirige hoy.

### LO QUE ESTO DEJA ABIERTO

**Diario del Sur era, el 2026-08-09, el único candidato de Nariño con feed.**
Ya no hace falta: **Nariño tiene a Abra Noticias en el catálogo**, y Nariño
Ahora quedó anotado como alternativa (`fichas/abra-noticias.md`).

Si se quiere retomar:

1. **Escribirles** para preguntar por la URL del feed tras el cambio del sitio y
   por la sociedad que edita hoy el periódico.
2. **Solo si el feed sigue sin fechas**, decidir explícitamente qué fecha se les
   pone y **declararlo en la página de transparencia** — nunca en silencio.

## Contratación pública

Contratación pública (SECOP I y II, NIT 891222292, consultado 2026-10-10): **0
contratos en los últimos 12 meses**; **24 por $1.214.849.816 contratados en
total desde 2017** (23 en SECOP I, 2017-2022, y 1 en SECOP II, 2020, cargado
con el dígito de verificación). Principales contratantes: **Alcaldía de Pasto,
$981.600.000 en dos contratos de arrendamiento de un inmueble de la sociedad**
(2018 y 2019), **no de publicidad**; Empresa Editora de Nariño (EDINAR, del
departamento), $109.000.000 en divulgación institucional (2019); Terminal de
Transporte de Ipiales, $40.710.000 (2022). **La Alcaldía de Pasto y el
departamento de Nariño son gobiernos que el medio cubre.** Ediciones
Periodísticas Diario del Sur S.A.S. (NIT 901804010): **1 contrato por
$2.700.000 en los últimos 12 meses** (Cámara de Comercio de Tumaco,
2026-09-11) y **2 por $7.700.000 desde 2025** (también Alcaldía de La Florida,
2025-07-24, publicación «en el periódico Diario del Sur»).

- Sin los dos arrendamientos, la contratación de publicidad, suscripciones y
  avisos es de $232.893.816 en 21 contratos.
- Por nombre aparecen 3 contratos más en SECOP I (2018-2019, $49.020.800)
  cargados con identificaciones mal escritas o con la de una persona natural.
  No entran en el recuento por igualdad exacta; se anotan para que nadie los
  sume sin saberlo.
- «Contratado», nunca «cobrado».

## Historial

### HALLAZGOS DEL CICLO 2 (2026-10-10)

Lo que la revisión externa del ciclo 2 y su verificación encontraron, con cada
fuente comprobada de nuevo el 2026-10-10. El responsable editorial decidió el 2026-10-10 que la
candidatura sigue sin alta, con los bloqueos reescritos. Fuente:
`revision-externa/respuestas/opus-5-5-diario-del-sur.md`, RESOLUCIÓN,
«Propuesta para la firma».

**Entran como hecho:**

1. **La editora histórica está en liquidación con la matrícula ACTIVA, no
   cancelada.** GRUPO EDITORIAL DIARIO DEL SUR SAS EN LIQUIDACION, NIT
   891222292, matrícula 13825 de Pasto: «ACTIVA», última renovación 2024
   (RUES abierto, registro actualizado el 2025-03-11; DataCrédito, «MATRÍCULA
   ACTIVA»). Solo un agregador (empresas.larepublica.co) la da por cancelada,
   sin fecha, y esa página no dice «en liquidación».
2. **Hay otra sociedad activa con el nombre del diario.** EDICIONES
   PERIODISTICAS DIARIO DEL SUR S.A.S, NIT **901804010**, matrícula 3786278 de
   Bogotá, constituida el 22-02-2024, activa, renovada el 14-07-2026;
   representante legal según el RUES: Miguel Ángel Arellano Cantillo. **Factura
   publicidad «en el periódico Diario del Sur»** (SECOP I, Alcaldía de La
   Florida, 24-07-2025, $5.000.000).
3. **El feed que se conocía ya no responde.** El Internet Archive registra
   `/feed/` como RSS 200 hasta mayo de 2026 y, el 2026-10-06, `/feed/` → 308 →
   `/feed` 404, con un `sitemap.xml` nuevo en lugar del `sitemap_index.xml` de
   Yoast. Solo metadatos CDX: no se descargó contenido.
4. **El robots.txt excluye a ClaudeBot, anthropic-ai, Claude-Web y Claude-User**
   y declara «Content-Signal: search=yes,ai-train=no,use=reference»
   (2026-10-10, 3.369 bytes).
5. **Los nombres de propietario y gerente no tienen fuente actual.** La página
   pública de DataCrédito no los trae; la Wikipedia los apoya en una página de
   Andiarios archivada en 2010.
6. **El 81 % de la contratación pública de la editora histórica es
   arrendamiento de un inmueble a la Alcaldía de Pasto, no pauta.** Ver
   «Contratación pública».

**Lo que NO entra como hecho:**

- que Ediciones Periodísticas Diario del Sur S.A.S. sea la editora, o que haya
  cesión de marca o de negocio;
- que la matrícula 13825 (NIT 891222292) esté cancelada;
- que Hernando Suárez Burgos siga siendo propietario o director, o que Ronald
  Tupaz Bustos sea el gerente hoy;
- que «Robert Atis Bernal», editor jefe según la Wikipedia, lo sea, ni que sea
  la misma persona que firma columnas en Abra Noticias;
- que el sitio haya migrado de plataforma (es compatible con los metadatos, no
  está probado);
- la «tirada» de 240.964 que da la Wikipedia;
- que el contrato de la Cámara de Comercio de Tumaco (2026-09-11) se publicara
  en Diario del Sur: su objeto no nombra el periódico.

### REVISIÓN EXTERNA

Ciclo 2, tanda 6: `revision-externa/respuestas/opus-5-5-diario-del-sur.md`. El
revisor es de la misma casa que el autor de esta ficha y que quien escribió la
resolución: el acuerdo entre los tres no es aval.
