# webdeonelabs

Página del catálogo de servicios de **DeOne Labs** (webs, bots de WhatsApp con IA, correo
corporativo y automatizaciones para pymes en Colombia).

## Stack

- [Astro 5](https://astro.build) — sitio 100% estático
- [Tailwind CSS 4](https://tailwindcss.com) (vía `@tailwindcss/vite`)
- Fuentes: Space Grotesk (títulos) + DM Sans (texto)

## Desarrollo

```bash
npm install
npm run dev      # http://localhost:4321
npm run build    # genera dist/
```

## Despliegue

Estático → S3 + CloudFront (cuenta AWS del equipo). Subir el contenido de `dist/`.

## Editar precios/servicios

Todo está en `src/pages/index.astro`: el arreglo `servicios` (precios, textos, qué incluye)
y la constante `WHATSAPP` (número al que llegan los botones de contacto).
