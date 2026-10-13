# Brian's Notes

Blog personal de Brian sobre tecnología, ideas y aprendizaje. Hecho con [Jekyll](https://jekyllrb.com/) y publicado con GitHub Pages.

## Publicar una nota nueva

1. Crea un archivo en `_posts/` con el formato `AAAA-MM-DD-titulo.md`
2. Al inicio del archivo pon:

```yaml
---
title: "Título de la nota"
subtitle: "Subtítulo opcional"
date: AAAA-MM-DD
---
```

3. Escribe el contenido en Markdown y haz commit. GitHub Pages lo publica solo.

## Ver el sitio en local

```bash
bundle exec jekyll serve
```
