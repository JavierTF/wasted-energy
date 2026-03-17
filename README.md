# Energía Solar Excedente — Mapa de Proyecto

Mapa interactivo de proyecto para la gestión y usos del excedente de energía solar fotovoltaica (532 horas/año).

## Estructura

```
mindmap/
├── index.html          # Aplicación principal
├── data/
│   ├── es.json         # Árbol de datos en español
│   └── en.json         # Árbol de datos en inglés
└── solar_map_v2.html   # Versión anterior (referencia)
```

## Uso local

Requiere un servidor HTTP (no funciona con `file://`):

```bash
npx serve .
```

Abre http://localhost:3000

## Deploy

Desplegado en Vercel. Para actualizar:

```bash
vercel
```

## Añadir idiomas

1. Crear `data/xx.json` con la misma estructura que `es.json`
2. Añadir el botón en `index.html`:
   ```html
   <button class="lang-btn" data-lang="xx">XX</button>
   ```
3. Añadir las cadenas de UI en el objeto `I18N` dentro de `index.html`
