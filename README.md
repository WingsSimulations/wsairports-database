# Wings Simulations Airport Database (wsairports)

A globally unified, clear-text JSON airport dataset containing run-time optimized runways, taxiways, markings, gate startups, radio frequencies, and spatial bounding boxes for 34,074 airports worldwide.

---

## License and Attribution

This dataset is compiled and derived from the X-Plane Airport Scenery Gateway global dataset and is licensed under the GNU General Public License v2.0 (GPLv2).

* Upstream Source: https://gateway.x-plane.com/
* Original Copyright: (C) Laminar Research and individual Gateway community scenery authors.
* Compilation and Format Author: (C) 2026 Wings Simulations.
* License Details: See the full LICENSE file for terms and conditions under GPLv2.

---

## Repository Structure

* airports_index.json: Master lightweight spatial index for fast world querying.
* <ICAO>.wsairport: Detailed individual airport layout definitions.

---

## Spatial Index Specification (airports_index.json)

An array of compact objects designed for fast viewport frustum culling:

```json
[
  {
    "icao": "LOWI",
    "name": "Innsbruck Kranebitten",
    "elevation_ft": 1906.0,
    "center": [47.259137, 11.346785],
    "bbox": [47.258827, 11.336914, 47.261623, 11.35782],
    "rwy_count": 1,
    "gate_count": 28
  }
]
