# CPAP Machala — Sitio piloto

Sitio de una sola página (Inicio, Productos, Contacto) para venta de equipos CPAP en Machala, Ecuador. Sin datos de contacto reales todavía (teléfono, dirección, mapa) — es un piloto.

## Contenido de la carpeta

- `index.html` — el sitio completo (HTML + CSS + JS en un solo archivo)
- `robots.txt` — permite indexación y apunta al sitemap
- `sitemap.xml` — mapa del sitio para buscadores
- `vercel.json` — configuración mínima de hosting (URLs limpias, headers de seguridad)

## Desplegar en Vercel desde Claude Code

Desde esta misma carpeta, en tu terminal:

```bash
# 1. Instala la CLI de Vercel si no la tienes
npm i -g vercel

# 2. Inicia sesión (abre el navegador para autenticarte)
vercel login

# 3. Despliega a producción
vercel --prod
```

Vercel te dará una URL del tipo `https://cpap-machala-xxxx.vercel.app`. Si quieres fijar siempre el mismo nombre de proyecto, en el primer `vercel` te preguntará el nombre — usa algo como `cpap-machala`.

## Después del primer deploy (importante para el SEO)

En `index.html`, `robots.txt` y `sitemap.xml` dejé como referencia el dominio `https://cpap-machala.vercel.app/`. Una vez que tengas la URL final (o un dominio propio conectado en Vercel), reemplaza ese valor en los 3 archivos:

- `index.html`: etiquetas `canonical`, `og:url`
- `robots.txt`: línea `Sitemap:`
- `sitemap.xml`: etiqueta `<loc>`

## Pendientes antes de salir de "piloto"

- Agregar teléfono / WhatsApp real
- Agregar dirección y Google Maps
- Confirmar modelos y precios reales de los equipos (hoy son de ejemplo)
- Conectar el formulario de contacto a un correo o servicio real (hoy es solo visual)
