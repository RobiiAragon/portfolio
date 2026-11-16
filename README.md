# Portfolio — Jesús Aragón

**Live:** https://robiiaragon.github.io/portfolio/ · **Resume:** [resume.pdf](https://robiiaragon.github.io/portfolio/resume.pdf)

An interactive portfolio styled as a macOS desktop: draggable project folders, windows, a dock, a working terminal with `fastfetch`, and a 3D point cloud in the background. It is a single static page with no framework and no build step, hosted on GitHub Pages.

**English** · [Español](#español)

## Features

- **Desktop metaphor:** every project is a folder on the desktop that opens in its own window, with screenshots or a generated cover.
- **Working terminal:** type commands to explore the profile, in the style of a macOS terminal.
- **Live GitHub data:** the **GitHub Repos** window loads public repositories from the GitHub API, with a built-in fallback list if the API does not answer.
- **Canvas background:** a 3D point cloud drawn on `<canvas>`.
- **Lightweight:** plain HTML, CSS and JavaScript (`index.html`, `style.css`).

## Editing the content

All the content is at the top of the `<script>` in `index.html`:

- `ME`: name, GitHub username, email and X.
- `PROJECTS`: each project is a desktop folder (`x`, `y` in % of the screen). Use `hero` for real screenshots or `art` (`mesh`, `grid`, `rings`, `bars`, `wave`, `nodes`) for a generated cover.
- `REPOS_FALLBACK`: repositories shown if the GitHub API does not answer.

Images go in `images/` and the resume in `resume.pdf`. Colors are the `:root` variables in `style.css`.

## Run locally

```sh
git clone https://github.com/RobiiAragon/portfolio.git
cd portfolio
python3 -m http.server 8000   # then open http://localhost:8000
```

---

## Español

Portafolio interactivo con estilo de escritorio de macOS: carpetas que se arrastran, ventanas, dock, terminal funcional con `fastfetch` y una nube de puntos 3D al fondo. Es una sola página estática, sin framework ni compilación, publicada en GitHub Pages.

### Editar contenido

Todo el contenido está al inicio del `<script>` en `index.html`:

- `ME`: nombre, usuario de GitHub, email y X.
- `PROJECTS`: cada proyecto es una carpeta del escritorio (`x`, `y` en % de pantalla). Usa `hero` para capturas reales o `art` (`mesh`, `grid`, `rings`, `bars`, `wave`, `nodes`) para una portada generada.
- `REPOS_FALLBACK`: repos que se muestran si la API de GitHub no responde. Normalmente la ventana **GitHub Repos** los carga en vivo.

Las imágenes van en `images/` y el CV en `resume.pdf`. Colores en las variables `:root` de `style.css`.

---

Inspired by [Yaya Ehsan's portfolio](https://itsyayaehsan.github.io/yayaehsansportfolio/) · Made by **[Jesús Aragón](https://github.com/RobiiAragon)**
