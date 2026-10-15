# Sucre Noticias (Sincelejo) — ficha de orientación

| | |
|---|---|
| **Medio** | Sucre Noticias · `sucre-noticias` · sucrenoticias.com |
| **Valor vigente** | **0,00** · Orientación mixta — **en catálogo, firmado en bloque el 2026-10-10** (antes, provisional y no firmado): sin nivel 1-3; alta con propiedad no comprobada |
| **Firma** | ☑ **FIRMADA el 2026-10-10 — el responsable editorial** (firma en bloque tras el ciclo 2; ver DECISIONES.md. Lo que más abajo dice «sin firmar», «no se firma» o «provisional» es el estado anterior a esta firma y se conserva como historia) |
| **Alta** | 2026-10-10 · sustituye a la candidatura del 2026-08-09 (decisión del responsable editorial: opción (c) de la resolución) |
| **Última revisión** | 2026-10-10 · ciclo 2, tanda 7; correcciones de hecho aplicadas; firmado en bloque el 2026-10-10 (antes, sin firmar) |
| **Departamento / ámbito** | Sucre — **es el primero del departamento en el catálogo** |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`sucre-noticias`): 6 fuentes |
| **Recogida** | `https://sucrenoticias.com/feed/` · vía `direct` |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

> **Lee «0,00» como «no sabemos», no como «equilibrado».** Es la Regla 2: no hay
> nivel 1, ni nivel 3, ni voz de la casa en los 12 meses. Entra porque dejar
> Sucre en blanco le diría al lector «aquí no hay medios» cuando lo cierto es
> «no sabemos de quién es». Es la distinción que motivó la AUSENCIA DECLARADA
> (`shared/mediaOwnership.js`).

**0,00, firmado en bloque el 2026-10-10** (antes, provisional sin firmar; ver DECISIONES.md). Condición de revisión: si pasa más de 30 días
sin publicar, se decide la baja.

## Evidencia

### Nivel 1 — Nada publicado, y el dominio no da titular

