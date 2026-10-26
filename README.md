# formaciondeyoga

Página estática (HTML) de la Formación Profesional en Yoga Tradicional con el Dr. Manmath Gharote, para publicar en Netlify.

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

### Dr. Manmath Gharote

- `gharote-retrato.jpg` — retrato sonriente de Gharote con kurta amarilla, frente a una diapositiva proyectada.
- `gharote-clase-manuscritos.jpg` — Gharote en el aula mostrando manuscritos antiguos a las alumnas (de espaldas en primer plano). Foto usada en el boceto `preview-mix.png`.
- `gharote-sonriendo-manuscritos.jpg` — Gharote con kurta roja, sonriendo y sosteniendo dos manuscritos antiguos en hoja de palma.
- `gharote-pizarra-alma-cuerpo.jpg` — Gharote dibujando en una pizarra un esquema de cuerpo y alma (estados de conciencia), con una diapositiva sobre Yoga Sūtra detrás.
- `gharote-conferencia-om-shanti.jpg` — Gharote con kurta naranja, manos en namasté, junto a una diapositiva "Om Shantih"; una persona con micrófono a la izquierda.
- `gharote-conferencia-kriti-rakshana.jpg` — Gharote con kurta amarilla dando una charla ante una diapositiva "Kriti Rakshana"; manuscrito desenfocado en primer plano.
- `gharote-parampara-linaje-bn.jpg` — Gharote en blanco y negro frente a la diapositiva "Parampara (Tradition)" con el linaje de maestros (Kuvalayananda, Gharote).
- `gharote-corrigiendo-postura.jpg` — Gharote ajustando la postura de un alumno recostado durante una práctica, en un salón luminoso.

### Directores de las tres instituciones

- `estela-natalia-gharote.jpg` — Estela Puchalski (izquierda), el Dr. Manmath Gharote (centro) y Natalia Solvey (derecha), sonriendo con las manos en namasté.
- `estela-retrato.jpg` — Estela Puchalski (directora de la Fundación Holística de la Selva), sentada, de perfil y sonriendo (vertical).
- `natalia-y-gharote.jpg` — retrato de Natalia Solvey (directora de Ātmabodha) junto a Gharote, al aire libre.
- `avatar-gharote.jpg`, `avatar-natalia.jpg`, `avatar-estela.jpg` — retratos cuadrados de 480×480 de cada director/a, recortados de las fotos de arriba. Se muestran en las tarjetas de las instituciones.

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

Fotos de la página: `gharote-clase-manuscritos.jpg` (apertura), `practica-sarvangasana-grupo.jpg` (módulo 8), `gharote-sonriendo-manuscritos.jpg` (Satsaṅga), `gharote-retrato.jpg` (maestro), `estela-natalia-gharote.jpg` (los tres directores), los retratos `avatar-*.jpg` y los logos. `gharote-retrato.jpg` es también la imagen de vista previa al compartir (`og:image`).

Cinta de fotos: al final del bloque 5 hay una banda de ancho completo con fondo azul marino y una tira de 24 fotos grandes (hasta 400 px de alto en celular y 560 px en escritorio) (incluye las de las cursadas en Misiones y los viajes a la India), sin textos. Avanza sola hacia un costado y también se maneja a mano, con flechas a los lados o deslizando con el dedo; al tocarla se frena unos segundos y retoma. Usa miniaturas de hasta 1100 px (unos 2,7 MB en total) en `assets/img/thumbs/` (mismo nombre que la foto grande, que queda disponible en `assets/img/`). Para sumar una foto: agregar su miniatura en `assets/img/thumbs/` y un `<img>` con su `alt` dentro de `.cinta-pista` en `index.html`. Nada más: el script repite el juego de fotos solo, para que el recorrido dé la vuelta sin saltos. La velocidad se cambia con `VELOCIDAD` en el script. Las fotos no son links. Con la opción de reducir movimiento activada no avanza sola, pero las flechas y el dedo siguen funcionando.

Instituciones (bloque 5): cada tarjeta muestra las primeras líneas de su descripción y el resto en un "Leer más" (un `<details class="d-mas d-inst">` nativo, sin JavaScript). En escritorio las tres tarjetas reservan el mismo alto para que el título, el "Leer más", el link y las redes queden a la misma altura; en celular y tablet van en una columna.

Todo lo que necesitás saber (bloque 6): en escritorio es una grilla de dos columnas con las piezas `i-cursada`, `i-inv`, `i-promos`, `i-cert` e `i-medios`, ubicadas para que las dos columnas terminen en la misma línea. Si se agrega o quita contenido en alguna de esas tarjetas, conviene volver a revisar que sigan parejas.

