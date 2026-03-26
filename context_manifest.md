# 🧠 AI Context Manifest
*Last Updated: March 26, 2026*

### Technical Environment
- **Platform:** Home Assistant (2026 Release)
- **View Type:** Panel (100vh layout)
- **Core Dependencies (HACS):** - `custom:button-card`
  - `custom:layout-card`
  - `custom:stack-in-card`
  - `custom:card-mod`

### Grid Geometry
The dashboard uses a master grid to maintain the OS 9 layout:
- **Header:** 38px Fixed.
- **Desktop Columns:** `60px` (Control Strip) | `1fr` (Workspace) | `160px` (Icons).
- **Height Calculation:** `calc(100vh - 38px)` to prevent vertical scrolling.

### State Dependencies
- **Sticky Note Toggle:** Requires an `input_boolean.macos_notepad` helper.
- **Centering Logic:** Uses `place-self: center` on the `desktop` grid area to bypass theme-specific padding.