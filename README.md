# [iamshift.dev](https://iamshift.dev) — Personal Identity System
**let shift : Moin**

`shift is standard // design is craft`

This repository contains the full source for **iamshift.dev** — a motion-driven identity system built using semantic HTML, precision CSS, and custom JavaScript.

No frameworks. No templates. Fully controlled front-end architecture.


## Live System

https://iamshift.dev

---

## Access Layers

- `/` → primary interface  
- `/source` → system-level identity layer  

Each layer exposes a different depth of the system.


## System Features

### **1. Custom Boot Sequence**
A multi-phase intro experience designed to simulate a system initialization:
- **Terminal-style line reveal**: Timed logs with specific boot assets (`boot-header-logo.png`).
- **Brand splash animation**: A dedicated, full-screen brand reveal (`boot-logo.png`).
- **Seamless Handoff**: Automatic transition from bootloader to the live environment.
- **Cinematic Entrance**: Sequential word animation for the site title and a "reverb" spin effect for the global logo upon initialization.
- **Interruptible Flow**: Boot sequence can be skipped via click, touch, or keyboard input.

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
- **Touch Optimization**: Custom touch handlers for the boot sequence and navigation.
- **Interaction Model Shift**: Mobile uses always-on visual states in place of hover-dependent interactions.

### **5. Section Design System**
Each section constitutes a distinct identity block with unique interactions:
- **`init`** — Brand origin and philosophical statement.
- **`code`** — Structured creation (includes expandable details and animated cursor prompt).
- **`pixel`** — Visual language (features randomized viewport "spark" particles).
- **`echo`** — Reflection & narrative.
- **`self`** — Identity (split-pane layout for desktop, unified stack for mobile).
- **`ping`** — Availability and system status.

### **6. Dynamic Theme Engine**
The site is self-aware of its visual context:
- **Meta-Theme Switching**: The browser UI color (Safari/Chrome bar) changes instantly as the user scrolls between sections (e.g., Orange for `init`, White for `self`, Black for `code`).
- **Transition Management**: Smooth CSS transitions for background colors and overlays.


## Interaction Model

The system adapts interaction based on input context:

- **Desktop** → hover-enabled, layered interaction states  
- **Mobile** → always-on states, no hover dependency  
- **Boot Sequence** → interruptible via keyboard, touch, or click  

All interaction paths resolve deterministically into the same system state.


## Architecture

The system is composed of tightly controlled layers:

- **Boot Engine** → initialization and state transitions  
- **Scroll Engine** → section locking and navigation  
- **Theme Engine** → dynamic UI and browser chrome adaptation  
- **Section System** → modular identity surfaces  

No abstraction layers or external runtimes are used.


## Zero Dependencies

- No React, Vue, Tailwind, jQuery, GSAP, etc.
- No build system required.
- Deploy-ready static front-end.


## Scope

This repository is **not** intended as a template or starter. **It exists as a complete, self-contained system.**
