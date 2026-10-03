# Toyota bZ4X eléctrica · Asesoría Harold Marín

App (PWA) de venta estilo Toyota para la **Toyota bZ4X Limited 2026**, SUV 100 % eléctrica AWD.
Pensada para presentarla a Autoamérica (concesionario Toyota en Antioquia, con sede en Apartadó) y para compartir por WhatsApp con clientes del Bajo Cauca, Córdoba, Nordeste, Urabá y Sucre.

**Sitio:** https://haroldco45.github.io/toyota-bz4x/

## Qué trae
- Portada con video de la unidad real, precio de referencia y botón de WhatsApp.
- Galería de fotos sacadas del video del concesionario.
- Seguridad, carga, garantía, ficha técnica y preguntas frecuentes.
- Calculadora de ahorro frente a la gasolina (gasolina de referencia de octubre de 2026, kWh editable).
- Beneficios de los eléctricos en Colombia en 2026.
- 4 videos reales de la bZ4X en Colombia desde YouTube (se cargan al tocarlos).
- Código de referido igual al de Vibras Motor (VM-TOY-AAMMDD-NNNN, con fecha en hora Colombia): el cliente llena nombre, ciudad, celular y forma de pago, autoriza datos (Ley 1581 de 2012) y se abre WhatsApp con la solicitud y el código. La app no guarda datos.
- Instalable como app (manifest + service worker) y vista previa para WhatsApp (og-image.jpg, 1200×630).

## Archivos
Las fotos y el video de portada van **dentro** de `index.html`, así que con ese archivo la app ya se ve completa.
En la raíz del repo van también: `og-image.jpg` (vista previa en WhatsApp), `video-bz4x.mp4` (botón «Ver el video completo»; si falta, el botón se oculta solo), `manifest.json`, `sw.js`, `icon-192.png` e `icon-512.png` (para instalarla como app).

## Concesionario aliado
Cuando Autoamérica u otro concesionario firme, edite `CONFIG.aliado` al inicio del script en `index.html` (nombre, ciudad, asesor y WhatsApp con 57 adelante). Desde ese momento las solicitudes le llegan directo al asesor y aparece el botón para mandarle copia a Harold.

## Actualizar
Al cambiar fotos o textos, suba la versión de `CACHE` en `sw.js` (`bz4x-v3`, `bz4x-v4`…) para que los teléfonos que ya la instalaron reciban el cambio. Si WhatsApp sigue mostrando la vista previa vieja, comparta el link con `?v=2` al final.

Precios y datos consultados el 3 de octubre de 2026 (hora Colombia). El concesionario confirma el valor final.

---
Desarrollada por Vibras Positivas HM — Derechos de Autor Reservados
