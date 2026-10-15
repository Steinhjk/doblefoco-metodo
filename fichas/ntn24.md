# NTN24 — ficha de orientación

| | |
|---|---|
| **Medio** | NTN24 · `ntn24` · ntn24.com |
| **Valor vigente** | **+0,30** · Derecha moderada · `reviewedAt: '2026-10-12'`. Firmado el 2026-10-12 por el barrido editorial del 2026-10-11, que cumple las cinco condiciones de la regla «Evidencia editorial histórica» (ver abajo) |
| **Firma** | ☑ **FIRMADA el 2026-10-12 — el responsable editorial**, en +0,30, el valor que resultaba del barrido (ver DECISIONES.md). Lo que más abajo dice «propuesta», «sin firmar» o «sigue en +0,35» es el estado anterior a la firma y se conserva como historia |
| **Alta** | 2026-10-11 (ficha mínima, abierta con el barrido) · 2026-10-12 (firma) |
| **Última revisión** | — |
| **Departamento / ámbito** | Canal internacional de noticias, panregional. `country: 'CO'` por la propiedad. En el mapa entra por su feed propio `/feed-kiosko-google` |
| **Fuentes de propiedad** | `shared/mediaOwnership.js` (`ntn24`): 1 fuentes; comprobada el 2026-08-24 |
| **Recogida** | `https://www.ntn24.com/feed-kiosko-google` · vía `direct` |
| **Protocolo** | `PROTOCOLO_JUICIO_EDITORIAL.md` |

## Estado

**Firmada el 2026-10-12 en +0,30.** El responsable editorial firmó el valor
que resultaba del barrido (77 a 0; tope de ±0,30 sin endoso). Se aplicó en el
registro (`bias`, `reviewedAt`, `biasSources`, `biasRationale`), en el texto
público (`shared/resumenesPublicos/ntn24.js`) y en esta ficha.

Queda en el tope de la banda moderada, por encima de La FM (+0,25) y de
Noticias RCN (+0,15), las dos de la misma casa y firmadas el mismo día tras sus
propios barridos. Sigue siendo una ficha mínima: las LAGUNAS de
arriba siguen abiertas.

*Estado anterior (2026-10-11):* ficha mínima, sin firmar; el valor seguía en
+0,35 hasta la decisión del responsable editorial.

## Evidencia

### Nivel 1 — Quién lo posee y quién lo dirige, hoy

