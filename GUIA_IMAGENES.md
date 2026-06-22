# Guía de Imágenes — Web Sumilor

## Estructura de carpetas que debes crear

```
Web-Sumilor/
├── img/
│   ├── logo.png              ← Tu logotipo principal
│   ├── hero-bg.jpg           ← (Opcional) Imagen de fondo para el Hero
│   └── productos/
│       ├── prod-01.jpg
│       ├── prod-02.jpg
│       ├── ...
│       └── prod-26.jpg
└── video/
    └── piscinas-sumilor.mp4  ← Vídeo de piscinas
```

---

## 1. Logotipo

| Archivo original | Nuevo nombre | Carpeta destino |
|------------------|-------------|-----------------|
| `Sumilor.jpg` | `logo.png` | `img/` |

> **Acción**: Convierte `Sumilor.jpg` a PNG con fondo transparente (si es posible) y guárdalo como `img/logo.png`. Si no puedes quitar el fondo, úsalo tal cual como `img/logo.png`.

---

## 2. Imagen de fondo Hero (OPCIONAL)

Si quieres usar una imagen de fondo en lugar de un degradado en la sección Hero, elige una imagen representativa de la tienda o fachada y guárdala como:

| Nuevo nombre | Carpeta destino |
|-------------|-----------------|
| `hero-bg.jpg` | `img/` |

> Si no añades esta imagen, el Hero usará un degradado con los colores corporativos que también queda muy profesional.

---

## 3. Imágenes de producto (estilo RRSS)

Renombra las imágenes de la carpeta `swisstransfer_8939d753-e7d8-4da7-b7da-3d35d51b24f4` según esta tabla. **Recomendación**: convierte los PNG a JPG (calidad 85%) para que la web cargue más rápido. Si no puedes convertir, la web funciona igual con PNG.

| # | Archivo original | Nuevo nombre | Carpeta destino |
|---|-----------------|-------------|-----------------|
| 1 | `creas-03.png` | `prod-01.jpg` | `img/productos/` |
| 2 | `creas-04.png` | `prod-02.jpg` | `img/productos/` |
| 3 | `creas-05.png` | `prod-03.jpg` | `img/productos/` |
| 4 | `creas-09.png` | `prod-04.jpg` | `img/productos/` |
| 5 | `creas-10.png` | `prod-05.jpg` | `img/productos/` |
| 6 | `creas-12.png` | `prod-06.jpg` | `img/productos/` |
| 7 | `creas-13.png` | `prod-07.jpg` | `img/productos/` |
| 8 | `creas-14.png` | `prod-08.jpg` | `img/productos/` |
| 9 | `creas-15.png` | `prod-09.jpg` | `img/productos/` |
| 10 | `creas-16.png` | `prod-10.jpg` | `img/productos/` |
| 11 | `creas_floculante-19.png` | `prod-11.jpg` | `img/productos/` |
| 12 | `creas junio_Mesa de trabajo 1.png` | `prod-12.jpg` | `img/productos/` |
| 13 | `creas junio-02.png` | `prod-13.jpg` | `img/productos/` |
| 14 | `creas julio_julio-11.png` | `prod-14.jpg` | `img/productos/` |
| 15 | `creas julio_julio-12.png` | `prod-15.jpg` | `img/productos/` |
| 16 | `creas julio_julio-10.png` | `prod-16.jpg` | `img/productos/` |
| 17 | `creas agosto_julio-11.png` | `prod-17.jpg` | `img/productos/` |
| 18 | `creas agosto_Mesa de trabajo 1.png` | `prod-18.jpg` | `img/productos/` |
| 19 | `creas agosto-06.png` | `prod-19.jpg` | `img/productos/` |
| 20 | `creas agosto_julio-10.png` | `prod-20.jpg` | `img/productos/` |
| 21 | `creas junio_26-09.png` | `prod-21.jpg` | `img/productos/` |
| 22 | `creas junio_26-13.png` | `prod-22.jpg` | `img/productos/` |
| 23 | `creas mayo_11.5-07.png` | `prod-23.jpg` | `img/productos/` |
| 24 | `creas mayo_26-08.png` | `prod-24.jpg` | `img/productos/` |
| 25 | `creas mayo_26-09.png` | `prod-25.jpg` | `img/productos/` |
| 26 | `creas mayo_26-12.png` | `prod-26.jpg` | `img/productos/` |

---

## 4. Vídeo de piscinas

| Archivo original | Nuevo nombre | Carpeta destino |
|-----------------|-------------|-----------------|
| `piscinas_sumilor1.mp4` | `piscinas-sumilor.mp4` | `video/` |

---

## Resumen rápido de acciones

```bash
# 1. Crear carpetas
mkdir img
mkdir img\productos
mkdir video

# 2. Copiar y renombrar logo
copy Sumilor.jpg img\logo.png

# 3. Copiar y renombrar imágenes de producto (una por cada línea de la tabla)
copy "swisstransfer_8939d753-e7d8-4da7-b7da-3d35d51b24f4\creas-03.png" "img\productos\prod-01.jpg"
# ... repetir para las 26 imágenes según la tabla

# 4. Copiar vídeo
copy "swisstransfer_8939d753-e7d8-4da7-b7da-3d35d51b24f4\piscinas_sumilor1.mp4" "video\piscinas-sumilor.mp4"
```

---

## Notas importantes

- **Formatos**: La web espera `.jpg` para productos y `.png` para el logo. Si tus imágenes se llaman `.png` en lugar de `.jpg`, edita `index.html` y cambia las rutas (busca `prod-` y cambia `.jpg` por `.png`).
- **Tamaños**: Las imágenes originales son de 1080×1350 o 2250×2813 píxeles — bastante grandes para web. Te recomiendo redimensionarlas a un máximo de 800px de ancho para que la página cargue rápido en móviles.
- **Optimización online**: Puedes usar [TinyPNG](https://tinypng.com/) o [Squoosh](https://squoosh.app/) para comprimir las imágenes sin perder calidad.
- **Logo**: La imagen `Sumilor.jpg` es de 1692×1696 px. Rediménsionala a unos 300×300 px para el logo de la web.

Una vez tengas todas las imágenes en su sitio, abre `index.html` en tu navegador y la web debería verse completa.
