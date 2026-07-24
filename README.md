# Carrera Docente — SLEP Petorca · Visores

Sitio estático con los visores HTML del equipo (versiones **anonimizadas**).
Cada archivo `.html` es autónomo; `index.html` es la página de inicio que los lista.

## Publicar en GitHub Pages (gratis)

1. Crea un repositorio en GitHub (ej. `visores-carrera-docente`). Puede ser
   público; recuerda que estos HTML ya están anonimizados.
2. Sube estos archivos (`index.html`, `visor-tramos.html`, este README).
   Puedes arrastrarlos en *Add file → Upload files*.
3. Ve a **Settings → Pages**, en *Source* elige la rama `main` y carpeta `/root`,
   y guarda.
4. En un par de minutos tu sitio queda en:
   `https://TU-USUARIO.github.io/visores-carrera-docente/`
   - Página de inicio: esa URL.
   - Visor de tramos: `.../visor-tramos.html`

> Si prefieres un subdominio propio (ej. `tramos.slep-petorca.cl`), se configura
> en Settings → Pages → *Custom domain* apuntando un registro DNS; opcional.

## Agregar otros visores

Solo copia el nuevo `.html` a este repositorio y agrega una tarjeta en
`index.html` (duplica el bloque `<a class="card">` y cambia título, texto y
`href`). El de "Próximamente" está listo para reemplazar.

## Actualización mensual del Visor de Tramos

El visor lleva los datos **incrustados** en el propio HTML, así que actualizarlo
es reemplazar el archivo:

1. Deja el nuevo Excel del mes en la carpeta de OneDrive de Carrera Docente
   (como haces hoy con los "Listado Asignaciones CD ... (para comparar)").
2. Pídele a Claude que regenere el visor con el mes nuevo (extiende la serie).
3. Reemplaza `visor-tramos.html` en el repositorio (*Upload files* sobre el
   mismo nombre → *Commit*). GitHub Pages se actualiza solo en un par de minutos.

Nada de los datos con RUT/nombre reales llega al repositorio: el visor publicado
usa códigos `DOC-####`.
