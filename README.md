# Calculadora de Calor SST

Calcula el índice de calor efectivo y el nivel de riesgo según el Protocolo de SST ante el Fenómeno El Niño (MTPE, octubre 2026). Genera el registro en PDF y Excel.

Sitio estático sin carpetas: los 10 archivos van juntos en la raíz del repositorio. No necesita compilar ni instalar nada.

## Subir a GitHub
1. Crea un repositorio nuevo en github.com (por ejemplo `calculadora-calor-sst`).
2. Entra al repositorio y elige **Add file > Upload files**.
3. Selecciona los 10 archivos a la vez (o arrástralos) y confirma con **Commit changes**.

## Desplegar en Vercel
1. En vercel.com elige **Add New > Project** e importa el repositorio.
2. **Framework Preset:** Other. Deja vacíos Build Command y Output Directory.
3. Pulsa **Deploy**.

## Probar en el celular
- Abre la dirección que entrega Vercel. Al ser https, el navegador puede pedir la ubicación.
- Para instalarla: menú del navegador > **Agregar a pantalla de inicio**.

## Archivos
- `index.html`: la aplicación completa.
- `jspdf.umd.min.js` (jsPDF 2.5.1) y `exceljs.min.js` (ExcelJS 4.4.0): generan el PDF y el Excel.
- `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`: instalación como app y uso sin conexión.
- `logo-gs.png`: logo de Good Solutions.
- `vercel.json`: encabezados para el service worker y el manifiesto.

## Fuente de datos automática
La ubicación consulta Open-Meteo (api.open-meteo.com). Revisa sus términos de uso antes de ofrecer la app a clientes, porque el acceso gratuito está pensado para uso no comercial.
