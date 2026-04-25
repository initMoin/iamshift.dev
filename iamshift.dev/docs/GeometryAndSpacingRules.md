# iamshift.dev — Geometry & Spacing Rules  
### Brand Identity System v1.0

## 1. Logomark Geometry  
The three-arm geometric logomark is constructed from uniform angular strokes.  
Its **stroke thickness defines the core spacing unit (1u)** used throughout the layout system.

- 1u = 4px  
- All distances in the system scale upward from this base value.

This ensures the visual rhythm of the interface is derived from the identity itself.

---

## 2. Spacing System in Production

### 2.1 Spacing Units
1u = 4px
2u = 8px
4u = 16px
8u = 32px   (section-level rhythm)
12u = 48px
16u = 64px

### 2.2 Section Containers  
Every top-level section (`init`, `code`, `pixel`, `echo`, `self`, `ping`) respects:

- A left margin aligned visually to the logomark axis  
- A right offset determined by `--nav-safe-right` to avoid conflict with the vertical nav bar  
- A vertical centering rhythm for primary content blocks  

These rules are applied differently per section depending on identity, but the grid foundation remains the same.

---

## 3. Vertical Rhythm  
A consistent vertical flow is maintained across sections:

- **Headlines** appear at approximately 4u below the top of the grid.
- **Taglines** sit 2u below their respective section headline.
- **Content blocks** maintain roughly 4u separation.
- The **axiom** (“shift is standard // design is craft”) floats according to contextual alignment rather than a strict grid rule.

Vertical rhythm is never purely mathematical — it is proportional to identity, spacing, and clarity of reading.

---

## 4. Global Logo System Geometry  
The global badge (circular container) and the site title follow strict positional geometry:

- The global badge sits at:
top: 2rem
left: 2rem

- Its clearspace requirement is **4u** minimum around the badge.

- The site title is positioned via:  
top: calc(2rem + badgeHeight/2)
left: calc(2rem + badgeWidth + gap)
transform: translateY(-50%);

This ensures the title vertically aligns with the badge center.

---

## 5. Navigation Geometry (Right-Side Nav Bar)

- The vertical nav uses Forge Orange for active state.
- Each dot is vertically spaced using a **2u grid** for even cadence.
- `--nav-safe-right` defines a universal content boundary so section content never collides with the nav.

---

## 6. Section-Level Geometry Notes

### **init**
- Now left-aligned for both headline and tagline.
- Maintains a forge orange background.
- Vertical spacing mirrors the other sections after animation cleanup.

### **code**
- The animated cursor (`code-cursor`) aligns horizontally to the headline text axis.
- The cursor placeholder (`start building`) uses a reduced opacity and positions via a small vertical optical adjustment.

### **pixel**
- Random pixel sprites appear anywhere in the viewport—not limited to the content block.
- The background grid remains subtle and does not dictate spacing, only texture.

### **echo**
- The waveform graphic sits below the social links, positioned with a **12u** top offset for balance.
- Waveform visually spans the full width available within the nav-safe area.

### **self**
- Portrait + text layout remains vertically centered at desktop sizes.
- At smaller widths, text left-aligns to match the content block while the portrait re-centers.
- Headline + tagline always align to the text block, not the portrait.

### **ping**
- Outward-propagating rings expand beyond the viewport.
- Rings follow exponential geometric spacing rather than linear increments for a natural "wave spread."

---

## 7. Motion Geometry  
All motion follows strict geometric discipline:

- **Orthogonal movement** (no curved paths unless identity-driven)
- **Snap-corrected spin** for global logo
- **Fade + translateY(4u)** for section reveal animations
- **Cinematic timing** from overshoot and rebound principles

Motion is spatially derived from the same unit system rather than random values.

---

## 8. Summary  
The geometry and spacing system ties together:

- Logomark  
- Navigation  
- Typography  
- Spacing  
- Animations  
- Section layout  
- Overall reading rhythm  

Every rule ultimately derives from the **1u logomark stroke**, ensuring visual unity across all identity surfaces of iamshift.dev.