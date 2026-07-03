# Site Map

**Figma File Key**: `QbuaAdXYCLMBhbkkKyRQR3`
**Source URL**: https://www.figma.com/design/QbuaAdXYCLMBhbkkKyRQR3/Untitled?node-id=1-7&t=7loCU8LKevBK9xqv-4
**Container Max-Width**: `1280px` (design frame is 1180px wide × 886px tall, content container 1116px, 32px outer padding)

## Pages

### Page: Fitness Dashboard (single screen)
Node ID: `1:7`

#### Sections

| Section | Node ID | Component | Background | Notes |
|---------|---------|-----------|------------|-------|
| Sidebar Navigation | `1:9` | Sidebar | transparent | 64px wide; logo + 4 round icon buttons (dashboard active) |
| Header - Top Navigation | `1:40` | Header | rgba(255,255,255,0.4) + blur 6px, full pill | Tabs: Home (active, dark), Activities, Health status, Training Planing; theme toggle, notifications, profile |
| Greeting & Actions | `1:75` | Greeting | transparent | "Hello, Anna" H1 + Search / Calendar / ChatBot Ai buttons |
| Dashboard Grid | `1:90` | Grid | transparent | 12-col grid, 20px gap, 666px row |
| Activities Card | `1:92` | Card | #C7DACB | Left col (cols 1–4). Streak alert, Week/Month/Year/All-time tabs, stacked bar chart Sun–Sat, footer summary |
| Sleep Score Card | `1:181` | Card | #F5F2EF | Left col. Hypnogram graphic, stage labels (Awake/REM/Light/Deep), Good / 8,5 / 8h 20m |
| Walk Metric | `1:287` | Metric card | #FFFFFF | Middle col (cols 5–8), ~104px wide. Circular progress ring (3986 steps, baked into SVG) |
| Heart Rate Card | `1:344` | Metric card | #FFFFFF | Middle col. Hourly dropdown, bar chart image, 9.00PM–11.00PM labels |
| Stress Metric | `1:409` | Metric card | #FFFFFF | Middle col. Big value "35" |
| Water Metric | `1:420` | Metric card | #FFFFFF | Middle col. Orange bar row + "1.5 liters" |
| Calories Analysis | `1:442` | Card | #FFFFFF | Middle col. BMI segmented bar (18,5 / 25,0 / 30,0), macros list (Protein/Carbs/Fat/Calories) |
| Hero Image & Run Stats | `1:502` | Hero card | photo + gradient | Right col (cols 9–12), radius 32px, full-height photo, bottom black gradient |
| Glassmorphism Easy Run Card | `1:506` | Glass card | rgba(255,255,255,0.4) + blur 5px | Route map, 06.50 km, date + 4 metric rows; floating "Burn It Fast" mini card (rotated −5°) intersecting the edge |

## Shared Components

| Component | Node ID (example) | Description |
|-----------|-------------------|-------------|
| Round icon button | `1:79` | 40px circle, white (or white/70%), FA icon, shadow 0 1px 1px rgba(0,0,0,.05) |
| Pill button w/ icon+label | `1:82` | White pill, 16px/10px padding, 14px Inter + FA icon (Calendar, ChatBot Ai) |
| Nav tab | `1:42` | Pill, px 20 / py 8; active = #1C1D21 bg + white text |
| Segmented tabs | `1:110` | Track #B5CBB9 pill, active segment #D9EADB pill |
| Card header row | `1:93` | 14px FA icon + 14px label left, 24px more-options circle right |
| More-options button | `1:98` | 24px circle, rgba(255,255,255,0.5) on tinted cards / transparent on light, ellipsis icon |
| Goal chip | `1:471` | #EFF6FF, radius 6, 96px wide, 12px text |
| Metric card header | `1:288` | icon + label + diagonal expand arrow (FA arrow-right rotated −45°) |

## Layout Analysis

- **Page background**: flat `#E2EFE7`, spans full viewport; content constrained to `max-width: 1280px` with 32px padding, min-height 822px.
- **Header**: full-width pill inside the content container (not viewport-wide); backdrop-blur glass.
- **Dashboard Grid**: 12 columns, three equal 4-col columns, `gap: 20px`, fixed 666px row height.
- **Hero column**: image spans the full column (radius 32, overflow hidden); gradient overlay transparent → rgba(0,0,0,0.6) bottom; glass card floats at bottom with 20px inset; the "Burn It Fast" mini card overflows the glass card (clipped only by the hero column bounds).
- **Bar chart decorations**: dashed horizontal grid lines (rgba(156,163,175,0.5)) span the full card content width; y-axis labels sit at the right edge on card-colored backgrounds.

## Design Tokens

### Colors
| Role | Value |
|------|-------|
| Page background | `#E2EFE7` |
| Card / surface | `#FFFFFF` |
| Activities card | `#C7DACB` |
| Activities alert box / active tab | `#D9EADB` |
| Activities tabs track | `#B5CBB9` |
| Sleep card | `#F5F2EF` |
| Dark (active nav, toggle, mini card) | `#1C1D21` |
| Accent lime (bars, BMI mid) | `#D7F576` |
| Accent orange (water, BMI high) | `#EA6328` |
| Bar olive-gray | `#9CA495` (80% opacity) |
| Notification dot | `#EF4444` |
| Goal chip | `#EFF6FF` |
| Text primary | `#1A1A1A` / `#1F2937` |
| Text secondary | `#374151` / `#4B5563` |
| Text muted | `#6B7280` / `#9CA3AF` |
| Neutrals | `#D1D5DB`, `#E5E7EB`, `#F3F4F6`, `#F9FAFB` |
| Glass surfaces | rgba(255,255,255,0.4–0.7) + backdrop-blur 5–6px |

### Typography
- Family: **Inter** (Regular 400 throughout); icons: **Font Awesome 5/6 Free** (Solid & Regular)
- Sizes: 30px/36 (H1), 32px (run distance, tracking −0.8px), 24px/32 (sleep 8,5), 14px/20 (body/labels), 12px/16 (secondary), 11px, 10px, 9px, 8px (chart axis)

### Spacing scale
4, 6, 8, 12, 16, 20, 24, 32 px. Card padding: 16px (small metric), 20px (large cards). Grid gap 20px, page gap 24px.

### Border radius
- 9999px pills/circles, 32px hero, 24px cards, 16px mini card, 12px alert/logo, 8px dropdown, 6px chips, 2px bar ends

### Shadows
- Cards/buttons: `0 1px 1px rgba(0,0,0,0.05)`
- Hero column: `0 1px 2px rgba(0,0,0,0.05)`
- Floating mini card: `0 10px 15px -3px rgba(0,0,0,0.1), 0 4px 6px -4px rgba(0,0,0,0.1)`

### `--container-max`
`1280px`
