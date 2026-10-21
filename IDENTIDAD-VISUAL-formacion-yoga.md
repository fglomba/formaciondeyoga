# Brief de identidad visual — Página de la Formación en Yoga Tradicional Nivel I

Página informativa (HTML estático, se publica en Netlify) que se envía a quienes "piden más info" sobre la formación.
La formación la respaldan dos marcas: **Fundación Holística de la Selva (FHS)** y **Ātmabodha – Escuela de Yoga Tradicional** (filial de The Lonavla Yoga Institute, India). La cara principal es el maestro **Dr. M. L. Gharote**.

Este documento tiene 3 partes: (1) identidad FHS, (2) identidad Ātmabodha, (3) el MIX que hay que usar en la página.

---

## 1. Fundación Holística de la Selva (FHS)

Fuente: manual de branding oficial (BRANDING.pdf, 2023).

**Personalidad:** calma, natural, femenina, orgánica, terapéutica. Mucho aire, mucho espacio vacío. Base de color crema.

**Paleta oficial (5 colores):**

| Nombre        | HEX       | Uso en su marca                        |
|---------------|-----------|----------------------------------------|
| Verde salvia  | `#607F6D` | Color principal: logo, títulos, íconos |
| Topo / taupe  | `#9A8B78` | Secundario, textos suaves              |
| Rosa viejo    | `#E5A3AA` | Acento (botones/etiquetas)             |
| Nude          | `#E6CDB9` | Fondos de bloque                       |
| Crema         | `#EFE2D9` | Fondo principal                        |

**Tipografía:** **Fugi Regular** (display, serif fina de alto contraste, elegante). Archivo incluido: `Fugi.woff` / `Fugi.ttf`.
⚠️ Fugi **NO tiene** los caracteres ¿ ¡ ni los diacríticos del sánscrito (ā ī ū ṇ ṣ ś ṅ ṃ ṭ ḍ). No usarla en textos con esas letras (ej. "Āsana", "Prāṇāyāma", "Patañjali" con diacríticos, preguntas con ¿).

**Logo:** isotipo de un árbol/figura humana con brazos abiertos y flores, sostenido por dos manos, dentro de un círculo de línea fina abierto, con el texto "Fundación Holística de la Selva" en curva. Versión horizontal: isotipo + texto en 3 líneas dentro de círculo. Sigla: **FHS**. Archivo incluido: `logo-fhs.png` (1080×1080, fondo transparente, verde salvia).

**Recursos gráficos:** íconos de línea fina (trazo ~1.5 px) en verde salvia: flor de loto, ojo con rayos, mano de Hamsa con ojo, figuras en postura de meditación y de āsana, sol. Círculos de línea fina como marco. Fotos con overlay gris/verde suave y logo blanco encima.

---

## 2. Ātmabodha – Escuela de Yoga Tradicional

Fuentes: sitio yogatmabodha.com e Instagram @yogatmabodha. (Colores tomados del logo y de las publicaciones; son aproximados al píxel, no de un manual oficial).

**Personalidad:** tradición, India, academia, autoridad, comunidad internacional. Más contraste y más color cálido que FHS. Tono de copy cálido, con voseo ("Formate", "Sumate").

**Paleta observada:**

| Nombre             | HEX aprox. | Dónde aparece                                     |
|--------------------|------------|---------------------------------------------------|
| Azul marino        | `#1B376A`  | Títulos y textos de los posts, aro del logo       |
| Azul noche (logo)  | `#0A1A63`  | Texto "ĀTMABODHA" del logo                        |
| Naranja azafrán    | `#E2823D`  | Fondos de posts destacados, degradés, figura logo |
| Naranja claro      | `#EBB16F`  | Extremo claro del degradé naranja                 |
| Celeste turquesa   | `#0AA0C6`  | Alas del logo                                     |
| Rojo bermellón     | `#BD271C`  | Bandas de urgencia ("ESTE FIN DE SEMANA")         |
| Blanco cálido      | `#FEFCF6`  | Fondos de posts claros                            |
| Gris azulado       | `#475F71`  | Fondos con foto + overlay                         |

**Tipografía observada en sus piezas:**
- Títulos: serif bold en MAYÚSCULAS, de alto contraste (estilo Playfair Display Bold / Cinzel).
- Acentos: caligráfica/script ("Seminario Bariloche", "Feliz cumpleaños", "Sumate a la").
- Textos: sans serif limpia (estilo Montserrat / Poppins).

