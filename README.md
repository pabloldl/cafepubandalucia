# Café-Pub Andalucía

Propuesta web no oficial para Café-Pub Andalucía, El Bosque, Cádiz. Pendiente de aprobación del establecimiento. Implementada con HTML5, CSS3 y JavaScript vanilla, sin dependencias, compilación ni instalación.

## Abrir y publicar

Abre `index.html` directamente en un navegador. Para publicar en cualquier hosting estático, sube el contenido de esta carpeta conservando las rutas: `index.html` debe quedar en la raíz pública. No es necesario ejecutar comandos ni utilizar Node.js.

## Archivos

- `index.html`: todo el contenido, enlaces, metadatos y datos estructurados.
- `css/style.css`: variables, estilos por sección, animaciones y reglas responsive.
- `js/script.js`: menú móvil, cabecera al hacer scroll, apariciones y año dinámico.
- `img/`: fotografías locales.
- `favicon.svg`: icono editable.

## Modificar contenido

**Textos:** edita directamente el HTML. Los comentarios identifican cada sección. Conserva los identificadores `inicio`, `nosotros`, `carta`, `ambiente` y `contacto`, o actualiza los enlaces internos si los cambias.

**Fotografías:** sustituye los JPG de `img/` o cambia sus rutas `src`. Actualiza el texto alternativo `alt` para describir cada nueva fotografía. Se usan recortes CSS con `object-fit: cover`; puedes ajustar `object-position`. Conserva dimensiones en las etiquetas para reservar espacio. La portada carga con prioridad; el resto usa carga diferida.

**Colores y tipografías:** edita las variables de `:root` al principio de `css/style.css`: `--cream`, `--paper`, `--ink`, `--muted`, `--amber`, `--serif` y `--sans`. Las tipografías del sistema evitan peticiones a proveedores externos.

**Carta y redes:** busca sus URL en `index.html` y modifica todas las apariciones, incluyendo `hasMenu` y `sameAs` en los datos estructurados. Se mantiene el enlace de Odibo suministrado; su disponibilidad depende del proveedor.

**Contacto:** actualiza dirección y teléfono tanto en el contenido como en el JSON-LD del `<head>`. Los enlaces de llamada usan `tel:+34956727049`. Google Maps utiliza una búsqueda con el nombre y la dirección; actualiza las dos URL si cambia la ubicación. No se integra un mapa, cookies ni analítica: Google Maps solo se abre cuando el visitante pulsa el enlace.

**SEO:** revisa `<title>`, descripción y datos estructurados antes de publicar. Solo se incluyen nombre, dirección, teléfono y enlaces facilitados. El año del pie se actualiza automáticamente. No se incluyen horarios, precios, reseñas, premios, WhatsApp ni Instagram no confirmados.

## Fotografías y derechos

Imágenes genéricas de Unsplash utilizadas como inspiración, sin atribuirlas al negocio. Licencia consultada: https://unsplash.com/license (permite descargar y utilizar imágenes de forma comercial y no comercial). No proceden de Google Maps, Facebook ni Tripadvisor. La galería y la portada indican su carácter representativo.

Fuentes de los recursos:

| Archivo | Recurso original |
| --- | --- |
| `hero.jpg` | https://images.unsplash.com/photo-1568901346375-23c9450c58cd |
| `cafe.jpg` | https://images.unsplash.com/photo-1442512595331-e89e73853f31 |
| `interior.jpg` | https://images.unsplash.com/photo-1514933651103-005eec06c04b |
| `compartir.jpg` | https://images.unsplash.com/photo-1547592180-85f173990554 |
| `cerveza.jpg` | https://images.unsplash.com/photo-1535958636474-b021ee887b13 |

Las fotos no prueban ingredientes, presentación, decoración ni servicios del negocio. Sustitúyelas por material propio autorizado antes de presentar la web como oficial. Los contenidos de las categorías son orientativos y remiten a la carta para consultar disponibilidad; no se inventan nombres de platos ni precios.

## Revisión antes de publicar

Comprueba en un navegador de escritorio y móvil la navegación, los recortes de las fotos y la ausencia de desbordamientos. En móvil, el botón abre y cierra el menú; los enlaces, Escape y un clic fuera lo cierran. Prueba navegación con teclado y la preferencia de movimiento reducido del sistema. Verifica manualmente la carta externa, Google Maps, Facebook y la llamada en un teléfono.

Los enlaces externos se abren en otra pestaña con `noopener noreferrer`. Las secciones permanecen visibles si JavaScript está desactivado. El diseño contiene puntos de adaptación a 1050, 760 y 380 píxeles.
