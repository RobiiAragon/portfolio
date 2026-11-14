# Portafolio — Jesús Aragón

Portafolio interactivo con estilo de escritorio de macOS: carpetas que se arrastran, ventanas, dock, terminal funcional y una nube de puntos 3D al fondo.

**En vivo:** https://robiiaragon.github.io/portfolio/

## Editar contenido

Todo el contenido está al inicio del `<script>` en `index.html`:

- `ME`: nombre, usuario de GitHub, email y X.
- `PROJECTS`: cada proyecto es una carpeta del escritorio (`x`, `y` en % de pantalla). Usa `hero` para capturas reales o `art` (`mesh`, `grid`, `rings`, `bars`, `wave`, `nodes`) para una portada generada.
- `REPOS_FALLBACK`: repos que se muestran si la API de GitHub no responde. Normalmente la ventana **GitHub Repos** los carga en vivo.

Las imágenes van en `images/` y el CV en `resume.pdf`. Colores en las variables `:root` de `style.css`.

Inspirado en el portafolio de [Yaya Ehsan](https://itsyayaehsan.github.io/yayaehsansportfolio/).
