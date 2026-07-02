# Agents Reference for Ultrachromic Jellyfin Theme

## Purpose
This repository contains a Jellyfin custom theme implemented as modular CSS files. The included `ultrachromic_all_in_one.css` file consolidates the theme source into one single file for AI analysis and reference.

## Included CSS modules
The consolidated file includes the following source files:

- `WIP.css`
- `accentlist.css`
- `base.css`
- `bottombarprogress.css`
- `cornerindicator/indicator_corner.css`
- `cornerindicator/indicator_floating.css`
- `effects/glassy.css`
- `effects/hoverglow.css`
- `effects/pan-animation.css`
- `episodelist/episodes_compactlist.css`
- `episodelist/episodes_grid.css`
- `fields/fields_border.css`
- `fields/fields_noborder.css`
- `fixes.css`
- `header/header_transparent-dashboard.css`
- `header/header_transparent.css`
- `jf_font.css`
- `login/login_frame.css`
- `login/login_minimalistic.css`
- `overlayprogress.css`
- `presets/kaleidochromic_preset.css`
- `presets/monochromic_preset.css`
- `presets/novachromic_preset.css`
- `progress/floating.css`
- `rounding.css`
- `rounding_circlehover.css`
- `saved.css`
- `smallercast.css`
- `titlepage/title_banner-logo.css`
- `titlepage/title_banner.css`
- `titlepage/title_simple-logo.css`
- `titlepage/title_simple.css`
- `type/colorful.css`
- `type/dark.css`
- `type/dark_withaccent.css`
- `type/light.css`

## How to use this file
1. Use `ultrachromic_all_in_one.css` as a reference source for AI analysis or model training.
2. Do not assume every section should be active together: many modules are alternate styling options.
3. For actual Jellyfin deployment, pick the desired variations and use the original modular file imports or manually copy only the active sections.

## Notes for AI agents
- The theme is built as a composable CSS system. Alternate options appear for:
  - rounding style (`rounding.css` / `rounding_circlehover.css`)
  - episode list layout (`episodelist/episodes_compactlist.css` / `episodelist/episodes_grid.css`)
  - field styling (`fields/fields_border.css` / `fields/fields_noborder.css`)
  - watch indicator style (`cornerindicator/indicator_corner.css` / `cornerindicator/indicator_floating.css`)
  - login style (`login/login_frame.css` / `login/login_minimalistic.css`)
  - title page style (`titlepage/title_simple.css`, `titlepage/title_simple-logo.css`, `titlepage/title_banner.css`, `titlepage/title_banner-logo.css`)
  - theme type (`type/dark.css`, `type/dark_withaccent.css`, `type/light.css`, `type/colorful.css`)
- `presets/*.css` are convenience combinations and may reference many of the individual files.
- `saved.css` contains legacy saved import references, not active theme source.

## Recommended custom CSS order
For a live Jellyfin installation, the repository README suggests loading:

1. `fixes.css`
2. `jf_font.css`
3. `base.css`
4. `accentlist.css`
5. one rounding style
6. optional modules (`smallercast.css`, episode list, header, login, fields, corner indicator, overlay progress, effects)
7. one type style

## File structure summary
- Root CSS files: theme base, fixes, accent colors, fonts, global modules
- `effects/`: visual effect modules
- `fields/`: input field styling variants
- `cornerindicator/`: watched/unwatched indicator variants
- `episodelist/`: episode list layout variants
- `header/`: header/transparency variants
- `login/`: login page styling variants
- `titlepage/`: title page styling variants
- `type/`: main theme palette variants
- `presets/`: full preset combinations using imports
