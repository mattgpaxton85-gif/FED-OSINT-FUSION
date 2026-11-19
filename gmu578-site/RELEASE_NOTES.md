# GMU 578 independent field map — hybrid release

Build: November 18, 2026. Standalone side project; unrelated to FED-OSINT-FUSION and Washington Hunt Atlas application.

Two basemaps only: Topo and Hybrid (Esri imagery plus transportation and place label reference tile overlays). WDFW GMU 578 boundary, historical elk-use areas, candidate search labels, WDFW-managed land layer, access references, and waypoints may be toggled separately. Offline fallback retains only embedded reference geometry and navigable GIS vectors, without roads or topography. Current WDFW land overlay depends on external network access. No hunt planner, draw odds, or hunting log.

Prepublication headless Chromium audit: 63 interactive checks, 6 failure-path checks, all passed with mocked third-party tile/forecast responses. Tests include basemap switching, road-label tile loading, overlay toggles without refetching basemap, map pan/zoom/fit/tap, snow scenarios and focus, measuring, coordinates, waypoints (CRUD, GPX/JSON), GPS mocked permission, forecast success/error, reference maps, import errors and cross-device width layout. Live third-party map tile service and physical iOS/Android device functionality still require field testing.

Source: separate ChatGPT Library folder `GMU 578 Field Guide`. The GitHub branch `gmu578-isolated-site` is isolated from the repository default branch.
