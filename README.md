# smk-firewood

An interactive map application for exploring forest management, land use and protected areas data across British Columbia. Built with [SMK (Simple Map Kit)](https://github.com/bcgov/smk) and powered by [Leaflet](https://leafletjs.com/).

## Overview

SMK Firewood provides easy access to BC's comprehensive forest and land management geospatial data. The application displays provincial datasets including municipalities, parks, protected areas, forest tenure, conservation lands and wildlife habitat areas sourced from authoritative BC government services.

## Features

- **Interactive Map Interface**: Zoom and pan across British Columbia to explore forest and land management data
- **Multiple Data Layers**: View and query:
  - Municipalities, administrative boundaries and natural resource districts
  - Provincial Parks, Protected Areas, Conservancy Areas and Ecological Reserves
  - Forest Tenure, Managed Licenses and Crown Land Leases
  - Conservation Lands and Wildlife Habitat Areas
  - Old Growth Management Areas (OGMAs) and Recreation Areas
- **Layer Control**: Toggle visibility of layers
- **Responsive Design**: Works on desktop and mobile devices

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher)
- npm (comes with Node.js)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/bcgov/smk-firewood.git
   cd smk-firewood
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

### Running Locally

To view and test the application locally:

```bash
npm run view
```

This will:
- Start a local HTTP server on port 8080
- Automatically open the application in your default browser

Access the application at `http://localhost:8080`

## Configuration

The application is configured through `smk-config.json`, which defines:

- **Map Viewer**: Leaflet-based viewer with initial zoom level and extent centered on BC
- **Base Map**: ESRI imagery basemap
- **Layers**: ESRI dynamic layers and WMS services for forest management, protected areas and land tenure data with custom styling and attributes
- **Tools**: Layer panel, Geomark and other interactive tools

## Data Sources

- **WMS Services**: OGC Web Map Services from BC government geospatial infrastructure
- **BC Geographic Warehouse**: Authoritative source for provincial forest and land management data

Each layer includes metadata URLs linking to the [BC Data Catalog](https://catalogue.data.gov.bc.ca/) for detailed dataset documentation.

## Technologies Used

- **[SMK (Simple Map Kit)](https://github.com/bcgov/smk)**: BC Government's map framework
- **[Leaflet](https://leafletjs.com/)**: Open-source mapping library
- **[ESRI ArcGIS APIs](https://developers.arcgis.com/)**: Dynamic mapping and services
- **[OGC Web Map Services](https://www.ogc.org/standard/wms/)**: Standard geospatial data access
- **[Caddy](https://caddyserver.com/)**: Lightweight web server
- **[Node.js](https://nodejs.org/)**: JavaScript runtime

## License

Licensed under the Apache License, Version 2.0. See the [LICENSE](LICENSE) file for details.
