# Hugolify Lab

Prototipo del framework [Hugolify](https://www.hugolify.io/) como experimento del laboratorio de pabloib.

**Objetivo:** Evaluar Hugolify como base para sitios de clientes (migraciones WP → Hugo).

**URL:** https://hugolify.lab.pabloib.com/
**CMS:** Sveltia en `/admin/`
**ADR:** [ADR-007](https://github.com/pabloalgo/pabloib/blob/main/docs/decisions/ADR-007-COMPONENT-LIBRARY.md)
**Fork:** [pabloalgo/hugolify-theme](https://github.com/pabloalgo/hugolify-theme)

## Setup

```bash
npm install
hugo mod get
hugo server -D
```

## Estructura

- `config/_default/` — Config Hugo (YAML)
- `content/pages/` — Páginas con bloques (core theme)
- `content/posts/` — Blog (hugolify-theme-posts)
- `content/persons/` — Autores (hugolify-theme-persons)

## Modules

- `hugolify-theme/v2` — Core layouts + blocks engine
- `hugolify-theme-bootstrap` — Bootstrap 5 styling layer
- `hugolify-admin` — CMS config generator (Sveltia/Decap/etc)
- `hugolify-theme-posts` — Blog posts content type
- `hugolify-theme-posts-categories` — Post categories taxonomy
- `hugolify-theme-posts-authors` — Post authors taxonomy
- `hugolify-theme-persons` — Person profiles
