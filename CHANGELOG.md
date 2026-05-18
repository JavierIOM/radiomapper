# Changelog

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
