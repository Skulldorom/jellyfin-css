# Jellyfin CSS – purple theme that extends [Elegantfin](https://github.com/lscambo13/ElegantFin)

A custom CSS theme for [Jellyfin](https://jellyfin.org/) featuring a purple aesthetic.

## Usage

### Minified

Paste the following URL into **Dashboard → General → Custom CSS**:

```
@import url("https://cdn.jsdelivr.net/gh/Skulldorom/jellyfin-css@main/main.min.css")
```

> **Note:** jsDelivr caches files for a short period. If you don't see your changes immediately, append a version tag to the URL (e.g. `@v1.0.0`) or wait for the cache to expire.

## How it works

`main.css` imports the following files:

| File | Description |
|---|---|
| `media-cards.css` | Styles for media cards |
| `editors-choice-plugin.css` | Editors' Choice plugin styles |
| `video-player.css` | Video player overrides |
| `elegantfin.css` | Base elegantfin theme styles |
