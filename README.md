# Jellyfin CSS – Skullflix Theme

A custom CSS theme for [Jellyfin](https://jellyfin.org/) featuring a purple Skullflix aesthetic.

## Usage

### Option 1 – Minified (recommended)

Paste the following URL into **Dashboard → General → Custom CSS**:

```
https://cdn.jsdelivr.net/gh/Skulldorom/jellyfin-css@main/main.min.css
```

### Option 2 – Unminified (latest source)

```
https://cdn.jsdelivr.net/gh/Skulldorom/jellyfin-css@main/main.css
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

On every push to `main`, a GitHub Actions workflow automatically minifies `main.css` (with all `@import`s inlined) and commits the result as `main.min.css`.
