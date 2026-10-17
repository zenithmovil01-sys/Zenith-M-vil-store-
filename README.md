# Zenith Móvil — tienda web inicial

Esta carpeta contiene una tienda estática inicial para probar y personalizar.

## Incluye
- Diseño adaptable a teléfonos y computadoras
- Catálogo de productos de demostración
- Filtros y búsqueda
- Carrito con cantidades y total estimado en lempiras
- Formulario de pedido que abre WhatsApp con el resumen
- Manifest y service worker básicos para preparar la PWA

## Antes de publicar (importante)
1. Abre `app.js` y verifica `STORE.whatsappNumber`. El número debe estar en formato internacional, sin `+`, espacios ni guiones.
2. Reemplaza los productos y precios de demostración en `PRODUCTS` por el catálogo real.
3. Añade fotos reales y autorizadas de tus productos; la versión inicial usa iconos ilustrativos.
4. Confirma las políticas de entrega, devoluciones, privacidad y condiciones de depósito.
5. No pongas contraseñas, claves bancarias ni datos privados de pago en archivos públicos.
6. El carrito no procesa pagos ni reserva inventario; el pedido se confirma manualmente por WhatsApp.
7. Prueba el sitio en teléfono y computadora antes de anunciarlo.

## Probar localmente
Abre `index.html` en un navegador. El catálogo y carrito deberían funcionar; algunas funciones de PWA/service worker solo funcionan cuando el sitio se sirve por HTTPS o localhost.

## Publicar gratis con GitHub Pages
1. Crea una cuenta en GitHub si aún no tienes una.
2. Crea un repositorio público llamado `zenith-movil-store`.
3. Sube todos los archivos y la carpeta `assets` conservando la estructura.
4. En el repositorio, entra a **Settings → Pages**.
5. En **Build and deployment**, selecciona **Deploy from a branch**, rama `main`, carpeta `/ (root)`, y guarda.
6. Espera a que GitHub Pages publique el sitio. La URL será similar a `https://TU-USUARIO.github.io/zenith-movil-store/` (no puedes elegir el nombre de usuario de GitHub de otra persona).
7. Abre la URL desde el teléfono y prueba agregar productos y enviar un pedido de prueba.

## Preparar Android / Google Play más adelante
1. Primero publica la web con HTTPS y prueba que funcione correctamente.
2. Comprueba que `manifest.webmanifest` y los iconos estén accesibles.
3. Abre PWABuilder y pega la URL pública para revisar la PWA y generar el paquete Android/TWA.
4. Sigue los pasos de PWABuilder para firma, Digital Asset Links y generación del Android App Bundle (`.aab`).
5. Crea la ficha en Google Play Console, completa privacidad y declaraciones, realiza las pruebas requeridas y envía la app a revisión.
6. No se garantiza aprobación; una app que sea solo una web dentro de un contenedor puede no cumplir las políticas de calidad. Revisa las políticas vigentes antes de pagar o publicar.

## Costes y límites
- Los archivos del sitio son gratuitos.
- GitHub Pages ofrece alojamiento estático para repositorios compatibles, pero el sitio en un repositorio público será visible para cualquiera.
- Google Play Console cobra una tarifa de registro de desarrollador (la documentación de PWABuilder indica US$25; verifica el importe y las condiciones actuales en Play Console).
- Esta versión no incluye base de datos, panel de administración, gestión de pedidos, inventario sincronizado, cuentas de usuario ni cobro automático.
