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
- Horarios: CONFIG.horarioSemana (Lun a Sáb, igual para todas, se muestra en cada tarjeta). Cada sucursal tiene su campo domingo: "de 10 a 14hs", "cerrado" (se ve "Dom Cerrado" en gris) o "". El nombre se muestra en mayúsculas por estilo; en los datos se escribe normal.
- Métricas: Umami (cloud.umami.is, cuenta de Buena Vibra). El script está en el <head>; cada botón activo manda un evento con su texto y la sucursal. No quitarlo al editar.
- WhatsApp: 549 + característica sin 0 + número sin 15 (ej. 5493511234567). Todas las sucursales usan el mismo número; CONFIG.mensajeWhatsApp lleva {sucursal}, que se reemplaza por el nombre de la sucursal del botón.
- Antes de publicar: mostrar el cambio y esperar confirmación.
- Un cambio por pedido, con un mensaje de guardado claro (ej. "Agrega sucursal Los Plátanos").
- Si algo sale mal, volver a la versión anterior con git.
