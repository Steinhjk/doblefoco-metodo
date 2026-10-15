# Quindío Noticias (Armenia) — ficha de orientación

| | |
|---|---|
| **Medio** | Quindío Noticias · `quindio-noticias` · quindionoticias.com |
| **Valor vigente** | **0,00** — orientación mixta por Regla 2 |
| **Firma** | ☑ **FIRMADA el 2026-10-10 — el responsable editorial** (firma en bloque tras el ciclo 2; ver DECISIONES.md. Lo que más abajo dice «sin firmar», «no se firma» o «provisional» es el estado anterior a esta firma y se conserva como historia) |
| **Alta** | 2026-08-14 (alta) · **corregida el 2026-10-08** con las correcciones de hecho del ciclo 2 (ver TENSIONES) |
| **Última revisión** | — |
| **Departamento / ámbito** | Quindío — **es el primero del departamento en el catálogo** |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`quindio-noticias`): 4 fuentes; comprobada el 2026-10-08 |
| **Recogida** | `https://quindionoticias.com/feed` · vía `direct` |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

> **Lee «0,00» como «no sabemos», no como «equilibrado».** Es la Regla 2: ante
> la duda entre dos bandas, la más cercana a la mixta. No es un elogio ni una
> absolución.
> Lo que se sabe desde el 2026-10-08 habla de **dependencia**: el titular es
> contratista de entidades que el medio cubre (ver «Contratación pública»). Y
> hay conducta que apunta a un lado, medida todavía solo en titulares (ver
> TENSIONES).

## Evidencia

### Nivel 1 — Quién lo edita, hoy

