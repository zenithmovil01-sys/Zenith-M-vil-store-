Zenith Móvil — tienda web inicial
Esta carpeta contiene una tienda estática inicial para probar y personalizar.
Incluye
Diseño adaptable a teléfonos y computadoras
Catálogo de productos de demostración
Filtros y búsqueda
Carrito con cantidades y total estimado en lempiras
Formulario de pedido que abre WhatsApp con el resumen
Manifest y service worker básicos para preparar la PWA
Antes de publicar (importante)
Abre app.js y verifica STORE.whatsappNumber. El número debe estar en formato internacional, sin +, espacios ni guiones.
Reemplaza los productos y precios de demostración en PRODUCTS por el catálogo real.
Añade fotos reales y autorizadas de tus productos; la versión inicial usa iconos ilustrativos.
Confirma las políticas de entrega, devoluciones, privacidad y condiciones de depósito.
No pongas contraseñas, claves bancarias ni datos privados de pago en archivos públicos.
El carrito no procesa pagos ni reserva inventario; el pedido se confirma manualmente por WhatsApp.
Prueba el sitio en teléfono y computadora antes de anunciarlo.
Probar localmente
Abre index.html en un navegador. El catálogo y carrito deberían funcionar; algunas funciones de PWA/service worker solo funcionan cuando el sitio se sirve por HTTPS o localhost.
Publicar gratis con GitHub Pages
Crea una cuenta en GitHub si aún no tienes una.
Crea un repositorio público llamado zenith-movil-store.
Sube todos los archivos y la carpeta assets conservando la estructura.
En el repositorio, entra a Settings → Pages.
En Build and deployment, selecciona Deploy from a branch, rama main, carpeta / (root), y guarda.
Espera a que GitHub Pages publique el sitio. La URL será similar a https://TU-USUARIO.github.io/zenith-movil-store/ (no puedes elegir el nombre de usuario de GitHub de otra persona).
Abre la URL desde el teléfono y prueba agregar productos y enviar un pedido de prueba.
Preparar Android / Google Play más adelante
Primero publica la web con HTTPS y prueba que funcione correctamente.
Comprueba que manifest.webmanifest y los iconos estén accesibles.
Abre PWABuilder y pega la URL pública para revisar la PWA y generar el paquete Android/TWA.
Sigue los pasos de PWABuilder para firma, Digital Asset Links y generación del Android App Bundle (.aab).
Crea la ficha en Google Play Console, completa privacidad y declaraciones, realiza las pruebas requeridas y envía la app a revisión.
No se garantiza aprobación; una app que sea solo una web dentro de un contenedor puede no cumplir las políticas de calidad. Revisa las políticas vigentes antes de pagar o publicar.
Costes y límites
Los archivos del sitio son gratuitos.
GitHub Pages ofrece alojamiento estático para repositorios compatibles, pero el sitio en un repositorio público será visible para cualquiera.
Google Play Console cobra una tarifa de registro de desarrollador (la documentación de PWABuilder indica US$25; verifica el importe y las condiciones actuales en Play Console).
Esta versión no incluye base de datos, panel de administración, gestión de pedidos, inventario sincronizado, cuentas de usuario ni cobro automático.
