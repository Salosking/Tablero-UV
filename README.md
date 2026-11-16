# Tablero Índice UV – Biodiversa

Tablero de Índice de Radiación UV para sucursales de Biodiversa (Chile), basado en el estándar preventivo ACHS y datos compatibles con la Dirección Meteorológica de Chile (DMC).

Es un único archivo (`index.html`), sin dependencias ni proceso de build.

## Publicar con GitHub Pages

1. Sube `index.html` y este `README.md` a la raíz de tu repositorio.
2. En GitHub: **Settings → Pages**.
3. En **Build and deployment**, elige **Deploy from a branch**, selecciona la rama `main` y la carpeta `/ (root)`, y guarda.
4. Tras un minuto estará disponible en `https://<usuario>.github.io/<repositorio>/`.

Abre esa URL en el monitor de cada sucursal y pulsa **Pantalla completa**.

## Personalización

- **Sucursales:** edita el arreglo `BRANCHES` al inicio del script (nombre, latitud y longitud).
- **Medidas adicionales:** edita `MEAS_EXTRA`.
- **Frecuencia de actualización:** `AUTO_REFRESH_MIN` (por defecto, 30 minutos).
- **Modo manual:** permite ingresar el IUV del reporte oficial de la DMC.

## Fuente de datos

El IUV se obtiene desde Open-Meteo con las coordenadas de cada ciudad, como respaldo compatible, porque el portal de la DMC (https://www.meteochile.gob.cl/PortalDMC-web/index.xhtml) no permite consultas directas desde el navegador (CORS).
