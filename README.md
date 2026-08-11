# Cero Digital — Landing page

Landing page de conversión para **Cero Fideliza**, el primer producto de Cero Digital.

## Antes de publicar

Edita `index.html` y busca la línea cerca del final del archivo:

```js
const WHATSAPP_NUMBER = "51900000000"; // reemplaza por tu número real
```

Cambia `51900000000` por tu número de WhatsApp real (código de país + número, sin espacios ni `+`). Todos los botones de la página ("Quiero fidelizar a mis clientes", "Quiero empezar con Start", etc.) apuntan automáticamente a ese número con un mensaje precargado.

### Logo de Cero Grados (sección "Caso Cero")

La sección Caso Cero busca cargar un archivo llamado `cero-grados-logo.png` en la misma carpeta que `index.html`. Si no lo encuentra, muestra automáticamente un placeholder con las iniciales "CG" — así que la página nunca se rompe, pero para verse completa solo tienes que:

1. Guardar el logotipo real de Cero Grados como `cero-grados-logo.png` en esta carpeta.
2. Subirlo al repositorio junto con `index.html`.

También puedes reemplazar:
- `S/ XX` y `S/ XX.XX` en la sección de precios (`#planes`) por tus montos reales.
- El enlace de Instagram (actualmente `href="#"` en el footer).
- El correo de contacto (`hola@cerodigital.pe`).

## Cómo subirlo a GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `cero-digital`).
2. Sube este archivo `index.html` (y este `README.md`) a la raíz del repositorio.
3. Ve a **Settings → Pages**.
4. En "Source", selecciona la rama `main` y la carpeta `/ (root)`.
5. Guarda. En un par de minutos tu web estará disponible en:
   `https://tu-usuario.github.io/cero-digital`

## Estructura

Es un único archivo `index.html` autocontenido (HTML + CSS + JS), sin dependencias de build — solo importa las fuentes de Google Fonts. No necesitas Node, npm ni ningún paso de compilación.