| Dato | Valor | Fuente |
|---|---|---|
| **Titular** | **Daniel Andrés Hincapié Ramírez, persona natural.** No hay sociedad conocida | SECOP I, constancia 21-4-12596549, y SECOP II, consultados el 2026-10-08 |
| Cómo consta | Contrato CS-430-2021 con Empresas Públicas de Armenia, firmado el 2021-11-26: razón social del contratista «QUINDIO NOTICIAS», tipo de documento «Cédula de Ciudadanía», representante legal «DANIEL ANDRES HINCAPIE RAMIREZ». El mismo documento figura con su nombre en otros 8 contratos de SECOP I y en 15 de SECOP II | ídem |
| Documento | **No se publica**: es un dato personal de una persona natural (Ley 1581; protocolo, «DATOS PERSONALES»). Es consultable en SECOP | — |
| **NIT** | No hay: ante el Estado opera con su cédula. En tres registros de la Universidad del Quindío el tipo de documento es «Nit de Persona Natural» | SECOP I |
| **Director / editor** | **no publicado**. Los firmantes del sitio son cuentas genéricas («Editora QN», «Quindío Noticias», «Editor QN WEB») | [API de WordPress](https://quindionoticias.com/wp-json/wp/v2/users) |
| Marca | «Quindío Noticias® — 2011-2025», con símbolo de marca registrada | pie de su portada |

**La cuenta de WordPress id 1** tiene el nombre visible «Quindío Noticias» y el
slug «dhincapier», y firma 110 de las 605 entradas publicadas entre el
2026-08-31 y el 2026-10-08, la última del 2026-10-06. Existe además un autor
«Daniel Hincapie» (id 11, última entrada del 2024-09-23). **Que «dhincapier» sea
el titular es sospecha, no prueba**, y la API pública no dice qué cuenta
administra el sitio.

**No procede aviso de quien dirige.** No consta candidatura ni cargo público del
titular. Un contrato de prestación de servicios no es cargo público.

### Nivel 4 — Lo que el medio dice de sí mismo

Su [`page-sitemap.xml`](https://quindionoticias.com/page-sitemap.xml) enlaza:

- [Términos de Servicio](https://quindionoticias.com/terminos-de-servicio-quindionoticias-com/)
  (actualizados el 2025-08-29): «QuindioNoticias.com es un medio de comunicación
  digital independiente que ofrece contenidos de carácter informativo,
  periodístico y de interés general», y «La contratación de publicidad no
  condiciona ni afecta la independencia editorial del medio».
- [Política de privacidad](https://quindionoticias.com/politica-de-privacidad/)
  (2025-04-01), a nombre de Quindío Noticias.
- [Contáctenos / Paute con nosotros](https://quindionoticias.com/contactenos-paute-con-nosotros/):
  «Somos Quindío Noticias. Periódico digital del Eje Cafetero.».

Los Términos y la Privacidad publican un teléfono y una dirección de contacto.
**No se copian aquí**: el titular es una persona natural (protocolo, «DATOS
PERSONALES»).

### Nivel 4 — Sección de opinión

Tiene categorías de opinión y de columnistas
([API de WordPress](https://quindionoticias.com/wp-json/wp/v2/categories)):
`opinion` (17 entradas), `c304-opinion` (92), Oliver Gómez Solarte (75), Jota
Domínguez Giraldo (24) y Pablo Jaramillo (5).

- La última columna firmada es de marzo de 2025: las de «Finito», archivadas
  bajo la categoría de Gómez Solarte. Eso no prueba que sean la misma persona.
- Entre ellas, una en defensa del empréstito de la Gobernación
  ([16-03-2025](https://quindionoticias.com/oposicion-porque-si-falta-de-argumentos-serios-en-contra-del-emprestito-de-la-gobernacion-opinion-por-finito-ok/)).
- **Tienen 19 meses**: quedan fuera de la regla del presente. Sirven para
  corregir la afirmación «no hay sección de opinión», no como evidencia de
  orientación.

### Cierra el hueco que el informe del 9 de agosto dejó anotado

Aquel informe corrigió el error de dar el Quindío por cubierto con Telecafé, que
emite desde Manizales —o sea Caldas—, y dejó escrito que **«Quindío sigue sin medio
suyo»**. Este lo cierra.

### AVISO DE COMPROBACIÓN: su servidor responde 200 a cualquier ruta

`/quienes-somos/`, `/nosotros/`, `/about/`, `/equipo/` y `/aviso-legal/` devuelven
**la misma portada**: 106 kB el 2026-08-14, 122 161 bytes el 2026-10-08. Es un
catch-all: ninguna de esas páginas existe.

**Quien las pruebe y vea «200» creerá haber mirado sus páginas institucionales.** La
comprobación tuvo que hacerse comparando tamaños de respuesta.

Es la misma clase de falso positivo que el feed que responde con cien titulares
rancios y pasa por bueno — el que obligó a añadir la comprobación de frescura a
`check:feeds`.

**Corregido el 2026-10-08.** El aviso era exacto, pero la conclusión que se
sacó de él no: las páginas institucionales existen, en otras rutas, y bastaba
mirar el sitemap.

## Argumento

### POR QUÉ 0,00

**Regla 2, con la razón corregida.** La razón anterior, «la ausencia es total»,
era falsa: hay titular, páginas institucionales, sección de opinión y conducta
observable.

El 0,00 se sostiene por otra cosa. La conducta que apunta a un lado —a favor
del gobierno nacional entrante y del gobernador— está medida solo en titulares,
durante 38 días y con el terremoto del Quindío de por medio. El protocolo no
mueve el número sin corpus (regla 3). Ante la duda entre dos bandas, se queda
en la más cercana a la mixta (regla 2).

**Se descartó la analogía regional**, por lo mismo que en EL DIARIO de Boyacá y El
Nuevo Día.

## El mejor caso en contra

**Hacia la derecha (el más fuerte).** De los 33 titulares políticos de la
ventana, **ninguno es crítico con el presidente ni con el gobernador**.
Escándalo para el gobierno saliente («¿TRAICIÓN A LA PATRIA?…», 25-06-2026);
celebración para De la Espriella ya desde que era presidente electo, y después
(«“Aquí nadie se acobarda”…», 02-09-2026; «¡Tiemblan los capos!…»,
01-10-2026); elogio uniforme al gobernador, y la oposición de tres alcaldes al
gobierno nacional encuadrada contra ellos (tensión 2). Es la forma que el polo
fijo sí admite como orientación: fiscalizar a un lado y celebrar al otro. Y los
titulares son voz de la casa: desde el 2026-10-09, un barrido de su archivo con
la regla «Evidencia editorial histórica» podría contarlo sin esperar 90 días
de corpus (REFUTACIÓN, 1).

**Por qué hoy no basta.** Se leyeron titulares, no cuerpos; son 38 días; el
terremoto del Quindío hace noticia por sí mismo de las visitas y las obras;
muchas piezas del gobernador parecen boletines, sin cotejar; y criticar a Petro
mientras gobernaba es fiscalizar, que no suma (tensión 2). No consta un
recuento con los mínimos de la regla: 10 piezas con postura, 3 a cada lado del
07-08-2026 sin contar la fiscalización, y 3 a 1.

**Hacia la izquierda:** la ficha no cita ninguna pieza.

**Lo que no es contra:** que el titular sea contratista de la CRQ y de
Indeportes, entidades que el medio cubre, es dependencia, no posición en el eje.
El spam de casinos y el corpus incompleto (496 de 605) afectan a la fiabilidad y
a la medición, no a la dirección.

## Qué cambiaría el número

### REFUTACIÓN — qué movería este número

1. **Que el trato asimétrico se sostenga en un barrido de 12 meses** del archivo
   del propio medio, a los dos lados del 07-08-2026 y medido en cuerpos
   (evidencia editorial histórica, 2026-10-09; ya no se esperan 90 días de corpus): escándalo para el gobierno saliente, celebración para el entrante y
   elogio uniforme al gobernador. Es la evidencia de polo fijo que movería el
   número a la derecha.
2. **Que aparezca crítica de la casa al presidente o al gobernador** en esa
   misma medición. Reforzaría el 0,00.
3. **Corpus propio, limpio.** Hay que conciliar los 496 artículos medidos con los
   605 publicados y excluir el spam antes de medir; ver
   `revision-externa/CONDUCTA-MEDIDA.md`.

## Tensiones declaradas

### TENSIONES — lo que la revisión del ciclo 2 deja abierto (2026-10-08)

1. **El titular es contratista de entidades que el medio cubre.** Firmó
   $39.100.000 en 12 meses con la CRQ e Indeportes, y antes trabajó en la
   Tesorería de la Gobernación (2020-2022). Es desvelamiento, no acusación, y no
   mueve el número.
2. **Sus titulares favorecen a De la Espriella y a Galvis**, de junio a octubre
   de 2026.
   - Escándalo para el gobierno saliente: «¿TRAICIÓN A LA PATRIA?…»
     ([25-06-2026](https://quindionoticias.com/traicion-a-la-patria-el-escandalo-por-audios-secretos-entre-el-gobierno-petro-y-el-clan-del-golfo-desata-un-terremoto-institucional-ok/)).
   - Celebración para De la Espriella, ya desde que era presidente electo
     (julio) y después: «¡Tiemblan los capos!…»
     ([01-10-2026](https://quindionoticias.com/tiemblan-los-capos-presidente-firma-extradiciones-a-un-ritmo-frenetico-dos-criminales-por-dia/)),
     «“Aquí nadie se acobarda”…»
     ([02-09-2026](https://quindionoticias.com/aqui-nadie-se-acobarda-de-la-espriella-declara-guerra-sin-cuartel-a-estructuras-criminales-tras-carro-bomba-en-cucuta/)).
   - Elogio uniforme al gobernador: «El Quindío cambia sus vías: el liderazgo de
     Juan Miguel Galvis impulsa tres grandes obras»
     ([26-09-2026](https://quindionoticias.com/el-quindio-cambia-sus-vias-el-liderazgo-de-juan-miguel-galvis-impulsa-tres-grandes-obras/)).
     La oposición de los alcaldes de Armenia, Filandia y Quimbaya al gobierno
     nacional se encuadra contra ellos (25-09-2026).
   - De los 33 titulares políticos de la ventana, **ninguno es crítico con el
     presidente ni con el gobernador**. La crítica local recae en alcaldías y en
     el Concejo.
   - **Lo que lo matiza:** se leyeron titulares, no cuerpos; son 38 días; el
     terremoto hace noticia por sí mismo de las visitas y las obras; y muchas
     piezas del gobernador parecen boletines, sin cotejar. Criticar a Petro
     mientras gobernaba es fiscalizar y no cuenta (regla del polo fijo).
3. **Publica spam de casinos: 19 piezas** entre el 2026-08-31 y el 2026-10-08,
   en alemán, francés, inglés, rumano, polaco, italiano, portugués y español.
   - Todas son de la cuenta «Editora QN» y de la categoría local principal. La
     portada del 2026-10-08 enlaza 17, y el spam viene de antes de la ventana.
   - No se identifican como publicidad, contra lo que dicen sus propios
     Términos: «Dichos espacios serán siempre identificados como publicidad».
   - No se sabe si es pauta vendida o una cuenta comprometida. Afecta a la
     fiabilidad del medio y puede contaminar el corpus.
4. **El corpus está incompleto: 496 de 605.** El envío del 2026-10-08 mide 496
   artículos desde el 2026-08-31; la API del sitio da 605 entradas publicadas.
   Los 19 de casino no explican toda la diferencia. Antes de usar el 58 % de
   agenda propia, calculado sobre 51 piezas, hay que conciliar las cifras.
5. **Las fuentes de este expediente.** Revisor y resolutor son de la misma casa
   que el autor (Claude). Que aquí no se contradiga algo no lo convierte en aval.

## Contratación pública

> Contratación pública (SECOP I y II, contratista persona natural Daniel Andrés
> Hincapié Ramírez, documento omitido por Ley 1581, consultado 2026-10-08): 3
> contratos por $39.100.000 **contratados** en los últimos 12 meses
> (2025-10-08 → 2026-10-08); 24 por $203.598.554 en total desde 2018 (SECOP I: 9
> por $46.030.000; SECOP II: 15 por $157.568.554). Principales contratantes:
> Gobernación del Quindío ($49.327.500, 2020-2022), CRQ ($46.700.000,
> 2018-2026), Indeportes Quindío ($41.850.000, 2024-2026), Empresas Públicas de
> Armenia ($18.480.000) y RAP Eje Cafetero ($16.000.000). **Son entidades que el
> medio cubre**: Indeportes es un instituto del departamento que gobierna Juan
> Miguel Galvis, y la CRQ es la autoridad ambiental del Quindío.

Los tres de los últimos 12 meses:

| Firma | Entidad | Valor | Contrato |
|---|---|---|---|
| 2025-10-08 | CRQ, Oficina Asesora de Planeación | 7.500.000 | CPS-920-2025 |
| 2026-01-15 | CRQ, Oficina Asesora de Planeación | 19.200.000 | CPS-265-2026, «Modificado», 60 días adicionados |
| 2026-01-17 | Indeportes Quindío | 12.400.000 | 086-CSP-2026, fin previsto el 2026-05-16 |

Fuente: SECOP I (datos.gov.co, `f789-7hwg`)
y SECOP II (`jbjy-vk9h`),
por igualdad exacta de documento (consulta del 2026-10-08; no se enlaza: lleva el documento de una persona natural). Se identifica a la persona por la
constancia 21-4-12596549.

- **Sin el contrato firmado el mismo 2025-10-08**, la cifra de 12 meses es
  $31.600.000.
- **La Gobernación contrató antes de Galvis.** Los contratos con la Gobernación
  central son de la Tesorería, de 2020 a 2022. Galvis asumió en 2024. Con él, el
  vínculo departamental es Indeportes, desde el 2024-05-02. La CRQ es una
  corporación autónoma, no la Gobernación.
- **Dos naturalezas distintas.** Pauta del medio (difusión institucional),
  2018-2021: $32.650.000. Servicios profesionales personales del titular,
  2018-2026: $170.948.554 (Tesorería de la Gobernación, Indeportes, Planeación de
  la CRQ, IGAC, RAP y EPA).
- **No se suma** un contrato de pauta con la Alcaldía de Armenia (2019-04-30,
  $12.000.000, SECOP I, constancia 19-13-9321865) a nombre de la misma persona,
  con un documento que difiere en dos dígitos. Es muy probablemente un error de
  digitación, pero la regla es la igualdad exacta.
- **«Contratado», no «cobrado».** Ningún contrato tiene fecha de fin posterior al
  2026-10-08 en los datos abiertos.

Es **desvelamiento, no acusación**, y no mueve la clasificación por sí solo
(protocolo, «CONTRATACIÓN PÚBLICA»).

## Propiedad y lo que no consta

### LO QUE FALTA

1. **El titular de la marca «Quindío Noticias»** en la Superintendencia de
   Industria y Comercio.
2. **La matrícula mercantil** del titular como persona natural comerciante, en
   el RUES o la Cámara de Comercio de Armenia.
3. **El barrido de 12 meses** del archivo del propio medio, en cuerpos y no solo
   en titulares (ver TENSIONES, punto 2). Sustituye al de 90 días de corpus que
   pedía esta ficha: desde el 2026-10-09 no se espera esa serie.
4. ~~**Cualquier nombre propio.**~~ ~~**La razón social.**~~ Resueltos el
   2026-10-08: opera como persona natural (ver Nivel 1).

## Recogida

```
https://quindionoticias.com/feed
HTTP 200 · 10 ítems · 10 de 10 dentro de la ventana de 72 h
más reciente 0,3 h · mediana 4,7 h
```

Sirve las fotos por la CDN de Jetpack (`i0.wp.com`), no desde su dominio: por eso
lleva `imageHosts` explícito en el registro. Comprobado el 2026-08-14.

## Fuentes

### FUENTES AÑADIDAS EL 2026-10-08

- SECOP I, constancia 21-4-12596549 (sin enlace: la página de contratos.gov.co muestra el documento del contratista)
- SECOP I en datos.gov.co (`f789-7hwg`), consulta por el documento del titular, 2026-10-08; no se enlaza
- SECOP II en datos.gov.co (`jbjy-vk9h`), consulta por el documento del titular, 2026-10-08; no se enlaza
- Sitemap de páginas: <https://quindionoticias.com/page-sitemap.xml>
- Términos de Servicio: <https://quindionoticias.com/terminos-de-servicio-quindionoticias-com/>
- Política de privacidad: <https://quindionoticias.com/politica-de-privacidad/>
- Contáctenos: <https://quindionoticias.com/contactenos-paute-con-nosotros/>
- API de WordPress, usuarios y categorías: <https://quindionoticias.com/wp-json/wp/v2/users>, <https://quindionoticias.com/wp-json/wp/v2/categories>
- Expediente completo: `revision-externa/respuestas/opus-5-5-quindio-noticias.md`.

## Historial

### CORREGIDO EL 2026-10-08

Esta ficha decía que el medio **«no publica absolutamente nada sobre sí mismo»**,
que no tenía **«ni sección de opinión identificable»** y que **«la ausencia es
total»**. Las tres cosas eran falsas
(`revision-externa/respuestas/opus-5-5-quindio-noticias.md`):

- **Sí hay titular**, y consta en SECOP: opera como persona natural.
- **Sí publica sobre sí mismo**: Términos de Servicio, Política de privacidad y
  Contáctenos. Están en su `page-sitemap.xml`, no en las rutas que se probaron.
- **Sí tiene sección de opinión**, con categorías de columnistas.

El valor no cambia. Cambia su razón (ver «Por qué 0,00»).
