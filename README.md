# Starpublisher

<p align="center">
  <img src="assets/starpublisher_icon.png" alt="Starpublisher Icon" width="160" height="160" />
</p>

<p align="center">
  <b>A high-performance, modern native desktop publishing suite for Windows.</b><br>
  Combining the intuitive ease of Microsoft Publisher, the prepress precision of Adobe InDesign, and the blistering real-time responsiveness of Xara Designer.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows%2010%20%2F%2011%20(x64)-0078D7.svg" alt="Platform" />
  <img src="https://img.shields.io/badge/Language-Modern%20C%2B%2B17-00599C.svg" alt="Language" />
  <img src="https://img.shields.io/badge/Graphics-Direct2D%20%2F%20DirectWrite-008080.svg" alt="Graphics" />
  <img src="https://img.shields.io/badge/Output-Vector%20PDF%201.5%20%7C%20Prepress-D32F2F.svg" alt="PDF" />
  <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License" />
</p>

---

## 🌟 Overview

**Starpublisher** is a clean-sheet, hardware-accelerated desktop publishing application engineered for speed, typography fidelity, and commercial print prepress. Built from the ground up in modern C++17 with Direct2D, DirectWrite, and the Windows Imaging Component (WIC), Starpublisher delivers instant launch times, 60+ FPS smooth canvas manipulation, and deep feature parity with commercial publishing standards—without external dependencies or runtime bloat.

---

## 🚀 Key Feature Highlights

### 1. Multi-Page Spreads & Master Pages
* **Facing Pages (Two-Page Spreads)**: Side-by-side spread layout with central binding spine fold divider, companion page shadows, and independent left/right page formatting.
* **Multiple Named Master Pages**: Create and manage multiple master templates (`Master A`, `Master B`, `Master C`...) and assign them per page.
* **Dynamic Page Numbering**: Real-time evaluation of `#Page#`, `[Page]`, `#PageNumber#`, `#TotalPages#`, `[Pages]`, and `#DocTitle#` across canvas views, master templates, mail merge passes, and PDF export.
* **Multi-Column Layout Guides & Rulers**: Customizable column counts and gutters, draggable cyan/teal ruler guides, and magnetic snapping.

