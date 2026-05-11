# 135 años de Rerum Novarum — Solidaridad UC

Web conmemorativa con 5 figuras del catolicismo social, manifiesto
descargable y enlace a Instagram, lista para publicar gratis en GitHub Pages
y enlazar desde un código QR en el poster.

---

## 📁 Estructura del proyecto

```
rerum-novarum-web/
├── index.html        ← La página completa (autocontenida)
├── img/              ← Retratos de los 5 personajes (PNG)
│   ├── abdon-cifuentes.png
│   ├── alberto-hurtado.png
│   ├── dorothy-day.png
│   ├── bernardo-leighton.png
│   └── mario-gongora.png
├── pdfs/             ← PDF descargable
│   └── somos-solidarios.pdf        ← Manifiesto del movimiento
└── README.md         ← Este archivo
```

**Ya viene listo:** las 5 imágenes de los personajes, el logo de Solidaridad UC
con fondo transparente y el PDF del manifiesto. No se incluyen PDFs individuales
por persona.

---

## 🎨 Paleta aplicada

La web ya está configurada con la paleta institucional de Solidaridad UC:

| Variable CSS | Color | Uso |
|--------------|-------|-----|
| `--bg-deep` | `#0C476F` | Fondo principal (azul institucional) |
| `--bg-darker` | `#083550` | Modales, tarjetas |
| `--red-primary` | `#E8262D` | Acentos, botones, títulos |
| `--cream` | `#EEEAD0` | Fondo de retratos y texto principal |

Si quieres modificar colores, están en las primeras líneas del CSS de
`index.html`, dentro del bloque `:root`.

---

## ✅ Antes de publicar: 2 cosas que verificar

### 1. El handle de Instagram
La web está configurada con `@solidaridaduc` (que coincide con tu logo de
marca). Si el handle real es distinto, busca y reemplaza en `index.html`:
- `https://www.instagram.com/solidaridaduc/`
- `@solidaridaduc`

### 2. El manifiesto
La página incluye solo el PDF del manifiesto `somos-solidarios.pdf`. Los perfiles
de cada figura se leen directamente en la web, dentro de una ventana emergente.

---

## 🚀 Cómo publicar en GitHub Pages (gratis, ~10 minutos)

### Paso 1 — Crear cuenta en GitHub
Si no tienes, ve a [github.com](https://github.com) y crea una cuenta.
Recomendación: cuenta institucional `solidaridaduc` si es para uso permanente.

### Paso 2 — Crear un repositorio nuevo
1. Click en el botón verde "New" (o en el "+" arriba a la derecha).
2. Nombre del repositorio: `rerum-novarum` (o el que prefieras).
3. Marca "Public".
4. No marques "Add README" (ya tenemos uno).
5. Click "Create repository".

### Paso 3 — Subir los archivos
En la página del repo vacío, click en "uploading an existing file".
Arrastra a esa ventana:
- `index.html`
- la carpeta `img/` completa
- la carpeta `pdfs/` completa (solo con `somos-solidarios.pdf`)
- `README.md`

Abajo, en "Commit changes", escribe "primera versión" y click en el botón verde.

### Paso 4 — Activar GitHub Pages
1. En la página del repo, click en "Settings" (arriba a la derecha).
2. En el menú lateral, busca "Pages".
3. En "Source", elige "Deploy from a branch".
4. En "Branch", elige `main` y carpeta `/ (root)`. Click "Save".
5. Espera ~1 minuto. Recarga la página. Aparecerá una URL como:
   `https://solidaridaduc.github.io/rerum-novarum/`

¡Esa es la URL del QR! Cópiala.

---

## 📱 Generar el QR

Una vez tengas la URL pública, genera el QR con:

- **[qr-code-generator.com](https://www.qr-code-generator.com/)** — descarga
  PNG/SVG sin marca de agua.
- **[qrcode-monkey.com](https://www.qrcode-monkey.com/)** — permite
  personalizar colores (usa el rojo institucional `#E8262D` sobre blanco) y
  agregar el logo de Solidaridad en el centro del QR.

**Recomendación:** descarga en **SVG** o **PNG ≥1000x1000 px** para imprenta
nítida. Mantén alto contraste para que el QR siga escaneable.

---

## 🔄 Cómo actualizar después

1. Ve a tu repo en GitHub.
2. Click sobre el archivo a editar (ej. `index.html`).
3. Click en el ícono de lápiz "Edit this file".
4. Edita, scroll abajo, "Commit changes".
5. La web se actualiza sola en ~1 minuto. **El QR sigue funcionando** porque
   la URL no cambia.

---

## 💡 Si algo no funciona

- **Las imágenes no aparecen:** verifica que los nombres en `img/` coincidan
  exactamente con los del HTML (atención a tildes, mayúsculas, guiones).
- **El PDF no se descarga:** mismo chequeo en `pdfs/`.
- **Local funciona pero GitHub Pages no:** los nombres de archivo son
  case-sensitive en GitHub. `Abdon.png` ≠ `abdon.png`.
- **El QR no escanea:** prueba la URL en tu celular antes de imprimir.

---

## 📞 Créditos

Web creada para la conmemoración de los 135 años de la encíclica
*Rerum Novarum* (1891) — Solidaridad UC, 2026.

Retratos: ilustraciones originales en estilo grabado.
Manifiesto: *Somos solidarios*, escrito por miembros del movimiento.