- No publica sociedad, NIT, propietario, director ni editor
  ([`/contacto/`](https://sucrenoticias.com/contacto/) y pie de
  [la portada](https://sucrenoticias.com/), 2026-10-10). Su JSON-LD declara
  una «Organization» llamada «sucrenoticiasof», sin razón social. No tiene
  aviso legal, política de privacidad ni términos (siete rutas habituales, 404).
- Dominio registrado el 24-05-2018, renovado (último cambio 25-05-2026, vence
  el 24-05-2027); el titular está oculto en el RDAP del registrador
  ([RDAP del registro](https://rdap.verisign.com/com/v1/domain/sucrenoticias.com)).
- Publica firmas: ocho cuentas de autor. La mayoría de las piezas de
  septiembre de 2026 las firma José Iriarte Díaz, y la cuenta «Redacción»
  tiene un identificador con su nombre. Que dirija el medio no consta.
- Declara que vende pauta (`[correo omitido]`).
- RUES abierto por razón social: 0 coincidencias
  ([consulta con `$select`](https://www.datos.gov.co/resource/c82u-588k.json?$select=razon_social,camara_comercio,estado_matricula&$where=upper(razon_social)%20like%20%27%25SUCRE%20NOTICIA%25%27),
  2026-10-10). El conjunto no incluye establecimientos de comercio.

### Nivel 4 — Lo que declara

Se define como «un medio de comunicación independiente honesto e imparcial»
([`/contacto/`](https://sucrenoticias.com/contacto/), bajo «¿Quiénes somos?»,
2026-10-10) y como «alternativa informativa y periodística independiente y de
calidad» con sede en Sincelejo (pie de [la portada](https://sucrenoticias.com/),
2026-10-10).

**Declararse independiente no es serlo.** El medio no dice quién es su dueño;
sí declara que vende pauta. No es una acusación: es la razón por la que este
proyecto mira la propiedad.

### Voz de la casa

La categoría Editorial existe (`/category/opinion/editorial/`) y su último
editorial institucional es del 25-09-2021. La última pieza de opinión es del
18-08-2025. **En los 12 meses no hay voz de la casa medible**, y la regla de la
evidencia editorial histórica no tiene material.

### Nivel 2 — Conducta medida

No ingerido hasta el alta: sin corpus propio. La ficha del 2026-08-09 medía
332 h sin artículo nuevo (último `lastmod` del sitemap: 2026-07-26 23:01 UTC),
exacto para su fecha. El 2026-10-10 publica de forma esporádica: 95 URL en 12
meses por `lastmod`, 13 en septiembre de 2026, 0 entre el 10-09 y el
23-11-2025. Último ítem: 30-09-2026.

### Contenido institucional

**Desvelamiento, no acusación.** En «Especial», de mayo a agosto de 2026, 10
piezas del Gobierno nacional (informes de gestión del MinTIC y del sector
TIC), de Afinia/Grupo EPM y de Veolia
([feed de la sección](https://sucrenoticias.com/category/especial/feed/),
recomprobado el 2026-10-10: 10 ítems del 13-05 al 20-08-2026). Son **informes
de gestión y contenidos corporativos marcados como tales, no como
publicidad**: 8 llevan en el subtítulo «Informe de gestión», «Informe
corporativo» o «Información corporativa», 2 no llevan marca y ninguna se marca
como publicidad. Que sea pauta pagada no consta. Por el polo fijo, reproducir
comunicados del gobierno saliente no mueve el eje.

## Argumento

### POR QUÉ 0,00, Y POR QUÉ ENTRA

- **Regla 3:** sin evidencia de nivel 1-3 no hay número firmable. Es una razón
  para no *firmar*, no para no dar de alta: así entraron La Razón.co, EL
  DIARIO de Boyacá, Vive el Meta, Lente Regional, LeticiaHoy y Quindío
  Noticias.
- **Regla 2:** la banda mixta, provisional, por ausencia de evidencia.
- **El ritmo** ya no es motivo: publica de forma esporádica pero sigue vivo,
  como LeticiaHoy cuando entró. Queda la **condición de los 30 días**.
- **Sucre era el único departamento con medios web que seguía en blanco.**

### SUCRE, ENTERO

Sucre tenía dos candidatos: Sucre Noticias, que entra hoy, y **Korraleja**
(`korraleja.co`), que sigue sin feed (`/feed/` da 404 el 2026-10-10, según la
resolución).

**El Meridiano**, el grupo de Montería, se define como el medio de «Córdoba,
Sucre y la región Caribe», y sigue sin feed y con 403 a los bots. Córdoba tiene
medio propio desde el 2026-08-11 (La Razón.co): El Meridiano solo
desbloquearía Sucre, y ahora como segunda voz.

## El mejor caso en contra

**Hacia «sin medir» (el más fuerte).** Este 0,00 no tiene nada debajo. No hay
nivel 1 (no publica sociedad, NIT, dueño ni director, y el RUES da 0
coincidencias), no hay nivel 3, no hay voz de la casa en 12 meses (último
editorial institucional del 25-09-2021; última opinión, del 18-08-2025) y no
hay corpus propio. Por analogía con la precisión del 2026-10-10, que manda a «sin medir» un valor sin
evidencia cuando no hay piezas para juzgar, como a Noticias Caracol el
2026-10-12. El alta en 0,00 se decidió para no dejar Sucre en blanco (opción
(c) de la resolución, 2026-10-10): es una razón de cobertura, no de medición. El
revisor y la ficha anterior recomendaban no darlo de alta.

**Hacia una dirección.** Las 10 piezas de «Especial» (mayo a agosto de 2026)
reproducen informes de gestión del Gobierno nacional (MinTIC y sector TIC) y
contenidos corporativos de Afinia/Grupo EPM y Veolia: 8 marcados como informe o
contenido corporativo, 2 sin marca y ninguno como publicidad. Reproducir comunicados del gobierno de turno no es orientación
(polo fijo), y que sean pauta no consta.

**Lo que no hay:** ninguna pieza con postura en voz propia, a ningún lado del
07-08-2026.

## Qué cambiaría el número

| | |
|---|---|
| **Condición de revisión** | **Si pasa más de 30 días sin publicar, se decide la baja.** Último ítem al alta: 30-09-2026 |

### REFUTACIÓN — qué reabriría el expediente

1. **Que Sucre Noticias publique quién lo edita** y quién lo dirige.
2. **Que El Meridiano habilite un feed** o acepte que lo leamos.
3. ~~Buscar en mapeomedios.com~~ — **hecho** el 2026-10-10: 38 medios en 28
   municipios, no lista a Sucre Noticias.
4. **El expediente de los procesos EXTRADEC-138-2024 y EXTRADEC-178-2024** en
   SECOP, para saber si el «espacio noticioso SUCRE NOTICIAS» es este medio y
   quién lo factura (leído con la regla de datos personales).
5. **La búsqueda por establecimiento en `rues.org.co`**, gratuita y no hecha,
   antes que el certificado de la Cámara de Comercio de Sincelejo.
6. **Más de 30 días sin publicar:** se decide la baja.

## Contratación pública

Contratación pública (SECOP I y II, por nombre, sin NIT conocido; consultado
2026-10-10): **0 contratos en los últimos 12 meses y 0 en total.** Sin NIT no
cabe la consulta exacta. En el conjunto de procesos de SECOP II, el Sorteo
Extraordinario de Colombia (Extradec) publicó en 2024 dos procesos de
publicidad cuyo objeto nombra un «espacio noticioso SUCRE NOTICIAS»
transmitido por Facebook y por plataformas de Korraleja.co (EXTRADEC-138-2024,
base $3.000.000; EXTRADEC-178-2024, base $5.000.000). Ninguno figura
adjudicado y no hay contrato asociado en los datos abiertos. **Vínculo no
probado:** que ese espacio sea este sitio no consta.

Consulta sin datos personales (con `$select`, comprobada el 2026-10-10: 2
filas, sin campos de identificación personal):
[procesos de SECOP II](https://www.datos.gov.co/resource/p6dx-8zbt.json?$select=entidad,referencia_del_proceso,fecha_de_publicacion_del,precio_base,adjudicado,nombre_del_proveedor,descripci_n_del_procedimiento&$where=upper(descripci_n_del_procedimiento)%20like%20%27%25SUCRE%20NOTICIAS%25%27).

## Recogida

```
https://sucrenoticias.com/feed/
HTTP 200 · application/rss+xml · 10 ítems · <language>es · WordPress
```

Comprobado el 2026-10-10 a las 20:44 UTC: 10 ítems del 03-09 al 30-09-2026,
**en orden cronológico**, con fechas RFC 822; `lastBuildDate` 30-09-2026 21:22
UTC. `npm run feed:descubrir -- sucrenoticias.com` lo encuentra declarado en el
HTML (último ítem de hace 239 h). Imágenes en `sucrenoticias.com/wp-content/`.

## Historial

### HALLAZGOS DEL CICLO 2 (2026-10-10)

Cada hallazgo se comprobó de nuevo en su fuente el 2026-10-10. Origen:
`revision-externa/respuestas/opus-5-5-sucre-noticias.md` (RESOLUCIÓN,
«Propuesta para la firma»), con la decisión del responsable editorial del 2026-10-10.

- **El feed no está parado: publica de forma esporádica.** El 2026-10-10 el
  feed trae 10 ítems del 03-09 al 30-09-2026, en orden cronológico; desde el
  último han pasado unos 10 días. Por el `lastmod` del sitemap (aproximación):
  95 URL en 12 meses, 13 en septiembre de 2026, y **un hueco de 74 días** sin
  ninguna (10-09 → 23-11-2025). Las 332 h de la ficha del 2026-08-09 eran
  exactas para su fecha; lo inexacto era la palabra «parado» como estado.
- **Condición de revisión, escrita y no supuesta:** si pasa más de 30 días sin
  publicar, se decide la baja (regla de los 30 días de la nota de Vorágine).
- **Sin voz de la casa medible.** La categoría Editorial existe
  (`/category/opinion/editorial/`) y su último editorial institucional es del
  25-09-2021; la última pieza de opinión, del 18-08-2025.
- **Contenido institucional en «Especial»:** informes de gestión y contenidos
  corporativos marcados como tales, no como publicidad. Ver «Contenido
  institucional».
- **Publica firmas**: ocho cuentas de autor; la cuenta «Redacción» tiene un
  identificador con el nombre del periodista que firma la mayoría de las
  piezas. No publica dueño, director ni sociedad.
- **Declara que vende pauta** («Para pautar con nosotros», `publicidad@`), así
  que «no dice quién lo sostiene» era inexacto: no dice quién es su dueño.
- **SECOP:** 0 contratos; 2 procesos de Extradec (2024) nombran un «espacio
  noticioso SUCRE NOTICIAS». Vínculo no probado. Ver «Contratación pública».
- **mapeomedios.com explorado:** 38 medios de Sucre, ninguno es este.
- **Córdoba tiene medio propio desde el 2026-08-11** (La Razón.co): El
  Meridiano ya no desbloquearía dos departamentos, solo Sucre.

**Lo que NO entra como hecho:**

- **Que las piezas de «Especial» sean pauta pagada.**
- **Que el «espacio noticioso SUCRE NOTICIAS»** de los procesos de Extradec
  sea `sucrenoticias.com`, ni que se contratara: vínculo no probado.
- **Que José Iriarte Díaz dirija o posea el medio**, aunque la cuenta
  «Redacción» lleve su nombre en el identificador.
- **Cualquier vínculo con «SINCELEJO NOTICIAS S.A.S» o «TELENOTICIAS DE SUCRE
  SAS»**, homónimas del RUES.
- **La región visible en el RDAP del registrador**, que no identifica a nadie
  y no se reproduce.

### REVISIÓN EXTERNA

☑ **Ciclo 2 hecho** (Claude Opus 5.5, `claude-opus-5-5`, resuelto el
2026-10-10): `revision-externa/respuestas/opus-5-5-sucre-noticias.md`. Siete
objeciones, ninguna rechazada entera; corregidas el recuento de septiembre (13,
no 10), el 0 de octubre de 2025, el rótulo de 8 de las 10 piezas de «Especial»
y los procesos de SECOP II que el revisor no consultó. El revisor y la ficha
recomendaban no dar de alta; el responsable editorial decidió el 2026-10-10 la opción (c): alta en
0,00 provisional, sin firmar, `ownerType: null`, con la condición de los 30
días. El revisor, quien resolvió y quien aplica son de la misma casa que el
autor de esta ficha: su acuerdo no cuenta como aval.

**Lo que se recomprobó al aplicar (2026-10-10):** robots.txt (Yoast, sin
vetos); el feed (10 ítems, último el 30-09); `/contacto/` (la cita de nivel 4,
sin ningún cargo); el feed de «Especial» (10 ítems, 13-05 a 20-08-2026); el
RUES por nombre (0) y los procesos de Extradec (2) con `$select`. Nada de lo
que la resolución daba dejó de sostenerse.
