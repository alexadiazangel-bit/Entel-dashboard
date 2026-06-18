# Entel Chile · Dashboard de Seguimiento

Dashboard de seguimiento de sitios de sensorización energética para Entel Chile, construido con el mismo formato y diseño que [Analytix Dashboard](https://alexadiazangel-bit.github.io/Analytix-dashboard/).

## Contenido

- **65 sitios** (pestaña "📡 Sitios"): estado de instalación, alertas, IP VPN, fecha de instalación, novedades y mediciones eléctricas por línea (C1-L1 a C2-L4), extraídos de la hoja `SITIOS_EN_OPERACION` del Excel.
- **6 cámaras** (pestaña "📷 Cámaras"): sitios con cámaras reportando novedades (vandalizado, sin reporte, chip sin datos).

## Funcionalidades

- KPIs: total de sitios, sitios OK, pendientes/revisita, cámaras con novedad.
- Búsqueda y filtro por estado, en cada pestaña.
- Crear, editar y eliminar sitios y cámaras.
- Historial de novedades por sitio (guarda versiones anteriores).
- Descarga de datos en JSON / CSV / XLSX.
- Sincronización opcional con GitHub (guarda los datos en un archivo `data/entel.json` de tu repositorio) — se configura con el ícono ⚙ de la barra superior.
- Tema claro / oscuro.
- Todo funciona 100% en el navegador (localStorage), sin necesidad de backend.

## Cómo publicarlo en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `Entel-dashboard`).
2. Sube el archivo `index.html` a la raíz del repositorio (puedes arrastrarlo desde la web de GitHub o hacer `git add/commit/push`).
3. Ve a **Settings → Pages**, selecciona la rama `main` y la carpeta `/ (root)`, y guarda.
4. En un par de minutos tu dashboard estará disponible en:
   `https://<tu-usuario>.github.io/<nombre-del-repo>/`

## Sincronización con GitHub (opcional)

Si quieres que los cambios se guarden automáticamente en el repositorio (y no solo en tu navegador):

1. Genera un **Personal Access Token** en GitHub (Settings → Developer settings → Personal access tokens) con permiso `repo`.
2. Abre el dashboard, haz clic en ⚙ (arriba a la derecha).
3. Completa usuario, nombre del repositorio y el token. El archivo por defecto es `data/entel.json`.
4. Usa "⬆ Guardar en GitHub" para subir los datos actuales, o deja que se sincronice automáticamente al editar.

⚠️ El token se guarda solo en tu navegador (localStorage). No lo compartas ni lo subas a un repositorio público.
