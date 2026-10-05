# Credits & Acknowledgments

Starpublisher is crafted with deep admiration for the pioneers of desktop publishing and digital vector design.

---

## 🏛️ Foundational Inspirations

Starpublisher stands on the shoulders of the great publishing and graphics suites that defined personal and commercial document design:

### 1. Microsoft Publisher (1991 – 2026)
* **The Inspiration**: For over three decades, Microsoft Publisher brought publication design within reach of educators, small businesses, clubs, and families.
* **Honored Concepts**: 
  - Authentic color schemes (*Alpine, Burgundy, Citrus, Glacier, Marine, Office, Solstice, Verve*, etc.)
  - Balanced font schemes (*Foundation, Modern, Perspective, Capital, Textbook, Office, Calligraphy*)
  - Reusable Page Parts & Building Blocks (decorative heading banners, coupons, pull quotes, calendars)
  - Intuitive frame-based document layout and scratchpad pasteboards
  - Support for legacy `.pub` document interchange

### 2. Adobe InDesign
* **The Inspiration**: The industry benchmark for commercial prepress accuracy, editorial design, and digital document delivery.
* **Honored Concepts**:
  - Commercial print prepress specifications (0.125" / 9 pt bleeds, corner crop marks, bleed ticks, registration targets, CMYK process calibration patches)
  - Facing pages (two-page spreads) with spine/binding fold separation
  - Multiple named master page templates (`Master A`, `Master B`) with per-page assignments
  - Interactive PDF AcroForm widgets (`/Tx` text fields, `/Btn` checkboxes)
  - PDF document outline bookmarks (`/Outlines`) and interactive hyperlinks (`/Link`)
  - Dynamic page numbering tokens (`#Page# of #TotalPages#`)
  - Preflight design inspection (Design Checker)

### 3. Xara Designer & CorelDRAW
* **The Inspiration**: The paragons of blazingly responsive, direct-manipulation vector graphics engines.
* **Honored Concepts**:
  - Zero-latency Direct2D canvas manipulation and 60+ FPS multi-core rendering
  - In-place cloning (`Ctrl+K`) and offset duplication (`Ctrl+D`)
  - Interactive on-canvas gradient arrows and multi-stop color controls
  - Single-key productivity shortcuts (`V`, `T`, `R`, `E`, `L`, `G`)

---

## ⚙️ Core Technology & Engineering

* **Direct2D (D2D1.1)**: Microsoft's hardware-accelerated, immediate-mode 2D graphics API providing sub-pixel anti-aliasing and GPU vector rasterization.
* **DirectWrite**: Advanced typographic rendering engine powering OpenType font metrics, multi-script layouts, and ClearType glyph rasterization.
* **Windows Imaging Component (WIC)**: Unified codec architecture for high-resolution PNG, JPEG, TIFF, BMP, and ICO decoding.
* **Windows Spell Checking API**: Deep Windows 10/11 operating system dictionary and language engine integration.
* **ISO 32000 / PDF 1.5 Specification**: Clean-room implementation of PDF vector graphics, zlib/deflate compression, and AcroForm dictionaries.
* **ISO C++17**: Modern native language features, smart pointers, RAII resource management, and clean memory safety.

---

## 👥 Contributors & Maintainers

* **Starpublisher Team**: Architecture, Direct2D renderer, prepress engine, PDF generator, and user interface.
* **Community Contributors & Testers**: Bug reports, layout validation, typography suggestions, and prepress testing across diverse commercial offset presses and digital copiers.

---

## 📜 Third-Party Licenses & Trademarks

* *Microsoft Publisher*, *Direct2D*, *DirectWrite*, *Windows*, and *Office* are trademarks of Microsoft Corporation.
* *Adobe*, *Adobe InDesign*, and *Adobe Acrobat* are trademarks of Adobe Systems Incorporated.
* *CorelDRAW* is a trademark of Corel Corporation.
* Reference to these products is for historical, compatiblity, and architectural context only. Starpublisher is an independent open-source native project.
