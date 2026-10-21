# formaciondeyoga

Página estática (HTML) de la Formación Profesional en Yoga Tradicional con el Dr. M. L. Gharote, para publicar en Netlify.

## Estructura de carpetas

```
formaciondeyoga/
├── index.html
├── README.md
├── IDENTIDAD-VISUAL-formacion-yoga.md   ← guía de marca (colores, tipografías, tono)
├── preview-mix.png                      ← boceto de referencia del estilo visual
└── assets/
    ├── fonts/
    │   ├── Fugi.ttf
    │   └── Fugi.woff
    └── img/
        └── (ver listado abajo)
```

Todas las imágenes viven solo en `assets/img/` y las fuentes en `assets/fonts/`. Rutas a usar desde `index.html`: `assets/img/<archivo>` y `assets/fonts/<archivo>`.

Convención de nombres: minúsculas, palabras separadas por guiones, sin tildes ni ñ, extensión `.jpg` o `.png`.

## Fuentes (`assets/fonts/`)

- `Fugi.woff`, `Fugi.ttf` — tipografía Fugi Regular de la marca FHS (Fundación Holística de la Selva).

## Imágenes (`assets/img/`)

Las fotos están optimizadas: máximo 1600 px en el lado más largo, JPG calidad ~80 (todas por debajo de 300 KB), orientación corregida y sin metadatos.

### Logos y marca

- `logo-atmabodha.png` — logo de Ātmabodha, Escuela de Yoga Tradicional ("En camino hacia la Sabiduría"), PNG con fondo transparente, 480×480.
- `logo-fhs.png` — logo de la Fundación Holística de la Selva, verde salvia sobre fondo transparente, 1080×1080.
- `logo-lonavla.png` — sello de The Lonavla Yoga Institute (India), PNG con fondo transparente, 360×360.
- `branding-fhs.png` — lámina del manual de marca FHS (logo, paleta, tipografía Fugi, íconos). Solo referencia.

### Dr. M. L. Gharote

- `gharote-retrato.jpg` — retrato sonriente de Gharote con kurta amarilla, frente a una diapositiva proyectada.
- `gharote-clase-manuscritos.jpg` — Gharote en el aula mostrando manuscritos antiguos a las alumnas (de espaldas en primer plano). Foto usada en el boceto `preview-mix.png`.
- `gharote-sonriendo-manuscritos.jpg` — Gharote con kurta roja, sonriendo y sosteniendo dos manuscritos antiguos en hoja de palma.
- `gharote-pizarra-alma-cuerpo.jpg` — Gharote dibujando en una pizarra un esquema de cuerpo y alma (estados de conciencia), con una diapositiva sobre Yoga Sūtra detrás.
- `gharote-conferencia-om-shanti.jpg` — Gharote con kurta naranja, manos en namasté, junto a una diapositiva "Om Shantih"; una persona con micrófono a la izquierda.
- `gharote-conferencia-kriti-rakshana.jpg` — Gharote con kurta amarilla dando una charla ante una diapositiva "Kriti Rakshana"; manuscrito desenfocado en primer plano.
- `gharote-parampara-linaje-bn.jpg` — Gharote en blanco y negro frente a la diapositiva "Parampara (Tradition)" con el linaje de maestros (Kuvalayananda, Gharote).
- `gharote-corrigiendo-postura.jpg` — Gharote ajustando la postura de un alumno recostado durante una práctica, en un salón luminoso.

### Directores de las tres instituciones

- `estela-natalia-gharote.jpg` — Estela Puchalski (izquierda), el Dr. M. L. Gharote (centro) y Natalia Solvey (derecha), sonriendo con las manos en namasté.
- `estela-retrato.jpg` — Estela Puchalski (directora de la Fundación Holística de la Selva), sentada, de perfil y sonriendo (vertical).
- `natalia-y-gharote.jpg` — retrato de Natalia Solvey (directora de Ātmabodha) junto a Gharote, al aire libre.
- `avatar-gharote.jpg`, `avatar-natalia.jpg`, `avatar-estela.jpg` — recortes cuadrados de 240×240 de cada director/a (hoy no se usan en la página).

### Grupos de alumnos

- `grupo-alumnos-gharote-bn.jpg` — foto grupal en blanco y negro de alumnos con Gharote sentado al centro; a la derecha, el banner de Ātmabodha.
- `grupo-alumnos-gharote-parque.jpg` — foto grupal a color en un parque arbolado, con Gharote de kurta amarilla entre los alumnos.

### Práctica y estudio

- `clase-yoga-tradicional-pizarra.jpg` — clase en un salón blanco: una instructora junto a un pizarrón con "Yoga Tradicional" y el Om, y alumnas con remeras de Ātmabodha levantando el brazo.
- `practica-asana-manos-arriba.jpg` — práctica de yoga (formato vertical): alumnas sentadas con las manos unidas sobre la cabeza, sobre mats violetas y piso de parqué.
- `practica-sarvangasana-grupo.jpg` — grupo de alumnas en Sarvangasana (postura sobre los hombros) sobre mats violetas, con una instructora sentada a la izquierda.
- `manos-manuscrito-antiguo.jpg` — primer plano de manos sosteniendo un manuscrito antiguo, con mats y almohadones de yoga de fondo.
- `libros-hatha-pradipika.jpg` — pila de libros con la *Haṭhapradīpikā* de Svātmārāma en primer plano.

## La página

Es una sola página de venta (landing) que se manda por WhatsApp. `index.html` es un único archivo con el CSS y el JS adentro, sin frameworks ni build, sin menú ni navegación. Solo carga Google Fonts (Cormorant Garamond y Jost) y la fuente local Fugi.

Tiene exactamente los 7 bloques de `CONTENIDO-PAGINA-formacion-yoga.md`, en ese orden: apertura, la propuesta, frase central, qué vas a estudiar, quiénes nos respaldan, todo lo que necesitás saber y cierre. El estilo sale de `IDENTIDAD-VISUAL-formacion-yoga.md`.

Fotos que usa la página (máximo 4): `gharote-clase-manuscritos.jpg` (apertura), `practica-sarvangasana-grupo.jpg` (módulo 8), `gharote-retrato.jpg` (maestro) y los logos. `gharote-retrato.jpg` es también la imagen de vista previa al compartir (`og:image`). El resto de las fotos queda disponible en `assets/img/` pero no se usa.

Constante para editar, arriba del `<script>` al final de `index.html`:

- `WHATSAPP_URL`: reemplazar `XXXXXXXXXXX` por el número con código de país. Los tres botones de inscripción y el botón flotante la usan.

Para probarla en local hace falta un servidor (por ejemplo `npx serve` en esta carpeta), porque abrir el archivo directo no carga bien las fuentes.

### Pendientes (marcados en la página como `[a confirmar]`)

- Días y horarios de las clases de práctica y del Satsaṅga.
- Tercera resolución de la certificación nacional.

### Pendientes que no se ven en la página

- Número de WhatsApp (`WHATSAPP_URL`).
- Dominio de Netlify en la meta `og:image` (reemplazar `SITIO-A-CONFIRMAR.netlify.app` en `index.html`), para que WhatsApp muestre la vista previa.
