# Lector PDF Web

Prototipo de lector de PDF con Text-to-Speech.

## Qué hace
- Selecciona un PDF desde el teléfono o computadora.
- Extrae el texto página por página.
- Lee el texto usando las voces disponibles en el navegador/dispositivo.
- Play/Pausa.
- Avance y retroceso por página.
- Cambia velocidad.
- Guarda la última página por documento.
- Incluye archivos de PWA para poder instalarla desde Chrome cuando se despliega por HTTPS.

## Limitaciones actuales
- Los PDFs escaneados como imagen necesitan OCR.
- La lectura con pantalla apagada puede detenerse dependiendo de Chrome/Android.
- PDFs con varias columnas o diseños complejos pueden extraerse en un orden imperfecto.
- Para que la PWA sea instalable de forma confiable, súbela a un sitio HTTPS (por ejemplo GitHub Pages, Netlify o Vercel).

## Probar en computadora
La forma más segura es servir la carpeta con un servidor local:

### Python
```bash
python -m http.server 8000
```

Después abre:
http://localhost:8000

## Probar en Android
La opción más cómoda es desplegar la carpeta en un servicio HTTPS.
Después abre la URL en Chrome y usa:
Menú ⋮ > Agregar a pantalla principal / Instalar app

## Siguiente versión
- OCR para PDFs escaneados.
- Reanudar dentro de una página, no solo por página.
- Temporizador de sueño.
- Marcadores.
- Detección de capítulos.
- Mejor tratamiento de encabezados/pies de página.
- Reproducción más robusta en segundo plano.
