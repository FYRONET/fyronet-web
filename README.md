# Fyronet — Guía de la Web

## ¿Cómo actualizar imágenes sin tocar el código?

Todas las imágenes de la web se cargan desde **Supabase Storage**.
Para actualizar cualquier imagen solo tenés que subir el archivo con el nombre correcto al bucket `Images` en Supabase y aparece sola en la web automáticamente.

**Formatos aceptados:** `.jpg` o `.png` (el código prueba los dos)
**Bucket:** `Images` (con I mayúscula)
**URL base:** `https://kogutxfhfluvdcvmoagn.supabase.co/storage/v1/object/public/Images/`

---

## Logos

| Nombre del archivo | Dónde aparece | Dimensiones recomendadas | Formato |
|---|---|---|---|
| `logo_icon` | Nav (arriba izquierda) + Favicon pestaña | 200x200px | `.png` fondo transparente |
| `logo_completo` | Footer (abajo, versión blanca) | 400x80px | `.png` fondo transparente |

> **Importante:** Los logos necesitan fondo transparente para verse bien sobre los fondos de la web.

---

## Portfolio

| Nombre del archivo | Dónde aparece | Dimensiones recomendadas | Notas |
|---|---|---|---|
| `portfolio_01` | Card 1 (primera posición) | 800x450px | Captura o imagen del cliente |
| `portfolio_02` | Card 2 (segunda posición) | 800x450px | Captura o imagen del cliente |
| `portfolio_03` | Card 3 (tercera posición) | 800x450px | Captura o imagen del cliente |
| `portfolio_04` | Card 4 (cuarta posición) | 800x450px | Captura o imagen del cliente |

> **Tip:** Usá capturas de pantalla del sitio web del cliente en formato 16:9. Podés usar `.jpg` para menor peso.

---

## Equipo

| Nombre del archivo | Dónde aparece | Dimensiones recomendadas | Notas |
|---|---|---|---|
| `equipo_01` | Foto de Brian (fundador) | 400x400px | Foto de perfil cuadrada |
| `equipo_02` | Foto diseñador web | 400x400px | Foto de perfil cuadrada |
| `equipo_03` | Foto community manager | 400x400px | Foto de perfil cuadrada |

> **Tip:** Las fotos de equipo se muestran en círculo, así que lo más importante tiene que estar centrado. Evitá fondos muy cargados.

---

## Pasos para subir una imagen

1. Entrá a [supabase.com](https://supabase.com) con tu cuenta
2. Abrí tu proyecto **Fyronet**
3. En el menú izquierdo hacé clic en **Storage**
4. Entrá al bucket **Images**
5. Hacé clic en **Upload files**
6. Subí el archivo con el nombre exacto de la tabla (ej: `portfolio_01.jpg`)
7. Listo — en segundos aparece en la web sin tocar código

---

## Recomendaciones generales

- **Peso máximo por imagen:** 500kb (para que la web cargue rápido)
- **Optimizar imágenes antes de subir:** usá [squoosh.app](https://squoosh.app) (gratis)
- **Portfolio:** siempre en formato apaisado (horizontal), ratio 16:9
- **Equipo:** siempre cuadradas o con el rostro bien centrado
- **Logos:** siempre con fondo transparente en `.png`
- Si subís una imagen nueva con el mismo nombre, **reemplaza la anterior automáticamente**

---

## Estructura del proyecto en GitHub

```
fyronet-web/
├── index.html        ← Toda la web en un solo archivo
└── README.md         ← Esta guía
```

> Las imágenes **no** van en GitHub, van en Supabase.

---

## Datos de contacto configurados en la web

| Campo | Valor |
|---|---|
| WhatsApp | +54 11 6359-6107 |
| Email | info@fyronet.com |
| Ubicación | Buenos Aires, Argentina |
| Formulario | Google Apps Script (llega a info@fyronet.com) |

---

## ¿Cuándo sí hay que tocar el código?

- Cambiar textos, precios o descripciones
- Agregar o quitar secciones
- Cambiar colores o tipografía
- Agregar un nuevo miembro al equipo
- Agregar una nueva card al portfolio

Para cualquiera de estos cambios, editar el archivo `index.html` y subir a GitHub.
