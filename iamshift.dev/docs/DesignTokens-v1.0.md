# iamshift.dev — Design Tokens

## 1. CSS Custom Properties

### 1.1 Root Tokens (Active)

These match the final production site.

```css
:root {
  /* Brand */
  --color-brand-forge-orange: #FF4E00;
  --color-brand-forge-orange-tint: #FF9500;

  /* Functional supports */
  --color-support-blue: #0C5DA5;
  --color-support-green: #00AC6B;

  /* Light Neutrals */
  --color-neutral-white: #FFFFFF;
  --color-neutral-surface-1: #F8F8F8;
  --color-neutral-surface-2: #EAEAEA;
  --color-neutral-black: #000000;
  --color-neutral-text: #1A1A1A;

  /* Typography */
  --font-brand: "Beepo", system-ui, sans-serif;
  --font-body: "Inter", system-ui, sans-serif;

  /* Spacing */
  --space-1u: 4px;
  --space-2u: 8px;
  --space-4u: 16px;
  --space-8u: 32px;
  --space-12u: 48px;
  --space-16u: 64px;

  /* Motion identity */
  --motion-fast: 120ms;
  --motion-default: 160ms;
  --motion-ease: cubic-bezier(0.4, 0.0, 0.2, 1);

  /* Layout safe area for right-side nav bar */
  --nav-safe-right: 5rem;
}