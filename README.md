# Aurum Minerals — Web

Sitio estático de una sola página para Aurum Minerals.

## Estructura

```
index.html      Home (HTML + CSS + JS embebidos)
submit.html     Postulación de proyectos — wizard con filtros y scoring
investors.html  Inversionistas — wizard con gate de ticket mínimo
assets/         Imágenes, logos de aliados y videos de fondo
```

## Formularios

Ambos wizards envían a FormSubmit (sin cuenta ni API key). El destino se
define en la constante `FORM_ENDPOINT` al inicio del `<script>` de cada
página. Para cambiar de correo basta editar esa línea.

El primer envío a un destino nuevo dispara un correo de activación que
hay que abrir una sola vez; hasta entonces los envíos no se entregan.

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
