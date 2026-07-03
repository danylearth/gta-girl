# Image Manifest

All assets downloaded from Figma MCP on 2026-07-03 (source URLs expire ~7 days from export). Stored in `assets/images/`.

| Filename | Dimensions | Actual type | Size | Description | Status |
|----------|-----------|-------------|------|-------------|--------|
| `hero-athletic-woman.png` | 381 × 658 | PNG (RGBA) | 395 KB | Smiling athletic woman against a green wall — right-column hero photo | OK |
| `run-card-thumbnail.png` | 111 × 211 | PNG (RGBA) | 51 KB | "Burn It Fast" fitness-equipment thumbnail in the floating mini card | OK |
| `header-user-avatar.png` | 35 × 40 | PNG (RGBA) | 4.3 KB | Anna's avatar in the header profile button | OK |
| `logo-s.svg` | viewBox 24 × 24 | SVG | 8.7 KB | "S" brand logo in the sidebar | OK (renamed from .png) |
| `walk-progress-ring.svg` | viewBox 71.91 × 71.91 | SVG | 27 KB | Circular step-progress ring, includes baked-in "3986 Steps" text | OK (renamed from .png) |
| `heart-rate-chart.svg` | viewBox 72.42 × 60 | SVG | 14 KB | Heart-rate bar chart (green/orange bars) | OK (renamed from .png) |
| `sleep-hypnogram.svg` | viewBox 40 × 40 | SVG | 30 KB | Sleep-stage hypnogram line graphic | OK (renamed from .png) |
| `run-route-map.svg` | viewBox 96 × 96 | SVG | 7.4 KB | Jogging-route outline map in the Easy Run glass card | OK (renamed from .png) |

## Notes
- Figma exported the 5 vector assets with a `.png` suggestion but the payloads are SVG; verified with `file` and renamed to `.svg`.
- All rasters are above the 5KB sanity threshold except `header-user-avatar.png` (4.3 KB) — verified as a real 35×40 PNG photo crop, not a placeholder.
- No failed downloads; no placeholders in use.
