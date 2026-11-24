# Changelog

## v2.1.2

### Fixed
- TizenTube on Tizen 9 and Tizen 10 (2025 and 2026 TVs). On these TVs also install **TizenTubeStarter.wgt** and always open **TizenTube Starter**: it starts the proxy service through `wrt:service`, waits for it and opens TizenTube.
- The proxy stays alive on Tizen 10 after other apps are used.
- TizenTube runs on its own Cobalt app, so a preloaded stock YouTube no longer opens in its place. You need to sign in to YouTube once more after updating.

### Tizen 10
Cobalt can't reach the default proxy address there. Use **TizenTubeCobaltTizenTubeProxyAddress.wgt** and make `tizentube` resolve to your TV's IP address, or build with your TV's address. See docs/README.md.

Based on the work of maxouxx, Luis Quezada and Kirill Chuprov. This build has not been tested on a TV yet.
