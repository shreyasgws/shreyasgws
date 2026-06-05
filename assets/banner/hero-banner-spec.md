# Hero Banner Specification

## Design Goals
- Premium dark theme matching GitHub profile README
- Professional, non-anime, non-generic aesthetic
- Communicates identity, role, and project scope immediately

## Specifications

### Capsule Render (Current Implementation)
Uses `capsule-render.vercel.app` for the dynamic banner.

```
URL: https://capsule-render.vercel.app/api?type=waving&height=240&color=0:0d1117,50:1a1a2e,100:4fd1ff&text=SHREYAS%20GWS&reversal=false&fontAlignY=38&desc=Full%20Stack%20Developer%20·%20AI%20Builder%20·%20Product%20Creator&descAlignY=55&fontColor=ffffff
```

- **Type:** Waving
- **Height:** 240px
- **Color Gradient:**
  - 0%: `#0d1117` (deep dark)
  - 50%: `#1a1a2e` (dark navy)
  - 100%: `#4fd1ff` (cyan accent)
- **Title:** SHREYAS GWS
- **Subtitle:** Full Stack Developer · AI Builder · Product Creator
- **Font Color:** White

### Custom SVG Banner (Alternative)
Use a custom SVG for full control over branding.

- **Dimensions:** 1280 x 240 px
- **Background:** Linear gradient from `#0a0a0f` → `#0d1117` → `#0a0a0f`
- **Accent Line:** Subtle 0.5px line at bottom with `#4fd1ff` at 30% opacity
- **Typography:**
  - Name: system-ui, 32px, 700 weight, white, 4px letter-spacing
  - Subtitle: system-ui, 14px, 400 weight, `#94a3b8`, 2px letter-spacing
- **Decorative Elements:** Subtle glow circles (low opacity) in corners

### Recommended Tools
1. **capsule-render.vercel.app** — Easy, dynamic, responsive
2. **Custom SVG** — Full control, matches brand exactly
3. **Canva / Figma** — For static PNG export if SVG not preferred

## Typography
- **Primary:** system-ui, -apple-system, sans-serif
- **Weights:** 700 (name), 400 (subtitle)
- **Color:** White (name), `#94a3b8` (subtitle)
- **Letter-spacing:** 4px (name), 2px (subtitle)

## Color Palette
| Color | Hex | Usage |
|---|---|---|
| Deep Dark | `#0a0a0f` | Background edges |
| GitHub Dark | `#0d1117` | Background center |
| Dark Navy | `#1a1a2e` | Gradient midpoint |
| Cyan | `#4fd1ff` | Primary accent |
| Indigo | `#6366f1` | Secondary accent |
| Muted White | `#94a3b8` | Subtitle text |
| White | `#ffffff` | Name text |
