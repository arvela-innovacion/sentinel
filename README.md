# Sentinel by ARVELA

Demostración web de monitorización inteligente de vídeo, preparada para despliegue estático en GitHub Pages.

## Funciones principales
- Cámara en directo, vídeo local y URL HTTPS directa.
- Detección y seguimiento de personas y vehículos.
- Registro local de personas autorizadas y matrículas.
- Reconocimiento multiframe y estados KNOWN / UNKNOWN / UNCERTAIN / AUTHORIZED.
- Editor gráfico de zonas sobre el vídeo.
- Líneas virtuales y detección de cruces/dirección.
- Reglas configurables asociadas a zonas.
- Incidentes con captura de evidencia, zona, permanencia y cronología.
- Flujo de incidente: abierto → reconocido → resuelto.
- Procesamiento en navegador y almacenamiento local de configuración.

## Publicación
Sube `index.html`, `styles.css`, `app.js` y este README a la raíz del repositorio y activa GitHub Pages desde la rama principal.

## Nota
Es un entorno de demostración. Los modelos y heurísticas deben validarse con cámaras, iluminación y escenarios representativos antes de cualquier uso operativo.
