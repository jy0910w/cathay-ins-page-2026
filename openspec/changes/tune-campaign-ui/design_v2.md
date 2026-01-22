# Visual Design Specification - Campaign 2026

## 1. Color System
- **Yellow (Primary/Accent):** `#FFC83B`
  - Usage: Buttons, Step Badges, Highlight text ("舞夠有禮", "\線上投保/")
- **Black (Text/Contrast):** `#3F3F3F`
  - Usage: Main body text, Headings, Button text
- **Green (Backgrounds):**
  - Steps Background: `#ccffe1`
  - Dots Texture: `#b8e6c9` (Adjusted for contrast with #ccffe1)
  - Divider Wave: Green trapezoid shape (#ccffe1)

## 2. Hero Section
- **Background:** `section1.svg`
  - Positioning: `top: 0`, `z-index: 0`.
  - Behavior: Independent from content padding via `::before`.
- **Typography:**
  - Title Line 1: "\線上投保/" (Yellow) + "選國泰產險" (Black).
  - Title Line 2: "會員召集" (Black) + "舞夠有禮" (Yellow). **No whitespace** between spans.
  - Subtitle: "完成 3 步驟 簡單抽好禮"
    - Location: Below CTA buttons.
    - Styling: "3" is enlarged (1.5em, Montserrat), Flexbox centered.
    - Spacing: Pushed down (`margin-top: 4rem+`) to sit near the bottom wave.
- **CTA Buttons:**
  - Flexbox row.
  - Arrow: SVG icon (`icon-arrow--line.svg`), not text character.
- **Characters:**
  - `cellphoneman.svg` (Left), `musicwoman.svg` (Right).
  - Absolute positioning at bottom corners.

## 3. Steps Section
- **Background:**
  - Base: `#E6F9EF`
  - Texture: Radial gradient dots (20px spacing).
- **Step Card Anatomy:**
  - **Container:** White background, rounded corners (`1rem`).
  - **Header (Badge):** Full-width Yellow (`#FFC83B`) bar at the top containing "步驟 X".
  - **Body:**
    - Title: Black text.
    - Image: SVG (`step1.svg`, etc.) centered.
    - Button: Yellow pill shape, floating visually at bottom (inside card but distinct).
      - Icon: SVG Arrow.
  - **Note:** Grey text below button.
- **Flow:**
  - Desktop: Green `>` arrows positioned between cards (absolute positioned on card `::after`).
  - Mobile: Stacked vertical layout.

## 4. Prizes Section
- **Layout:** Grid system (1st prize center/highlighted).
- **Cards:**
  - Similar visual language to Steps (White card, Yellow/Gold accents).

## 5. Assets
- **Icons:** `icon-arrow--line.svg`
- **Illustrations:** `cellphoneman.svg`, `musicwoman.svg`, `step[1-3].svg`
