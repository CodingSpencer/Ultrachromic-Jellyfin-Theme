Ultrachromic local CSS app bootstrap

This directory is the new build target for the old theme source.
Start here and migrate one module at a time from old_assets/assets/css.

Recommended initial files:
- fixes.css
- jf_font.css
- base.css
- accentlist.css
- rounding.css or rounding_circlehover.css
- smallercast.css
- overlayprogress.css
- bottombarprogress.css

Next steps:
1. Review each migrated file and fix any broken selectors.
2. Add module folders and files from old_assets/assets/css when ready.
3. Use assets/css/index.css as the local import manifest.

Keep the import order stable: fixes, font, base, accent, rounding, extras.
