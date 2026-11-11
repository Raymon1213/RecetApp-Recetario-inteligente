# RecetApp – Recetario inteligente

Prototipo funcional (Metodología de Desarrollo de Software, PUCV 2026-02). Sitio estático sin dependencias: HTML + CSS + JavaScript.

## Funcionalidades
Registro/inicio de sesión simulado, inventario de ingredientes, filtros (receta objetivo, utensilios, tiempo, tipo de comida, dieta), tarjetas con coincidencia de inventario, detalle de receta, recetas guardadas, **planificador de meal prep semanal** y **lista de compras consolidada**.

## Ejecutar localmente
Abrir `index.html` en el navegador (o `python3 -m http.server` y visitar http://localhost:8000).

## Publicar en GitHub Pages
1. Crear un repositorio en GitHub y subir este proyecto (`git remote add origin <url>` y `git push -u origin main`).
2. En *Settings → Pages*, elegir *Source: GitHub Actions*. El workflow `.github/workflows/pages.yml` publica en cada push a `main`.

## Estructura
- `index.html` – pantallas · `css/styles.css` – estilos
- `js/data.js` – catálogo de recetas (editar aquí para agregar recetas)
- `js/app.js` – lógica: filtrado, inventario, meal prep, compras

## Limitaciones
Los datos del usuario se guardan en el navegador (localStorage). Backend (Express), PostgreSQL y autenticación con hash/salt son la siguiente etapa.
