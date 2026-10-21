# Página de enlaces — Buena Vibra Barbería

Página única para la bio de Instagram. El sitio está en la carpeta public/ (index.html + logo.png); Cloudflare publica solo esa carpeta. Se publica sola en Cloudflare Pages al guardar cambios en GitHub.

## Reglas para editar

- Los pedidos del día a día (sucursales, nombres, números, links, horario, mensaje de WhatsApp) se resuelven SOLO editando el bloque "DATOS DE LA PÁGINA" (CONFIG y SUCURSALES) al principio de public/index.html.
- No tocar estilos ni la lógica salvo que se pida explícitamente un cambio de diseño o de funcionamiento.
- Agregar sucursal: copiar una ficha completa con los mismos campos.
- Ocultar un botón: dejar el dato en "". "PENDIENTE" lo muestra en gris.
- Links de Google por sucursal (con su Place ID):
  mapa:   https://www.google.com/maps/search/?api=1&query=Buena%20Vibra%20Barberia&query_place_id=PLACE_ID
  reseña: https://search.google.com/local/writereview?placeid=PLACE_ID
- Horarios: CONFIG.horario (lunes a sábado, igual para todas). Cada sucursal tiene su campo domingo: "10 a 14 h", "cerrado" o "".
- WhatsApp: 549 + característica sin 0 + número sin 15 (ej. 5493511234567).
- Antes de publicar: mostrar el cambio y esperar confirmación.
- Un cambio por pedido, con un mensaje de guardado claro (ej. "Agrega sucursal Los Plátanos").
- Si algo sale mal, volver a la versión anterior con git.
