# Tambay Discord Theme

Vencord theme for the **Tambay sa Skwela** server. Styles only apply inside that server.

## Install

Vencord → Settings → Themes → **Edit QuickCSS**, then paste at the very top:

```css
@import url("https://cdn.jsdelivr.net/gh/JanoAngulo/TambayDiscordTheme@main/quickCss.css");
```

Reload Discord with `Ctrl + R`.

## Recolor

Override the palette below the import:

```css
:root {
    --tambay-primary: #dc794e;
    --tambay-secondary: #613e31;
    --tambay-tertiary: #f2af45;
}
```

Animation speeds are variables too (`--tambay-shimmer-speed`, `--tambay-drift-speed`, `--tambay-dur`). Animations turn off when Discord's **Reduce Motion** setting is on.

## Updating

jsDelivr caches `@main` for up to 12 hours. After pushing, open this link to refresh it right away:

https://purge.jsdelivr.net/gh/JanoAngulo/TambayDiscordTheme@main/quickCss.css

## When Discord updates break it

Discord renames its CSS classes (e.g. `panels_pog62O`) every few months. Open DevTools with `Ctrl + Shift + I`, inspect the broken element, and update the class names in `quickCss.css`. Class hashes were last mapped on 2026-11-10.
