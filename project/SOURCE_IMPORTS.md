```css
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/fixes.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/jf_font.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/base.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/accentlist.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/rounding.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/smallercast.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/episodelist/episodes_compactlist.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/header/header_transparent.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/fields/fields_border.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/cornerindicator/indicator_corner.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/type/dark_withaccent.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/titlepage/title_simple.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/overlayprogress.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/effects/hoverglow.css');
@import url('https://cdn.jsdelivr.net/gh/CodingSpencer/Ultrachromic-Jellyfin-Theme@main/effects/glassy.css');

:root {
    --accent: 0, 164, 220;
    --rounding: 12px;
}

.backdropImage {
    filter: blur(24px) saturate(120%) contrast(120%) brightness(35%);
}

/* Desktop Viewport Adjustments */
@media (min-width: 992px) {
    /* Revert broken flex rules back to native block formatting */
    .detailPagePrimaryContainer {
        display: block !important;
        padding-right: 16px !important;
    }

    /* Pushes the entire episode/cast shelf down safely past the hanging poster */
    .detailPageSecondaryContainer {
        margin-top: 130px !important;
        padding-right: 16px !important;
        box-sizing: border-box !important;
        clear: both !important;
    }
}
```