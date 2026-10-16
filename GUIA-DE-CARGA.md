# Guía de carga — Impresión 3D

## Editar el contenido
1. Abrí `data/contenido.json` en GitHub y presioná el lápiz.
2. Cambiá el texto entre comillas. Conservá las comas, llaves y corchetes.
3. Usá «Commit changes» para guardar en `main`. GitHub Pages publica la actualización cuando termina su despliegue.

## Diseños
Cada elemento de `disenos` tiene `id` único, `titulo`, `categoria`, `imagen`, `descripcion`, `material`, `formato`, `archivo` y `estado`.
- Los tres ejemplos iniciales son ilustrativos, sin archivos disponibles. Reemplazalos por proyectos propios comprobados.
- Para usar una foto propia, subila a `assets/` y agregá `"imagenUrl": "assets/mi-pieza.jpg"` al diseño.
- Para descarga pública, subí el STL o 3MF a `archivos/` y usá `"archivo": "archivos/mi-pieza.stl"`.
- Para solicitud por permiso dejá `"archivo": ""`. El botón prepara un correo; la autorización y la entrega son manuales.
- No subas archivos reservados a este repositorio público. Ocultar un botón no protege un archivo.
- No distribuyas G-code genérico para impresoras distintas.

## Videos
En `videos`, reemplazá `url` vacío por el enlace HTTPS al video. Se abre en una pestaña nueva. Podés alojar videos pequeños en `assets/`, pero para videos largos conviene un servicio de video y conservar el enlace en GitHub. `imagenUrl` permite una portada propia. Sin URL se muestra «Próximamente».

## Sponsors
Reemplazá `"sponsors": []` por una lista como:
```json
"sponsors": [
  {"nombre": "Nombre autorizado", "logo": "assets/logo-marca.png", "url": "https://ejemplo.com"}
]
```
Los espacios iniciales no representan acuerdos existentes. Cargá únicamente marcas autorizadas.

## Novedades
```json
"novedades": [
  {"titulo": "Título de la publicación", "resumen": "Texto breve", "url": "https://fuente-original.com"}
]
```
Agregá fuentes verificadas y respetá sus derechos de reproducción.

## Contacto e Instagram
`email` recibe las solicitudes mediante la aplicación de correo del visitante. El formulario no almacena envíos en un servidor. `instagram` acepta el enlace completo a tu perfil; mientras esté vacío, el icono lleva a Contacto.

## Diseño y publicación
- HTML: `index.html` y `administrar.html`.
- Estilos: `styles.css`. Interacción: `app.js`.
- Todo usa rutas relativas y funciona bajo `/estudio-3D/`.
- Pages: Settings → Pages → Deploy from a branch → main → / (root) → Save.
- El primer despliegue puede demorar unos minutos. Consultá Actions para ver el resultado.
- Los permisos de edición los controla GitHub; no hay contraseñas ni tokens guardados en el sitio.
