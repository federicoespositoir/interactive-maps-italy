# Interactive Maps: The 2024 European Election in Italy

Federico Esposito · Data science coursework in R · 2026

Two interactive maps of the 2024 European Parliament election. Each map has four layers: turnout, the populist radical right vote as a whole, Fratelli d'Italia and Lega. Click an area to see its values.

| Map | Areas | Open |
| --- | --- | --- |
| Italy | 107 provinces and metropolitan cities | [Open the map](https://federicoespositoir.github.io/interactive-maps-italy/maps/italy-provinces-eu2024.html) |
| Metropolitan City of Rome | 121 municipalities | [Open the map](https://federicoespositoir.github.io/interactive-maps-italy/maps/rome-metropolitan-city-eu2024.html) |

## How they are made

I built the maps in R with `sf` and `leaflet`, joining municipal election results to the ISTAT administrative boundaries for 2024. The code is in [code](code/):

- [rome_italy_eu2024_data_and_static_maps.qmd](code/rome_italy_eu2024_data_and_static_maps.qmd) prepares the election data and draws the static maps.
- [interactive_maps.qmd](code/interactive_maps.qmd) builds the interactive maps, with a legend that changes with the selected layer.

The file paths in the code refer to my own computer. To make the maps lighter for the web, I simplified the boundary lines of the published versions; the data and colours are unchanged.

## Sources

- Election results: Italian Ministry of the Interior, 2024 European election open data (CC BY 4.0).
- Boundaries: ISTAT, administrative boundaries at 1 January 2024 (CC BY 4.0).
- Background map tiles: CARTO and Esri.

[Federico Esposito: research portfolio](https://federicoespositoir.github.io/)
