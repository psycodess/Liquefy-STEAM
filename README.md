# Liquefy-STEAM

A Millennium (SteamBrew) Windows 11 glassmorphism theme for Steam using a Minimal-Dark-compatible structure and a Glasscord/Liquify-inspired aesthetic.

## What this theme does

- Forces top-level Steam CEF containers transparent so desktop/DWM can bleed through.
- Replaces dark solid cards with frosted-glass panels.
- Uses a reusable glass variable system in `styles/colors.css`.
- Applies high-intensity blur/saturation and layered lighting gradients.

## Key required overrides included

```css
.steamui_SteamUI_Check,
.client_root_container,
.library_AppDetailsMain_1p8qX {
  background: transparent !important;
}
```

## Files

- `skin.json` – Millennium theme manifest.
- `styles/colors.css` – Glass variable system.
- `styles/main.css` – Full glassmorphism overrides.

## Tuning tips

- Increase blur: raise `--glass-blur` / `--glass-blur-strong`.
- Increase transparency: lower alpha values in `--glass-bg*` and `--md-bg-*`.
- Increase contrast: raise `--text-primary` opacity and reduce ambient gradients.
