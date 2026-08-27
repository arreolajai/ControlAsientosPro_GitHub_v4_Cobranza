# Control de Asientos Pro v4.0 Cobranza

Aplicación profesional para administrar viajes de autobús con 45, 47 o 50 pasajeros.

## Descarga y prueba inmediata

1. Descomprime el ZIP completo.
2. Abre `index.html`.
3. La interfaz, el croquis, la lista, los registros y los reportes funcionan también sin servidor porque CSS y JavaScript están integrados dentro de `index.html`.

> La instalación PWA y el Service Worker requieren HTTPS, por lo que se activan al publicar en GitHub Pages. El modo local no intenta registrar el Service Worker.

## Funciones incluidas

- Croquis profesional de autobús, incluido fondo, escalera y WC.
- Capacidades de 45, 47 y 50 pasajeros.
- Registro de nombre, teléfono, origen, destino y boleto.
- Estados Vacante, Apartado, Pagado/Abordado y Ausente.
- Vista lista en tarjetas, buscador y filtros.
- Configuración de ruta, fecha, salida, conductor y placa.
- Indicadores automáticos de ocupación.
- Persistencia local en el navegador.
- Exportación e importación de respaldo JSON.
- Reporte manifiesto con lista de pasajeros.
- Generación y descarga de PDF sin conexión.
- Reporte PNG/JPG.
- Compartir mediante el menú del dispositivo.
- Resumen para WhatsApp.
- Apertura de correo con asunto y cuerpo prellenados.
- PWA instalable y caché offline al publicarse con HTTPS.
- Diseño adaptable para celular, tablet y computadora.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo.
2. Descomprime este paquete.
3. Sube a la raíz del repositorio todos los archivos, incluyendo `.nojekyll` y la carpeta `icons`.
4. En GitHub entra a `Settings > Pages`.
5. En `Build and deployment`, selecciona `Deploy from a branch`.
6. Selecciona `main` y `/(root)`.
7. Guarda la configuración.

## Archivos

- `index.html`: aplicación autónoma completa. Incluye CSS y JavaScript para evitar páginas sin formato al abrir localmente.
- `styles.css`: copia editable de estilos.
- `app.js`: copia editable de la lógica.
- `manifest.webmanifest`: instalación PWA.
- `sw.js`: caché offline para HTTPS.
- `.nojekyll`: compatibilidad con GitHub Pages.
- `icons/icon.svg`: icono de la aplicación.

## Actualizaciones

La caché actual es `control-asientos-pro-v4-cobranza`. Cuando publiques una actualización, cambia ese nombre en `sw.js` para que los dispositivos descarguen la nueva versión.

## Nota sobre adjuntos de correo y WhatsApp

En dispositivos compatibles, el botón Compartir PDF entrega el archivo al menú nativo para elegir WhatsApp, Outlook, Gmail u otra aplicación. Cuando el navegador no permite compartir archivos, la aplicación descarga el PDF y abre WhatsApp o el cliente de correo con el texto preparado. En ese caso el archivo se adjunta manualmente, porque los enlaces web de correo no admiten adjuntos automáticos.

## Control de cobranza por pasajero o asiento

Cada asiento permite capturar y modificar la cantidad a cobrar y la cantidad abonada. El saldo se calcula automáticamente. El reporte y el PDF incluyen totales del viaje y detalle de cobro, abono y saldo por pasajero. El resumen de WhatsApp también incluye la cobranza.
