# WPMC Homepage Blueprint (Astra + Gutenberg)

## Brand Intent
**Positioning statement:** *Woburn’s home for community media and local storytelling.*

Design tone: warm, modern, local, and media-forward. Avoid government-portal stiffness, corporate stock-template feel, or OTT streaming-grid clone.

---

## 1) Homepage Structure (Top to Bottom)

1. **Hero Section**
2. **Featured Productions**
3. **Watch Live + Government Meetings**
4. **Community Spotlight**
5. **Classes & Training**
6. **Facilities & Studios**
7. **Membership / Get Involved CTA**
8. **Footer**

---

## 2) Global Layout Settings (Astra + Gutenberg)

### Astra Customizer Baseline
- **Container width:** 1200–1280px
- **Content layout:** Full Width / Stretched for homepage template
- **Global spacing:** comfortable vertical rhythm (mobile-first)
- **Header:** sticky optional, but lightweight; include quick “Watch Live” button in header CTA slot

### Gutenberg Global Defaults (recommended)
- **Group block** as primary section wrapper
- Use **wide alignment** for section backgrounds, inner constrained container for text/cards
- Prefer **Columns**, **Stack**, **Row**, **Buttons**, **Cover**, **Media & Text**, **Query Loop** blocks
- Save repeated sections as **Patterns** (e.g., card grids, CTA bars)

### Spacing Scale
Use a consistent spacing system:
- 8, 12, 16, 24, 32, 48, 64, 80px
- Section vertical padding:
  - Desktop: 72–96px
  - Tablet: 56–72px
  - Mobile: 40–56px

---

## 3) Color Palette (Accessible + Warm)

```css
:root {
  --wpmc-navy-900: #0E1A2B;
  --wpmc-slate-700: #2F3E52;
  --wpmc-slate-500: #5F6F86;
  --wpmc-bg-50: #F7F9FC;
  --wpmc-white: #FFFFFF;
  --wpmc-orange-500: #F47C2D;
  --wpmc-orange-600: #DD6A1E;
  --wpmc-teal-500: #2FA89A;
  --wpmc-border-200: #E3E8F0;
}
```

Usage:
- Primary text/background contrast: navy/slate on white or very light bg
- Accent actions: orange (buttons, highlights)
- Secondary tag accents: teal for classes/community labels

---

## 4) Typography Recommendations

Use easy-to-read modern sans fonts (Google fonts supported in WP):
- **Headings:** `Poppins` or `Manrope`
- **Body:** `Inter` or `Source Sans 3`

Suggested scale:
- H1: 44–56px desktop, 34–40px tablet, 30–34px mobile
- H2: 32–40px desktop, 28–32px tablet, 24–28px mobile
- H3: 22–28px
- Body Large: 20px
- Body: 17–18px
- Small/meta: 14px

Line-height:
- Headings: 1.15–1.25
- Body: 1.55–1.75

---

## 5) Section-by-Section Blueprint + Gutenberg Block Layouts

## Section 1: Hero

### Purpose
Drive viewership and set emotional tone immediately.

### Block structure
- Group (full-width, dark navy gradient bg)
  - Group (constrained container)
    - Columns (60/40)
      - Left:
        - Eyebrow text (“WOBURN PUBLIC MEDIA CENTER”)
        - H1
        - Paragraph
        - Buttons (Watch Live, Explore Productions)
        - Optional small trust row (e.g., “Local stories • Government coverage • Youth media”)
      - Right:
        - Cover/Image block with rounded corners (placeholder still from local production)

### Suggested copy (placeholder)
- H1: **Woburn’s home for community media and local storytelling.**
- Text: “Watch local programming, follow important town meetings, and discover classes that help you create.”
- CTA 1: **Watch Live**
- CTA 2: **See Featured Productions**

---

## Section 2: Featured Productions

### Purpose
Showcase quality programming and increase viewing depth.

### Block structure
- Group (light background)
  - Heading row (H2 + “View All Productions” text link)
  - Query Loop or Columns (3 cards desktop / 2 tablet / 1 mobile)
    - Card (Group)
      - Image (16:9)
      - Title
      - Meta row (category + runtime or date)
      - Short description
      - Button/link (“Watch Episode”)

### Card style
- Rounded corners: 16px
- Soft shadow on hover
- Maintain equal card heights when possible

---

## Section 3: Watch Live / Government Meetings

### Purpose
Make live and civic content easy to find fast.

