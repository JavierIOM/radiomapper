# Changelog

## [0.1.4] — 2026-05-19

### Added
- Click any marker to open that operator's QRZ.com page in a new tab

## [0.1.3] — 2026-05-19

### Added
- Hover popups on all markers — callsign details appear on mouseover, no click needed
- Demo button — cycles continuously through a worldwide contact sequence (18-contact burst + 6 live arrivals), click Stop to end
- Line draw animation on file load — all contact lines animate outward from home QTH simultaneously

### Fixed
- TypeScript implicit `any` on `parseADIF` text parameter
- Removed unused `liveRenderCount` variable

## [0.1.2] — 2026-05-19

### Added
- Live file watch — click Watch, pick the WSJT-X ADIF file, map updates every 15 seconds as new contacts are logged (Chrome/Edge only via File System Access API)
- Pulsing ● Live indicator in header while watching; click again to stop
- QRZ result cache — repeated re-renders during live watch don't re-query already-resolved callsigns

## [0.1.1] — 2026-05-19

### Added
- Live grey line (solar terminator) — night side polygon + orange terminator lines, updates every 60 seconds
- GL toggle button in header to show/hide the grey line
- `suncalc` dependency for solar position calculations

## [0.1.0] — 2026-05-18

### Added
- Initial release
- ADIF file parser — handles WSJT-X, Minos, and any standard ADIF logger output
- Maidenhead grid square to lat/lon conversion (4-char and 6-char grids)
- Interactive world map (Leaflet + CartoDB dark tiles)
- Lines from home QTH to each worked station with a grid square
- Markers coloured by band with glow effect
- Click-to-popup: callsign, grid, band, mode, date/time, SNR
- Stats bar: total QSOs, mapped count, unmapped count, bands worked
- Band legend (auto-populated from log data)
- Drag-and-drop file loading — drop anywhere on the page
- Home station auto-detected from `my_gridsquare` / `station_callsign` fields
- Dark theme throughout, orange (#f56400) accent
