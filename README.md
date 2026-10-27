# static_studio website

Landing page for Static Studio, built with Hugo.

```sh
hugo server   # http://localhost:1313
hugo          # build into ./public
```

- Hero copy: `content/_index.md` (frontmatter — editable in Static Studio itself)
- Links, license, download URLs: `[params]` in `hugo.toml` (all `[...]` values are placeholders)
- Page layout: `layouts/index.html`, header/footer in `layouts/partials/`
- Styles: `static/css/main.css` (accent color = `--accent`)
