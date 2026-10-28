# Portafolio Personal — Rainier Erey Peña Bolívar

Sitio personal estático (HTML/CSS/JS, sin dependencias ni build) con mi experiencia
profesional como Desarrollador Backend.

## Estructura

```
├── index.html              # Página principal (toda la estructura y contenido)
└── src/
    ├── styles.css          # Estilos (tema oscuro, responsive, animaciones)
    ├── script.js           # Menú móvil, scroll suave y animaciones de aparición
    └── assets/
        ├── carnet.png      # Foto de perfil (hero)
        └── Rainier_cv_2026.pdf  # CV descargable (colocar aquí el PDF)
```

> Nota: el botón "Descargar CV" apunta a `src/assets/Rainier_cv_2026.pdf`.
> Coloca el PDF del CV en esa carpeta para que el enlace funcione.

## Probar en local

No necesita servidor: abre `index.html` directamente en el navegador.
Opcionalmente, con Python:

```powershell
python -m http.server 8000
# http://localhost:8000
```

## Despliegue

### GitHub Pages (recomendado, este repo ya está en GitHub)

```powershell
git add .
git commit -m "Sitio personal"
git push origin main
```

Luego en GitHub: **Settings → Pages → Source: Deploy from a branch → main / (root) → Save**.
El sitio quedará en `https://<tu-usuario>.github.io/mysite/`.

### Netlify

Arrastra la carpeta a [app.netlify.com/drop](https://app.netlify.com/drop), o conecta el
repo. No requiere comando de build; el directorio de publicación es la raíz (`/`).

### Vercel

```powershell
npx vercel
```

Detecta el sitio estático automáticamente (sin build ni framework).

## Personalización

- **Colores**: variables CSS en `:root` de `src/styles.css` (`--accent`, `--bg`, etc.).
- **Contenido**: edita directamente las secciones en `index.html`.
