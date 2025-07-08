# Minimalist Design Changes

This version of the ZMK dongle screen module has been modified for a more aesthetic, minimalist appearance.

## Changes Made

### Visual Layout
- **Removed USB/BLE indicator**: The top output status widget has been completely removed for a cleaner look
- **Centered layer display**: The layer indicator is now the main focal point in the center with a subtle circular background
- **Repositioned elements**: All widgets have been repositioned for better visual balance

### Widget Improvements

#### Layer Status (Main Focus)
- Added subtle circular background with transparency
- Positioned in center as primary focus element
- Uses Montserrat 40pt font for clear visibility

#### WPM Status (Top Left)
- Smaller, more subtle design (80x30 pixels)
- Transparent background
- Gray color (#888888) for non-intrusive display
- Shows "wmp" suffix when active, "---" when idle
- Uses Montserrat 14pt font

#### Modifier Status (Below Layer)
- Compact design (120x30 pixels)
- Uses standard Unicode symbols instead of NerdFont icons:
  - ⌃ for Ctrl
  - ⇧ for Shift  
  - ⌥ for Alt
  - ⌘ for GUI/Win
- Light gray color (#CCCCCC)
- Transparent background
- Uses Montserrat 18pt font

#### Battery Status (Bottom)
- Text-only display, no graphical battery icons
- Shows percentage with "%" suffix
- Color coded:
  - Red warning icon (⚠) for <1%
  - Orange for ≤20%
  - Gray (#888888) for normal levels
- Smaller, more compact design (100x25 pixels)
- Uses Montserrat 12pt font

### Configuration Changes
- Output status widget disabled by default (`CONFIG_DONGLE_SCREEN_OUTPUT_ACTIVE=n`)
- Maintains all existing functionality while providing cleaner appearance

## Result
The display now features a clean, minimalist design focused on essential information:
- Layer number prominently displayed in center
- Subtle WPM counter in corner
- Compact modifier indicators
- Simple battery percentage
- No distracting connection status indicators

All widgets use consistent styling with transparent backgrounds, subtle colors, and modern typography for a cohesive, professional appearance.
