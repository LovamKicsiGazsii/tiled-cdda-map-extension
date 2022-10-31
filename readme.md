# Tiled extension for Cataclysm: Dark Days Ahead

What works
- nothing

What kind of works
- saving config
- - it doesn't remember project location... edit the extension and make your project path the autofill default for the path to project prompt for convenience
- import CDDA Tilesets
- - cannot handle items with multiple definitions well at all. Many such items are mislabled as one of their variations, or are missing their IDs
- import CDDA map
- - because the tilesets are incomplete or mislabled in the case of multiple definitions, maps are not complete either
- - items and entities are not imported
- - relative definitions such as inner and outer walls and fences from palettes are not calculated, fallback is used

What doesnt work
- export CDDA map
- - kind of looks like the correct format
- - doesn't actually calculate symbols for map, chooses character from ID. It would need to compare chosen tiles in map to palettes and find a suitable palette, assign it, compare placement of other layers, and export that