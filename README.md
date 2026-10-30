# Tokyo 23 wards — building energy and carbon

Interactive visualization of all 1,972,342 source building objects in Tokyo’s 23 special wards. The map retains source polygons, source attributes, linked evidence and the three energy/carbon indicators. Gzip compression is lossless. Tama and island buildings are outside the study scope.

Estimates combine EnergyPlus surrogate predictions, Japanese reference parameters and explicitly labelled scenarios. These are not metered observations. The web package omits bulk local research databases; unavailable bulk-download links are clearly labelled. Source attributions and methodology are retained in the map and reports.

Open `map/index.html` using any static HTTP server. Local preview: `python -m http.server 8000`.

Published with GitHub Pages from the main branch root. No server or credentials are embedded.

## Deployment package

The complete static site (including all map resources) is stored in numbered snapshot parts. `python build_site.py` verifies each part and every extracted file, then restores the original directory structure to `_site/`. GitHub Actions publishes `_site/` to GitHub Pages. Parts are each below GitHub’s browser upload file limit. The source HTML, CSS and JavaScript are all included in the snapshot.

Website: https://XiPeng415.github.io/tokyo-building-energy/