**Logo:** sello circular. Aro azul marino con el texto "ESCUELA DE YOGA TRADICIONAL" en curva, figura naranja meditando con alas celestes, abajo "ĀTMABODHA" y "En camino hacia la Sabiduría". También tiene versión circular simplificada.
URLs del logo (descargar manualmente si hace falta):
- https://yogatmabodha.com/wp-content/uploads/2024/07/final-Logo-Atmabodh-01.avif
- https://yogatmabodha.com/wp-content/uploads/2025/01/Logo-Atmabodh-CIRC-1.avif

**Estilo de imagen:** fotos reales de grupo (diplomas, retiros en Salta, seminarios), retratos del Dr. Gharote sonriente con kurta naranja/rojo y tilak rojo, paisajes de montaña. Mucho contenido documental y cálido.

---

## 3. EL MIX para la página de la Formación

### Concepto: "La selva y la India"
- **De FHS** viene la **base**: el fondo crema, el verde salvia, el aire, la línea fina, la calma. Es la "tierra" (Misiones, la selva, lo orgánico).
- **De Ātmabodha** vienen la **autoridad y el fuego**: el **azul marino** para los títulos (seriedad académica y certificación) y el **naranja azafrán** como único acento fuerte (India, la tradición, el kurta del Dr. Gharote).

La regla de proporción es **70 / 20 / 10**:
- 70 % neutros cálidos (crema y nude)
- 20 % verde salvia y azul marino (textos, títulos, líneas)
- 10 % azafrán (botones, números clave, detalles). Si hay más naranja, la página pierde la calma de FHS.

Se **descartan** el rosa (`#E5A3AA`) y el celeste (`#0AA0C6`): pelean con el azafrán y le quitan seriedad. El celeste solo aparece dentro del logo de Ātmabodha. El rojo `#BD271C` se usa como máximo una vez (ej. "Cupos limitados" o la promo "antes de 2027"), o directamente no se usa.

### Tokens de color (CSS)

```css
:root {
  /* Fondos */
  --crema:        #F4ECE4; /* fondo principal: crema FHS apenas más claro, se lee mejor en pantalla */
  --crema-fhs:    #EFE2D9; /* bloques alternos */
  --nude:         #E6CDB9; /* tarjetas, bandas suaves */
  --blanco:       #FEFCF6; /* tarjetas sobre crema */

  /* Texto y estructura */
  --marino:       #1B376A; /* H1/H2, texto fuerte (Ātmabodha) */
  --tinta:        #2E3A40; /* cuerpo de texto (gris tinta, más suave que negro) */
  --salvia:       #607F6D; /* H3, íconos de línea, bordes, links (FHS) */
  --salvia-osc:   #4A6555; /* hover / textos verdes sobre crema (mejor contraste) */
  --topo:         #9A8B78; /* SOLO separadores, bordes y decoración (no texto) */
  --topo-osc:     #6F6252; /* textos secundarios y metadatos */

  /* Acento */
  --azafran:      #E2823D; /* fondo de botones principales, puntos, subrayados (Ātmabodha) */
  --azafran-osc:  #C96A28; /* hover del botón */
  --azafran-texto:#A9541C; /* cuando el azafrán es TEXTO (cifras clave, etiquetas) sobre crema */
  --azafran-claro:#EBB16F; /* degradé, subrayados */

  /* Bloque oscuro (sección Dr. Gharote / cierre) */
  --noche:        #1B376A; /* fondo con texto crema */
}
```

Contraste (verificado WCAG):
- El cuerpo de texto va en `--tinta` (10:1) o `--marino` (10:1) sobre crema.
- El botón azafrán lleva texto **marino en bold, ≥ 17 px** (4.2:1). **Nunca texto blanco** sobre `#E2823D`, porque no da (2.8:1).
- Las cifras y textos en naranja van en `--azafran-texto` `#A9541C` (4.5:1). El `#E2823D` como texto sobre crema no se lee (2.4:1).
- El salvia `#607F6D` sobre crema (3.8:1) solo sirve para títulos grandes, íconos y bordes. Para links y texto verde chico se usa `--salvia-osc` (5.5:1).
- El topo `#9A8B78` no se usa como texto. Para textos secundarios se usa `--topo-osc` (5:1).

### Tipografía

