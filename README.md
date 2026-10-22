# twoisone maps

Offline map files for the twoisone app: one [PMTiles](https://github.com/protomaps/PMTiles)
file per region, downloaded by the app when someone asks for a map of their area,
and drawn on their phone with no further connection.

Each release holds every region and `regions.json`, the list the app reads
(each file's size, SHA-256 and address). The app reads the list of the latest
release.

## Where the files come from

Each region is cut from a [Protomaps](https://protomaps.com) basemap daily build
to the region's outline (an OpenStreetMap boundary, buffered about 2 km), up to
zoom level 14, with `pmtiles extract`.

## Licence

Map data © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright),
available under the [Open Database License](https://opendatacommons.org/licenses/odbl/).
These files are a Produced Work of that database. Basemap schema by Protomaps.