### Block structure
- Group (white bg)
  - Columns (55/45)
    - Left: “Watch Live” feature card
      - H3
      - Live status pill
      - Short description
      - Primary button
    - Right: “Government Meetings” card stack
      - Next meeting highlight card
      - Two quick links (Recent Meetings, Full Schedule)

### UX notes
- Keep this section high on page.
- Use clear labels, not bureaucratic language.
- Prefer “Town Meetings” in user-facing copy with “Government Meetings” subtitle.

---

## Section 4: Community Spotlight

### Purpose
Signal inclusivity and neighborhood impact.

### Block structure
- Group (subtle tinted bg)
  - H2 + short intro
  - 3 spotlight cards (people/org/project)
    - Circular photo or rounded thumbnail
    - Name/title
    - 2–3 line blurb
    - Link (“Read Story” / “Watch Segment”)

Optional alt pattern:
- Horizontal scroll cards on mobile (if plugin/theme supports cleanly)

---

## Section 5: Classes & Training

### Purpose
Support memberships and participation.

### Block structure
- Group (white bg)
  - Columns (40/60)
    - Left: heading, description, CTA button (“View Classes”)
    - Right: 2x2 mini cards
      - Intro to Video Production
      - Editing Basics
      - Studio Orientation
      - Youth Media Workshop

Each class card:
- icon/emoji marker
- title
- short detail (e.g., “Beginner • 2 hours”)

---

## Section 6: Facilities & Studios

### Purpose
Promote studio/equipment reservations and professionalism.

### Block structure
- Group (dark slate background)
  - H2 + short text
  - 3 feature cards with photos:
    - Production Studio
    - Podcast Room
    - Editing Stations
  - CTA buttons:
    - “Reserve a Studio” (primary)
    - “View Equipment” (secondary)

Style:
- Inverted text (white/light)
- Orange accents for interactive elements

---

## Section 7: Membership / Get Involved CTA

### Purpose
Convert interest into action (membership, volunteering, donating).

### Block structure
- Group (gradient bg, rounded large panel)
  - Centered H2 + paragraph
  - Button row:
    - Become a Member
    - Volunteer
    - Donate

Keep concise and positive, with action-oriented language.

---

## Section 8: Footer

### Suggested blocks
- Columns (4)
  1. WPMC summary + mini mission line
  2. Watch links (Live, Meetings, Productions)
  3. Get involved links (Membership, Classes, Volunteer, Donate)
  4. Contact + social icons
- Sub-footer row: copyright + policy links

---

## 6) Reusable Gutenberg Patterns to Save

Create block patterns for:
1. **Section Intro Row** (eyebrow + H2 + supporting text)
2. **Media Card (16:9 + title + meta + CTA)**
3. **Three-Card Grid**
4. **Split Feature (content + image)**
5. **CTA Banner with button group**

These patterns speed future editing and preserve design consistency.

---

## 7) Button Styles

### Primary button
- Background: orange 500
- Text: white
- Radius: 999px (pill)
- Padding: 12px 22px
- Hover: orange 600 + slight lift

### Secondary button
- Background: transparent or white
- Border: 1.5px solid slate
- Text: navy
- Radius: 999px
- Hover: light slate background

### Tertiary text links
- Navy text + arrow icon
- Underline on hover/focus

---

## 8) Custom CSS (Astra + Gutenberg friendly)

Add in **Customizer → Additional CSS** or a child theme stylesheet.

