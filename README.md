# iamshift.dev — Personal Identity System  
**let shift : Moin**  
Shift is standard; design is craft.

This repository contains the complete source code for **iamshift.dev**, a motion-driven identity system and portfolio website built from the ground up using semantic HTML, precision CSS, scroll-driven micro-interactions, and a fully custom boot sequence.  
No frameworks. No templates. Pure hand-crafted front-end architecture.

---

## ✦ Features

### **1. Custom Boot Sequence**
A multi-phase intro experience including:
- Terminal-style line reveal  
- Brand splash animation  
- Cinematic logo spin-reverb  
- Sequential word animation for the site title

### **2. Global Header System**
Persistent top-left identity marker:
- Rotational logo with boot animation  
- Scroll-direction-aware spin (CW/CCW)  
- Word-by-word title reveal  
- Adaptive theme-based color handling

### **3. Vertical Snap Navigation**
Sections are navigated through
- `scroll-snap-type: y mandatory`  
- Cloudflare-friendly, JS-enhanced scroll detection  
- Keyboard navigation (`j/k`, arrows, and spacebar)  
- Section highlighting via intersection observers  

### **4. Section Design System**
Each section is a distinct identity block:
- `init` — brand origin  
- `code` — structured creation (includes animated cursor prompt)  
- `pixel` — visual language (with randomized viewport “spark” pixels)  
- `echo` — reflection & narrative  
- `self` — identity  
- `ping` — availability  

Every section implements:
- Its own reveal timing  
- Its own spatial rhythm  
- Its own micro-interaction vocabulary  

### **5. Performance-Focused Animations**
- No layout thrashing  
- No scroll jank  
- Reflow-safe class toggles  
- Keyframes tuned for cinematic movement  
- Snap container scroll tracking instead of window scroll  

### **6. Zero Dependencies**
- No React, Vue, Tailwind, jQuery, GSAP, etc.  
- No build system required  
- Deploy-ready static front-end  

---

## ✦ File Structure
/

├── index.html          # Complete site markup

├── style.css           # Full custom design system & animations

├── assets/

│   ├── logo-orange.png

│   ├── logo-dark.png   # Optional future theme variant

│   ├── moin.png        # Portrait asset for “self” section

│   └── …other images

└── README.md

---
