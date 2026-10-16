# Estudio 3D · Aula virtual

Sitio educativo de impresión 3D, diseño y fabricación. Implementación estática del diseño aprobado, con fondo blanco, acentos verdes, biblioteca de diseños, videotutoriales, sponsors, novedades y contacto.

## Sitio
URL prevista de GitHub Pages: https://patagoniatec-ux.github.io/estudio-3D/

## Publicar
En Settings → Pages, elegir **Deploy from a branch**, rama **main**, carpeta **/ (root)**. No hay instalación, compilación ni dependencias externas. `.nojekyll` permite servir los archivos directamente.

## Administrar
Abrí `administrar.html` desde el sitio para acceder a las herramientas de edición de GitHub. Solo los usuarios autorizados en el repositorio pueden guardar cambios. Los contenidos están en `data/contenido.json`; ver [Guía de carga](GUIA-DE-CARGA.md).

## Estado inicial
- Tres diseños ilustrativos sin STL adjuntos; la solicitud por correo funciona y la entrega es manual.
- Dos espacios de video preparados, marcados como próximos hasta cargar enlaces reales.
- Sponsors y novedades listos para completar, sin marcas ni noticias inventadas.
- Contacto con `mailto:`; requiere una aplicación de correo configurada. No hay almacenamiento de mensajes.
- Instagram pendiente de cargar.

## Archivos
`index.html`, `styles.css`, `app.js`, `administrar.html`, `data/contenido.json`, `assets/`, `archivos/`.

Las fotografías ilustrativas se presentan desde la imagen de diseño aprobada mediante recortes CSS. Se pueden sustituir individualmente con `imagenUrl` en el JSON. El original se conserva en `assets/diseno-aprobado.png`.

## Descargas con permiso
Este repositorio es público: todo archivo subido es público. Los archivos reservados o futuros contenidos pagos requieren almacenamiento protegido separado. Esta versión recibe solicitudes por correo y no implementa pagos ni acceso privado.

## Verificación local
Servir la carpeta con cualquier servidor estático, por ejemplo `python3 -m http.server 8000`, y abrir http://localhost:8000. No abrir el HTML como `file://`, ya que el navegador debe cargar el JSON mediante HTTP.
