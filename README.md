# Rail-Insights-and-Demand-Dashboard

## Overview
The Rail Insights and Demand Dashboard is an interactive **rail demand exploration dashboard** built in **Dash** to help users analyse passenger volumes across **origin–destination (OD) station pairs** over time.

The application combines:
- A **map-first interface** for spatial exploration,
- A **filter panel** for selecting years, regions, and stations,
- A **data table + chart** view for inspection and reporting,
- A one-click **export** workflow for downstream analysis.

> ⚠️ Note: This public repo contains an **anonymised** version of the project.  
> All organisation-specific identifiers, internal assets, and proprietary datasets/queries have been removed or abstracted.

---

## Key Features
- **Multi-filter OD exploration**
  - Year selection (multi)
  - Region selection (multi)
  - Origin station (required)
  - Destination station (optional, multi)

- **Interactive map markers**
  - Region-coloured markers using a consistent legend
  - Marker tooltips and popups for quick OD context

- **Demand visualisation**
  - Stacked bar chart of passenger volumes by year
  - Destination-wise breakdown for a selected origin (when filtered)

- **Data inspection**
  - Paginated DataTable of filtered OD records

- **Exports**
  - Export filtered results to Excel (`.xlsx`)
  - Export respects user filters and keeps only relevant columns

- **UX improvements**
  - “Show/Hide Options” collapsible filter pane
  - Fullscreen chart view for presentations/screensharing
  - Terms of use modal gate (anonymised copy)

---

## Tech Stack
- **Python**
- **Dash** (with DashProxy transforms for scalable callbacks)
- **dash-leaflet** (map + markers)
- **Plotly Express** (bar charts)
- **Pandas / NumPy**
- **SQLAlchemy / Postgres** (private version; abstracted in this repo)
- **Dash Bootstrap Components**
- **Dash Design Kit**

---

## Data & Anonymisation
This repo intentionally:
- Replaces database queries with **stubbed/representative loaders**
- Removes internal file paths and organisation identifiers
- Treats station codes/names as **non-sensitive labels** (or uses masked examples)
- Omits any proprietary schema, governance language, and infrastructure details
