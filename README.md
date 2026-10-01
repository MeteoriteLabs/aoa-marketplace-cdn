# AoA Marketplace Catalog (Public CDN)

This repository distributes public catalog data consumed by Army of Agents (AoA). It is a delivery mirror; the source of truth for marketplace content is the [AoA Marketplace repository](https://github.com/tandavkrishna27/aoa-marketplace). Treat that repository as the place to author marketplace items.

## For users

Open the **Marketplace** in the [Army of Agents app](https://github.com/tandavkrishna27/Army-of-Agents) to browse and install agents, skills, plugins, and other catalog items.

## For developers

This repository contains the distributed catalog data in [`catalog.json`](catalog.json) and [`connectors.json`](connectors.json). The catalog declares its schema version in each file. No deployment endpoint or refresh schedule is documented here; use the consuming AoA application's configuration for the active distribution URL and the marketplace source repository for catalog changes.

## AoA ecosystem

- [Army of Agents](https://github.com/tandavkrishna27/Army-of-Agents) — the application
- [AoA Marketplace](https://github.com/tandavkrishna27/aoa-marketplace) — source of truth for marketplace content
- [AoA Marketplace CDN](https://github.com/tandavkrishna27/aoa-marketplace-cdn) — public catalog distribution mirror
- [AoA Skills](https://github.com/tandavkrishna27/AoA-Skills)
- [AoA Community](https://github.com/tandavkrishna27/aoa-community)

## License

This repository is available under the MIT License; see [`LICENSE`](LICENSE). Catalog entries point to separately maintained artifacts; check each artifact's source repository for its applicable license before reusing that artifact.
