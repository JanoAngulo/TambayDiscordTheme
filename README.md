# Tambay Discord Theme

Vencord theme for the **Tambay sa Skwela** server. Styles only apply inside that server.

## Install

Vencord → Settings → Themes → **Edit QuickCSS**, then paste at the very top:

```css
@import url("https://janoangulo.github.io/TambayDiscordTheme/quickCss.css");
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

Animation speeds are variables too (`--tambay-shimmer-speed`, `--tambay-drift-speed`, `--tambay-dur`, `--tambay-pop-dur`, `--tambay-layer-dur`). Animations turn off when Discord's **Reduce Motion** setting is on.

## BetterAnimations-style enters

The theme recreates the enter animations of the [BetterAnimations](https://github.com/okdevme/DiscordPlugins) plugin's preinstalled pack in pure CSS: messages, the channel list, popouts, tooltips, and modals **slip** in (5px + fade, 200ms, `outBack` overshoot); context menus and the settings layer **scale** in; the modal backdrop fades. Tooltips slip from the side they're anchored to. Exit animations require JavaScript, so a CSS theme can only recreate enters — install the actual plugin (BetterDiscord only) if you want exits too.

## Updating

Push to `main`. GitHub Pages republishes in a minute or two and caches for up to 10 minutes, then `Ctrl + R` in Discord picks it up.

## When Discord updates break it

Discord renames its CSS classes (e.g. `panels_pog62O`) every few months. Open DevTools with `Ctrl + Shift + I`, inspect the broken element, and update the class names in `quickCss.css`. Class hashes were last mapped on 2026-11-10.