| Rol | Fuente | Por qué |
|-----|--------|---------|
| Display / palabras sueltas grandes ("Formarse para enseñar", "Nivel I", números de módulo) | **Fugi** (incluida, `@font-face`) | Es la firma de FHS. **Solo** en textos sin ¿¡ ni diacríticos sánscritos. |
| Títulos H1–H3, nombres de módulos, términos sánscritos | **Cormorant Garamond** 500/600 (Google Fonts) | Serif clásica que une la elegancia de Fugi con la autoridad serif de Ātmabodha, y **sí** tiene ā ī ū ṇ ṣ ś ṅ ṃ. |
| Cuerpo, listas, tablas, botones | **Jost** 400/500 (Google Fonts) | Sans geométrica y liviana: limpia como la de Ātmabodha, pero con la suavidad de FHS. |
| Acento caligráfico (opcional, 1–2 veces en toda la página) | **Pinyon Script** (Google Fonts) | Guiño a los títulos script de Ātmabodha ("con el Dr. Gharote"). No abusar. |

Escala sugerida: H1 clamp(2.4rem, 6vw, 4.2rem) · H2 clamp(1.8rem, 4vw, 2.6rem) · cuerpo 17–18 px · interlineado 1.65.
Los términos sánscritos van en Cormorant Garamond *itálica* (āsana, prāṇāyāma, Nāḍī Śuddhi, satsaṅga).

### Elementos gráficos
- **Círculo de línea fina** (FHS) como marco de fotos clave: retrato del Dr. Gharote y foto de clase.
- **Íconos de línea** en salvia para los 8 módulos (loto, columna/postura, pulmón/respiración, gota/purificación, figura meditando, libro/rollo para filosofía…). Trazo 1.5 px, sin relleno.
- **Separadores**: línea fina topo con un punto o pequeño loto en el centro.
- **Detalle azafrán**: subrayado fino o punto naranja bajo los títulos de sección; números grandes de datos clave (512 · 10 meses · 8 módulos) en `--azafran-texto`.
- **Bordes redondeados suaves** (12–16 px) en tarjetas; botones tipo píldora (radio completo), como los de los posts de FHS.
- Sombras casi nulas; jerarquía por color y espacio, no por sombra.
- Fotos con overlay cálido suave (no gris frío) para mantener la calidez.

### Estructura sugerida de secciones (con su tratamiento de color)
1. **Hero** — fondo crema, logos de FHS + Ātmabodha arriba (chicos, lado a lado, con divisor fino), título en marino, "Nivel I" en Fugi, foto del Dr. Gharote en círculo de línea fina. Botón azafrán "Quiero inscribirme".
2. **Datos clave** — banda crema-fhs con 4 cifras en `--azafran-texto`: 512 h cátedra · 10 meses · Online en vivo · Certificación Lonavla.
3. **Concepto** — frase grande en Cormorant marino: "Todo instructor de Yoga tiene que ser un buen practicante."
4. **Programa (8 módulos)** — tarjetas blancas sobre crema, ícono salvia + número en Fugi + nombre en Cormorant + horas en topo; desplegables (acordeón) con el detalle.
5. **Cursada y agenda 2027** — línea de tiempo marzo → noviembre en salvia, con hitos en azafrán (inicio 13/3, receso julio, cierre 27/11).
6. **El maestro: Dr. M. L. Gharote** — bloque oscuro marino con texto crema y acento azafrán; foto de él dando clase.
7. **Inversión y promos** — tarjetas limpias, la promo destacada con borde azafrán.
8. **Respaldo** — logos FHS, Ātmabodha, The Lonavla Yoga Institute; normativa.
9. **Cierre / CTA** — "Formarse para enseñar. Practicar para comprender." en Fugi + botón WhatsApp azafrán.

### Lo que NO hacer
- No usar rosa ni celeste como colores de interfaz.
- No usar Fugi con ¿ ¡ ā ṇ ś etc. (se rompen las letras).
- No poner bloques grandes de naranja de fondo (ese es el estilo "post de Instagram" de Ātmabodha; acá solo acento).
- No usar negro puro ni blanco puro de fondo.
- No mezclar más de 3 familias tipográficas a la vez en una misma vista.

---

## Archivos incluidos en el paquete
- `IDENTIDAD-VISUAL-formacion-yoga.md` (este brief)
- `logo-fhs.png` — logo FHS, verde salvia, fondo transparente
- `Fugi.woff`, `Fugi.ttf` — tipografía de FHS
- `branding-fhs.png` — lámina del manual de marca FHS (referencia)
