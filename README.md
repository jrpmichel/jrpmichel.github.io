jorge-parra-michel-site
Sitio personal / científico de Jorge Ramón Parra Michel, Ph.D. — Ingeniero Mecánico e Investigador en Metrología Óptica (ESPI, luz estructurada 3D, DIC, deep learning informado por física).
Sitio estático de una sola página, bilingüe (ES/EN), sin dependencias de build (HTML + CSS + JS puro). Listo para GitHub Pages.
Estructura
```
index.html                  ← página completa (HTML + CSS + JS inline)
favicon.svg                 ← ícono de anillos de interferencia
.nojekyll                   ← evita que GitHub Pages procese el sitio con Jekyll
assets/
  img/
    jorge-parra-michel.jpg      ← foto principal (760px)
    jorge-parra-michel@2x.jpg   ← foto para pantallas retina (1140px)
  cv/
    Parra-Michel_CV.pdf         ← CV descargable desde el botón "Download CV"
```
Publicarlo en GitHub Pages (repo `jrpmichel.github.io`)
En GitHub, crea un repositorio nuevo llamado exactamente `jrpmichel.github.io` (público). Este nombre especial hace que GitHub Pages lo publique automáticamente en `https://jrpmichel.github.io`, sin configuración extra.
En tu computadora, dentro de esta carpeta (`site-project`), ejecuta:
```bash
   git init
   git add .
   git commit -m "Sitio personal inicial"
   git branch -M main
   git remote add origin https://github.com/jrpmichel/jrpmichel.github.io.git
   git push -u origin main
   ```
En GitHub → tu repo → Settings → Pages, confirma que la fuente sea la rama `main` (carpeta raíz `/`). Con el nombre especial del repo normalmente ya queda activo automáticamente.
Espera 1–2 minutos y abre https://jrpmichel.github.io — ese es tu sitio.
Para actualizarlo después
Edita `index.html` (o cambia la foto/CV en `assets/`), y vuelve a hacer:
```bash
git add .
git commit -m "Actualización de contenido"
git push
```
Los cambios se reflejan en 1–2 minutos.
Qué contiene el sitio
Hero con nombre, rol, resumen y enlaces directos a Google Scholar, ORCID, Web of Science y GitHub.
Sobre mí (objetivo + metas profesionales, tomado del CV).
Líneas de investigación: ESPI, luz estructurada 3D, DIC, deep learning informado por física, ingeniería inversa, diseño mecánico y FEA.
Experiencia profesional (línea de tiempo).
Formación académica (Ph.D., M.Sc., Ingeniería).
Distinciones y patentes (SNI, Beca Santander–FIMPES, 2 patentes).
Publicaciones seleccionadas con DOI enlazado (7 artículos del CV).
Habilidades y herramientas (MATLAB, Python, SolidWorks, ANSYS, LabVIEW, LaTeX, etc.) e idiomas.
Docencia actual.
Perfiles (tarjetas a Scholar / ORCID / WoS / GitHub).
Contacto (correos institucionales).
Selector de idioma (ES/EN, arriba a la derecha) y selector de tema claro/oscuro (además de seguir automáticamente el modo del sistema). Ambos se recuerdan entre visitas (`localStorage`).
Notas de privacidad
Deliberadamente no incluí tu teléfono ni tu domicilio (sí aparecían en el CV) porque este sitio será público e indexable por buscadores. Si de todas formas quieres mostrarlos, agrégalos tú mismo en la sección de contacto de `index.html`.
Personalización rápida
Foto: reemplaza los archivos en `assets/img/` (mismo nombre) por otra imagen, o cámbialos y actualiza las rutas `src`/`srcset` del `<img>` en el hero.
Colores: los tokens de color están al inicio del `<style>` (`--paper`, `--ink`, `--gold`, `--teal`, etc.), separados para tema claro y oscuro.
Nuevas publicaciones: copia un bloque `.pub-item` dentro de `#publications` y ajusta año, título, autores, revista y DOI.
Dominio propio: si más adelante quieres un dominio como `jorgeparramichel.com`, agrega un archivo `CNAME` en la raíz con ese dominio y configura el DNS según la documentación de GitHub Pages.
