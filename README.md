# Jellyfin CSS – Skullflix purple theme

A custom CSS theme for Jellyfin featuring a purple aesthetic. The current theme supports Jellyfin 12 while retaining legacy variables used by ElegantFin and optional plugins.

## Usage

### Minified

Paste the following into **Dashboard → General → Custom CSS**:

```css
@import url("https://cdn.jsdelivr.net/gh/Skulldorom/jellyfin-css@main/main.min.css");
```

> **Note:** jsDelivr caches files for a short period. For predictable production updates, use a tagged release such as `@v2.0.0` instead of `@main`.

## Compatibility

- Jellyfin 12: supported, including the React/MUI header and `--jf-*` theme tokens.
- Legacy Jellyfin/plugin markup: retained where practical through compatibility variables and selectors.
- Jellyfin Featured and Pause Screen rules only apply when their respective plugins inject the expected markup.

Do not target generated MUI classes such as `.css-iqm7ky`; those class names may change between Jellyfin builds.

## How it works

`main.css` imports the following files:

| File | Description |
|---|---|
| `media-cards.css` | Media cards and collection-folder styling |
| `jellyfin-featured.css` | Optional Jellyfin Featured styling |
| `video-player.css` | Legacy and current video-player overrides |
| `elegantfin.css` | Legacy ElegantFin-compatible layout variables |
| `pausescreen.css` | Optional Pause Screen plugin styling |