| Dato | Valor | Fuente |
|---|---|---|
| Grupo | **Organización Ardila Lülle** (casa RCN). `controlGroup: 'ardila-lulle'` | `shared/mediaOwnership.js`, entrada `ntn24` (verificada el 2026-08-24); [MOM, Organización Ardila Lülle S.A.](https://colombia.mom-gmr.org/en/owners/companies/detail/company/company/show/organizacion-ardila-luelle-sa/) |
| Medios del mismo grupo en el catálogo | Noticias RCN, La FM y La República. **Con NTN24 son cuatro:** el conjunto más grande de un solo dueño del catálogo | ídem |
| Sociedad que edita el canal | **No consta.** No se buscó en el registro mercantil: el alta se hizo por la vía del grupo | ídem; `docs/certificados-camaras.md` (buscar «NTN24», «NUESTRA TELE»; Cámara de Bogotá, por confirmar) |
| Autor que declara la página | «Nuestra Tele Noticias 24» (JSON-LD de cada pieza) | Las 1.551 piezas del barrido |

**Hereda el nivel 1 de la casa con sus defectos:** la página del MOM lista
como titulares a dos personas fallecidas en 2021 y deja el 63,4 % del holding
en una sociedad panameña sin llegar a persona natural. El detalle está en
`fichas/noticias-rcn.md`. No se documenta aquí dos veces.

### Nivel 2 — Conducta medida

No consta en el repositorio un envío con la conducta medida de NTN24.

### Nivel 4 — Lo que declara de sí mismo

No se consultó para esta ficha.

### Nivel 5 — Hechos editoriales de los últimos 12 meses: el barrido

**Barrido completo, con cada pieza, su URL, su fecha y su clase:**
[`revision-externa/barridos/ntn24.md`](../revision-externa/barridos/ntn24.md).
Lo hizo Claude Opus 5.5 el 2026-10-11, a petición del responsable editorial.
Es de la misma casa que el autor del valor vigente: su acuerdo no es aval.

- **Universo:** 1.551 piezas sobre política nacional colombiana entre el
  2025-10-11 y el 2026-10-11 (967 antes del 07-08-2026 y 584 después), sacadas
  de los sitemaps mensuales del propio medio y leídas del sitio vivo. El
  `robots.txt` lo permite. Ninguna pieza lleva firma personal: la voz de la casa
  es lo que dicen el titular y la entradilla sin atribuirlo a una fuente.
- **Con postura en voz propia: 78.** 77 hacia la derecha (32 fuertes y 45
  leves), 0 hacia la izquierda y 1 mixta. Antes del cambio, 13; desde el
  cambio, 65.
- **Polo fijo:** fiscaliza al Gobierno Petro en voz propia 41 veces (no cuenta)
  y no fiscaliza al Gobierno De la Espriella ni una vez: lo celebra en 64
  piezas. Las 6 piezas de control del nuevo Gobierno son informativas y
  neutras.
- **No hay endoso explícito** en voz propia. Los respaldos a De la Espriella
  que publica son citas de terceros.
- **No cuentan:** 105 columnas firmadas de opinión, la selección de invitados
  (no medida) y el encuadre de Venezuela.

## Argumento

El **+0,35 vigente** entró al mapa por comparación: «a la altura de La FM
(+0,35), su hermana de grupo, y por encima de Noticias RCN (+0,25)», con la
descripción de un canal «con línea editorial marcadamente crítica de los
gobiernos de izquierda de la región». Esa descripción no citaba ninguna pieza.
Se apoya solo en los niveles 4 y 5.

El **barrido del 2026-10-11** documenta la dirección: 77 a 0 en voz de la casa,
con asimetría a través del cambio de gobierno. Cumple las cinco condiciones de
la regla. Por la precisión del 2026-10-10, un valor que solo se apoya en los
niveles 4 y 5 cede ante el barrido, que manda **con el tope de ±0,30**, porque
no hay endoso explícito ni nivel 1 con posición conocida. **Propuesta: +0,30**,
**firmada el 2026-10-12.**

## El mejor caso en contra

- **La voz de la casa de un canal de noticias es más tenue que un editorial.**
  Aquí no hay editoriales: se cuentan titulares y entradillas. Una parte de las
  piezas «leves» usa el léxico estándar del orden público («golpe», «cerco»,
  «mano dura») y repite la comunicación del Gobierno. Sin ellas, el recuento
  sigue en 32 a 0.
- **El filtro es por URL y solo se leyó el titular completo** de todas las
  piezas; el cuerpo, en unas 60. Podría haber contrapesos fuera de lo leído.
  Harían falta 26 piezas hacia la izquierda (11 sin las leves) para bajar del 3
  a 1.
- **Es un solo lector**, de la misma casa que el autor del valor vigente.

## Qué cambiaría el número

1. **Hacia el centro:** que la casa fiscalice en voz propia al Gobierno De la
   Espriella con la frecuencia con que fiscalizó al de Petro, o que un recuento
   del cuerpo de las piezas encuentre contrapesos que lleven la proporción por
   debajo de 3 a 1.
2. **Por encima del tope:** un endoso explícito en voz propia, o un nivel 1 que
   documente la posición política del dueño.

## Propiedad y lo que no consta

### LAGUNAS

- La sociedad que edita el canal y su registro mercantil.
- Quién controla hoy la Organización Ardila Lülle, a persona natural.
- Cómo se financia el canal.
- Conducta medida (nivel 2).
- La selección de invitados, que es lo más visible del canal y no se midió.

## Fuentes

- `shared/mediaRegistry.js` y `shared/mediaOwnership.js`, entrada `ntn24`.
- [MOM, Organización Ardila Lülle S.A.](https://colombia.mom-gmr.org/en/owners/companies/detail/company/company/show/organizacion-ardila-luelle-sa/).
- [Barrido editorial de NTN24](../revision-externa/barridos/ntn24.md), 2025-10-11 → 2026-10-11, hecho el 2026-10-11.
- [robots.txt de NTN24](https://www.ntn24.com/robots.txt) y [su índice de sitemaps](https://www.ntn24.com/sitemapindex), consultados el 2026-10-11.

## Historial

### Cabecera anterior (filas superadas)

| | |
|---|---|
| **Valor anterior** | +0,35, sin firmar (`reviewedAt: null`): una comparación con La FM, sin piezas detrás |
