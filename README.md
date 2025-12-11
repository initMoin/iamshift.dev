# [iamshift.dev](https://iamshift.dev) — Personal Identity System
**let shift : Moin**

`shift is standard // design is craft`

This repository contains the complete source code for **iamshift.dev**, a motion-driven identity system and portfolio website built from the ground up using semantic HTML, precision CSS, scroll-driven micro-interactions, and a fully custom boot sequence.
No frameworks. No templates. Pure hand-crafted front-end architecture.

---

## Features

### **1. Custom Boot Sequence**
A multi-phase intro experience designed to simulate a system initialization:
- **Terminal-style line reveal**: Timed logs with specific boot assets (`boot-header-logo.png`).
- **Brand splash animation**: A dedicated, full-screen brand reveal (`boot-logo.png`).
- **Seamless Handoff**: Automatic transition from bootloader to the live environment.
- **Cinematic Entrance**: Sequential word animation for the site title and a "reverb" spin effect for the global logo upon initialization.

### **2. Global Header System**
Persistent top-left identity marker that anchors the experience:
- **Reverb Entrance**: Logo executes a precision spin-scale animation upon boot completion.
- **Word-by-Word Reveal**: The "let shift : moin" title sequences in via CSS offsets.
- **Theme-Aware**: Adapts visually based on the active section's color palette.

### **3. Vertical Snap Navigation**
Sections are navigated through a rigorous scroll-snap architecture:
- `scroll-snap-type: y mandatory` for definite section locking.
- **Keyboard Navigation**: Full support for `j/k`, arrow keys, and spacebar (with modifier support for reverse navigation).
- **Active State Monitoring**: Intersection Observers update navigation dots and URL hashes in real-time.
- **Visual Masking**: Content fade-out masks applied dynamically post-boot.

### **4. Adaptive Mobile Architecture**
A responsive system that maintains design integrity across viewports:
- **Fluid Typography**: Extensive use of `clamp()` for font sizing that scales from mobile to ultra-wide.
- **Layout Switching**: Grid systems in the `self` and `ping` sections automatically reflow to vertical stacks on mobile devices.
- **Touch Optimization**: Custom touch handlers for the boot sequence and navigation arrows.

### **5. Section Design System**
Each section constitutes a distinct identity block with unique interactions:
- **`init`** — Brand origin and philosophical statement.
- **`code`** — Structured creation (includes expandable details and animated cursor prompt).
- **`pixel`** — Visual language (features randomized viewport "spark" particles).
- **`echo`** — Reflection & narrative.
- **`self`** — Identity (split-pane layout for desktop, unified stack for mobile).
- **`ping`** — Availability and status status.

### **6. Dynamic Theme Engine**
The site is self-aware of its visual context:
- **Meta-Theme Switching**: The browser UI color (Safari/Chrome bar) changes instantly as the user scrolls between sections (e.g., Orange for `init`, White for `self`, Black for `code`).
- **Transition Management**: Smooth CSS transitions for background colors and overlays.

### **7. Zero Dependencies**
- No React, Vue, Tailwind, jQuery, GSAP, etc.
- No build system required.
- Deploy-ready static front-end.

---
