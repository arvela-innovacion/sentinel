# VisionGuard IA v7

Prototipo estático para GitHub Pages. Todo el procesamiento se ejecuta en el navegador.

## v7: motor de visión
- Fuentes: cámara, MP4/WebM local y URL HTTPS directa (si el servidor permite CORS).
- Catálogo visible de datasets públicos verificados: OTW y People in Public.
- Detección asíncrona de objetos; el vídeo no espera a cada inferencia.
- Tracking con IDs y estimación básica de movimiento.
- Reconocimiento facial multiframe: una identidad KNOWN/UNKNOWN se consolida tras varias evidencias.
- Quality gate facial: caras pequeñas o de baja confianza no fuerzan UNKNOWN.
- OCR desacoplado y más lento que detección.
- Diagnóstico de FPS de vídeo, latencia total, detección, caras y evidencias de identidad.
- Mantiene reglas, incidentes, perfiles faciales y matrículas de v6.

## Fuentes públicas
### Out the Window (OTW)
Vídeo real de seguridad, personas/vehículos/actividades. CC BY 4.0.
https://github.com/stresearch/otw

### People in Public (PIP)
Vídeos de personas en lugares públicos. CC BY 4.0. El proyecto indica que los sujetos han consentido compartir su información identificable para investigación de visión artificial; caras de no consentidos están difuminadas.
https://visym.github.io/collector/pip_250k_stabilized/

Los datasets no se redistribuyen dentro de este ZIP. Descarga clips desde la fuente y cárgalos con `Cargar MP4`. Esto conserva la atribución y evita depender de hotlinks/CORS inestables.

## GitHub Pages
Sube `index.html`, `app.js`, `styles.css` y este README al repositorio y activa Pages. Se necesita conexión a Internet para descargar las librerías/modelos CDN.

## Aviso
Prototipo académico. El reconocimiento biométrico y ANPR no deben usarse como único mecanismo de seguridad. Para despliegues reales hay que evaluar protección de datos, base jurídica, seguridad, sesgos y tasas de error.
