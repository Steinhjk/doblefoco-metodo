# Ciclo 2, fase 2 — plan de tandas

**Decisión del responsable editorial, 2026-10-07:** las 43 fichas que nunca pasaron por revisión
se revisan con el método completo, en **tandas de 5, una al día**, de forma
ordenada. El revisor es Claude Opus 5.5, con los límites escritos en
`DECISIONES.md` (2026-10-07).

## El método, igual en cada ficha

1. **El envío se arma el mismo día** con `npm run envio -- <ids> --ciclo=2`,
   porque un envío es válido para el día en que se armó (`LEEME.md`).
   **Antes**, `npm run conducta -- <ids> --json=data/conducta.json`: el envío
   solo lleva el nivel 2 de los medios que estén en ese archivo, y si faltan
   no avisa (la tanda 4 salió así, ver DECISIONES.md 2026-10-08).
2. **Revisor**, con red y sin el repositorio: ataca la ficha. **Cita desde el HTML
   crudo** de cada página y no desde un resumen; si no puede, lo dice. Esa es la
   lección de la fase 1.
3. **Verificador**, con el repositorio: abre cada fuente, la coteja literal y
   escribe la RESOLUCIÓN con su propuesta para la firma.
4. **Consolidación:** un cuadro por tanda, con lo que el responsable editorial tiene que decidir.
**Dos reglas añadidas después de la tanda 2 (2026-10-07):**

- **`robots.txt` antes de descargar.** Antes de bajar nada de un dominio, quien
  revisa lee su `robots.txt`. Si excluye a `ClaudeBot`, `Claude-Web` o
  `anthropic-ai`, no lo descarga y verifica por terceros. En la tanda 2, un
  revisor bajó una página de El Tiempo, que los excluye, y otro leyó Wikipedia
  por rutas vetadas. Bloqueados conocidos: `eltiempo.com`, `cambiocolombia.com`
  y `diariodelsur.com.co` (excluye ClaudeBot, anthropic-ai, Claude-Web y
  Claude-User, 2026-10-10). **Es una lista de revisión, no de ingesta**: el
  motor se presenta como `DobleFocoBot` (`shared/userAgent.js`), y un dominio
  que excluye a los agentes de Anthropic puede seguir en el catálogo, como
  `eltiempo.com`. Valora Analitik **no** está bloqueado (un revisor lo afirmó y era falso).
- **Contratación pública siempre.** Cada revisión consulta SECOP I y II por el
  NIT, con el formato de `PROTOCOLO_JUICIO_EDITORIAL.md`. Queda una deuda: las
  fichas ya cerradas (tanda 1 y las cinco de la fase 1) se completan en una
  pasada aparte.

5. **El responsable editorial decide.** Las correcciones de hecho y las firmas van en una PR por
   tanda.

## El orden, y por qué

Primero lo que **más pesa en el sitio**, medido en artículos de los últimos 36
días (`data/conducta.json`, 07-10). Se adelantan las fichas con **señales de
riesgo** (fuentes caídas, casos abiertos) y se dejan al final las que esperan
una **re-medición con fecha**. Los no noticiosos van casi al final: no están en
el mapa.

| Tanda | Día | Medios | Por qué aquí |
|---|---|---|---|
| 1 | 07-10 | Diario La Libertad, El País (España), Cambio, Boyacá Digital, Valora Analitik | Los de más volumen. La Libertad lleva el aviso de la directora candidata. El País en −0,20 fue uno de los dos «izquierda» del caso de Brasil. Boyacá tiene una fuente caída (#67) |
| 2 | 08-10 | La Razón (Córdoba), El Diario (Pereira), La Nación (Neiva), Seguimiento, El Nuevo Día | Volumen. La Nación tiene la pieza del centinela sobre Olave |
| 3 | 09-10 | Diario del Norte, Diario del Huila, El Pilón, Cablenoticias, Quindío Noticias | Volumen. El Pilón: fuente corregida en #67. Cablenoticias: la propiedad no está comprobada |
| 4 | 10-10 | Proclama del Pacífico, Lente Regional, El Diario (Boyacá), MiPutumayo, Periodismo Público | Regionales del centinela |
| 5 | 11-10 | Prensa Libre Casanare, Chocó 7 Días, Vive el Meta, Abra Noticias, Archipiélago Press | Chocó 7 Días tiene una fuente caída |
| 6 | 12-10 | Al Aire Noticias, Telecafé, El Morichal, Diario de Cundinamarca, Diario del Sur | Volumen bajo o nulo; Telecafé no es comprobable desde la nube |
| 7 | 13-10 | Ecos del Combeima, El Informador, El Isleño, El Manduco, Sucre Noticias | Sin artículos en la ventana: hay que ver por qué |
| 8 | 14-10 | Razón Pública, Volcánicas, Revista RAYA, Cuestión Pública, CasaMacondo | No noticiosos: fuera del mapa |
| 9 | 15-10 | RTVC, Las2Orillas, Vorágine | Esperan la re-medición del ~15-10 |

`cordoba-narino-segunda-vuelta` no es un medio y queda fuera.

## Avance

| Tanda | Revisada | Verificada | Decidida | PR |
|---|---|---|---|---|
| 1 | 07-10 | 07-10 | 07-10 | #75 |
| 2 | 07-10 | 07-10 | 07-10 | #76 |
| 3 | 08-10 | 08-10 | 08-10 | #77 |
| 4 | 08-10 | 08-10 | 08-10 | #78 |
| 5 | 08-10 | 09-10 | 09-10 | #79 |
| 6 | 10-10 | 10-10 | 10-10 | #83 |
| 7 | 10-10 | 10-10 | 10-10 | #87 |
| 8 | 10-10 | 10-10 | 10-10 | (esta PR) |
| 9 | 10-10 | 10-10 | 10-10 | (esta PR) |