Plantel docente (dentro del bloque 5, antes de la cinta de fotos): una hilera chica y de bajo perfil. Son tarjetas compactas (foto redonda, nombre y dos o tres líneas) que se corren hacia el costado con las flechas de arriba a la derecha o deslizando con el dedo; no avanza sola. Si todas entran en pantalla, las flechas se ocultan. La biografía completa de Natalia Solvey se abre con "Leer más" en un recuadro (un `<dialog>` nativo) que se cierra con la X, con la tecla Esc o tocando afuera. Fotos en `assets/img/`: `docente-andrea-glomba.jpg` y `docente-natalia-solvey.jpg`. Marcela Peper y Graciela Bonboni todavía no tienen foto: sus tarjetas muestran un círculo con las iniciales. Para poner la foto, subir el archivo a `assets/img/` y reemplazar el `<div class="d-av sin-foto">` por `<img class="d-av" src="assets/img/NOMBRE.jpg" width="..." height="..." loading="lazy" alt="Retrato de ...">`. Para Graciela falta también su información: reemplazar el `<p class="d-pend">` por una lista `<ul class="d-roles">`. Para sumar a otra persona, copiar una tarjeta `<article class="d-card">`.

En las fotos `diploma-escuela-hatha-yoga-misiones.jpg` y `egresadas-diplomas-escuela-hatha-yoga-misiones.jpg` están tapados con un mosaico los nombres y DNI de los diplomas. Si se agregan fotos con documentos o datos personales legibles, conviene taparlos antes de publicarlas.

Tipografía: Cormorant Garamond para títulos, números, frases y sánscrito; Jost para texto, etiquetas y botones; Fugi solo en la frase final de cierre.

Links a las webs y redes de las tres instituciones: en el bloque 5 cada logo lleva a su web, debajo se ve la dirección escrita y después van los íconos de sus redes (SVG inline, definidos una vez al comienzo del `<body>` y reutilizados con `<use>`). El pie repite los logos con link y suma una fila con todas las webs y redes, con las direcciones a la vista.

Ningún link usa `target="_blank"`: todos abren en la misma pestaña, porque el navegador interno de WhatsApp e Instagram en iPhone bloquea las pestañas nuevas y el toque no hace nada. No hay links armados con JavaScript. El botón flotante de WhatsApp está a 96 px del borde inferior (más el área segura de iPhone) para no quedar tapado por el cartel de Netlify.

Constante para editar, arriba del `<script>` al final de `index.html`:

- `WHATSAPP_URL`: ya tiene el número +54 9 376 411-8610. Los tres botones de inscripción y el botón flotante la usan. Para cambiar el número, editar solo esa línea (y el `href` de respaldo `https://wa.me/5493764118610` de los botones).

Para probarla en local hace falta un servidor (por ejemplo `npx serve` en esta carpeta), porque abrir el archivo directo no carga bien las fuentes.

### Contacto por email y formulario

El email de contacto es yoga.lonavla@gmail.com. Aparece en el cierre (dentro de la tarjeta de contacto, con botones para escribir y para copiarlo), junto al botón de inscripción del bloque 6 y en el pie. Todos son links `mailto:` normales, sin `target`.

La tarjeta de contacto también tiene un formulario (nombre, email y consulta) que usa **Netlify Forms**: no hace falta servidor propio. Cada consulta se guarda en Netlify (solapa **Forms** del sitio), pero para que además llegue un aviso por email hay que activarlo una sola vez:

1. Entrar a app.netlify.com y abrir el sitio.
2. Ir a **Forms** y abrir **Submission notifications** (link directo: https://app.netlify.com/projects/hathayogaformacion/forms?tab=notifications).
3. Tocar **Add notification** y elegir **Email notification**.
4. En el email de destino poner yoga.lonavla@gmail.com y elegir el formulario `consulta` (o todos).
5. Guardar.

Los nombres exactos de los botones pueden variar un poco, porque Netlify los cambia de vez en cuando. Los avisos salen de formresponses@netlify.com (revisar la carpeta de spam la primera vez). Como el formulario tiene un campo `email`, al tocar Responder en ese aviso la respuesta va directo a la persona que escribió.

El formulario se envía sin salir de la página y muestra un mensaje de gracias o de error. Si el navegador no tuviera JavaScript, Netlify lleva a `gracias.html`. Tiene un campo trampa (`bot-field`) contra el spam.

### Pendientes

- Foto de Marcela Peper, y foto e información de Graciela Bonboni (plantel docente; Graciela aparece marcada como `[a confirmar]`).
- En la página no queda ningún dato marcado como `[a confirmar]`.
- Fuera de la página: activar en Netlify la notificación por email del formulario `consulta` (ver arriba).
- Los datos para pagar (alias, CBU, cuenta en dólares) no están en la página: se envían a quien se inscribe.