### 2. Commercial Print Prepress
* **Bleed Margin System**: Document bleed configuration (standard 0.125" / 9 pt) with live red dashed boundary guides.
* **Prepress PDF Engine**: Export commercial print-ready PDFs with:
  - 0.5 pt hairline corner crop marks and bleed ticks
  - Concentric bullseye registration targets with crosshairs
  - 100% and 50% CMYK process color calibration patches
  - Publication slug margin metadata lines (document name, page index, timestamp)
* **CMYK Gamut Soft-Proofing**: Interactive on-canvas SWOP/ISO 4-color process proofing simulation mode.

### 3. Interactive Digital PDF & Forms
* **Interactive PDF Forms (`/AcroForm`)**:
  - Fillable text fields (`/Tx`) with custom names and default values
  - Clickable checkboxes (`/Btn`) with active state tracking
  - Standard Adobe Acrobat / ISO 32000 compatibility
* **Navigation Bookmarks (`/Outlines`)**: Automatic hierarchy trees indexing publication pages and major headings for instant navigation in PDF viewers.
* **Clickable Web Hyperlinks (`/Link`)**: Assign `http://`, `https://`, and `mailto:` destinations to shapes, frames, and text boxes.

### 4. Advanced Typography & Story Flow
* **Linked Text Frames (Story Threading)**: Multi-box story flows where text naturally cascades across columns, pages, and spreads.
* **Polygonal Text Wrapping**: Tight, Square, and Top-and-Bottom text wrap around vector obstacles and picture frames.
* **DirectWrite Rich Text**: Per-character fonts, sizes, weights, slants, tracking, colors, baseline offsets, drop caps, and paragraph indents.
* **WordArt Decorative Typography**: Curving arches, waves, 3D extruded gold, neon glow, and rainbow arc text presets.
* **Built-in Spell Checking**: Windows Spell Checking API integration (F7) with suggestion replacements and custom dictionaries.

### 5. Vector Graphics & Photo Framing
* **Boolean Pathfinder Operations**: Union, Subtract, Intersect, and Exclude combiners for vector shape geometry.
* **Picture Frame Masks**: Crop photographs into Rounded Rectangles, Ovals, 5-Point Stars, Hearts, Heraldic Diamonds, and Banners.
* **Image Filters**: Real-time grayscale tint, warm sepia antique filters, and high-key washout watermarks.
* **Fills & Gradients**: Linear and radial multi-stop color ramps, color palette swatches, and Xara-style interactive gradient sliders.

### 6. Personalization & Automation
* **Catalog & Mail Merge**: Connect CSV data sources, insert `«Field»` tokens into text frames, preview individual records live, and batch-generate full multi-page publications.
* **Design Checker (Preflight Audit)**: Proactive preflight scanner detecting overflowing text frames, margin breaches, placeholder text, and prepress boundary violations.
* **Reusable Building Blocks**: Headers, callouts, pull quotes, coupons, monthly calendars, and sidebar stories.

### 7. Document Workflow & Productivity
* **Multi-Tab Document Interface**: Tabbed workspace system with independent zoom, pan, and selection states.
* **Crash-Proof AutoSave**: Periodic background snapshot engine with non-destructive journal recovery.
* **Pack and Go**: Archive entire publications, embedded media, vector assets, and font manifests into portable folders.

---

## ⌨️ Keyboard Shortcuts Reference

| Shortcut | Action |
|:---|:---|
| `Ctrl + N` | New Blank Publication |
| `Ctrl + O` | Open Existing Publication |
| `Ctrl + S` | Save Current Document |
| `Ctrl + P` | Print Publication |
| `Ctrl + Shift + P` | Print Preview |
| `Ctrl + Shift + E` | Export Standard Vector PDF |
| `Ctrl + T` | New Document Tab |
| `Ctrl + W` | Close Document Tab |
| `Ctrl + Tab` | Next Document Tab |
| `Ctrl + Z` / `Ctrl + Y` | Undo / Redo |
| `Ctrl + C` / `Ctrl + V` | Copy / Paste Object |
| `Ctrl + D` | Duplicate Object (+20pt offset) |
| `Ctrl + K` | Clone Object In-Place (0 offset) |
| `Ctrl + G` / `Ctrl + U` | Group / Ungroup Shapes |
| `Ctrl + Shift + H` / `+ V` | Flip Horizontal / Flip Vertical |
| `Ctrl + F` / `Ctrl + H` | Find Text / Replace Text |
| `F7` | Spell Check |
| `F4` / `Shift + F4` | Cycle Color Schemes / Auto-Stretch UI |
| `Ctrl + 1` / `Ctrl + 0` | 100% Zoom / Fit to Screen |
| `Ctrl + [` / `Ctrl + ]` | Decrease / Increase Text Font Size |
| `T` / `R` / `E` / `L` | Quick Insert Text / Rectangle / Ellipse / Line |

---

## 🛠️ Building Starpublisher

### Prerequisites
* **Operating System**: Windows 10 (1809+) or Windows 11 (x64)
* **Compiler**: Microsoft Visual C++ 2022 (MSVC v143 toolset)
* **SDK**: Windows 10/11 SDK (Direct2D 1.1, DirectWrite, WIC, GDI+)

### Build Commands
Starpublisher includes an automated build driver (`build.cmd`) that manages version stamping, compiling, resource packaging, and release zips:

```cmd
:: Build Release x64 binary and release archive
build.cmd

:: Build Debug x64 binary with debug symbols
build.cmd debug

:: Direct clean rebuild
build.cmd __run
```

Output binaries are placed in:
* `bin/Starpublisher.exe`
* `releases/Starpublisher_v<version>_Build<number>.zip`

---

## 📂 Source Architecture

```
Starpublisher/
├── assets/                  # High-resolution logos, app icons, and graphics
├── bin/                     # Compiled executables
├── releases/                # Numbered release archives (.zip)
├── src/
│   ├── App.h / App.cpp      # Main application window, Ribbon UI, canvas viewport
│   ├── DocumentModel.h/.cpp # Page model, multi-master pages, spreads, bleeds, undo/redo
│   ├── DrawObject.h/.cpp    # Vector shapes, text boxes, picture frames, form fields
│   ├── OutputExport.h/.cpp  # Prepress PDF exporter, image rasterizers, SVG output
│   ├── PdfWriter.h/.cpp     # Custom PDF 1.5 engine (bookmarks, links, AcroForm, deflate)
│   ├── PdfRenderTarget.h    # Direct2D to PDF vector conversion backend
│   ├── RichText.h/.cpp      # Paragraph and character formatting run models
│   ├── PropertyPanel.h/.cpp # Interactive property inspector panel
│   ├── MailMerge.h/.cpp     # CSV parsing and dynamic field substitution
│   ├── DesignChecker.h/.cpp # Preflight audit rules and auto-fix repair engine
│   ├── PubFormat.h/.cpp     # Native .starpub XML serialization
│   ├── PubImport.h/.cpp     # Legacy Microsoft Publisher (.pub) binary import
│   ├── Starpublisher.rc     # Win32 version info and application icon resource
│   └── Version.h            # Semantic version numbers and continuous build counter
└── tests/                   # Standalone test suite (PDF writer, text search, rich text)
```

---

## 📄 License

Starpublisher is distributed under the [MIT License](LICENSE). See [CREDITS.md](CREDITS.md) for full project acknowledgments.