```css
/* ===== Base tokens ===== */
:root {
  --wpmc-navy-900: #0E1A2B;
  --wpmc-slate-700: #2F3E52;
  --wpmc-slate-500: #5F6F86;
  --wpmc-bg-50: #F7F9FC;
  --wpmc-white: #FFFFFF;
  --wpmc-orange-500: #F47C2D;
  --wpmc-orange-600: #DD6A1E;
  --wpmc-teal-500: #2FA89A;
  --wpmc-border-200: #E3E8F0;
  --wpmc-radius-lg: 16px;
  --wpmc-radius-xl: 24px;
  --wpmc-shadow-sm: 0 6px 18px rgba(12, 24, 44, 0.08);
  --wpmc-shadow-md: 0 12px 28px rgba(12, 24, 44, 0.14);
}

/* ===== Typography ===== */
body {
  color: var(--wpmc-slate-700);
  line-height: 1.65;
}

h1, h2, h3, h4 {
  color: var(--wpmc-navy-900);
  line-height: 1.2;
  letter-spacing: -0.02em;
}

/* ===== Shared section wrapper ===== */
.wpmc-section {
  padding: clamp(2.75rem, 6vw, 5.5rem) 1rem;
}

.wpmc-inner {
  max-width: 1200px;
  margin-inline: auto;
}

/* ===== Hero ===== */
.wpmc-hero {
  background: linear-gradient(140deg, #0E1A2B 0%, #172A44 60%, #1F3A58 100%);
  color: #fff;
}

.wpmc-hero h1,
.wpmc-hero p,
.wpmc-hero .wp-block-heading {
  color: #fff;
}

.wpmc-hero-media img {
  border-radius: var(--wpmc-radius-xl);
  box-shadow: var(--wpmc-shadow-md);
}

/* ===== Cards ===== */
.wpmc-card {
  background: var(--wpmc-white);
  border: 1px solid var(--wpmc-border-200);
  border-radius: var(--wpmc-radius-lg);
  overflow: hidden;
  box-shadow: var(--wpmc-shadow-sm);
  transition: transform .2s ease, box-shadow .2s ease;
}

.wpmc-card:hover {
  transform: translateY(-3px);
  box-shadow: var(--wpmc-shadow-md);
}

.wpmc-card-body {
  padding: 1rem 1rem 1.1rem;
}

/* ===== Buttons ===== */
.wp-block-button.is-style-wpmc-primary .wp-block-button__link,
.wpmc-btn-primary {
  background: var(--wpmc-orange-500);
  color: #fff;
  border-radius: 999px;
  padding: 0.75rem 1.4rem;
  font-weight: 600;
  border: 0;
}

.wp-block-button.is-style-wpmc-primary .wp-block-button__link:hover,
.wpmc-btn-primary:hover {
  background: var(--wpmc-orange-600);
}

.wp-block-button.is-style-wpmc-secondary .wp-block-button__link,
.wpmc-btn-secondary {
  background: transparent;
  color: var(--wpmc-navy-900);
  border-radius: 999px;
  border: 1.5px solid var(--wpmc-slate-500);
  padding: 0.72rem 1.35rem;
  font-weight: 600;
}

.wp-block-button.is-style-wpmc-secondary .wp-block-button__link:hover,
.wpmc-btn-secondary:hover {
  background: #eef3fa;
}

/* ===== Utility ===== */
.wpmc-pill {
  display: inline-block;
  font-size: 0.82rem;
  font-weight: 600;
  border-radius: 999px;
  padding: 0.35rem 0.65rem;
  background: #ffe9db;
  color: #8a3d0f;
}

.wpmc-dark-section {
  background: var(--wpmc-slate-700);
  color: #eaf0f8;
}

.wpmc-dark-section h2,
.wpmc-dark-section h3,
.wpmc-dark-section p {
  color: #fff;
}

/* ===== Responsive ===== */
@media (max-width: 1024px) {
  .wpmc-section {
    padding: clamp(2.5rem, 5vw, 4.5rem) 1rem;
  }
}

@media (max-width: 781px) {
  .wpmc-hero {
    text-align: left;
  }

  .wpmc-card {
    border-radius: 14px;
  }

  .wp-block-buttons {
    gap: .65rem;
  }
}
```

---

## 9) Responsive Behavior Notes

- **Desktop (1200+)**: 3-column card grids, split layouts for hero/live/classes.
- **Tablet (782–1199)**: collapse to 2-column cards where needed.
- **Mobile (<782)**:
  - stack all split sections into single column
  - keep text left-aligned
  - button groups wrap naturally
  - reduce heading sizes and spacing, preserve tap targets (44px+ height)

---

## 10) Accessibility Checklist

- Color contrast minimum WCAG AA for text/buttons
- Clear heading hierarchy (single H1)
- Descriptive button labels (“Watch Live Now”, not “Click Here”)
- Alt text on all imagery and thumbnails
- Visible focus states for links/buttons
- Avoid text over busy images without overlays
- Keep paragraph width readable (~65–75 characters where possible)

---

## 11) Easy-Edit Content Model (Future Proofing)

For ongoing updates, map sections to editable WP content:
- **Featured productions:** Query Loop pulling from “Productions” posts/CPT
- **Classes:** posts in “Classes” category or CPT
- **Meetings:** posts/CPT with date metadata
- **Spotlight:** “Community Stories” category

Add a simple editorial workflow:
1. Update hero monthly.
2. Swap featured productions weekly.
3. Pin current/next meetings.
4. Rotate spotlight stories biweekly.

