# Aurum Minerals — Web

Sitio estático de una sola página para Aurum Minerals.

## Estructura

```
index.html      Página completa (HTML + CSS + JS embebidos)
assets/         Imágenes, logos y aliados
```

No hay build ni dependencias: se sirve tal cual.

## Desarrollo local

Abrir `index.html` en el navegador, o levantar un servidor estático:

```bash
python3 -m http.server 8000
```

## Despliegue

Vercel, preset **Other**, sin build command y con el directorio raíz como output.

## Dependencias externas (CDN)

- Google Fonts — Work Sans
- Leaflet 1.9.4 — mapa de proyectos
- api.gold-api.com — precios de oro, plata y cobre en vivo
