# North Carolina County & Parcel Explorer

An interactive map of all 100 North Carolina counties with live statewide parcels, built for the GPN Carolina chapter website.

**Live map:** https://geodegarmo.github.io/nc-parcel-map/

## What it does

- Shows every NC county with labels and a "Jump to a county" list
- Clicking a county zooms to it and shows its parcel count
- Zooming to street level draws parcels; clicking one shows its parcel number, address, acres, values, use and last sale
- Light street map or imagery basemap

## Data

- Parcels: [NC OneMap statewide parcels](https://www.nconemap.gov/pages/parcels), standardized from all 100 counties and the Eastern Band of Cherokee Indians. Counties are the authoritative source.
- County boundaries: NC OneMap regional boundaries service
- Basemaps: Esri Light Gray Canvas, USGS The National Map (Topo) and Esri World Imagery. None need an API key.

Data is read live from public services. No API key is needed and no data is stored in this repo.

## Settings

All settings are in the `CONFIG` block at the top of the script in `index.html`, including the zoom level where parcels appear and whether owner names show in pop-ups (off by default).

## Embedding

```html
<iframe src="https://geodegarmo.github.io/nc-parcel-map/" style="width:100%;height:750px;border:0" loading="lazy"></iframe>
```
