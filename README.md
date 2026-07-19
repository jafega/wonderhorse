# 🐴 Wonderhorse — Tienda Shopify

Tema de Shopify para **Wonderhorse**, la marca de equipación equina con personalidad:
**hippie, moderna y con alma del salvaje oeste**. Menos serio, más caballo.

Está basado en [Dawn](https://github.com/Shopify/dawn) (el tema oficial de Shopify,
Online Store 2.0) y personalizado de arriba a abajo con la identidad Wonderhorse.

---

## 🎨 Identidad de marca

**Paleta de color** (definida en `config/settings_data.json` → `color_schemes`):

| Uso | Color | Hex |
|-----|-------|-----|
| Crema base | Fondo principal | `#F7EFDD` |
| Marrón cuero | Texto / tinta | `#33261B` |
| Terracota | Acento y botones | `#B7502F` |
| Verde salvia | Naturaleza | `#5E6B41` |
| Azul cielo | Guiño a los patitos 🦆 | `#A9D2DE` |
| Mostaza | La estrella de la espuela del logo | `#E3A93C` |

**Tipografías:** titulares en *Poppins* (redonda y amable, en sintonía con el logo),
cuerpo en *Assistant*. Esquinas redondeadas en botones, tarjetas e imágenes para
un aire moderno y artesanal.

**Toques de personalidad:** ver `assets/wonderhorse.css` (hover con "salto" en botones
y tarjetas, badges tipo pegatina, captions con sello artesanal).

---

## 🗂️ Estructura del tema

```
config/settings_data.json     → paleta, tipografías, bordes y copy de marca
templates/index.json          → la home (hero, manifiesto, sudaderos, valores, naturaleza, newsletter)
sections/header-group.json    → barra de anuncios + cabecera
sections/footer-group.json    → pie de página
assets/wonderhorse.css        → CSS extra de personalidad
```

La **home** ya trae 6 secciones montadas:
1. **Hero** — "Tu caballo también quiere destacar"
2. **Manifiesto** — "Nacimos hartos de lo aburrido"
3. **Sudaderos** — colección destacada
4. **Valores** — por qué Wonderhorse (3 columnas)
5. **Naturaleza** — "Del campo a la pista"
6. **Newsletter** — "Únete a la manada"

---

## 🚀 Cómo conectar este repo con Shopify

Este tema vive en GitHub y se conecta a Shopify sin necesidad de hosting aparte.

1. Entra en tu **Shopify Admin** → **Tienda online** → **Temas**.
2. Pulsa **Añadir tema** → **Conectar desde GitHub**.
3. Autoriza tu cuenta de GitHub y elige el repositorio **`wonderhorse`** y la rama **`main`**.
4. Shopify importará el tema. Verás "Wonderhorse" en tu lista de temas.
5. Pulsa **Personalizar** para abrir el editor visual (todo lo de arriba ya sale montado).

> A partir de ahí, cada cambio que se suba a GitHub (rama `main`) se sincroniza con el
> tema conectado, y los cambios que hagas en el editor de Shopify se pueden guardar de vuelta.

---

## 📸 Qué tienes que subir tú (2 minutos en Shopify)

Estas cosas **no van en el código**, se suben desde el editor de Shopify:

- **Logo:** Personalizar → **Encabezado** → *Logo* → sube el círculo de la bota Wonderhorse.
- **Foto del hero:** Personalizar → sección **Hero** → *Imagen* → una foto de caballo + naturaleza
  (como la del bosque que enviaste queda genial).
- **Foto "Del campo a la pista":** sección **Naturaleza** → *Imagen*.
- **Productos (sudaderos):** Admin → **Productos** → añade cada sudadero con sus fotos
  (el de patitos 🦆 y el western). Luego crea una **colección** llamada `Sudaderos` y, en la
  sección **Sudaderos** de la home, selecciónala.
- **Página "Nuestra historia":** Admin → **Tienda online** → **Páginas** → crea una con
  el *handle* `nuestra-historia` (los botones de la home ya apuntan ahí).

---

## 🛠️ Desarrollo local (opcional)

Si quieres previsualizar cambios en local necesitas la [Shopify CLI](https://shopify.dev/docs/themes/tools/cli):

```bash
npm install -g @shopify/cli @shopify/theme
shopify theme dev --store tu-tienda.myshopify.com
```

---

Basado en Dawn (MIT © Shopify). Personalización de marca © Wonderhorse.
