# AoA Marketplace Catalog (Public CDN)

This repository hosts the public catalog data for the [AoA](https://armyofagents.org) marketplace. AoA installs fetch `catalog.json` from this location every few hours to populate their marketplace.

## For users

Looking for the marketplace? It's inside the AoA app — install AoA from [armyofagents.org](https://armyofagents.org) and look for the **Marketplace** button in your lobby.

## For developers

The catalog is published as a static JSON file:

- **URL:** [`https://meteoritelabs.github.io/aoa-marketplace-cdn/catalog.json`](https://meteoritelabs.github.io/aoa-marketplace-cdn/catalog.json)
- **Schema:** see [marketplace V1 spec](https://github.com/MeteoriteLabs/aoa) (or your local AoA install's `packages/shared/src/marketplace.ts`)
- **Update cadence:** rebuilt nightly + on-demand by the private aggregator. Cache TTL: 5 minutes.

## How this is generated

The source-of-truth lives in the private [`MeteoriteLabs/aoa-marketplace`](https://github.com/MeteoriteLabs/aoa-marketplace) repo. This public repo is automatically populated by CI on every aggregation run. **Do not commit manual edits here** — they will be overwritten.

## License

The catalog metadata is published under MIT. Individual items in the catalog have their own licenses (see each item's `license` field).
